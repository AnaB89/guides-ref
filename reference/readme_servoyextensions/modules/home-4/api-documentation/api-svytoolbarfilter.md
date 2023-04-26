# API svyToolbarFilter

### Classes

[ListComponentFilterRenderer](api-svytoolbarfilter.md#listcomponentfilterrenderer-abstracttoolbarfilterux) ⇐ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)[NgGridListComponentFilterRenderer](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer-listcomponentfilterrenderer) ⇐ [`ListComponentFilterRenderer`](api-svytoolbarfilter.md#listcomponentfilterrenderer-abstracttoolbarfilterux)

### Members

[FILTER\_TYPES](api-svytoolbarfilter.md#filter\_types)

### Functions

[createFilterToolbar(listComponent, tableOrFoundSet)](api-svytoolbarfilter.md#createfiltertoolbar-listcomponent-tableorfoundset-nggridlistcomponentfilterrenderer) ⇒ [`NgGridListComponentFilterRenderer`](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer-listcomponentfilterrenderer)

Creates a filter toolbar implementation using the custom list from the custom-rendered-components package.

This implementation expects an NG "Data Grid" table component and a "Custom List" component.

The filters offered from this implementation are generated from the table provided as follows:

* any column with its `filterType` property set to TEXT will be offered as a token popup, allowing the user to enter any number of Strings to match
* any column with its `filterType` property set to TEXT and the `valuelist` will be offered as a lookup where the user can search for and select any number of values
* any column with its `filterType` property set to NUMBER will be offered as a number filter with a number of operators
* any column with its `filterType` property set to DATE will be offered as a date filter with a number of operators

You should create a toolbar filter instance at the onLoad of your form and assign it to a form variable.

Make sure to re-direct the onClick event of the "List Component" to the toolbar.onClick(entry, index, dataTarget, event);

[createSimpleFilterToolbar(listComponent, \[foundsetToFilter\])](api-svytoolbarfilter.md#createsimplefiltertoolbar-listcomponent-foundsettofilter-listcomponentfilterrenderer) ⇒ [`ListComponentFilterRenderer`](api-svytoolbarfilter.md#listcomponentfilterrenderer-abstracttoolbarfilterux)

Creates a filter toolbar implementation using the custom list from the custom-rendered-components package.

This implementation expects a "Custom List" component. An optional foundset to be filtered can be provided. If not given, the foundset of the form of the given list component is used.

Filters to be offered need to be added via the API method `addFilter(titleText, dataProvider, filterType)`.

You should create a toolbar filter instance at the onLoad of your form and assign it to a form variable.

Make sure to re-direct the onClick event of the "List Component" to the toolbar.onClick(entry, index, dataTarget, event);

[getConfigSortPickerAlphabetically()](api-svytoolbarfilter.md#getconfigsortpickeralphabetically-boolean) ⇒ `Boolean`

Returns true if the filter picker is sorted alphabetically

[setConfigDateDisplayFormat(displayFormat)](api-svytoolbarfilter.md#setconfigdatedisplayformat-displayformat)

Sets global display date format to be used

[setConfigSortPickerAlphabetically(sortAlphabetically)](api-svytoolbarfilter.md#setconfigsortpickeralphabetically-sortalphabetically)

Sort the the filter picker alphabetically. Default sort is based on column's position in grid.

[setConfigUseNonVisibleColumns(useNonVisibleColumns)](api-svytoolbarfilter.md#setconfigusenonvisiblecolumns-usenonvisiblecolumns)

Use only visible columns of the grid when set to false

[setPopupDefaultOperator(formType, operator)](api-svytoolbarfilter.md#setpopupdefaultoperator-formtype-operator)

[setPopupRendererForm(formType, form)](api-svytoolbarfilter.md#setpopuprendererform-formtype-form)

### ListComponentFilterRenderer ⇐ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

**Extends**: [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

* [ListComponentFilterRenderer](api-svytoolbarfilter.md#listcomponentfilterrenderer-abstracttoolbarfilterux) ⇐ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)
  * [.addFilter(titleText, dataProvider, filterType)](api-svytoolbarfilter.md#listcomponentfilterrenderer.addfilter-titletext-dataprovider-filtertype-filter) ⇒ [`Filter`](api-svytoolbarfilter.md#new\_Filter\_new)
  * [.applyFilters()](api-svytoolbarfilter.md#listcomponentfilterrenderer.applyfilters-boolean) ⇒ `Boolean`
  * [.clearFilterUI()](api-svytoolbarfilter.md#listcomponentfilterrenderer.clearfilterui-boolean) ⇒ `Boolean`
  * [.executeSearch(\[searchText\])](api-svytoolbarfilter.md#listcomponentfilterrenderer.executesearch-searchtext)
  * [.getActiveFilters()](api-svytoolbarfilter.md#listcomponentfilterrenderer.getactivefilters-array-.less-than-scopes.svypopupfilter.abstractpopupfil) ⇒ `[ 'Array' ].<scopes.svyPopupFilter.AbstractPopupFilter>`
  * [.getDataSource()](api-svytoolbarfilter.md#listcomponentfilterrenderer.getdatasource-string) ⇒ `String`
  * [.getDefaultSearch()](api-svytoolbarfilter.md#listcomponentfilterrenderer.getdefaultsearch-scopes.svysearch.simplesearch) ⇒ `scopes.svySearch.SimpleSearch`
  * [.getElement()](api-svytoolbarfilter.md#listcomponentfilterrenderer.getelement-runtimecomponent) ⇒ `RuntimeComponent`
  * [.getFilter(dataprovider)](api-svytoolbarfilter.md#listcomponentfilterrenderer.getfilter-dataprovider-filter) ⇒ [`Filter`](api-svytoolbarfilter.md#new\_Filter\_new)
  * [.getFilters()](api-svytoolbarfilter.md#listcomponentfilterrenderer.getfilters-array-.less-than-filter-greater-than) ⇒ [`[ 'Array' ].<Filter>`](api-svytoolbarfilter.md#new\_Filter\_new)
  * [.getFoundSet()](api-svytoolbarfilter.md#listcomponentfilterrenderer.getfoundset-jsfoundset) ⇒ `JSFoundSet`
  * [.getQuery()](api-svytoolbarfilter.md#listcomponentfilterrenderer.getquery-qbselect) ⇒ `QBSelect`
  * [.getSearchProvider(columnOrDataProvider)](api-svytoolbarfilter.md#listcomponentfilterrenderer.getsearchprovider-columnordataprovider-scopes.svysearch.searchprovider) ⇒ `scopes.svySearch.SearchProvider`
  * [.getSearchText()](api-svytoolbarfilter.md#listcomponentfilterrenderer.getsearchtext-string) ⇒ `String`
  * [.getSimpleSearch()](api-svytoolbarfilter.md#listcomponentfilterrenderer.getsimplesearch-scopes.svysearch.simplesearch) ⇒ `scopes.svySearch.SimpleSearch`
  * [.getToolbarFiltersState()](api-svytoolbarfilter.md#listcomponentfilterrenderer.gettoolbarfiltersstate-array-.less-than-id-string-dataprovider-string-op) ⇒ `[ 'Array' ].<{id: String, dataprovider: String, operator: String, params: Object, text: String, values: Array}>`
  * [.hasFilters()](api-svytoolbarfilter.md#listcomponentfilterrenderer.hasfilters-boolean) ⇒ `Boolean`
  * [.onClick(entry, index, dataTarget, event)](api-svytoolbarfilter.md#listcomponentfilterrenderer.onclick-entry-index-datatarget-event)
  * [.removeFilter(filter)](api-svytoolbarfilter.md#listcomponentfilterrenderer.removefilter-filter)
  * [.restoreToolbarFiltersState(jsonState)](api-svytoolbarfilter.md#listcomponentfilterrenderer.restoretoolbarfiltersstate-jsonstate)
  * [.search(\[searchText\])](api-svytoolbarfilter.md#listcomponentfilterrenderer.search-searchtext)
  * [.setAutoApplyFilters(autoApply)](api-svytoolbarfilter.md#listcomponentfilterrenderer.setautoapplyfilters-autoapply-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)
  * [.setFilterValue(filter, values, operator)](api-svytoolbarfilter.md#listcomponentfilterrenderer.setfiltervalue-filter-values-operator)
  * [.setOnFilterAddedCallback(callback)](api-svytoolbarfilter.md#listcomponentfilterrenderer.setonfilteraddedcallback-callback-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)
  * [.setOnFilterApplyCallback(callback)](api-svytoolbarfilter.md#listcomponentfilterrenderer.setonfilterapplycallback-callback-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)
  * [.setOnFilterApplyQueryCondition(callback)](api-svytoolbarfilter.md#listcomponentfilterrenderer.setonfilterapplyquerycondition-callback-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)
  * [.setOnFilterCreate(callback)](api-svytoolbarfilter.md#listcomponentfilterrenderer.setonfiltercreate-callback-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)
  * [.setOnFilterRemovedCallback(callback)](api-svytoolbarfilter.md#listcomponentfilterrenderer.setonfilterremovedcallback-callback-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)
  * [.setOnSearchCommand(callback)](api-svytoolbarfilter.md#listcomponentfilterrenderer.setonsearchcommand-callback-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)
  * [.setSearchText()](api-svytoolbarfilter.md#listcomponentfilterrenderer.setsearchtext-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)
  * [.showPopupFilterPicker(target)](api-svytoolbarfilter.md#listcomponentfilterrenderer.showpopupfilterpicker-target)
  * [.autoApply](api-svytoolbarfilter.md#listcomponentfilterrenderer.autoapply-boolean) : `Boolean`
  * [.filters](api-svytoolbarfilter.md#listcomponentfilterrenderer.filters-array-.less-than-filter-greater-than) : [`[ 'Array' ].<Filter>`](api-svytoolbarfilter.md#new\_Filter\_new)
  * [new ListComponentFilterRenderer(listComponent, \[foundsetToFilter\])](api-svytoolbarfilter.md#new-listcomponentfilterrenderer-listcomponent-foundsettofilter)

***

#### listComponentFilterRenderer.addFilter(titleText, dataProvider, filterType) ⇒ [`Filter`](api-svytoolbarfilter.md#new\_Filter\_new)

| Param        | Type     | Description                          |
| ------------ | -------- | ------------------------------------ |
| titleText    | `String` |                                      |
| dataProvider | `String` |                                      |
| filterType   | `String` | any of the FILTER\_TYPES enum values |

***

#### listComponentFilterRenderer.applyFilters() ⇒ `Boolean`

Applies all filters

**Returns**: `Boolean` - true if records are loaded, false otherwise

***

#### listComponentFilterRenderer.clearFilterUI() ⇒ `Boolean`

Clears all filters from the UI and fires the onFilterRemovedEvent

***

#### listComponentFilterRenderer.executeSearch(\[searchText])

Executes the search

| Param         | Type     | Description                                                                                                                           |
| ------------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| \[searchText] | `String` | optional searchText to search for; if not provided here, call setSearchText() to set the search criteria before performing the search |

***

#### listComponentFilterRenderer.getActiveFilters() ⇒ `[ 'Array' ].<scopes.svyPopupFilter.AbstractPopupFilter>`

***

#### listComponentFilterRenderer.getDataSource() ⇒ `String`

Returns the datasource to be filtered as the datasource of the form the filter UI Component is on

This method can be overwritten by subclasses to return for example the datasource of an NG Grid

***

#### listComponentFilterRenderer.getDefaultSearch() ⇒ `scopes.svySearch.SimpleSearch`

***

#### listComponentFilterRenderer.getElement() ⇒ `RuntimeComponent`

Returns the element used to display the filters

**Overrides**: [`getElement`](api-svytoolbarfilter.md#AbstractToolbarFilterUX+getElement)

***

#### listComponentFilterRenderer.getFilter(dataprovider) ⇒ [`Filter`](api-svytoolbarfilter.md#new\_Filter\_new)

Returns the Filter for the given dataprovider

| Param        | Type     |
| ------------ | -------- |
| dataprovider | `String` |

***

#### listComponentFilterRenderer.getFilters() ⇒ [`[ 'Array' ].<Filter>`](api-svytoolbarfilter.md#new\_Filter\_new)

***

#### listComponentFilterRenderer.getFoundSet() ⇒ `JSFoundSet`

Returns the foundset to be filtered as the foundset of the form the filter UI Component is on

This method can be overwritten by subclasses to return for example the foundset of an NG Grid

***

#### listComponentFilterRenderer.getQuery() ⇒ `QBSelect`

Applies all filters and returns the query for this toolbar

***

#### listComponentFilterRenderer.getSearchProvider(columnOrDataProvider) ⇒ `scopes.svySearch.SearchProvider`

Returns the SearchProvider for the given column or dataprovider

| Param                | Type                                                   |
| -------------------- | ------------------------------------------------------ |
| columnOrDataProvider | `CustomType.<aggrid-groupingtable.column>` \| `String` |

***

#### listComponentFilterRenderer.getSearchText() ⇒ `String`

Returns the search text for the simple search

***

#### listComponentFilterRenderer.getSimpleSearch() ⇒ `scopes.svySearch.SimpleSearch`

Returns the SimpleSearch

***

#### listComponentFilterRenderer.getToolbarFiltersState() ⇒ `[ 'Array' ].<{id: String, dataprovider: String, operator: String, params: Object, text: String, values: Array}>`

Returns the filters' state of the toolbar

**Returns**: `[ 'Array' ].<{id: String, dataprovider: String, operator: String, params: Object, text: String, values: Array}>` - jsonState

***

#### listComponentFilterRenderer.hasFilters() ⇒ `Boolean`

Returns true if the toolbar has any dataprovider it can filter on

***

#### listComponentFilterRenderer.onClick(entry, index, dataTarget, event)

Called when the mouse is clicked on a list entry.

| Param      | Type      |
| ---------- | --------- |
| entry      | `object`  |
| index      | `Number`  |
| dataTarget | `string`  |
| event      | `JSEvent` |

***

#### listComponentFilterRenderer.removeFilter(filter)

Removes the given filter

| Param  | Type                                                 |
| ------ | ---------------------------------------------------- |
| filter | [`Filter`](api-svytoolbarfilter.md#new\_Filter\_new) |

***

#### listComponentFilterRenderer.restoreToolbarFiltersState(jsonState)

Restores the filters' state

| Param     | Type                                                                                                              |
| --------- | ----------------------------------------------------------------------------------------------------------------- |
| jsonState | `[ 'Array' ].<{id: String, dataprovider: String, operator: String, params: Object, text: String, values: Array}>` |

***

#### listComponentFilterRenderer.search(\[searchText])

Applies all filters and executes the search

| Param         | Type     | Description                                                                                                                           |
| ------------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| \[searchText] | `String` | optional searchText to search for; if not provided here, call setSearchText() to set the search criteria before performing the search |

***

#### listComponentFilterRenderer.setAutoApplyFilters(autoApply) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

| Param     | Type      |
| --------- | --------- |
| autoApply | `Boolean` |

***

#### listComponentFilterRenderer.setFilterValue(filter, values, operator)

Sets a filter value for the given filter

| Param    | Type                                                 |
| -------- | ---------------------------------------------------- |
| filter   | [`Filter`](api-svytoolbarfilter.md#new\_Filter\_new) |
| values   | `Array`                                              |
| operator | `String`                                             |

***

#### listComponentFilterRenderer.setOnFilterAddedCallback(callback) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

Sets a callback method that is fired whenever a filter has been added

The callback method receives the Filter object of the filter added as argument

| Param    | Type       |
| -------- | ---------- |
| callback | `function` |

***

#### listComponentFilterRenderer.setOnFilterApplyCallback(callback) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

Sets a callback method that is fired whenever the filter is applied\
The callback method receives an array of values, the operator and the filter as arguments

| Param    | Type       |
| -------- | ---------- |
| callback | `function` |

***

#### listComponentFilterRenderer.setOnFilterApplyQueryCondition(callback) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

Sets a callback method that is fired whenever a query for a given filter is applied

This can be used to either modify the filter before the query is created or to enhance the provided QBSelect yourself

To prevent the filter from adding criteria to the query as it would normally do, the method being called can return `false`

The method called receives these parameters

* `@param {QBSelect} qbSelect the query to enhance`\
  `@param {String} dataprovider the column/dataprovider of this filter`\
  `@param {String} operator the operator used`\
  `@param {Array} values the filter's values`\
  `@param {scopes.svyPopupFilter.AbstractPopupFilter} filter the filter object`

| Param    | Type       |
| -------- | ---------- |
| callback | `function` |

***

#### listComponentFilterRenderer.setOnFilterCreate(callback) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

Allows to provide a method that will be called when the filter UI for a specific dataprovider is created\
That method then can create and return any filter that will then be used for this column

| Param    | Type       | Description                                                                                                      |
| -------- | ---------- | ---------------------------------------------------------------------------------------------------------------- |
| callback | `function` | function that receives the Filter object as argument and must return a scopes.svyPopupFilter.AbstractPopupFilter |

***

#### listComponentFilterRenderer.setOnFilterRemovedCallback(callback) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

Sets a callback method that is fired whenever a filter is removed

| Param    | Type       |
| -------- | ---------- |
| callback | `function` |

***

#### listComponentFilterRenderer.setOnSearchCommand(callback) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

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

***

#### listComponentFilterRenderer.setSearchText() ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

Sets the search text for the simple search

***

#### listComponentFilterRenderer.showPopupFilterPicker(target)

Shows the filter picker popup

| Param  | Type               |
| ------ | ------------------ |
| target | `RuntimeComponent` |

***

#### listComponentFilterRenderer.autoApply : `Boolean`

***

#### listComponentFilterRenderer.filters : [`[ 'Array' ].<Filter>`](api-svytoolbarfilter.md#new\_Filter\_new)

***

#### new ListComponentFilterRenderer(listComponent, \[foundsetToFilter])

Filter Toolbar implementation using the custom list from the custom-rendered-components package. This implementation requires a "List Component" element and a foundset to filter. You should create a toolbar filter instance at the onLoad of your form and assign it to a form variable. Make sure to re-direct the onClick event of the "List Component" to the toolbar.onClick(entry, index, dataTarget, event);

| Param               | Type                                                                                                                           |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| listComponent       | `RuntimeWebComponent.<customrenderedcomponents-customlist>` \| `RuntimeWebComponent.<customrenderedcomponents-customlist_abs>` |
| \[foundsetToFilter] | `JSFoundSet`                                                                                                                   |

**Example**

```js
//keep track of toolbarFilter object in a form variable
var toolbarFilter;

//init the toolbarFilter at the onLoad.
function onLoad(event) {
 toolbarFilter = new scopes.svyToolbarFilter.ListComponentFilterRenderer(elements.filterToolbar, foundset)
}

//propagate the onClick event of the "List Component" to the toolbar filter.
function onClick(entry, index, dataTarget, event) {
 toolbarFilter.onClick(entry, index, dataTarget, event);
}

//optionally set a searchText for a cross-field search to further filter the result set
function search() {
 toolbarFilter.setSearchText(searchText);
 toolbarFilter.search();
}
```

***

### NgGridListComponentFilterRenderer ⇐ [`ListComponentFilterRenderer`](api-svytoolbarfilter.md#listcomponentfilterrenderer-abstracttoolbarfilterux)

**Extends**: [`ListComponentFilterRenderer`](api-svytoolbarfilter.md#listcomponentfilterrenderer-abstracttoolbarfilterux)

* [NgGridListComponentFilterRenderer](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer-listcomponentfilterrenderer) ⇐ [`ListComponentFilterRenderer`](api-svytoolbarfilter.md#listcomponentfilterrenderer-abstracttoolbarfilterux)
  * [.addFilter(titleText, dataProvider, filterType)](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.addfilter-titletext-dataprovider-filtertype-filter) ⇒ [`Filter`](api-svytoolbarfilter.md#new\_Filter\_new)
  * [.applyFilters()](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.applyfilters-boolean) ⇒ `Boolean`
  * [.clearFilterUI()](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.clearfilterui-boolean) ⇒ `Boolean`
  * [.executeSearch(\[searchText\])](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.executesearch-searchtext)
  * [.getActiveFilters()](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.getactivefilters-array-.less-than-scopes.svypopupfilter.abstractpo) ⇒ `[ 'Array' ].<scopes.svyPopupFilter.AbstractPopupFilter>`
  * [.getDataSource()](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.getdatasource-string) ⇒ `String`
  * [.getDefaultSearch()](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.getdefaultsearch-scopes.svysearch.simplesearch) ⇒ `scopes.svySearch.SimpleSearch`
  * [.getElement()](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.getelement-runtimecomponent) ⇒ `RuntimeComponent`
  * [.getFilter(dataprovider)](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.getfilter-dataprovider-filter) ⇒ [`Filter`](api-svytoolbarfilter.md#new\_Filter\_new)
  * [.getFilters()](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.getfilters-array-.less-than-filter-greater-than) ⇒ [`[ 'Array' ].<Filter>`](api-svytoolbarfilter.md#new\_Filter\_new)
    * [\~filters](api-svytoolbarfilter.md#getfilters-filters)
  * [.getFoundSet()](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.getfoundset-jsfoundset) ⇒ `JSFoundSet`
  * [.getQuery()](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.getquery-qbselect) ⇒ `QBSelect`
  * [.getSearchProvider(columnOrDataProvider)](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.getsearchprovider-columnordataprovider-scopes.svysearch.searchprov) ⇒ `scopes.svySearch.SearchProvider`
  * [.getSearchText()](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.getsearchtext-string) ⇒ `String`
  * [.getSimpleSearch()](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.getsimplesearch-scopes.svysearch.simplesearch) ⇒ `scopes.svySearch.SimpleSearch`
  * [.getToolbarFiltersState()](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.gettoolbarfiltersstate-array-.less-than-id-string-dataprovider-str) ⇒ `[ 'Array' ].<{id: String, dataprovider: String, operator: String, params: Object, text: String, values: Array}>`
  * [.hasFilters()](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.hasfilters-boolean) ⇒ `Boolean`
  * [.onClick(entry, index, dataTarget, event)](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.onclick-entry-index-datatarget-event)
  * [.removeFilter(filter)](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.removefilter-filter)
  * [.restoreToolbarFiltersState(jsonState)](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.restoretoolbarfiltersstate-jsonstate)
  * [.search(\[searchText\])](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.search-searchtext)
  * [.setAutoApplyFilters(autoApply)](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.setautoapplyfilters-autoapply-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)
  * [.setFilterValue(filter, values, operator)](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.setfiltervalue-filter-values-operator)
  * [.setOnFilterAddedCallback(callback)](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.setonfilteraddedcallback-callback-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)
  * [.setOnFilterApplyCallback(callback)](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.setonfilterapplycallback-callback-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)
  * [.setOnFilterApplyQueryCondition(callback)](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.setonfilterapplyquerycondition-callback-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)
  * [.setOnFilterCreate(callback)](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.setonfiltercreate-callback-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)
  * [.setOnFilterRemovedCallback(callback)](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.setonfilterremovedcallback-callback-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)
  * [.setOnSearchCommand(callback)](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.setonsearchcommand-callback-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)
  * [.setSearchText()](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.setsearchtext-abstracttoolbarfilterux) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)
  * [.showPopupFilterPicker(target)](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.showpopupfilterpicker-target)
  * [.autoApply](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer.autoapply-boolean) : `Boolean`
  * [new NgGridListComponentFilterRenderer(listComponent, tableComponent)](api-svytoolbarfilter.md#new-nggridlistcomponentfilterrenderer-listcomponent-tablecomponent)

***

#### ngGridListComponentFilterRenderer.addFilter(titleText, dataProvider, filterType) ⇒ [`Filter`](api-svytoolbarfilter.md#new\_Filter\_new)

| Param        | Type     | Description                          |
| ------------ | -------- | ------------------------------------ |
| titleText    | `String` |                                      |
| dataProvider | `String` |                                      |
| filterType   | `String` | any of the FILTER\_TYPES enum values |

***

#### ngGridListComponentFilterRenderer.applyFilters() ⇒ `Boolean`

Applies all filters

**Returns**: `Boolean` - true if records are loaded, false otherwise

***

#### ngGridListComponentFilterRenderer.clearFilterUI() ⇒ `Boolean`

Clears all filters from the UI and fires the onFilterRemovedEvent

***

#### ngGridListComponentFilterRenderer.executeSearch(\[searchText])

Executes the search

| Param         | Type     | Description                                                                                                                           |
| ------------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| \[searchText] | `String` | optional searchText to search for; if not provided here, call setSearchText() to set the search criteria before performing the search |

***

#### ngGridListComponentFilterRenderer.getActiveFilters() ⇒ `[ 'Array' ].<scopes.svyPopupFilter.AbstractPopupFilter>`

***

#### ngGridListComponentFilterRenderer.getDataSource() ⇒ `String`

Returns the datasource to be filtered as the datasource of the NG Grid

**Overrides**: [`getDataSource`](api-svytoolbarfilter.md#listcomponentfilterrenderer.getdatasource-string)

***

#### ngGridListComponentFilterRenderer.getDefaultSearch() ⇒ `scopes.svySearch.SimpleSearch`

***

#### ngGridListComponentFilterRenderer.getElement() ⇒ `RuntimeComponent`

Returns the element used to display the filters

***

#### ngGridListComponentFilterRenderer.getFilter(dataprovider) ⇒ [`Filter`](api-svytoolbarfilter.md#new\_Filter\_new)

Returns the Filter for the given dataprovider

| Param        | Type     |
| ------------ | -------- |
| dataprovider | `String` |

***

#### ngGridListComponentFilterRenderer.getFilters() ⇒ [`[ 'Array' ].<Filter>`](api-svytoolbarfilter.md#new\_Filter\_new)

Returns all filters of this ToolbarFilter

**Overrides**: [`getFilters`](api-svytoolbarfilter.md#listcomponentfilterrenderer.getfilters-array-.less-than-filter-greater-than)

***

#### **getFilters\~filters**

Array

***

#### ngGridListComponentFilterRenderer.getFoundSet() ⇒ `JSFoundSet`

Returns the foundset to be filtered as the foundset of the NG Grid

**Overrides**: [`getFoundSet`](api-svytoolbarfilter.md#listcomponentfilterrenderer.getfoundset-jsfoundset)

***

#### ngGridListComponentFilterRenderer.getQuery() ⇒ `QBSelect`

Applies all filters and returns the query for this toolbar

***

#### ngGridListComponentFilterRenderer.getSearchProvider(columnOrDataProvider) ⇒ `scopes.svySearch.SearchProvider`

Returns the SearchProvider for the given column or dataprovider

| Param                | Type                                                   |
| -------------------- | ------------------------------------------------------ |
| columnOrDataProvider | `CustomType.<aggrid-groupingtable.column>` \| `String` |

***

#### ngGridListComponentFilterRenderer.getSearchText() ⇒ `String`

Returns the search text for the simple search

***

#### ngGridListComponentFilterRenderer.getSimpleSearch() ⇒ `scopes.svySearch.SimpleSearch`

Returns the SimpleSearch

***

#### ngGridListComponentFilterRenderer.getToolbarFiltersState() ⇒ `[ 'Array' ].<{id: String, dataprovider: String, operator: String, params: Object, text: String, values: Array}>`

Returns the filters' state of the toolbar

**Returns**: `[ 'Array' ].<{id: String, dataprovider: String, operator: String, params: Object, text: String, values: Array}>` - jsonState

***

#### ngGridListComponentFilterRenderer.hasFilters() ⇒ `Boolean`

Returns true if the toolbar has any dataprovider it can filter on

***

#### ngGridListComponentFilterRenderer.onClick(entry, index, dataTarget, event)

Called when the mouse is clicked on a list entry.

| Param      | Type      |
| ---------- | --------- |
| entry      | `object`  |
| index      | `Number`  |
| dataTarget | `string`  |
| event      | `JSEvent` |

***

#### ngGridListComponentFilterRenderer.removeFilter(filter)

Removes the given filter

| Param  | Type                                                 |
| ------ | ---------------------------------------------------- |
| filter | [`Filter`](api-svytoolbarfilter.md#new\_Filter\_new) |

***

#### ngGridListComponentFilterRenderer.restoreToolbarFiltersState(jsonState)

Restores the filters' state

| Param     | Type                                                                                                              |
| --------- | ----------------------------------------------------------------------------------------------------------------- |
| jsonState | `[ 'Array' ].<{id: String, dataprovider: String, operator: String, params: Object, text: String, values: Array}>` |

***

#### ngGridListComponentFilterRenderer.search(\[searchText])

Applies all filters and executes the search

| Param         | Type     | Description                                                                                                                           |
| ------------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| \[searchText] | `String` | optional searchText to search for; if not provided here, call setSearchText() to set the search criteria before performing the search |

***

#### ngGridListComponentFilterRenderer.setAutoApplyFilters(autoApply) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

| Param     | Type      |
| --------- | --------- |
| autoApply | `Boolean` |

***

#### ngGridListComponentFilterRenderer.setFilterValue(filter, values, operator)

Sets a filter value for the given filter

| Param    | Type                                                 |
| -------- | ---------------------------------------------------- |
| filter   | [`Filter`](api-svytoolbarfilter.md#new\_Filter\_new) |
| values   | `Array`                                              |
| operator | `String`                                             |

***

#### ngGridListComponentFilterRenderer.setOnFilterAddedCallback(callback) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

Sets a callback method that is fired whenever a filter has been added

The callback method receives the Filter object of the filter added as argument

| Param    | Type       |
| -------- | ---------- |
| callback | `function` |

***

#### ngGridListComponentFilterRenderer.setOnFilterApplyCallback(callback) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

Sets a callback method that is fired whenever the filter is applied\
The callback method receives an array of values, the operator and the filter as arguments

| Param    | Type       |
| -------- | ---------- |
| callback | `function` |

***

#### ngGridListComponentFilterRenderer.setOnFilterApplyQueryCondition(callback) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

Sets a callback method that is fired whenever a query for a given filter is applied

This can be used to either modify the filter before the query is created or to enhance the provided QBSelect yourself

To prevent the filter from adding criteria to the query as it would normally do, the method being called can return `false`

The method called receives these parameters

* `@param {QBSelect} qbSelect the query to enhance`\
  `@param {String} dataprovider the column/dataprovider of this filter`\
  `@param {String} operator the operator used`\
  `@param {Array} values the filter's values`\
  `@param {scopes.svyPopupFilter.AbstractPopupFilter} filter the filter object`

| Param    | Type       |
| -------- | ---------- |
| callback | `function` |

***

#### ngGridListComponentFilterRenderer.setOnFilterCreate(callback) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

Allows to provide a method that will be called when the filter UI for a specific dataprovider is created\
That method then can create and return any filter that will then be used for this column

| Param    | Type       | Description                                                                                                      |
| -------- | ---------- | ---------------------------------------------------------------------------------------------------------------- |
| callback | `function` | function that receives the Filter object as argument and must return a scopes.svyPopupFilter.AbstractPopupFilter |

***

#### ngGridListComponentFilterRenderer.setOnFilterRemovedCallback(callback) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

Sets a callback method that is fired whenever a filter is removed

| Param    | Type       |
| -------- | ---------- |
| callback | `function` |

***

#### ngGridListComponentFilterRenderer.setOnSearchCommand(callback) ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

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

***

#### ngGridListComponentFilterRenderer.setSearchText() ⇒ [`AbstractToolbarFilterUX`](api-svytoolbarfilter.md#new\_AbstractToolbarFilterUX\_new)

Sets the search text for the simple search

***

#### ngGridListComponentFilterRenderer.showPopupFilterPicker(target)

Shows the filter picker popup

| Param  | Type               |
| ------ | ------------------ |
| target | `RuntimeComponent` |

***

#### ngGridListComponentFilterRenderer.autoApply : `Boolean`

***

#### new NgGridListComponentFilterRenderer(listComponent, tableComponent)

| Param          | Type                                                                                                                           |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| listComponent  | `RuntimeWebComponent.<customrenderedcomponents-customlist>` \| `RuntimeWebComponent.<customrenderedcomponents-customlist_abs>` |
| tableComponent | `RuntimeWebComponent.<aggrid-groupingtable>` \| `RuntimeWebComponent.<aggrid-groupingtable_abs>`                               |

***

### createFilterToolbar(listComponent, tableOrFoundSet) ⇒ [`NgGridListComponentFilterRenderer`](api-svytoolbarfilter.md#nggridlistcomponentfilterrenderer-listcomponentfilterrenderer)

Creates a filter toolbar implementation using the custom list from the custom-rendered-components package.\\

This implementation expects an NG "Data Grid" table component and a "Custom List" component.\\

The filters offered from this implementation are generated from the table provided as follows:

* any column with its `filterType` property set to TEXT will be offered as a token popup, allowing the user to enter any number of Strings to match
* any column with its `filterType` property set to TEXT and the `valuelist` will be offered as a lookup where the user can search for and select any number of values
* any column with its `filterType` property set to NUMBER will be offered as a number filter with a number of operators
* any column with its `filterType` property set to DATE will be offered as a date filter with a number of operators

You should create a toolbar filter instance at the onLoad of your form and assign it to a form variable.

Make sure to re-direct the onClick event of the "List Component" to the toolbar.onClick(entry, index, dataTarget, event);

| Param           | Type                                                                                                                           |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| listComponent   | `RuntimeWebComponent.<customrenderedcomponents-customlist>` \| `RuntimeWebComponent.<customrenderedcomponents-customlist_abs>` |
| tableOrFoundSet | `RuntimeWebComponent.<aggrid-groupingtable>` \| `RuntimeWebComponent.<aggrid-groupingtable_abs>`                               |

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

***

### createSimpleFilterToolbar(listComponent, \[foundsetToFilter]) ⇒ [`ListComponentFilterRenderer`](api-svytoolbarfilter.md#listcomponentfilterrenderer-abstracttoolbarfilterux)

Creates a filter toolbar implementation using the custom list from the custom-rendered-components package.\\

This implementation expects a "Custom List" component. An optional foundset to be filtered can be provided. If not given, the foundset of the form of the given list component is used.\\

Filters to be offered need to be added via the API method `addFilter(titleText, dataProvider, filterType)`.\\

You should create a toolbar filter instance at the onLoad of your form and assign it to a form variable.\\

Make sure to re-direct the onClick event of the "List Component" to the toolbar.onClick(entry, index, dataTarget, event);

| Param               | Type                                                                                                                           | Description                                                                                                                  |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------- |
| listComponent       | `RuntimeWebComponent.<customrenderedcomponents-customlist>` \| `RuntimeWebComponent.<customrenderedcomponents-customlist_abs>` | the component to render the filter                                                                                           |
| \[foundsetToFilter] | `JSFoundSet`                                                                                                                   | optional foundset to filter; if not provided, the foundset of the form containing the listComponent element will be filtered |

**Example**

```js
//keep track of toolbarFilter object in a form variable
var toolbarFilter;

//init the toolbarFilter at the onLoad.
function onLoad(event) {
 	toolbarFilter = scopes.svyToolbarFilter.createSimpleFilterToolbar(elements.filters);
 
 	var filter = toolbarFilter.addFilter('Customer', 'customerid', scopes.svyToolbarFilter.FILTER_TYPES.SELECT);
 	filter.setValueList('vlPopupCustomers');
 
		toolbarFilter.addFilter('City', 'shipcity', scopes.svyToolbarFilter.FILTER_TYPES.TOKEN);
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

***

### getConfigSortPickerAlphabetically() ⇒ `Boolean`

Returns true if the filter picker is sorted alphabetically

**Since**: v1.3.0

***

### setConfigDateDisplayFormat(displayFormat)

Sets global display date format to be used

| Param         | Type     |
| ------------- | -------- |
| displayFormat | `String` |

***

### setConfigSortPickerAlphabetically(sortAlphabetically)

Sort the the filter picker alphabetically. Default sort is based on column's position in grid.

**Since**: v1.3.0

| Param              | Type      | Description    |
| ------------------ | --------- | -------------- |
| sortAlphabetically | `Boolean` | Default false. |

***

### setConfigUseNonVisibleColumns(useNonVisibleColumns)

Use only visible columns of the grid when set to false

**Since**: v1.1.0

| Param                | Type      | Description   |
| -------------------- | --------- | ------------- |
| useNonVisibleColumns | `Boolean` | Default true. |

***

### setPopupDefaultOperator(formType, operator)

**Since**: v1.1.0

| Param    | Type     | Description                                                                           |
| -------- | -------- | ------------------------------------------------------------------------------------- |
| formType | `String` | any of the FILTER\_TYPES                                                              |
| operator | `String` | the default operator to be used. Use enum value from scopes.svyToolbarFilter.OPERATOR |

**Example**

```js
 // change default operator for TEXT token filters.
 scopes.svyToolbarFilter.setPopupDefaultOperator(scopes.svyToolbarFilter.FILTER_TYPES.TOKEN, scopes.svyPopupFilter.OPERATOR.LIKE);
```

***

### setPopupRendererForm(formType, form)

| Param    | Type                                                                  | Description              |
| -------- | --------------------------------------------------------------------- | ------------------------ |
| formType | `String`                                                              | any of the FILTER\_TYPES |
| form     | `RuntimeForm.<AbstractPopupFilter>` \| `RuntimeForm.<AbstractLookup>` | the form to set          |

***

### FILTER\_TYPES

* [FILTER\_TYPES](api-svytoolbarfilter.md#FILTER\_TYPES)
  * [.CHECK](api-svytoolbarfilter.md#filter\_types.check)
  * [.DATE](api-svytoolbarfilter.md#filter\_types.date)
  * [.INTEGER](api-svytoolbarfilter.md#filter\_types.integer)
  * [.NUMBER](api-svytoolbarfilter.md#filter\_types.number)
  * [.SELECT](api-svytoolbarfilter.md#filter\_types.select)
  * [.TOKEN](api-svytoolbarfilter.md#filter\_types.token)

***

#### FILTER\_TYPES.CHECK

Check filter

***

#### FILTER\_TYPES.DATE

Date filter

***

#### FILTER\_TYPES.INTEGER

INTEGER filter

***

#### FILTER\_TYPES.NUMBER

Number filter

***

#### FILTER\_TYPES.SELECT

Select filter

***

#### FILTER\_TYPES.TOKEN

Tokens filter

***
