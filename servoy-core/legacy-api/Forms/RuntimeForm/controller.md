#  controller

## **Supported Clients**

    SmartClient
    WebClient
    NGClient
    MobileClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../../JSLib/Boolean.md) | [enabled](controller.md#enabled)                   | Gets or sets the enabled state of a form; also known as "grayed-out"..                                    |
| [Boolean](../../JSLib/Boolean.md) | [readOnly](controller.md#readOnly)                   | Gets or sets the read-only state of a form; also known as "editable"  Note: The field(s) in a form set as read-only can be selected and the field data can be copied to clipboard..                                    |
| [Number](../../JSLib/Number.md) | [view](controller.md#view)                   | Get/Set the current type of view of this form..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../../JSLib/Boolean.md) | [find()](controller.md#find)                   | Set the foundset in find mode..                                    |
| [Boolean](../../JSLib/Boolean.md) | [focusField(fieldName, skipReadonly)](controller.md#focusfield-fieldname-skipreadonly)                   | Sets focus to a field specified by its name..                                    |
| [Boolean](../../JSLib/Boolean.md) | [focusFirstField()](controller.md#focusfirstfield)                   | Sets focus to the first field of the form; based on tab order sequence..                                    |
| [Number](../../JSLib/Number.md) | [getDataProviderMaxLength(name)](controller.md#getdataprovidermaxlength-name)                   | Returns the maximum length allowed in the specified dataprovider..                                    |
| [Object](../../JSLib/Object.md) | [getDataProviderValue(dataProvider)](controller.md#getdataprovidervalue-dataprovider)                   | Gets a value based on the specified dataprovider name..                                    |
| [String](../../JSLib/String.md) | [getDataSource()](controller.md#getdatasource)                   | Get the used datasource..                                    |
| [Boolean](../../JSLib/Boolean.md) | [getDesignMode()](controller.md#getdesignmode)                   | Returns the state of this form designmode..                                    |
| [Object](../../JSLib/Object.md) | [getDesignProperties()](controller.md#getdesignproperties)                   | Get the design-time properties of the form..                                    |
| [Object](../../JSLib/Object.md) | [getDesignTimeProperty(key)](controller.md#getdesigntimeproperty-key)                   | Get a design-time property of a form..                                    |
| [JSDataSet](../../Database%20Manager/JSDataSet.md) | [getFormContext()](controller.md#getformcontext)                   | Gets the forms context where it resides, returns a dataset of its structure to the main controller..                                    |
| [Number](../../JSLib/Number.md) | [getFormWidth()](controller.md#getformwidth)                   | Gets the form width in pixels..                                    |
| [String](../../JSLib/String.md) | [getName()](controller.md#getname)                   | Get the name of this form..                                    |
| [Number](../../JSLib/Number.md) | [getPartHeight(partType)](controller.md#getpartheight-parttype)                   | Gets the part height in pixels..                                    |
| [Number](../../JSLib/Number.md) | [getPartYOffset(partType)](controller.md#getpartyoffset-parttype)                   | Returns the Y offset of a given part of the form..                                    |
| [Number](../../JSLib/Number.md) | [getSelectedIndex()](controller.md#getselectedindex)                   | Gets the current record index of the current foundset..                                    |
| [Array](../../JSLib/Array.md) | [getTabSequence()](controller.md#gettabsequence)                   | Get an array with the names of the components that are part of the tab sequence..                                    |
| [JSWindow](../../Application/JSWindow.md) | [getWindow()](controller.md#getwindow)                   | Returns the JSWindow that the form is shown in, or null if the form is not currently showing in a window..                                    |
| [Boolean](../../JSLib/Boolean.md) | [loadRecords(foundset)](controller.md#loadrecords-foundset)                   | Loads a (related) foundset into the form..                                    |
| [Boolean](../../JSLib/Boolean.md) | [loadRecords(foundset)](controller.md#loadrecords-foundset)                   | Loads a (related) foundset into the form..                                    |
|void | [print()](controller.md#print)                   | Print this form with current foundset, without preview..                                    |
|void | [print(printCurrentRecordOnly)](controller.md#print-printcurrentrecordonly)                   | Print this form with current foundset, without preview..                                    |
|void | [print(printCurrentRecordOnly, showPrinterSelectDialog)](controller.md#print-printcurrentrecordonly-showprinterselectdialog)                   | Print this form with current foundset, without preview..                                    |
|void | [print(printCurrentRecordOnly, showPrinterSelectDialog, printerJob)](controller.md#print-printcurrentrecordonly-showprinterselectdialog-printerjob)                   | Print this form with current foundset, without preview..                                    |
| [String](../../JSLib/String.md) | [printXML()](controller.md#printxml)                   | Print this form with current foundset records to xml format..                                    |
| [String](../../JSLib/String.md) | [printXML(printCurrentRecordOnly)](controller.md#printxml-printcurrentrecordonly)                   | Print this form with current foundset records to xml format..                                    |
| [Boolean](../../JSLib/Boolean.md) | [recreateUI()](controller.md#recreateui)                   | Recreates the forms UI components, to reflect the latest solution model..                                    |
| [Number](../../JSLib/Number.md) | [search()](controller.md#search)                   | Start the database search and use the results, returns the number of records, make sure you did "find" function first..                                    |
| [Number](../../JSLib/Number.md) | [search(clearLastResults)](controller.md#search-clearlastresults)                   | Start the database search and use the results, returns the number of records, make sure you did "find" function first..                                    |
| [Number](../../JSLib/Number.md) | [search(clearLastResults, reduceSearch)](controller.md#search-clearlastresults-reducesearch)                   | Start the database search and use the results, returns the number of records, make sure you did "find" function first..                                    |
|void | [setDataProviderValue(dataprovider, value)](controller.md#setdataprovidervalue-dataprovider-value)                   | Sets the value based on a specified dataprovider name..                                    |
|void | [setDesignMode(designMode)](controller.md#setdesignmode-designmode)                   | Sets this form in designmode with param true, false will return to normal browse/edit mode..                                    |
|void | [setDesignMode(ondrag)](controller.md#setdesignmode-ondrag)                   | Sets this form in designmode with one or more callback methods..                                    |
|void | [setDesignMode(ondrag, ondrop)](controller.md#setdesignmode-ondrag-ondrop)                   | Sets this form in designmode with one or more callback methods..                                    |
|void | [setDesignMode(ondrag, ondrop, onselect)](controller.md#setdesignmode-ondrag-ondrop-onselect)                   | Sets this form in designmode with one or more callback methods..                                    |
|void | [setDesignMode(ondrag, ondrop, onselect, onresize)](controller.md#setdesignmode-ondrag-ondrop-onselect-onresize)                   | Sets this form in designmode with one or more callback methods..                                    |
|void | [setDesignMode(ondrag, ondrop, onselect, onresize, ondblclick)](controller.md#setdesignmode-ondrag-ondrop-onselect-onresize-ondblclick)                   | Sets this form in designmode with one or more callback methods..                                    |
|void | [setDesignMode(ondrag, ondrop, onselect, onresize, ondblclick, onrightclick)](controller.md#setdesignmode-ondrag-ondrop-onselect-onresize-ondblclick-onrightclick)                   | Sets this form in designmode with one or more callback methods..                                    |
|void | [setPageFormat(width, height, leftmargin, rightmargin, topmargin, bottommargin)](controller.md#setpageformat-width-height-leftmargin-rightmargin-topmargin-bottommargin)                   | Set the page format to use when printing..                                    |
|void | [setPageFormat(width, height, leftmargin, rightmargin, topmargin, bottommargin, orientation)](controller.md#setpageformat-width-height-leftmargin-rightmargin-topmargin-bottommargin-orientation)                   | Set the page format to use when printing..                                    |
|void | [setPageFormat(width, height, leftmargin, rightmargin, topmargin, bottommargin, orientation, units)](controller.md#setpageformat-width-height-leftmargin-rightmargin-topmargin-bottommargin-orientation-units)                   | Set the page format to use when printing..                                    |
|void | [setPreferredPrinter(printerName)](controller.md#setpreferredprinter-printername)                   | Set the preferred printer name to use when printing..                                    |
|void | [setSelectedIndex(index)](controller.md#setselectedindex-index)                   | Sets the current record index of the current foundset..                                    |
|void | [setTabSequence(arrayOfElements)](controller.md#settabsequence-arrayofelements)                   | Set the tab order sequence programatically, by passing the elements references in a javascript array..                                    |
|void | [show()](controller.md#show)                   | Shows the form (makes the form visible) This function does not affect the form foundset in any way..                                    |
|void | [show(window)](controller.md#show-window)                   | Shows the form (makes the form visible) This function does not affect the form foundset in any way..                                    |
|void | [show(window)](controller.md#show-window)                   | Shows the form (makes the form visible) This function does not affect the form foundset in any way..                                    |
|void | [showPrintPreview()](controller.md#showprintpreview)                   | Show this form in print preview..                                    |
|void | [showPrintPreview(printCurrentRecordOnly)](controller.md#showprintpreview-printcurrentrecordonly)                   | Show this form in print preview..                                    |
|void | [showPrintPreview(printCurrentRecordOnly, printerJob)](controller.md#showprintpreview-printcurrentrecordonly-printerjob)                   | Show this form in print preview..                                    |
|void | [showPrintPreview(printCurrentRecordOnly, printerJob, zoomFactor)](controller.md#showprintpreview-printcurrentrecordonly-printerjob-zoomfactor)                   | Show this form in print preview..                                    |
|void | [showRecords(foundset)](controller.md#showrecords-foundset)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(foundset, window)](controller.md#showrecords-foundset-window)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(foundset, window)](controller.md#showrecords-foundset-window)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(pkdataset)](controller.md#showrecords-pkdataset)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(pkdataset, window)](controller.md#showrecords-pkdataset-window)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(pkdataset, window)](controller.md#showrecords-pkdataset-window)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(query)](controller.md#showrecords-query)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(query, window)](controller.md#showrecords-query-window)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(query, window)](controller.md#showrecords-query-window)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(UUIDpk)](controller.md#showrecords-uuidpk)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(UUIDpk, window)](controller.md#showrecords-uuidpk-window)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(UUIDpk, window)](controller.md#showrecords-uuidpk-window)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(singleNumber_pk)](controller.md#showrecords-singlenumber_pk)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(singleNumber_pk, window)](controller.md#showrecords-singlenumber_pk-window)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(singleNumber_pk, window)](controller.md#showrecords-singlenumber_pk-window)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(query)](controller.md#showrecords-query)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(query, window)](controller.md#showrecords-query-window)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(query, argumentsArray)](controller.md#showrecords-query-argumentsarray)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(query, argumentsArray, window)](controller.md#showrecords-query-argumentsarray-window)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(query, argumentsArray, window)](controller.md#showrecords-query-argumentsarray-window)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [showRecords(query, window)](controller.md#showrecords-query-window)                   | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                                    |
|void | [sortDialog()](controller.md#sortdialog)                   | Show the sort dialog to the user a preselection sortString can be passed, to sort the form foundset..                                    |
|void | [sortDialog(sortString)](controller.md#sortdialog-sortstring)                   | .                                    |

## Properties Details

### enabled

Gets or sets the enabled state of a form; also known as "grayed-out".

Notes:
-A disabled element(s) cannot be selected by clicking the form.
-The disabled "grayed" color is dependent on the LAF set in the Servoy Smart Client Application Preferences.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
//gets the enabled state of the form
var state = controller.enabled;
//enables the form for input
controller.enabled = true;
```
### readOnly

Gets or sets the read-only state of a form; also known as "editable"

Note: The field(s) in a form set as read-only can be selected and the field data can be copied to clipboard.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//gets the read-only state of the form
var state = controller.readOnly;
//sets the read-only state of the form
controller.readOnly = true
```
### view

Get/Set the current type of view of this form. Can be one of the JSForm.xxxx_VIEW constants.
In NGClient only RECORD_VIEW is fully supported, the List and TableViews should be replaced by components.

**Returns**\
[Number](../../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//gets the type of view for this form
var view = controller.view;
//sets the form to Record view
controller.view = JSForm.RECORD_VIEW;
//sets the form to List view
controller.view = JSForm.LIST_VIEW;
```

## Methods Details

### find()

Set the foundset in find mode. (Start a find request), use the "search" function to perform/exit the find.

Before going into find mode, all unsaved records will be saved in the database.
If this fails (due to validation failures or sql errors) or is not allowed (autosave off), the foundset will not go into find mode.
Make sure the operator and the data (value) are part of the string passed to dataprovider (included inside a pair of quotation marks).
Note: always make sure to check the result of the find() method.

When in find mode, columns can be assigned string expressions (including operators) that are evaluated as:
General:
      c1||c2    (condition1 or condition2)
      c|format  (apply format on condition like 'x|dd-MM-yyyy')
      !c        (not condition)
      #c        (modify condition, depends on column type)
      ^         (is null)
      ^=        (is null or empty)
      &lt;x     (less than value x)
      &gt;x     (greater than value x)
      &lt;=x    (less than or equals value x)
      &gt;=x    (greater than or equals value x)
      x...y     (between values x and y, including values)
      x         (equals value x)

 Number fields:
      =x       (equals value x)
      ^=       (is null or zero)

 Date fields:
      #c       (equals value x, entire day)
      now      (equals now, date and or time)
      //       (equals today)
      today    (equals today)

 Text fields:
      #c	        (case insensitive condition)
      = x      (equals a space and 'x')
      ^=       (is null or empty)
      %x%      (contains 'x')
      %x_y%    (contains 'x' followed by any char and 'y')
      \%      (contains char '%')
      \_      (contains char '_')

Related columns can be assigned, they will result in related searches.
For example, "employees_to_department.location_id = headoffice" finds all employees in the specified location).

Searching on related aggregates is supported.
For example, "orders_to_details.total_amount = '&gt;1000'" finds all orders with total order details amount more than 1000.

Arrays can be used for searching a number of values, this will result in an 'IN' condition that will be used in the search.
The values are not restricted to strings but can be any type that matches the column type.
For example, "record.department_id = [1, 33, 99]"


**Returns**\
[Boolean](../../JSLib/Boolean.md) true if the foundset is now in find mode, false otherwise.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (foundset.find()) //find will fail if autosave is disabled and there are unsaved records
{
	columnTextDataProvider = 'a search value'
	// for numbers you have to make sure to format it correctly so that the decimal point is in your locales notation (. or ,)
	columnNumberDataProvider = '>' + utils.numberFormat(anumber, '####.00');
	columnDateDataProvider = '31-12-2010|dd-MM-yyyy'
	foundset.search()
}
```
### focusField(fieldName, skipReadonly)

Sets focus to a field specified by its name.
If the second parameter is set to true, then readonly fields will be skipped
(the focus will be set to the first non-readonly field located after the field with the specified name; the tab sequence is respected when searching for the non-readonly field).

**Parameters**\
[String](../../JSLib/String.md) fieldName the name of the field to be focussed\
[Boolean](../../JSLib/Boolean.md) skipReadonly indication to skip read only fields, if the named field happens to be read only

**Returns**\
[Boolean](../../JSLib/Boolean.md) true if component was found and can be focused

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var tabseq = controller.getTabSequence();
if (tabseq.length > 1) {
	// If there is more than one field in the tab sequence,
	// focus the second one and skip over readonly fields.
	controller.focusField(tabseq[1], true);
}
else {
	// If there is at most one field in the tab sequence, then focus
	// whatever field is first, and don't bother to skip over readonly fields.
	controller.focusField(null, false);
}
```
### focusFirstField()

Sets focus to the first field of the form; based on tab order sequence.


**Returns**\
[Boolean](../../JSLib/Boolean.md) true if component was found and can be focused

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.focusFirstField();
```
### getDataProviderMaxLength(name)

Returns the maximum length allowed in the specified dataprovider.

**Parameters**\
[String](../../JSLib/String.md) name the dataprovider name

**Returns**\
[Number](../../JSLib/Number.md) the length

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.getDataProviderMaxLength('name');
```
### getDataProviderValue(dataProvider)

Gets a value based on the specified dataprovider name.

**Parameters**\
[String](../../JSLib/String.md) dataProvider the dataprovider name to retieve the value for

**Returns**\
[Object](../../JSLib/Object.md) the dataprovider value (null if unknown dataprovider)

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var val = controller.getDataProviderValue('contact_name');
```
### getDataSource()

Get the used datasource.


**Returns**\
[String](../../JSLib/String.md) the datasource

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var dataSource = controller.getDataSource();
```
### getDesignMode()

Returns the state of this form designmode.


**Returns**\
[Boolean](../../JSLib/Boolean.md) the design mode state (true/fase)

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var success = controller.getDesignMode();
```
### getDesignProperties()

Get the design-time properties of the form.


**Returns**\
[Object](../../JSLib/Object.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var prop = fforms.orders.controller.getDesignProperties()
```
### getDesignTimeProperty(key)

Get a design-time property of a form.

**Parameters**\
[String](../../JSLib/String.md) key the property name

**Returns**\
[Object](../../JSLib/Object.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var prop = forms.orders.controller.getDesignTimeProperty('myprop')
```
### getFormContext()

Gets the forms context where it resides, returns a dataset of its structure to the main controller.
Note1: can't be called in onload, because no context is yet available at this time.
Note2: tabindex is 1 (left) or 2 (right) for a SplitPane and 0 based for the other tabpanels; tabindex1based is the same as tabindex but is 1 based.


**Returns**\
[JSDataSet](../../Database%20Manager/JSDataSet.md) the dataset with form context

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//dataset columns: [containername(1),formname(2),tabpanel or beanname(3),tabname(4),tabindex(5),tabindex1based(6)]
//dataset rows: mainform(1) -> parent(2)  -> current form(3) (when 3 forms deep)
/** @type {JSDataSet} */
var dataset = controller.getFormContext();
if (dataset.getMaxRowIndex() > 1)
{
	// form is in a tabpanel
	var parentFormName = dataset.getValue(1,2)
}
```
### getFormWidth()

Gets the form width in pixels.


**Returns**\
[Number](../../JSLib/Number.md) the width in pixels

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var width = controller.getFormWidth();
```
### getName()

Get the name of this form.


**Returns**\
[String](../../JSLib/String.md) the name

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var formName = controller.getName();
```
### getPartHeight(partType)

Gets the part height in pixels.

**Parameters**\
[Number](../../JSLib/Number.md) partType The type of the part whose height will be returned.

**Returns**\
[Number](../../JSLib/Number.md) the part height in pixels

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var height = controller.getPartHeight(JSPart.BODY);
```
### getPartYOffset(partType)

Returns the Y offset of a given part of the form.

**Parameters**\
[Number](../../JSLib/Number.md) partType The type of the part whose Y offset will be returned.

**Returns**\
[Number](../../JSLib/Number.md) A number holding the Y offset of the specified form part.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var offset = controller.getPartYOffset(JSPart.BODY);
```
### getSelectedIndex()

Gets the current record index of the current foundset.


**Returns**\
[Number](../../JSLib/Number.md) the index

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
//gets the current record index in the current foundset
var current = controller.getSelectedIndex();
//sets the next record in the foundset, will be reflected in UI
controller.setSelectedIndex(current+1);
```
### getTabSequence()

Get an array with the names of the components that are part of the tab sequence.
The order of the names respects the order of the tab sequence.
Components that are not named will not appear in the returned array, although they may be in the tab sequence.


**Returns**\
[Array](../../JSLib/Array.md) array of names

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var tabseq = controller.getTabSequence();
if (tabseq.length > 1) {
	// If there is more than one field in the tab sequence,
	// focus the second one and skip over readonly fields.
	controller.focusField(tabseq[1], true);
}
else {
	// If there is at most one field in the tab sequence, then focus
	// whatever field is first, and don't bother to skip over readonly fields.
	controller.focusField(null, false);
}
```
### getWindow()

Returns the JSWindow that the form is shown in, or null if the form is not currently showing in a window.


**Returns**\
[JSWindow](../../Application/JSWindow.md) the JSWindow that the form is shown in, or null if the form is not currently showing in a window.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var currentWindow = controller.getWindow();
if (currentWindow != null) {
	currentWindow.title = 'We have a new title';
} else {
	currentWindow = application.createWindow("Window Name", JSWindow.WINDOW, null);
	currentWindow(650, 700, 450, 350);
	currentWindow = "Window Title";
	controller.show(currentWindow);
}
```
### loadRecords(foundset)

Loads a (related) foundset into the form.
The form will no longer share the default foundset with forms of the same datasource, use loadAllRecords to restore the default foundset.

This will really change the foundset instance itself of the form, so no existing foundset is altered just the new foundset that is given is used..
This is different then doing foundset.loadRecords(foundset) because that just alters the current foundset and doesn't do anything with the foundset that is given.

So controller.loadRecords(fs) does overwrite the foundset instance completely, foundset filters set previously on the forms foundset are gone, only the foundset filters on the given foundset are set.

foundset.loadRecords(fs) will adjust the current forms foundset and the foundset filters that are set are kept and merged with the filters of the given foundset.

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundset to load

**Returns**\
[Boolean](../../JSLib/Boolean.md) true if successful

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//to load a (related)foundset into the form.
//the form will no longer share the default foundset with forms of the same datasource, use loadAllRecords to restore the default foundset
controller.loadRecords(order_to_orderdetails);
```
### loadRecords(foundset)

Loads a (related) foundset into the form.
The form will no longer share the default foundset with forms of the same datasource, use loadAllRecords to restore the default foundset.

This will really update the foundset instance itself of the form, so now existing foundset is altered just the new foundset is shown.
This is different then doing foundset.loadRecords(foundset) because that just alters the current foundset and doesn't do anything with the foundset
that is given.

When the form uses a seperate foundset, foundset filter params are copied over from the source foundset and are merged with the existing filters.

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundset to load

**Returns**\
[Boolean](../../JSLib/Boolean.md) true if successful

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//to load a (related)foundset into the form.
//the form will no longer share the default foundset with forms of the same datasource, use loadAllRecords to restore the default foundset
controller.loadRecords(order_to_orderdetails);
```
### print()

Print this form with current foundset, without preview.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
//print this form (with foundset records)
controller.print();
//print only current record (no printerSelectDialog) to pdf plugin printer
//controller.print(true,false,plugins.pdf_output.getPDFPrinter('c:/temp/out.pdf'));
```
### print(printCurrentRecordOnly)

Print this form with current foundset, without preview.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) printCurrentRecordOnly to print the current record only

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
//print this form (with foundset records)
controller.print();
//print only current record (no printerSelectDialog) to pdf plugin printer
//controller.print(true,false,plugins.pdf_output.getPDFPrinter('c:/temp/out.pdf'));
```
### print(printCurrentRecordOnly, showPrinterSelectDialog)

Print this form with current foundset, without preview.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) printCurrentRecordOnly to print the current record only\
[Boolean](../../JSLib/Boolean.md) showPrinterSelectDialog to show the printer select dialog (default printer is normally used)

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
//print this form (with foundset records)
controller.print();
//print only current record (no printerSelectDialog) to pdf plugin printer
//controller.print(true,false,plugins.pdf_output.getPDFPrinter('c:/temp/out.pdf'));
```
### print(printCurrentRecordOnly, showPrinterSelectDialog, printerJob)

Print this form with current foundset, without preview.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) printCurrentRecordOnly to print the current record only\
[Boolean](../../JSLib/Boolean.md) showPrinterSelectDialog to show the printer select dialog (default printer is normally used)\
[Object](../../JSLib/Object.md) printerJob print to plugin printer job, see pdf printer plugin for example

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
//print this form (with foundset records)
controller.print();
//print only current record (no printerSelectDialog) to pdf plugin printer
//controller.print(true,false,plugins.pdf_output.getPDFPrinter('c:/temp/out.pdf'));
```
### printXML()

Print this form with current foundset records to xml format.


**Returns**\
[String](../../JSLib/String.md) the XML

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
//TIP: see also plugins.file.writeXMLFile(...)
var xml = controller.printXML();
//print only current record
//var xml = controller.printXML(true);
```
### printXML(printCurrentRecordOnly)

Print this form with current foundset records to xml format.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) printCurrentRecordOnly to print the current record only

**Returns**\
[String](../../JSLib/String.md) the XML

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
//TIP: see also plugins.file.writeXMLFile(...)
var xml = controller.printXML();
//print only current record
//var xml = controller.printXML(true);
```
### recreateUI()

Recreates the forms UI components, to reflect the latest solution model.
Use this after altering the elements via solutionModel at the JSForm of this form.


**Returns**\
[Boolean](../../JSLib/Boolean.md) true if successful

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// get the solution model JSForm
var form = solutionModel.getForm("myForm");
// get the JSField of the form
var field = form.getField("myField");
// alter the field
field.x = field.x + 10;
// recreate the runtime forms ui to reflect the changes.
controller.recreateUI();
```
### search()

Start the database search and use the results, returns the number of records, make sure you did "find" function first.
Clear results from previous searches.

Note: Omitted records are automatically excluded when performing a search - meaning that the foundset result by default will not include omitted records.


**Returns**\
[Number](../../JSLib/Number.md) the recordCount

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var recordCount = foundset.search();
//var recordCount = foundset.search(false,false); //to extend foundset
```
### search(clearLastResults)

Start the database search and use the results, returns the number of records, make sure you did "find" function first.
Reduce results from previous searches.

Note: Omitted records are automatically excluded when performing a search - meaning that the foundset result by default will not include omitted records.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) clearLastResults boolean, clear previous search, default true

**Returns**\
[Number](../../JSLib/Number.md) the recordCount

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var recordCount = foundset.search();
//var recordCount = foundset.search(false,false); //to extend foundset
```
### search(clearLastResults, reduceSearch)

Start the database search and use the results, returns the number of records, make sure you did "find" function first.

Note: Omitted records are automatically excluded when performing a search - meaning that the foundset result by default will not include omitted records.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) clearLastResults boolean, clear previous search, default true\
[Boolean](../../JSLib/Boolean.md) reduceSearch boolean, reduce (true) or extend (false) previous search results, default true

**Returns**\
[Number](../../JSLib/Number.md) the recordCount

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var recordCount = foundset.search();
//var recordCount = foundset.search(false,false); //to extend foundset
```
### setDataProviderValue(dataprovider, value)

Sets the value based on a specified dataprovider name.

**Parameters**\
[String](../../JSLib/String.md) dataprovider the dataprovider name to set the value for\
[Object](../../JSLib/Object.md) value the value to set in the dataprovider

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.setDataProviderValue('contact_name','mycompany');
```
### setDesignMode(designMode)

Sets this form in designmode with param true, false will return to normal browse/edit mode.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) designMode sets form in design mode if true, false ends design mode.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = forms["selectedFormName"];
if (!form.controller.getDesignMode())
{
	// Set the current form in designmode with no callbacks
	form.controller.setDesignMode(true);
	// Set the current form in designmode with callbacks
	// where onDrag, onDrop, onSelect, onResize are names of form methods (not from "selectedFormName" form)
	// form.controller.setDesignMode(onDrag, onDrop, onSelect, onResize);
}
//Set the current form out of designmode (to normal browse)
//form.controller.setDesignMode(false);
```
### setDesignMode(ondrag)

Sets this form in designmode with one or more callback methods.

**Parameters**\
[Function](../../JSLib/Function.md) ondrag onDrag method reference

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = forms["selectedFormName"];
if (!form.controller.getDesignMode())
{
	// Set the current form in designmode with no callbacks
	form.controller.setDesignMode(true);
	// Set the current form in designmode with callbacks
	// where onDrag, onDrop, onSelect, onResize are names of form methods (not from "selectedFormName" form)
	// form.controller.setDesignMode(onDrag, onDrop, onSelect, onResize);
}
//Set the current form out of designmode (to normal browse)
//form.controller.setDesignMode(false);
```
### setDesignMode(ondrag, ondrop)

Sets this form in designmode with one or more callback methods.

**Parameters**\
[Function](../../JSLib/Function.md) ondrag onDrag method reference\
[Function](../../JSLib/Function.md) ondrop onDrop method reference

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = forms["selectedFormName"];
if (!form.controller.getDesignMode())
{
	// Set the current form in designmode with no callbacks
	form.controller.setDesignMode(true);
	// Set the current form in designmode with callbacks
	// where onDrag, onDrop, onSelect, onResize are names of form methods (not from "selectedFormName" form)
	// form.controller.setDesignMode(onDrag, onDrop, onSelect, onResize);
}
//Set the current form out of designmode (to normal browse)
//form.controller.setDesignMode(false);
```
### setDesignMode(ondrag, ondrop, onselect)

Sets this form in designmode with one or more callback methods.

**Parameters**\
[Function](../../JSLib/Function.md) ondrag onDrag method reference\
[Function](../../JSLib/Function.md) ondrop onDrop method reference\
[Function](../../JSLib/Function.md) onselect onSelect method reference

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = forms["selectedFormName"];
if (!form.controller.getDesignMode())
{
	// Set the current form in designmode with no callbacks
	form.controller.setDesignMode(true);
	// Set the current form in designmode with callbacks
	// where onDrag, onDrop, onSelect, onResize are names of form methods (not from "selectedFormName" form)
	// form.controller.setDesignMode(onDrag, onDrop, onSelect, onResize);
}
//Set the current form out of designmode (to normal browse)
//form.controller.setDesignMode(false);
```
### setDesignMode(ondrag, ondrop, onselect, onresize)

Sets this form in designmode with one or more callback methods.

**Parameters**\
[Function](../../JSLib/Function.md) ondrag onDrag method reference\
[Function](../../JSLib/Function.md) ondrop onDrop method reference\
[Function](../../JSLib/Function.md) onselect onSelect method reference\
[Function](../../JSLib/Function.md) onresize onResize method reference

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = forms["selectedFormName"];
if (!form.controller.getDesignMode())
{
	// Set the current form in designmode with no callbacks
	form.controller.setDesignMode(true);
	// Set the current form in designmode with callbacks
	// where onDrag, onDrop, onSelect, onResize are names of form methods (not from "selectedFormName" form)
	// form.controller.setDesignMode(onDrag, onDrop, onSelect, onResize);
}
//Set the current form out of designmode (to normal browse)
//form.controller.setDesignMode(false);
```
### setDesignMode(ondrag, ondrop, onselect, onresize, ondblclick)

Sets this form in designmode with one or more callback methods.

**Parameters**\
[Function](../../JSLib/Function.md) ondrag onDrag method reference\
[Function](../../JSLib/Function.md) ondrop onDrop method reference\
[Function](../../JSLib/Function.md) onselect onSelect method reference\
[Function](../../JSLib/Function.md) onresize onResize method reference\
[Function](../../JSLib/Function.md) ondblclick onDblClick method reference

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = forms["selectedFormName"];
if (!form.controller.getDesignMode())
{
	// Set the current form in designmode with no callbacks
	form.controller.setDesignMode(true);
	// Set the current form in designmode with callbacks
	// where onDrag, onDrop, onSelect, onResize are names of form methods (not from "selectedFormName" form)
	// form.controller.setDesignMode(onDrag, onDrop, onSelect, onResize);
}
//Set the current form out of designmode (to normal browse)
//form.controller.setDesignMode(false);
```
### setDesignMode(ondrag, ondrop, onselect, onresize, ondblclick, onrightclick)

Sets this form in designmode with one or more callback methods.

**Parameters**\
[Function](../../JSLib/Function.md) ondrag onDrag method reference\
[Function](../../JSLib/Function.md) ondrop onDrop method reference\
[Function](../../JSLib/Function.md) onselect onSelect method reference\
[Function](../../JSLib/Function.md) onresize onResize method reference\
[Function](../../JSLib/Function.md) ondblclick onDblClick method reference\
[Function](../../JSLib/Function.md) onrightclick onRightClick method reference

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = forms["selectedFormName"];
if (!form.controller.getDesignMode())
{
	// Set the current form in designmode with no callbacks
	form.controller.setDesignMode(true);
	// Set the current form in designmode with callbacks
	// where onDrag, onDrop, onSelect, onResize are names of form methods (not from "selectedFormName" form)
	// form.controller.setDesignMode(onDrag, onDrop, onSelect, onResize);
}
//Set the current form out of designmode (to normal browse)
//form.controller.setDesignMode(false);
```
### setPageFormat(width, height, leftmargin, rightmargin, topmargin, bottommargin)

Set the page format to use when printing.

Orientation values:
0 - Landscape mode
1 - Portrait mode

Units values:
0 - millimeters
1 - inches
2 - pixels

Note: The unit specified for width, height and all margins MUST be the same.

**Parameters**\
[Number](../../JSLib/Number.md) width the specified width of the page to be printed.\
[Number](../../JSLib/Number.md) height the specified height of the page to be printed.\
[Number](../../JSLib/Number.md) leftmargin the specified left margin of the page to be printed.\
[Number](../../JSLib/Number.md) rightmargin the specified right margin of the page to be printed.\
[Number](../../JSLib/Number.md) topmargin the specified top margin of the page to be printed.\
[Number](../../JSLib/Number.md) bottommargin the specified bottom margin of the page to be printed.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
//Set page format to a custom size of 100x200 pixels with 10 pixel margins on all sides in portrait mode
controller.setPageFormat(100, 200, 10, 10, 10, 10);

//Set page format to a custom size of 100x200 pixels with 10 pixel margins on all sides in landscape mode
controller.setPageFormat(100, 200, 10, 10, 10, 10, SM_ORIENTATION.LANDSCAPE);

//Set page format to a custom size of 100x200 mm in landscape mode
controller.setPageFormat(100, 200, 0, 0, 0, 0, SM_ORIENTATION.LANDSCAPE, SM_UNITS.MM);

//Set page format to a custom size of 100x200 inch in portrait mode
controller.setPageFormat(100, 200, 0, 0, 0, 0, SM_ORIENTATION.PORTRAIT, SM_UNITS.INCH);
```
### setPageFormat(width, height, leftmargin, rightmargin, topmargin, bottommargin, orientation)

Set the page format to use when printing.

Orientation values:
0 - Landscape mode
1 - Portrait mode

Units values:
0 - millimeters
1 - inches
2 - pixels

Note: The unit specified for width, height and all margins MUST be the same.

**Parameters**\
[Number](../../JSLib/Number.md) width the specified width of the page to be printed.\
[Number](../../JSLib/Number.md) height the specified height of the page to be printed.\
[Number](../../JSLib/Number.md) leftmargin the specified left margin of the page to be printed.\
[Number](../../JSLib/Number.md) rightmargin the specified right margin of the page to be printed.\
[Number](../../JSLib/Number.md) topmargin the specified top margin of the page to be printed.\
[Number](../../JSLib/Number.md) bottommargin the specified bottom margin of the page to be printed.\
[Number](../../JSLib/Number.md) orientation the specified orientation of the page to be printed; the default is Portrait mode

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
//Set page format to a custom size of 100x200 pixels with 10 pixel margins on all sides in portrait mode
controller.setPageFormat(100, 200, 10, 10, 10, 10);

//Set page format to a custom size of 100x200 pixels with 10 pixel margins on all sides in landscape mode
controller.setPageFormat(100, 200, 10, 10, 10, 10, SM_ORIENTATION.LANDSCAPE);

//Set page format to a custom size of 100x200 mm in landscape mode
controller.setPageFormat(100, 200, 0, 0, 0, 0, SM_ORIENTATION.LANDSCAPE, SM_UNITS.MM);

//Set page format to a custom size of 100x200 inch in portrait mode
controller.setPageFormat(100, 200, 0, 0, 0, 0, SM_ORIENTATION.PORTRAIT, SM_UNITS.INCH);
```
### setPageFormat(width, height, leftmargin, rightmargin, topmargin, bottommargin, orientation, units)

Set the page format to use when printing.

Orientation values:
0 - Landscape mode
1 - Portrait mode

Units values:
0 - millimeters
1 - inches
2 - pixels

Note: The unit specified for width, height and all margins MUST be the same.

**Parameters**\
[Number](../../JSLib/Number.md) width the specified width of the page to be printed.\
[Number](../../JSLib/Number.md) height the specified height of the page to be printed.\
[Number](../../JSLib/Number.md) leftmargin the specified left margin of the page to be printed.\
[Number](../../JSLib/Number.md) rightmargin the specified right margin of the page to be printed.\
[Number](../../JSLib/Number.md) topmargin the specified top margin of the page to be printed.\
[Number](../../JSLib/Number.md) bottommargin the specified bottom margin of the page to be printed.\
[Number](../../JSLib/Number.md) orientation the specified orientation of the page to be printed; the default is Portrait mode\
[Number](../../JSLib/Number.md) units the specified units for the width and height of the page to be printed; the default is pixels

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
//Set page format to a custom size of 100x200 pixels with 10 pixel margins on all sides in portrait mode
controller.setPageFormat(100, 200, 10, 10, 10, 10);

//Set page format to a custom size of 100x200 pixels with 10 pixel margins on all sides in landscape mode
controller.setPageFormat(100, 200, 10, 10, 10, 10, SM_ORIENTATION.LANDSCAPE);

//Set page format to a custom size of 100x200 mm in landscape mode
controller.setPageFormat(100, 200, 0, 0, 0, 0, SM_ORIENTATION.LANDSCAPE, SM_UNITS.MM);

//Set page format to a custom size of 100x200 inch in portrait mode
controller.setPageFormat(100, 200, 0, 0, 0, 0, SM_ORIENTATION.PORTRAIT, SM_UNITS.INCH);
```
### setPreferredPrinter(printerName)

Set the preferred printer name to use when printing.

**Parameters**\
[String](../../JSLib/String.md) printerName The name of the printer to be used when printing.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
controller.setPreferredPrinter('HP Laser 2200');
```
### setSelectedIndex(index)

Sets the current record index of the current foundset.

**Parameters**\
[Number](../../JSLib/Number.md) index the index to select

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
//gets the current record index in the current foundset
var current = controller.getSelectedIndex();
//sets the next record in the foundset, will be reflected in UI
controller.setSelectedIndex(current+1);
```
### setTabSequence(arrayOfElements)

Set the tab order sequence programatically, by passing the elements references in a javascript array.

**Parameters**\
[Array](../../JSLib/Array.md) arrayOfElements array containing the element references

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.setTabSequence([elements.fld_order_id, elements.fld_order_amount]);
```
### show()

Shows the form (makes the form visible)
This function does not affect the form foundset in any way.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
// show the form in the current window/dialog
controller.show();
// show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.show(w);
// show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.show(w);
// or controller.show("mydialog");
//show the form in the main window
//controller.show(null);
```
### show(window)

Shows the form (makes the form visible)
This function does not affect the form foundset in any way.

**Parameters**\
[JSWindow](../../Application/JSWindow.md) window the window in which this form should be shown, given as a window object

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// show the form in the current window/dialog
controller.show();
// show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.show(w);
// show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.show(w);
// or controller.show("mydialog");
//show the form in the main window
//controller.show(null);
```
### show(window)

Shows the form (makes the form visible)
This function does not affect the form foundset in any way.

**Parameters**\
[String](../../JSLib/String.md) window the window in which this form should be shown, specified by the name of an existing window

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// show the form in the current window/dialog
controller.show();
// show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.show(w);
// show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.show(w);
// or controller.show("mydialog");
//show the form in the main window
//controller.show(null);
```
### showPrintPreview()

Show this form in print preview.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
//shows this form (with foundset records) in print preview
controller.showPrintPreview();
//to print preview current record only
//controller.showPrintPreview(true);
//to print preview current record only with 125% zoom factor;
//controller.showPrintPreview(true, null, 125);
```
### showPrintPreview(printCurrentRecordOnly)

Show this form in print preview.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) printCurrentRecordOnly to print the current record only

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
//shows this form (with foundset records) in print preview
controller.showPrintPreview();
//to print preview current record only
//controller.showPrintPreview(true);
//to print preview current record only with 125% zoom factor;
//controller.showPrintPreview(true, null, 125);
```
### showPrintPreview(printCurrentRecordOnly, printerJob)

Show this form in print preview.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) printCurrentRecordOnly to print the current record only\
[Object](../../JSLib/Object.md) printerJob print to plugin printer job, see pdf printer plugin for example (incase print is used from printpreview)

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
//shows this form (with foundset records) in print preview
controller.showPrintPreview();
//to print preview current record only
//controller.showPrintPreview(true);
//to print preview current record only with 125% zoom factor;
//controller.showPrintPreview(true, null, 125);
```
### showPrintPreview(printCurrentRecordOnly, printerJob, zoomFactor)

Show this form in print preview.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) printCurrentRecordOnly to print the current record only\
[Object](../../JSLib/Object.md) printerJob print to plugin printer job, see pdf printer plugin for example (incase print is used from printpreview)\
[Number](../../JSLib/Number.md) zoomFactor a specified number value from 10-400

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
//shows this form (with foundset records) in print preview
controller.showPrintPreview();
//to print preview current record only
//controller.showPrintPreview(true);
//to print preview current record only with 125% zoom factor;
//controller.showPrintPreview(true, null, 125);
```
### showRecords(foundset)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundset the foundset to load before showing the form.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(foundset, window)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundset the foundset to load before showing the form.\
[JSWindow](../../Application/JSWindow.md) window the window in which this form should be shown, given as a window object.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(foundset, window)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundset the foundset to load before showing the form.\
[String](../../JSLib/String.md) window the window in which this form should be shown, specified by the name of an existing window.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(pkdataset)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[JSDataSet](../../Database%20Manager/JSDataSet.md) pkdataset the pkdataset to load before showing the form.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(pkdataset, window)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[JSDataSet](../../Database%20Manager/JSDataSet.md) pkdataset the pkdataset to load before showing the form.\
[JSWindow](../../Application/JSWindow.md) window the window in which this form should be shown, given as a window object.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(pkdataset, window)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[JSDataSet](../../Database%20Manager/JSDataSet.md) pkdataset the pkdataset to load before showing the form.\
[String](../../JSLib/String.md) window the window in which this form should be shown, specified by the name of an existing window.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(query)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[QBSelect](../../Database%20Manager/QBSelect.md) query the query to load before showing the form.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(query, window)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[QBSelect](../../Database%20Manager/QBSelect.md) query the query to load before showing the form.\
[JSWindow](../../Application/JSWindow.md) window the window in which this form should be shown, given as a window object.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(query, window)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[QBSelect](../../Database%20Manager/QBSelect.md) query the query to load before showing the form.\
[String](../../JSLib/String.md) window the window in which this form should be shown, specified by the name of an existing window.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(UUIDpk)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[UUID](../../Application/UUID.md) UUIDpk the UUIDpk to load before showing the form.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(UUIDpk, window)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[UUID](../../Application/UUID.md) UUIDpk the UUIDpk to load before showing the form.\
[JSWindow](../../Application/JSWindow.md) window the window in which this form should be shown, given as a window object.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(UUIDpk, window)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[UUID](../../Application/UUID.md) UUIDpk the UUIDpk to load before showing the form.\
[String](../../JSLib/String.md) window the window in which this form should be shown, specified by the name of an existing window.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(singleNumber_pk)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[Number](../../JSLib/Number.md) singleNumber_pk the singleNumber_pk to load before showing the form.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(singleNumber_pk, window)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[Number](../../JSLib/Number.md) singleNumber_pk the singleNumber_pk to load before showing the form.\
[JSWindow](../../Application/JSWindow.md) window the window in which this form should be shown, given as a window object

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(singleNumber_pk, window)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[Number](../../JSLib/Number.md) singleNumber_pk the singleNumber_pk to load before showing the form.\
[String](../../JSLib/String.md) window the window in which this form should be shown, specified by the name of an existing window.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(query)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[String](../../JSLib/String.md) query the query to load before showing the form.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(query, window)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[String](../../JSLib/String.md) query the query to load before showing the form.\
[JSWindow](../../Application/JSWindow.md) window the window in which this form should be shown, given as a window object

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(query, argumentsArray)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[String](../../JSLib/String.md) query the query to load before showing the form.\
[Array](../../JSLib/Array.md) argumentsArray the array of arguments for the query

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(query, argumentsArray, window)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[String](../../JSLib/String.md) query the query to load before showing the form.\
[Array](../../JSLib/Array.md) argumentsArray the array of arguments for the query\
[JSWindow](../../Application/JSWindow.md) window the window in which this form should be shown, given as a window object

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(query, argumentsArray, window)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[String](../../JSLib/String.md) query the query to load before showing the form.\
[Array](../../JSLib/Array.md) argumentsArray the array of arguments for the query\
[String](../../JSLib/String.md) window the window in which this form should be shown, specified by the name of an existing window.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### showRecords(query, window)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[String](../../JSLib/String.md) query the query to load before showing the form.\
[String](../../JSLib/String.md) window the window in which this form should be shown, specified by the name of an existing window.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
controller.showRecords(foundset);
// load foundset & show the form in newly created named modal dialog
var w = application.createWindow("mydialog", JSWindow.MODAL_DIALOG);
controller.showRecords(foundset, w);
// load foundset & show the form in an existing window/dialog
var w = application.getWindow("mydialog"); // use null name for main app. window
controller.showRecords(foundset, w);
//controller.showRecords(foundset, "mydialog");
```
### sortDialog()

Show the sort dialog to the user a preselection sortString can be passed, to sort the form foundset.
TIP: You can use the Copy button in the developer Select Sorting Fields dialog to get the needed syntax string for the desired sort fields/order.


**Returns**\
void 

**Supported Clients**\
SmartClient

**Sample**

```javascript
controller.sortDialog('columnA desc,columnB asc');
```
### sortDialog(sortString)



**Parameters**\
[String](../../JSLib/String.md) sortString the specified columns (and sort order)

**Returns**\
void 

**Supported Clients**\
SmartClient

**Sample**

```javascript
controller.sortDialog('columnA desc,columnB asc');
```

