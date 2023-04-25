# API svyNavigationHistory

### Functions

[back()](API-svyNavigationHistory.md#back-scopes.svynavigation.navigationitem) ⇒ `scopes.svyNavigation.NavigationItem`

Goes back one step in the navigation history from the current position

[clearHistory()](API-svyNavigationHistory.md#clearhistory)

Clears the history

[getHistory()](API-svyNavigationHistory.md#gethistory-array-.less-than-scopes.svynavigation.navigationitem-greater-than) ⇒ `[ 'Array' ].<scopes.svyNavigation.NavigationItem>`

Returns the history of navigation items

[getHistoryIndex()](API-svyNavigationHistory.md#gethistoryindex-number) ⇒ `Number`

Returns the current index when navigating through the history or -1, when not navigating

[getNavigationItemFromHistory(id)](API-svyNavigationHistory.md#getnavigationitemfromhistory-id-scopes.svynavigation.navigationitem) ⇒ `scopes.svyNavigation.NavigationItem`

Returns the item with the given ID from the history stack when found and null otherwise

[hasNext()](API-svyNavigationHistory.md#hasnext-boolean) ⇒ `Boolean`

Returns `true` when a historyNext can be performed

[hasPrevious()](API-svyNavigationHistory.md#hasprevious-boolean) ⇒ `Boolean`

Returns `true` when a historyBack can be performed

[next()](API-svyNavigationHistory.md#next-scopes.svynavigation.navigationitem) ⇒ `scopes.svyNavigation.NavigationItem`

Goes forward one step in the navigation history from the current position

[removeItemFromHistory(itemToRemove)](API-svyNavigationHistory.md#removeitemfromhistory-itemtoremove)

[setMaxHistoryLength(historyLength)](API-svyNavigationHistory.md#setmaxhistorylength-historylength)

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
