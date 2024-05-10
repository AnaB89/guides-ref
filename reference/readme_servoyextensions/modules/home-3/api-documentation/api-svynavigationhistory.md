# API svyNavigationHistory

### Functions

[back()](api-svynavigationhistory.md#back-scopes.svynavigation.navigationitem) ⇒ `scopes.svyNavigation.NavigationItem`

Goes back one step in the navigation history from the current position

[clearHistory()](api-svynavigationhistory.md#clearhistory)

Clears the history

[getHistory()](api-svynavigationhistory.md#gethistory-array-.less-than-scopes.svynavigation.navigationitem-greater-than) ⇒ `[ 'Array' ].<scopes.svyNavigation.NavigationItem>`

Returns the history of navigation items

[getHistoryIndex()](api-svynavigationhistory.md#gethistoryindex-number) ⇒ `Number`

Returns the current index when navigating through the history or -1, when not navigating

[getNavigationItemFromHistory(id)](api-svynavigationhistory.md#getnavigationitemfromhistory-id-scopes.svynavigation.navigationitem) ⇒ `scopes.svyNavigation.NavigationItem`

Returns the item with the given ID from the history stack when found and null otherwise

[hasNext()](api-svynavigationhistory.md#hasnext-boolean) ⇒ `Boolean`

Returns `true` when a historyNext can be performed

[hasPrevious()](api-svynavigationhistory.md#hasprevious-boolean) ⇒ `Boolean`

Returns `true` when a historyBack can be performed

[next()](api-svynavigationhistory.md#next-scopes.svynavigation.navigationitem) ⇒ `scopes.svyNavigation.NavigationItem`

Goes forward one step in the navigation history from the current position

[removeItemFromHistory(itemToRemove)](api-svynavigationhistory.md#removeitemfromhistory-itemtoremove)

[setMaxHistoryLength(historyLength)](api-svynavigationhistory.md#setmaxhistorylength-historylength)

Sets the maximum number of items held in the navigation history A maximum number of -1 means there is no limit to the number of items in the history

### back() ⇒ `scopes.svyNavigation.NavigationItem`

Goes back one step in the navigation history from the current position

***

### clearHistory()

Clears the history

***

### getHistory() ⇒ `[ 'Array' ].<scopes.svyNavigation.NavigationItem>`

Returns the history of navigation items

***

### getHistoryIndex() ⇒ `Number`

Returns the current index when navigating through the history or -1, when not navigating

***

### getNavigationItemFromHistory(id) ⇒ `scopes.svyNavigation.NavigationItem`

Returns the item with the given ID from the history stack when found and null otherwise

| Param | Type     |
| ----- | -------- |
| id    | `String` |

***

### hasNext() ⇒ `Boolean`

Returns `true` when a historyNext can be performed

***

### hasPrevious() ⇒ `Boolean`

Returns `true` when a historyBack can be performed

***

### next() ⇒ `scopes.svyNavigation.NavigationItem`

Goes forward one step in the navigation history from the current position

***

### removeItemFromHistory(itemToRemove)

| Param        | Type                                  |
| ------------ | ------------------------------------- |
| itemToRemove | `scopes.svyNavigation.NavigationItem` |

***

### setMaxHistoryLength(historyLength)

Sets the maximum number of items held in the navigation history A maximum number of -1 means there is no limit to the number of items in the history

| Param         | Type     |
| ------------- | -------- |
| historyLength | `Number` |

***
