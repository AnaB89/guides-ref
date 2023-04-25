# Table

Servoy Extra Table is a **lightweight read-only** table. It can be used both in responsive forms and absolute forms. If used in responsive mode, its 'responsiveHeight' property must be set in _Properties View_ (which is the fixed height it will occupy).

It has typical table features, (fixed) table header, formats, styling, paging, column resize, column sort, valuelist support (for translating a real value to a display value). The model and API can be seen in Servoy Developer.

The purpose of this table component is to be able to **show large numbers of rows with acceptable or fast response times**.

The table is highly configurable from _Properties View_ - in Developer. It can be configured to do paging and/or incremental scrolling.

## Table of contents

* [Paging](Table.md#1.-paging)
* [Incremental scrolling](Table.md#2.-incremental-scrolling)
* [Columns size](Table.md#3.-columns-size)
* [Table properties](Table.md#4.-table-properties)
* [Column custom type](Table.md#5.-column-custom-type)
* [Table events](Table.md#6.-table-events)
* [Table API](Table.md#7.-table-api)
* [Key Code Settings](Table.md#8.-key-code-settings)

## 1. Paging

You can set pageSize > 0 for **fixed page sizes**, or pageSize 0 to **disable paging**; we intend to add pageSize -1 for auto-determining page size based on available height but that is not implemented yet.

## 2. Incremental scrolling

This can work together with paging as well, so you can have a large page size and incremental scrolling would still work.

Incremental scrolling means that if many rows are available (hundreds/thousands) only then rows surrounding the ones that need to be shown will be loaded from server and only a part of those will initially be rendered (added to the browser's DOM).

When the user scrolls, more rows will be loaded from server if needed and more rows will be rendered as needed.

The purpose of all this is that, for example, if you have 1000 rows and selected row is 823, we don't send to the browser the data for all 1000 rows and render thousands of cells in browser. Just some rows around the visible area (which initially will show selected row 823) will be loaded and some of them rendered. This can drop initial show time from tens of seconds or minutes (depending also on the data in each column, connection speed, hardware, ...) to less then one second.

Incremental scrolling can be controlled/customized or virtually disabled by modifying the following properties in properties view:

```
performanceSettings : {
	minBatchSizeForRenderingMoreRows: 10,
	minBatchSizeForLoadingMoreRows: 20,
	maxRenderedRows: 450,
	maxLoadedRows: 1000,
	fastScrollRenderThresholdFactor : 3.0,
	fastScrollLoadThresholdFactor : 2.3
}
```

The values above are the **default values that should be fine** for most situations. If you want to tweak them, here is what they mean:

* **performanceSettings.minBatchSizeForRenderingMoreRows**: influences **the minimum of**:
  * how many rows around the initial visible area will be rendered initially;
  *   (when scrolling) how many more rows get rendered each time in the direction of the scroll - in advance. This is done so that when the user scrolls, content is prepared for being shown. The **default value is 10**.

      The real value of initial rendered rows and of additional batch sizes for rendering is actually calculated from the visible height that the table has to work with in the browser, but it cannot go lower then what this setting requires.

      If you want to disable incremental rendering, just set a very high value for this setting and then all available (loaded from server) rows will be rendered right away (this makes sense when combined with paging - acceptable page size).
* **performanceSettings.minBatchSizeForLoadingMoreRows**: influences **the minimum of**:
  * how many rows around the initial visible area will be loaded from server initially;
  *   (when scrolling) how many more rows get loaded from server each time in the direction of the scroll - in advance. When the user scrolls, row data is received from server ahead of the scroll so that more rows can be rendered. The **default value is 20**.

      The real value of initial loaded rows and of additional batch sizes for loading rows from server is actually calculated based on the visible height that the table has to work with in the browser, but it cannot go lower then what this setting requires.

      If you want to disable incremental loading of row data, just set a very high value in there and then all needed rows will be loaded from server (this makes sense when combined with paging - acceptable page size).
*   **performanceSettings.maxRenderedRows**: in order to not slow down browser UI due to a huge number of DOM elements being created, this limits the number of rows that the table will render.

    If the user scrolls a lot and this results in more then 'maxRenderedRows' being rendered - the table will discard a part of the rendered rows and start fresh - as if it was rendering initially around the visible area.

    If you set a high value, many rows can get rendered in the browser and then you will have a more natural feel when scrolling fast back to already rendered rows. But if the value is too high and the browser slows down too much it is better to start fresh with less rendered rows more often (so have this set to a lower value).

    **Default value is 450** (although some browser & hardware can handle nicely even more rendered rows, depending also on content).
*   **performanceSettings.maxLoadedRows**: in order to not use too much memory in the browser due to a huge number of rows (row data) being loaded, this limits the number of rows that the table will keep loaded.

    If the user scrolls a lot and this results in more then 'maxLoadedRows' being loaded - the table will discard a part of the loaded rows.

    If you set a high value, many rows can get loaded in the browser and then you will have a more natural feel when scrolling fast back to already loaded rows. But if the value is too high the browser memory usage might grow too much and it is better to discard part of the loaded rows (from the opposite side then user is scrolling to).

    **Default value is 1000** (although some hardware can handle nicely even more loaded rows, depending also on content).
*   **performanceSettings.fastScrollRenderThresholdFactor**: **Default value: 3.0 (float)**; if for example you have a table with 1000 rows and initially the selected row is shown at index 700 - rendered rows and loaded rows will be around the visible area. Then if the user grabs the scroll knob with the mouse and drags fast upwards to the beginning we have to discard what we have rendered and render the first set of rows instead.

    We cannot just render batches of rows one by one upwards until we reach the first row because that will take a very long time. This setting determines when the table component considers a scroll operation to be a "**fast-scroll**" that needs a discard of currently rendered rows and a render of the new visible area.

    When the scroll position is more then 'fastScrollRenderThresholdFactor \* initiallyRenderedRows' apart from currently rendered rows, the scroll operation is considered to need a completely new set of rendered rows.
*   **performanceSettings.fastScrollLoadThresholdFactor**: **Default value: 2.3 (float)**; if for example you have a table with 1000 rows and initially the selected row is shown at index 700 - rendered rows and loaded rows will be around the visible area. Then if the user grabs the scroll knob with the mouse and drags fast upwards to the beginning we have to discard what we have loaded and load the first set of rows instead.

    We cannot just load from server batches of rows one by one upwards until we reach the first row because that will take a very long time. This setting determines when the table component considers a scroll operation to be a "**fast-scroll**" that needs a discard of currently loaded rows and a load of rows from the new visible area.

    When the scroll position is more then 'fastScrollLoadThresholdFactor \* initiallyLoadedRows' apart from currently loaded rows, the scroll operation is considered to need a completely new set of loaded rows.

If you modify any of these performance settings, please make sure that:

```
minBatchSizeForRenderingMoreRows < minBatchSizeForLoadingMoreRows
maxRenderedRows < maxLoadedRows
minBatchSizeForRenderingMoreRows  < maxRenderedRows (by a lot)
minBatchSizeForLoadingMoreRows < maxLoadedRows (by a lot)
```

## 3. Columns size

Columns width can be set as pixel value (ex. "50px"), as a percentage of the table width ( "25%" ), or it can be left empty, and in this case it will have an automatic value calculated to fill the table width;

If the "autoResize" flag of a column is set, the width of the column will increase/decrease when the width of the table is increasing/decreasing (ex. the table is anchored to right, and the window is resized), in order to fill/empty the extra width of the table;

In order to enable column resizing in the table UI, the "enableColumnResize" flag of the table component need to be set;

As for now there is no support for horizontal scrolling, you need to set the minimum width of the table to the sum of the columns width (the actual width for fixed columns and 1px for auto-resize columns with no width set)

## 4. Table properties

| Property                  | Type            | Default                       | Description                                                                                                                                          |
| ------------------------- | --------------- | ----------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| columns                   | column\[]       | null                          | Table columns                                                                                                                                        |
| currentPage               | int             | 1                             | Current page of the table                                                                                                                            |
| foundset                  | foundset        | form foundset                 | Table foundset                                                                                                                                       |
| pageSize                  | int             | 20                            | Table page size                                                                                                                                      |
| styleClass                | styleclass      | null                          | Additional style class(es) of the component                                                                                                          |
| selectionClass            | styleclass      | null                          | Additional style class(es) of the selected row of the component                                                                                      |
| rowStyleClassDataprovider | dataprovider    | null                          | Additional style class(es) of the component, given by a dataprovider                                                                                 |
| tabSeq                    | tabseq          | null                          | Tab sequence number                                                                                                                                  |
| visible                   | visible         | true                          | When false component is not visible                                                                                                                  |
| enableColumnResize        | boolean         | false                         | Whether columns can be resized from browser                                                                                                          |
| enableSort                | boolean         | true                          | Sort enable on table columns                                                                                                                         |
| responsiveHeight          | int             | 300                           | Height of the table in responsive form                                                                                                               |
| responsiveDynamicHeight   | boolean         | false                         | When is set, the height is defined by the number of rows; if the calculated height exceeds 'responsiveHeight', then the later will be used as height |
| minRowHeight              | string          | "25px"                        | Min height of the row                                                                                                                                |
| sortupClass               | styleclass      | "table-servoyextra-sort-up"   | CSS class for ascending sort of a column                                                                                                             |
| sortdownClass             | styleclass      | "table-servoyextra-sort-down" | CSS class for descending sort of a column                                                                                                            |
| sortDirection             | string          | null                          | 'up' or 'down' value indicating current sort direction                                                                                               |
| performanceSettings       | settings        | null                          | See above for full explanation                                                                                                                       |
| keyCodeSettings           | keyCodeSettings | null                          | See below for full explanation                                                                                                                       |

## 5. Column custom type

| Property               | Type         | Default      | Description                                                                 |
| ---------------------- | ------------ | ------------ | --------------------------------------------------------------------------- |
| dataprovider           | dataprovider | null         | Column dataprovider to be displayed in table cell                           |
| format                 | format       | type default | Format for the dataprovider                                                 |
| headerStyleClass       | styleclass   | null         | Header styleclass to be added                                               |
| headerText             | tagstring    | null         | Header text                                                                 |
| styleClass             | styleclass   | null         | Additional style class(es) to be added to the column                        |
| styleClassDataprovider | dataprovider | null         | Additional style class(es) to be added to the column, given by dataprovider |
| valuelist              | valuelist    | null         | Column valuelist                                                            |
| width                  | string       | 'auto'       | Column width (see Column size section)                                      |
| autoResize             | boolean      | false        | Column autoresize (see Column size section)                                 |
| showAs                 | string       | 'auto'       | Type of the text, can be 'text' , 'html' or 'sanitizedHtml'                 |

## 6. Table events

| Event                 | Params                                                                | Return  | Description                                                               |
| --------------------- | --------------------------------------------------------------------- | ------- | ------------------------------------------------------------------------- |
| onCellClick           | foundsetindex: int , columnindex: int, record: record, event: JSEvent |         | Fired when you click a cell in table                                      |
| onCellDoubleClick     | foundsetindex: int , columnindex: int, record: record, event: JSEvent | boolean | Fired when you double click a table cell                                  |
| onCellRightClick      | foundsetindex: int , columnindex: int, record: record, event: JSEvent | boolean | Fired when you right click a table cell                                   |
| onHeaderClick         | columnindex: int , sortdirection: string, event: JSEvent              | boolean | Fired when you click a table header. Sort direction can be 'up' or 'down' |
| onFocusGainedMethodID | event:JSEvent                                                         |         | Fired when table gets focus                                               |
| onFocusLostMethodID   | event:JSEvent                                                         |         | Fired when table looses focus                                             |

## 7. Table API

| Method           | Params                                  | Return  | Description                                                                |
| ---------------- | --------------------------------------- | ------- | -------------------------------------------------------------------------- |
| requestFocus     | mustExecuteOnFocusGainedMethod: boolean |         | Gives focus to the table. Parameter decides if focus event will be called. |
| getColumnsCount  |                                         | int     | Returns number of columns.                                                 |
| getColumn        | index: int                              | column  | Returns a column by index.                                                 |
| newColumn        | dataprovider: string, \[index: int]     | column  | Creates a new column.                                                      |
| removeColumn     | index: int                              | boolean | Remove a column.                                                           |
| removeAllColumns |                                         | boolean | Remove all columns from table.                                             |

Adding a table in a flex-content layout and setting the table responsiveHeight property to 0, let the table grow up to 100% height of parent element. Used with other containers than flex-content layout in order to grow the table to 100% height, the parent element must have a fixed size.

## 8. Key Code Settings

On key press of any below keyboard codes we can activate different actions on the table.\
Also allows us to enable or disable this option per key.

pageUp : Move down to last visible item in view

pageDown : Move up to first visible item in view

arrowUp : Move up one record in table

arrowDown : Move down one record in table

home : Move to the first record in the table

end : Move to the last record in the table

enter : Fire the onCellClick event
