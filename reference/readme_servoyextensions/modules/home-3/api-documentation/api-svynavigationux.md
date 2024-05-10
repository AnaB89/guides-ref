# API svyNavigationUX

### Functions

[addGlobalSearchListener(listener)](api-svynavigationux.md#addglobalsearchlistener-listener)

[getVersion()](api-svynavigationux.md#getversion-string) ⇒ `String`

Gets the version of this module

[removeGlobalSearchListener(listener)](api-svynavigationux.md#removeglobalsearchlistener-listener)

[triggerGlobalSearch(searchText)](api-svynavigationux.md#triggerglobalsearch-searchtext)

### addGlobalSearchListener(listener)

| Param    | Type       |
| -------- | ---------- |
| listener | `function` |

**Example**

```js
function onShow(firstShow, event) {
	// listen for a global search event
	scopes.svyNavigationUX.addGlobalSearchListener(globalSearchListener);
}

function globalSearchListener(searchText) {
	// perform a search
}

function onHide(event) {
	// stop listening when hiding the form
	scopes.svyNavigationUX.removeGlobalSearchListener(globalSearchListener)
	return true
}
```

***

### getVersion() ⇒ `String`

Gets the version of this module

**Returns**: `String` - the version of the module using the format Major.Minor.Revision

***

### removeGlobalSearchListener(listener)

| Param    | Type       |
| -------- | ---------- |
| listener | `function` |

**Example**

```js
function onShow(firstShow, event) {
	// listen for a global search event
	scopes.svyNavigationUX.addGlobalSearchListener(globalSearchListener);
}

function globalSearchListener(searchText) {
	// perform a search
}

function onHide(event) {
	// stop listening when hiding the form
	scopes.svyNavigationUX.removeGlobalSearchListener(globalSearchListener)
	return true
}
```

***

### triggerGlobalSearch(searchText)

| Param      | Type     |
| ---------- | -------- |
| searchText | `String` |

***
