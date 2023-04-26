# API svyNavigation

### Classes

[NavigationItem](api-svynavigation.md#NavigationItem)

### Functions

[addNavigationListener(listener)](api-svynavigation.md#addNavigationListener)

[createNavigationItem(\[formName\], \[text\], \[tooltipText\])](api-svynavigation.md#createNavigationItem) ⇒ [`NavigationItem`](api-svynavigation.md#NavigationItem)

Creates a NavigationItem object to the given formName

[getCurrentItem()](api-svynavigation.md#getCurrentItem) ⇒ [`NavigationItem`](api-svynavigation.md#NavigationItem)[getVersion()](api-svynavigation.md#getVersion) ⇒ `String`

Gets the version of this module

[open(itemOrID, \[dataToShow\], \[dataSelectionType\])](api-svynavigation.md#open) ⇒ `Boolean`

Opens the navigation item. If the item already exists in the stack, then all items after the specified item are closed beforeClose event will be fired allowing a chance to react or cancel afterOpen will fire allowing UIs to update

[removeNavigationListener(listener)](api-svynavigation.md#removeNavigationListener) ⇒ `Boolean`

### NavigationItem

* [NavigationItem](api-svynavigation.md#navigationitem)
  * [.getCustomData()](api-svynavigation.md#navigationitem.getcustomdata) ⇒ `*`
  * [.getFormName()](api-svynavigation.md#navigationitem.getformname-string) ⇒ `String`
  * [.getID()](api-svynavigation.md#navigationitem.getid-string) ⇒ `String`
  * [.getText()](api-svynavigation.md#navigationitem.gettext-string) ⇒ `String`
  * [.getTooltipText()](api-svynavigation.md#navigationitem.gettooltiptext-string) ⇒ `String`
  * [.setCustomData(customData)](api-svynavigation.md#navigationitem.setcustomdata-customdata-navigationitem) ⇒ [`NavigationItem`](api-svynavigation.md#navigationitem)
  * [.setFormName(formName)](api-svynavigation.md#navigationitem.setformname-formname-navigationitem) ⇒ [`NavigationItem`](api-svynavigation.md#navigationitem)
  * [.setText(text)](api-svynavigation.md#navigationitem.settext-text-navigationitem) ⇒ [`NavigationItem`](api-svynavigation.md#navigationitem)
  * [.setTooltipText(tooltipText)](api-svynavigation.md#navigationitem.settooltiptext-tooltiptext-navigationitem) ⇒ [`NavigationItem`](api-svynavigation.md#navigationitem)
  * [.stringify()](api-svynavigation.md#navigationitem.stringify)
  * [new NavigationItem(\[formName\], \[text\], \[tooltipText\])](api-svynavigation.md#new-navigationitem-formname-text-tooltiptext)

***

#### navigationItem.getCustomData() ⇒ `*`

**Example**

```js
function onShow() {
  // get the current navigation item
   var item = scopes.svyNavigation.getCurrentItem();
   var customData = item.getCustomData();
   if (customData && customData.filter) {
      var filter = customData.filter;
      foundset.addFoundSetFilterParam(filter.dataprovider, filter.operator, filter.values);
      foundset.loadRecords();
   }
}
```

***

#### navigationItem.getFormName() ⇒ `String`

Gets the name of the form associated with this navigation item.

***

#### navigationItem.getID() ⇒ `String`

***

#### navigationItem.getText() ⇒ `String`

***

#### navigationItem.getTooltipText() ⇒ `String`

***

#### navigationItem.setCustomData(customData) ⇒ [`NavigationItem`](api-svynavigation.md#navigationitem)

| Param      | Type |
| ---------- | ---- |
| customData | `*`  |

**Example**

```js
var item = new scopes.svyNavigation.NavigationItem("ordersTableView");
item.setCustomData({ filter: { dataprovider: "orderdate", operator: "between", values: [startDate, endDate] } });
scopes.svyNavigation.open(item);
```

***

#### navigationItem.setFormName(formName) ⇒ [`NavigationItem`](api-svynavigation.md#navigationitem)

Sets the name of the form associated with this navigation item.

| Param    | Type     |
| -------- | -------- |
| formName | `String` |

***

#### navigationItem.setText(text) ⇒ [`NavigationItem`](api-svynavigation.md#navigationitem)

| Param | Type     |
| ----- | -------- |
| text  | `String` |

***

#### navigationItem.setTooltipText(tooltipText) ⇒ [`NavigationItem`](api-svynavigation.md#navigationitem)

| Param       | Type     |
| ----------- | -------- |
| tooltipText | `String` |

***

#### navigationItem.stringify()

***

#### new NavigationItem(\[formName], \[text], \[tooltipText])

| Param          | Type     |
| -------------- | -------- |
| \[formName]    | `String` |
| \[text]        | `String` |
| \[tooltipText] | `String` |

***

### NAVIGATION\_EVENT

**Properties**

| Name          | Default        | Description                                                                                                                                                                                                           |
| ------------- | -------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BEFORE\_CLOSE | `before-close` | register for navigation event to listen for this event (@see addNavigationListener) beforeClose event will be fired before navigating allowing a chance to react or cancel                                            |
| AFTER\_OPEN   | `after-open`   | register for navigation event to listen for this event (@see addNavigationListener) afterOpen event will be fired when a navigation item has been opened; react to the after\_open event to implement your navigation |

***

### NAVIGATION\_SELECTION\_TYPE

Enumeration for the data selection type specified in the open function. The chosen selection type is passed to the open function \[open]\(@link open) \[afterOpen]\(@link afterOpen) and needs to be implemented accordingly. The Default value is LOAD\_RECORDS

**See**: open(itemOrId, dataToShow, dataSelectionType)\
**Properties**

| Name                  | Default               | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| --------------------- | --------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| LOAD\_RECORDS         | `load-records`        | <p>This is the DEFAULT selection type. Will run foundset.loadRecords(dataToShow) on the form to be shown.<br>Load records into the form's foundset. If you load a relation into this foundset, then this foundset will not be a related foundset, it will not automatically update its state of records are updated or added that belong to that relation. It will only be a snapshot of that related foundsets state. Foundset filter params are copied over from the source foundset and are merged with the existing filters on this foundset.</p>                                                                                                           |
| SET\_FOUNDSET         | `set-foundset`        | <p>Can be used only when the dataToShow is of type JSFoundSet. Will run controller.loadRecords(dataToShow) for the target form.<br>Replace the default form's foundset with setting the (related) foundset into the form. The form will no longer share the default foundset with forms of the same datasource, use loadAllRecords to restore the default foundset. This will really update the foundset instance itself of the form, so now existing foundset is altered just the new foundset is shown. When the form uses a seperate foundset, foundset filter params are copied over from the source foundset and are merged with the existing filters.</p> |
| SELECT\_RECORD        | `select-record`       | Can be used only when the dataToShow is a JSRecord. Selects the record with the given pk in the foundset even if the record is not loaded in foundset yet. Warning: can be very expensive, as the entire foundset may needs to be loaded. Returns false if the record cannot be found in the entire foundset.                                                                                                                                                                                                                                                                                                                                                   |
| FORCE\_SELECT\_RECORD | `force-select-record` | Can be used only when the dataToShow is a JSRecord. Selects the record with the given pk in the foundset even if the record is not loaded in foundset yet. Warning: can be very expensive, as the entire foundset may needs to be loaded. Returns false if the record cannot be found in the entire foundset. If the record is not present in the foundset will force the selection by loading all records into the foundset. If there are active foundset or table filters these won't be removed, they will still apply.                                                                                                                                      |

***

### addNavigationListener(listener)

| Param    | Type       |
| -------- | ---------- |
| listener | `function` |

**Example**

```js
// register for navigation event
scopes.svyNavigation.addNavigationListener(onOpen);

function onOpen(event) {
	var type = event.getEventType();
	if (type == scopes.svyNavigation.NAVIGATION_EVENT.AFTER_OPEN) {
		var item = event.getNavigationItem();
		var formName = item.getFormName();
		var dataToShow = event.getDataToShow();
		var dataSelectionType = event.getDataSelectionType();
		
		// get the form instance
		var form = forms[formName];
		
		switch (dataSelectionType) {
		case scopes.svyNavigation.NAVIGATION_SELECTION_TYPE.LOAD_RECORDS:
		// load the given data into the foundset form
		if (dataToShow instanceof JSFoundSet) {
			// load the passed foundset into the form's foundset
			form.foundset.loadRecords(dataToShow);
		} else if (dataToShow instanceof QBSelect) {
			// load the QBSelect into the form's foundset
			form.foundset.loadRecords(dataToShow);
		} else if (dataToShow instanceof JSRecord) {
			// load the record into the form's foundset
			scopes.svyDataUtils.loadRecords(form.foundset, dataToShow.getPKs());
		}
		break;
		case scopes.svyNavigation.NAVIGATION_SELECTION_TYPE.SET_FOUNDSET:
			form.controller.loadRecords(dataToShow);
			break;
		default:
			break;
		}
		
		// show the form
		application.showForm(form);
	} else if (event.getEventType() == scopes.svyNavigation.NAVIGATION_EVENT.BEFORE_CLOSE) {
     // cancel navigation if there are pending edits to be saved
     if (databaseManager.getEditedRecords().length) {
         return false;   // or ask in a dialog
     }
 }
	return true;
}
```

***

### createNavigationItem(\[formName], \[text], \[tooltipText]) ⇒ [`NavigationItem`](api-svynavigation.md#navigationitem)

Creates a NavigationItem object to the given formName

| Param          | Type     |
| -------------- | -------- |
| \[formName]    | `String` |
| \[text]        | `String` |
| \[tooltipText] | `String` |

***

### getCurrentItem() ⇒ [`NavigationItem`](api-svynavigation.md#navigationitem)

***

### getVersion() ⇒ `String`

Gets the version of this module

**Returns**: `String` - the version of the module using the format Major.Minor.Revision

***

### open(itemOrID, \[dataToShow], \[dataSelectionType]) ⇒ `Boolean`

Opens the navigation item. If the item already exists in the stack, then all items after the specified item are closed beforeClose event will be fired allowing a chance to react or cancel afterOpen will fire allowing UIs to update

| Param                | Type                                                                | Description                                                                                                                                                                                                                                                                                                                                  |
| -------------------- | ------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| itemOrID             | [`NavigationItem`](api-svynavigation.md#navigationitem) \| `String` |                                                                                                                                                                                                                                                                                                                                              |
| \[dataToShow]        | `JSRecord` \| `JSFoundSet` \| `QBSelect`                            | The data to show for the given navigation item. The data is passed to the afterOpen event                                                                                                                                                                                                                                                    |
| \[dataSelectionType] | `String`                                                            | Determine the type of selection in the target navigation item with the given dataToShow [NAVIGATION\_SELECTION\_TYPE](api-svynavigation.md#navigation\_selection\_type) enumeration options. The chosen selection type is passed to the afterOpen and needs to be implemented accordingly. Default NAVIGATION\_SELECTION\_TYPE.LOAD\_RECORDS |

**Example**

```js
//open a form
var item = new scopes.svyNavigation.NavigationItem(formName);
scopes.svyNavigation.open(item);

//open an item and pass data selection
var item = new scopes.svyNavigation.NavigationItem(formName);
scopes.svyNavigation.open(item,foundset.getSelectedRecord(),scopes.svyNavigation.NAVIGATION_SELECTION_TYPE.LOAD_RECORDS);

// open a form and pass custom data
var item = new scopes.svyNavigation.NavigationItem("ordersTableView");
item.setCustomData({ filter: { dataprovider: "orderdate", operator: "between", values: [startDate, endDate] } });
scopes.svyNavigation.open(item);
```

***

### removeNavigationListener(listener) ⇒ `Boolean`

| Param    | Type       |
| -------- | ---------- |
| listener | `function` |

**Example**

```js
scopes.svyNavigation.removeNavigationListener(onOpen);
```

***
