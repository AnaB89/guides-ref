# API svyToolbarFilter v1

### Classes

[ListComponentFilterRenderer](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer-abstracttoolbarfilterux) ⇐ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)

### Members

[FILTER\_TYPES](API-svyToolbarFilter-v1.md#filter\_types)

### Functions

[createFilterToolbar(listComponent, table)](API-svyToolbarFilter-v1.md#createfiltertoolbar-listcomponent-table-abstracttoolbarfilterux) ⇐ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)

Creates a filter toolbar implementation using the custom list from the custom-rendered-components package.


This implementation expects an NG "Data Grid" table component and a "Custom List" component.


The filters offered from this implementation are generated from the table provided as follows:

* any column with its `filterType` property set to TEXT will be offered as a token popup, allowing the user to enter any number of Strings to match
* any column with its `filterType` property set to TEXT and the `valuelist` will be offered as a lookup where the user can search for and select any number of values
* any column with its `filterType` property set to NUMBER will be offered as a number filter with a number of operators
* any column with its `filterType` property set to DATE will be offered as a date filter with a number of operators

You should create a toolbar filter instance at the onLoad of your form and assign it to a form variable.

Make sure to re-direct the onClick event of the "List Component" to the toolbar.onClick(entry, index, dataTarget, event);

[setPopupRendererForm(formType, form)](API-svyToolbarFilter-v1.md#setpopuprendererform-formtype-form)

### ListComponentFilterRenderer ⇐ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)

**Extends**: [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)

* [ListComponentFilterRenderer](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer-abstracttoolbarfilterux) ⇐ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)
  * [.clearGridFilters()](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.cleargridfilters-boolean) ⇒ `Boolean`
  * [.getElement()](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.getelement-runtimecomponent) ⇒ `RuntimeComponent`
  * [.getQuery()](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.getquery-qbselect) ⇒ `QBSelect`
  * [.getSearchProvider(column)](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.getsearchprovider-column-scopes.svysearch.searchprovider) ⇒ `scopes.svySearch.SearchProvider`
  * [.getSearchText()](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.getsearchtext-string) ⇒ `String`
  * [.getSimpleSearch()](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.getsimplesearch-scopes.svysearch.simplesearch) ⇒ `scopes.svySearch.SimpleSearch`
  * [.getToolbarFiltersState()](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.gettoolbarfiltersstate-array-.less-than-id-string-dataprovider-string-op) ⇒ `[ 'Array' ].<{id: String, dataprovider: String, operator: String, params: Object, text: String, values: Array}>`
  * [.hasFilters()](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.hasfilters-boolean) ⇒ `Boolean`
  * [.onClick(entry, index, dataTarget, event)](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.onclick-entry-index-datatarget-event)
  * [.restoreToolbarFiltersState(jsonState)](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.restoretoolbarfiltersstate-jsonstate)
  * [.search(\[searchText\])](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.search-searchtext)
  * [.setAutoApplyFilters(autoApply)](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.setautoapplyfilters-autoapply-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)
  * [.setFilterValue(column, values, operator)](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.setfiltervalue-column-values-operator)
  * [.setOnFilterAddedCallback(callback)](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.setonfilteraddedcallback-callback-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)
  * [.setOnFilterApplyCallback(callback)](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.setonfilterapplycallback-callback-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)
  * [.setOnFilterCreate(callback)](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.setonfiltercreate-callback-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)
  * [.setOnFilterRemovedCallback(callback)](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.setonfilterremovedcallback-callback-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)
  * [.setOnSearchCommand(callback)](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.setonsearchcommand-callback-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)
  * [.setSearchText()](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.setsearchtext-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)
  * [.showPopupFilterPicker(target)](API-svyToolbarFilter-v1.md#listcomponentfilterrenderer.showpopupfilterpicker-target)
  * [new ListComponentFilterRenderer(listComponent, table)](API-svyToolbarFilter-v1.md#new-listcomponentfilterrenderer-listcomponent-table)

#### listComponentFilterRenderer.clearGridFilters() ⇒ `Boolean`

Clears all grid filters

#### listComponentFilterRenderer.getElement() ⇒ `RuntimeComponent`

Returns the element used to display the filters

**Overrides**: [`getElement`](API-svyToolbarFilter-v1.md#AbstractToolbarFilterUX+getElement)

#### listComponentFilterRenderer.getQuery() ⇒ `QBSelect`

Applies all filters and returns the query for this toolbar

#### listComponentFilterRenderer.getSearchProvider(column) ⇒ `scopes.svySearch.SearchProvider`

Returns the SearchProvider for the given column

| Param  | Type                                             |
| ------ | ------------------------------------------------ |
| column | `[ 'CustomType' ].<aggrid-groupingtable.column>` |

#### listComponentFilterRenderer.getSearchText() ⇒ `String`

Returns the search text for the simple search

#### listComponentFilterRenderer.getSimpleSearch() ⇒ `scopes.svySearch.SimpleSearch`

Returns the SimpleSearch

#### listComponentFilterRenderer.getToolbarFiltersState() ⇒ `[ 'Array' ].<{id: String, dataprovider: String, operator: String, params: Object, text: String, values: Array}>`

Returns the filters' state of the toolbar

**Returns**: `[ 'Array' ].<{id: String, dataprovider: String, operator: String, params: Object, text: String, values: Array}>` - jsonState

#### listComponentFilterRenderer.hasFilters() ⇒ `Boolean`

Returns true if the table has any column it can filter on

#### listComponentFilterRenderer.onClick(entry, index, dataTarget, event)

Called when the mouse is clicked on a list entry.

| Param      | Type      |
| ---------- | --------- |
| entry      | `object`  |
| index      | `Number`  |
| dataTarget | `string`  |
| event      | `JSEvent` |

#### listComponentFilterRenderer.restoreToolbarFiltersState(jsonState)

Restores the filters' state

| Param     | Type                                                                                                              |
| --------- | ----------------------------------------------------------------------------------------------------------------- |
| jsonState | `[ 'Array' ].<{id: String, dataprovider: String, operator: String, params: Object, text: String, values: Array}>` |

#### listComponentFilterRenderer.search(\[searchText])

Applies all filters and executes the search

| Param         | Type     | Description                                                                                                                           |
| ------------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| \[searchText] | `String` | optional searchText to search for; if not provided here, call setSearchText() to set the search criteria before performing the search |

#### listComponentFilterRenderer.setAutoApplyFilters(autoApply) ⇒ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)

| Param     | Type      |
| --------- | --------- |
| autoApply | `Boolean` |

#### listComponentFilterRenderer.setFilterValue(column, values, operator)

Sets a filter value for the given column

| Param    | Type                                             |
| -------- | ------------------------------------------------ |
| column   | `[ 'CustomType' ].<aggrid-groupingtable.column>` |
| values   | `Array`                                          |
| operator | `String`                                         |

#### listComponentFilterRenderer.setOnFilterAddedCallback(callback) ⇒ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)

Sets a callback method that is fired whenever a filter has been added

| Param    | Type       |
| -------- | ---------- |
| callback | `function` |

#### listComponentFilterRenderer.setOnFilterApplyCallback(callback) ⇒ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)

Sets a callback method that is fired whenever the filter is applied\
The callback method receives an array of values, the operator and the filter as arguments

| Param    | Type       |
| -------- | ---------- |
| callback | `function` |

#### listComponentFilterRenderer.setOnFilterCreate(callback) ⇒ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)

Allows to provide a method that will be called when the filter for a specific column is created\
That method then can create and return any filter that will then be used for this column

| Param    | Type       | Description                                                                                                                   |
| -------- | ---------- | ----------------------------------------------------------------------------------------------------------------------------- |
| callback | `function` | function that receives an aggrid-groupingtable Column as argument and must return a scopes.svyPopupFilter.AbstractPopupFilter |

#### listComponentFilterRenderer.setOnFilterRemovedCallback(callback) ⇒ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)

Sets a callback method that is fired whenever a filter is removed

| Param    | Type       |
| -------- | ---------- |
| callback | `function` |

#### listComponentFilterRenderer.setOnSearchCommand(callback) ⇒ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)

Set the onSearchCommand function to override the search behavior. You can add custom conditions to the filter query object;

| Param    | Type       |
| -------- | ---------- |
| callback | `function` |

**Example**

```js
function onSearch(query, fs) {
  // add custom conditions to the query
  query.where.add(query.columns.orderdate.not.isNull);
  
  // apply the query to the foundset
  fs.loadRecords(query);
}
```

#### listComponentFilterRenderer.setSearchText() ⇒ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)

Sets the search text for the simple search

#### listComponentFilterRenderer.showPopupFilterPicker(target)

Shows the filter picker popup

| Param  | Type               |
| ------ | ------------------ |
| target | `RuntimeComponent` |

#### new ListComponentFilterRenderer(listComponent, table)

Filter Toolbar implementation using the custom list from the custom-rendered-components package. This implementation requires a "List Component" element and an "Data-Grid" element. You should create a toolbar filter instance at the onLoad of your form and assign it to a form variable. Make sure to re-direct the onClick event of the "List Component" to the toolbar.onClick(entry, index, dataTarget, event);

| Param         | Type                                                                                                                           |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| listComponent | `RuntimeWebComponent.<customrenderedcomponents-customlist>` \| `RuntimeWebComponent.<customrenderedcomponents-customlist_abs>` |
| table         | `RuntimeWebComponent.<aggrid-groupingtable>` \| `RuntimeWebComponent.<aggrid-groupingtable_abs>`                               |

**Example**

```js
//keep track of toolbarFilter object in a form variable
var toolbarFilter;

//init the toolbarFilter at the onLoad.
function onLoad(event) {
 toolbarFilter = new scopes.svyToolbarFilter.ListComponentFilterRenderer(elements.filterToolbar, elements.table)
}

//propagate the onClick event of the "List Component" to the toolbar filter.
function onClick(entry, index, dataTarget, event) {
 toolbarFilter.onClick(entry,index,dataTarget,event);
}

//optionally set a searchText for a cross-field search to further filter the result set
function search() {
 toolbarFilter.setSearchText(searchText);
 toolbarFilter.search();
}
```

### createFilterToolbar(listComponent, table) ⇐ [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)

Creates a filter toolbar implementation using the custom list from the custom-rendered-components package.\


This implementation expects an NG "Data Grid" table component and a "Custom List" component.\


The filters offered from this implementation are generated from the table provided as follows:

* any column with its `filterType` property set to TEXT will be offered as a token popup, allowing the user to enter any number of Strings to match
* any column with its `filterType` property set to TEXT and the `valuelist` will be offered as a lookup where the user can search for and select any number of values
* any column with its `filterType` property set to NUMBER will be offered as a number filter with a number of operators
* any column with its `filterType` property set to DATE will be offered as a date filter with a number of operators

You should create a toolbar filter instance at the onLoad of your form and assign it to a form variable.

Make sure to re-direct the onClick event of the "List Component" to the toolbar.onClick(entry, index, dataTarget, event);

**Extends**: [`AbstractToolbarFilterUX`](API-svyToolbarFilter-v1.md#new\_AbstractToolbarFilterUX\_new)

| Param         | Type                                                                                                                           |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| listComponent | `RuntimeWebComponent.<customrenderedcomponents-customlist>` \| `RuntimeWebComponent.<customrenderedcomponents-customlist_abs>` |
| table         | `RuntimeWebComponent.<aggrid-groupingtable>` \| `RuntimeWebComponent.<aggrid-groupingtable_abs>`                               |

**Example**

```js
//keep track of toolbarFilter object in a form variable
var toolbarFilter;

//init the toolbarFilter at the onLoad.
function onLoad(event) {
 toolbarFilter = scopes.svyToolbarFilter.createFilterToolbar(elements.filterToolbar, elements.table)
}

//propagate the onClick event of the "Custom List" component to the toolbar filter.
function onClick(entry, index, dataTarget, event) {
 toolbarFilter.onClick(entry, index, dataTarget, event);
}

//optionally set a searchText for a cross-field search to further filter the result set
function search() {
 toolbarFilter.search(searchText);
}
```

### setPopupRendererForm(formType, form)

| Param    | Type                                                                  | Description              |
| -------- | --------------------------------------------------------------------- | ------------------------ |
| formType | `String`                                                              | any of the FILTER\_TYPES |
| form     | `RuntimeForm.<AbstractPopupFilter>` \| `RuntimeForm.<AbstractLookup>` | the form to set          |



### FILTER\_TYPES

* [FILTER\_TYPES](API-svyToolbarFilter-v1.md#filter\_types)
  * [.DATE](API-svyToolbarFilter-v1.md#filter\_types.date)
  * [.NUMBER](API-svyToolbarFilter-v1.md#filter\_types.number)
  * [.SELECT](API-svyToolbarFilter-v1.md#filter\_types.select)
  * [.TOKEN](API-svyToolbarFilter-v1.md#filter\_types.token)

#### FILTER\_TYPES.DATE

Date filter

#### FILTER\_TYPES.NUMBER

Number filter

#### FILTER\_TYPES.SELECT

Select filter

#### FILTER\_TYPES.TOKEN

Tokens filter

***
