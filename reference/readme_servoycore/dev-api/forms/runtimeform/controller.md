# controller

## Property Summary

| Type                               | Name                               | Summary                                                                                                                                                                            |
| ---------------------------------- | ---------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Boolean](../../js-lib/boolean.md) | [enabled](controller.md#enabled)   | Gets or sets the enabled state of a form; also known as "grayed-out"..                                                                                                             |
| [Boolean](../../js-lib/boolean.md) | [readOnly](controller.md#readOnly) | Gets or sets the read-only state of a form; also known as "editable" Note: The field(s) in a form set as read-only can be selected and the field data can be copied to clipboard.. |
| [Number](../../js-lib/number.md)   | [view](controller.md#view)         | Get/Set the current type of view of this form..                                                                                                                                    |

## Methods Summary

| Type                                             | Name                                                                                                                                                               | Summary                                                                                                                 |
| ------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------- |
| [Boolean](../../js-lib/boolean.md)               | [find()](controller.md#find)                                                                                                                                       | Set the foundset in find mode..                                                                                         |
| [Boolean](../../js-lib/boolean.md)               | [focusField(fieldName, skipReadonly)](controller.md#focusfield-fieldname-skipreadonly)                                                                             | Sets focus to a field specified by its name..                                                                           |
| [Boolean](../../js-lib/boolean.md)               | [focusFirstField()](controller.md#focusfirstfield)                                                                                                                 | Sets focus to the first field of the form; based on tab order sequence..                                                |
| [Number](../../js-lib/number.md)                 | [getDataProviderMaxLength(name)](controller.md#getdataprovidermaxlength-name)                                                                                      | Returns the maximum length allowed in the specified dataprovider..                                                      |
| [Object](../../js-lib/object.md)                 | [getDataProviderValue(dataProvider)](controller.md#getdataprovidervalue-dataprovider)                                                                              | Gets a value based on the specified dataprovider name..                                                                 |
| [String](../../js-lib/string.md)                 | [getDataSource()](controller.md#getdatasource)                                                                                                                     | Get the used datasource..                                                                                               |
| [Boolean](../../js-lib/boolean.md)               | [getDesignMode()](controller.md#getdesignmode)                                                                                                                     | Returns the state of this form designmode..                                                                             |
| [Object](../../js-lib/object.md)                 | [getDesignProperties()](controller.md#getdesignproperties)                                                                                                         | Get the design-time properties of the form..                                                                            |
| [Object](../../js-lib/object.md)                 | [getDesignTimeProperty(key)](controller.md#getdesigntimeproperty-key)                                                                                              | Get a design-time property of a form..                                                                                  |
| [JSDataSet](../../database-manager/jsdataset.md) | [getFormContext()](controller.md#getformcontext)                                                                                                                   | Gets the forms context where it resides, returns a dataset of its structure to the main controller..                    |
| [Number](../../js-lib/number.md)                 | [getFormWidth()](controller.md#getformwidth)                                                                                                                       | Gets the form width in pixels..                                                                                         |
| [String](../../js-lib/string.md)                 | [getName()](controller.md#getname)                                                                                                                                 | Get the name of this form..                                                                                             |
| [Number](../../js-lib/number.md)                 | [getPartHeight(partType)](controller.md#getpartheight-parttype)                                                                                                    | Gets the part height in pixels..                                                                                        |
| [Number](../../js-lib/number.md)                 | [getPartYOffset(partType)](controller.md#getpartyoffset-parttype)                                                                                                  | Returns the Y offset of a given part of the form..                                                                      |
| [Number](../../js-lib/number.md)                 | [getSelectedIndex()](controller.md#getselectedindex)                                                                                                               | Gets the current record index of the current foundset..                                                                 |
| [Array](../../js-lib/array.md)                   | [getTabSequence()](controller.md#gettabsequence)                                                                                                                   | Get an array with the names of the components that are part of the tab sequence..                                       |
| [JSWindow](../../application/jswindow.md)        | [getWindow()](controller.md#getwindow)                                                                                                                             | Returns the JSWindow that the form is shown in, or null if the form is not currently showing in a window..              |
| [Boolean](../../js-lib/boolean.md)               | [loadRecords(foundset)](controller.md#loadrecords-foundset)                                                                                                        | Loads a (related) foundset into the form..                                                                              |
| [Boolean](../../js-lib/boolean.md)               | [loadRecords(foundset)](controller.md#loadrecords-foundset)                                                                                                        | Loads a (related) foundset into the form..                                                                              |
| [Boolean](../../js-lib/boolean.md)               | [recreateUI()](controller.md#recreateui)                                                                                                                           | Recreates the forms UI components, to reflect the latest solution model..                                               |
| [Number](../../js-lib/number.md)                 | [search()](controller.md#search)                                                                                                                                   | Start the database search and use the results, returns the number of records, make sure you did "find" function first.. |
| [Number](../../js-lib/number.md)                 | [search(clearLastResults)](controller.md#search-clearlastresults)                                                                                                  | Start the database search and use the results, returns the number of records, make sure you did "find" function first.. |
| [Number](../../js-lib/number.md)                 | [search(clearLastResults, reduceSearch)](controller.md#search-clearlastresults-reducesearch)                                                                       | Start the database search and use the results, returns the number of records, make sure you did "find" function first.. |
| void                                             | [setDataProviderValue(dataprovider, value)](controller.md#setdataprovidervalue-dataprovider-value)                                                                 | Sets the value based on a specified dataprovider name..                                                                 |
| void                                             | [setDesignMode(designMode)](controller.md#setdesignmode-designmode)                                                                                                | Sets this form in designmode with param true, false will return to normal browse/edit mode..                            |
| void                                             | [setDesignMode(ondrag)](controller.md#setdesignmode-ondrag)                                                                                                        | Sets this form in designmode with one or more callback methods..                                                        |
| void                                             | [setDesignMode(ondrag, ondrop)](controller.md#setdesignmode-ondrag-ondrop)                                                                                         | Sets this form in designmode with one or more callback methods..                                                        |
| void                                             | [setDesignMode(ondrag, ondrop, onselect)](controller.md#setdesignmode-ondrag-ondrop-onselect)                                                                      | Sets this form in designmode with one or more callback methods..                                                        |
| void                                             | [setDesignMode(ondrag, ondrop, onselect, onresize)](controller.md#setdesignmode-ondrag-ondrop-onselect-onresize)                                                   | Sets this form in designmode with one or more callback methods..                                                        |
| void                                             | [setDesignMode(ondrag, ondrop, onselect, onresize, ondblclick)](controller.md#setdesignmode-ondrag-ondrop-onselect-onresize-ondblclick)                            | Sets this form in designmode with one or more callback methods..                                                        |
| void                                             | [setDesignMode(ondrag, ondrop, onselect, onresize, ondblclick, onrightclick)](controller.md#setdesignmode-ondrag-ondrop-onselect-onresize-ondblclick-onrightclick) | Sets this form in designmode with one or more callback methods..                                                        |
| void                                             | [setSelectedIndex(index)](controller.md#setselectedindex-index)                                                                                                    | Sets the current record index of the current foundset..                                                                 |
| void                                             | [setTabSequence(arrayOfElements)](controller.md#settabsequence-arrayofelements)                                                                                    | Set the tab order sequence programatically, by passing the elements references in a javascript array..                  |
| void                                             | [show()](controller.md#show)                                                                                                                                       | Shows the form (makes the form visible) This function does not affect the form foundset in any way..                    |
| void                                             | [show(window)](controller.md#show-window)                                                                                                                          | Shows the form (makes the form visible) This function does not affect the form foundset in any way..                    |
| void                                             | [show(window)](controller.md#show-window)                                                                                                                          | Shows the form (makes the form visible) This function does not affect the form foundset in any way..                    |
| void                                             | [showRecords(foundset)](controller.md#showrecords-foundset)                                                                                                        | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(foundset, window)](controller.md#showrecords-foundset-window)                                                                                         | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(foundset, window)](controller.md#showrecords-foundset-window)                                                                                         | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(pkdataset)](controller.md#showrecords-pkdataset)                                                                                                      | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(pkdataset, window)](controller.md#showrecords-pkdataset-window)                                                                                       | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(pkdataset, window)](controller.md#showrecords-pkdataset-window)                                                                                       | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(query)](controller.md#showrecords-query)                                                                                                              | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(query, window)](controller.md#showrecords-query-window)                                                                                               | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(query, window)](controller.md#showrecords-query-window)                                                                                               | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(UUIDpk)](controller.md#showrecords-uuidpk)                                                                                                            | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(UUIDpk, window)](controller.md#showrecords-uuidpk-window)                                                                                             | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(UUIDpk, window)](controller.md#showrecords-uuidpk-window)                                                                                             | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(singleNumber\_pk)](controller.md#showrecords-singlenumber\_pk)                                                                                        | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(singleNumber\_pk, window)](controller.md#showrecords-singlenumber\_pk-window)                                                                         | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(singleNumber\_pk, window)](controller.md#showrecords-singlenumber\_pk-window)                                                                         | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(query)](controller.md#showrecords-query)                                                                                                              | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(query, window)](controller.md#showrecords-query-window)                                                                                               | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(query, argumentsArray)](controller.md#showrecords-query-argumentsarray)                                                                               | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(query, argumentsArray, window)](controller.md#showrecords-query-argumentsarray-window)                                                                | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(query, argumentsArray, window)](controller.md#showrecords-query-argumentsarray-window)                                                                | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |
| void                                             | [showRecords(query, window)](controller.md#showrecords-query-window)                                                                                               | Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'..                  |

## Properties Details

### enabled

Gets or sets the enabled state of a form; also known as "grayed-out".

Notes: -A disabled element(s) cannot be selected by clicking the form. -The disabled "grayed" color is dependent on the LAF set in the Servoy Smart Client Application Preferences.

**Returns**\
[Boolean](../../js-lib/boolean.md)

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
[Boolean](../../js-lib/boolean.md)

**Sample**

```javascript
//gets the read-only state of the form
var state = controller.readOnly;
//sets the read-only state of the form
controller.readOnly = true
```

### view

Get/Set the current type of view of this form. Can be one of the JSForm.xxxx\_VIEW constants. In NGClient only RECORD\_VIEW is fully supported, the List and TableViews should be replaced by components.

**Returns**\
[Number](../../js-lib/number.md)

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

Before going into find mode, all unsaved records will be saved in the database. If this fails (due to validation failures or sql errors) or is not allowed (autosave off), the foundset will not go into find mode. Make sure the operator and the data (value) are part of the string passed to dataprovider (included inside a pair of quotation marks). Note: always make sure to check the result of the find() method.

When in find mode, columns can be assigned string expressions (including operators) that are evaluated as: General: c1||c2 (condition1 or condition2) c|format (apply format on condition like 'x|dd-MM-yyyy') !c (not condition) #c (modify condition, depends on column type) ^ (is null) ^= (is null or empty) \<x (less than value x) >x (greater than value x) <=x (less than or equals value x) >=x (greater than or equals value x) x...y (between values x and y, including values) x (equals value x)

Number fields: =x (equals value x) ^= (is null or zero)

Date fields: #c (equals value x, entire day) now (equals now, date and or time) // (equals today) today (equals today)

Text fields: #c (case insensitive condition) = x (equals a space and 'x') ^= (is null or empty) %x% (contains 'x') %x\_y% (contains 'x' followed by any char and 'y') % (contains char '%') \_ (contains char '\_')

Related columns can be assigned, they will result in related searches. For example, "employees\_to\_department.location\_id = headoffice" finds all employees in the specified location).

Searching on related aggregates is supported. For example, "orders\_to\_details.total\_amount = '>1000'" finds all orders with total order details amount more than 1000.

Arrays can be used for searching a number of values, this will result in an 'IN' condition that will be used in the search. The values are not restricted to strings but can be any type that matches the column type. For example, "record.department\_id = \[1, 33, 99]"

**Returns**\
[Boolean](../../js-lib/boolean.md) true if the foundset is now in find mode, false otherwise.

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

Sets focus to a field specified by its name. If the second parameter is set to true, then readonly fields will be skipped (the focus will be set to the first non-readonly field located after the field with the specified name; the tab sequence is respected when searching for the non-readonly field).

**Parameters**\
[String](../../js-lib/string.md) fieldName the name of the field to be focussed\
[Boolean](../../js-lib/boolean.md) skipReadonly indication to skip read only fields, if the named field happens to be read only

**Returns**\
[Boolean](../../js-lib/boolean.md) true if component was found and can be focused

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
[Boolean](../../js-lib/boolean.md) true if component was found and can be focused

**Sample**

```javascript
controller.focusFirstField();
```

### getDataProviderMaxLength(name)

Returns the maximum length allowed in the specified dataprovider.

**Parameters**\
[String](../../js-lib/string.md) name the dataprovider name

**Returns**\
[Number](../../js-lib/number.md) the length

**Sample**

```javascript
controller.getDataProviderMaxLength('name');
```

### getDataProviderValue(dataProvider)

Gets a value based on the specified dataprovider name.

**Parameters**\
[String](../../js-lib/string.md) dataProvider the dataprovider name to retieve the value for

**Returns**\
[Object](../../js-lib/object.md) the dataprovider value (null if unknown dataprovider)

**Sample**

```javascript
var val = controller.getDataProviderValue('contact_name');
```

### getDataSource()

Get the used datasource.

**Returns**\
[String](../../js-lib/string.md) the datasource

**Sample**

```javascript
var dataSource = controller.getDataSource();
```

### getDesignMode()

Returns the state of this form designmode.

**Returns**\
[Boolean](../../js-lib/boolean.md) the design mode state (true/fase)

**Sample**

```javascript
var success = controller.getDesignMode();
```

### getDesignProperties()

Get the design-time properties of the form.

**Returns**\
[Object](../../js-lib/object.md)

**Sample**

```javascript
var prop = fforms.orders.controller.getDesignProperties()
```

### getDesignTimeProperty(key)

Get a design-time property of a form.

**Parameters**\
[String](../../js-lib/string.md) key the property name

**Returns**\
[Object](../../js-lib/object.md)

**Sample**

```javascript
var prop = forms.orders.controller.getDesignTimeProperty('myprop')
```

### getFormContext()

Gets the forms context where it resides, returns a dataset of its structure to the main controller. Note1: can't be called in onload, because no context is yet available at this time. Note2: tabindex is 1 (left) or 2 (right) for a SplitPane and 0 based for the other tabpanels; tabindex1based is the same as tabindex but is 1 based.

**Returns**\
[JSDataSet](../../database-manager/jsdataset.md) the dataset with form context

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
[Number](../../js-lib/number.md) the width in pixels

**Sample**

```javascript
var width = controller.getFormWidth();
```

### getName()

Get the name of this form.

**Returns**\
[String](../../js-lib/string.md) the name

**Sample**

```javascript
var formName = controller.getName();
```

### getPartHeight(partType)

Gets the part height in pixels.

**Parameters**\
[Number](../../js-lib/number.md) partType The type of the part whose height will be returned.

**Returns**\
[Number](../../js-lib/number.md) the part height in pixels

**Sample**

```javascript
var height = controller.getPartHeight(JSPart.BODY);
```

### getPartYOffset(partType)

Returns the Y offset of a given part of the form.

**Parameters**\
[Number](../../js-lib/number.md) partType The type of the part whose Y offset will be returned.

**Returns**\
[Number](../../js-lib/number.md) A number holding the Y offset of the specified form part.

**Sample**

```javascript
var offset = controller.getPartYOffset(JSPart.BODY);
```

### getSelectedIndex()

Gets the current record index of the current foundset.

**Returns**\
[Number](../../js-lib/number.md) the index

**Sample**

```javascript
//gets the current record index in the current foundset
var current = controller.getSelectedIndex();
//sets the next record in the foundset, will be reflected in UI
controller.setSelectedIndex(current+1);
```

### getTabSequence()

Get an array with the names of the components that are part of the tab sequence. The order of the names respects the order of the tab sequence. Components that are not named will not appear in the returned array, although they may be in the tab sequence.

**Returns**\
[Array](../../js-lib/array.md) array of names

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
[JSWindow](../../application/jswindow.md) the JSWindow that the form is shown in, or null if the form is not currently showing in a window.

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

Loads a (related) foundset into the form. The form will no longer share the default foundset with forms of the same datasource, use loadAllRecords to restore the default foundset.

This will really change the foundset instance itself of the form, so no existing foundset is altered just the new foundset that is given is used.. This is different then doing foundset.loadRecords(foundset) because that just alters the current foundset and doesn't do anything with the foundset that is given.

So controller.loadRecords(fs) does overwrite the foundset instance completely, foundset filters set previously on the forms foundset are gone, only the foundset filters on the given foundset are set.

foundset.loadRecords(fs) will adjust the current forms foundset and the foundset filters that are set are kept and merged with the filters of the given foundset.

**Parameters**\
[JSFoundSet](../../database-manager/jsfoundset.md) foundset to load

**Returns**\
[Boolean](../../js-lib/boolean.md) true if successful

**Sample**

```javascript
//to load a (related)foundset into the form.
//the form will no longer share the default foundset with forms of the same datasource, use loadAllRecords to restore the default foundset
controller.loadRecords(order_to_orderdetails);
```

### loadRecords(foundset)

Loads a (related) foundset into the form. The form will no longer share the default foundset with forms of the same datasource, use loadAllRecords to restore the default foundset.

This will really update the foundset instance itself of the form, so now existing foundset is altered just the new foundset is shown. This is different then doing foundset.loadRecords(foundset) because that just alters the current foundset and doesn't do anything with the foundset that is given.

When the form uses a seperate foundset, foundset filter params are copied over from the source foundset and are merged with the existing filters.

**Parameters**\
[JSFoundSet](../../database-manager/jsfoundset.md) foundset to load

**Returns**\
[Boolean](../../js-lib/boolean.md) true if successful

**Sample**

```javascript
//to load a (related)foundset into the form.
//the form will no longer share the default foundset with forms of the same datasource, use loadAllRecords to restore the default foundset
controller.loadRecords(order_to_orderdetails);
```

### recreateUI()

Recreates the forms UI components, to reflect the latest solution model. Use this after altering the elements via solutionModel at the JSForm of this form.

**Returns**\
[Boolean](../../js-lib/boolean.md) true if successful

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

Start the database search and use the results, returns the number of records, make sure you did "find" function first. Clear results from previous searches.

Note: Omitted records are automatically excluded when performing a search - meaning that the foundset result by default will not include omitted records.

**Returns**\
[Number](../../js-lib/number.md) the recordCount

**Sample**

```javascript
var recordCount = foundset.search();
//var recordCount = foundset.search(false,false); //to extend foundset
```

### search(clearLastResults)

Start the database search and use the results, returns the number of records, make sure you did "find" function first. Reduce results from previous searches.

Note: Omitted records are automatically excluded when performing a search - meaning that the foundset result by default will not include omitted records.

**Parameters**\
[Boolean](../../js-lib/boolean.md) clearLastResults boolean, clear previous search, default true

**Returns**\
[Number](../../js-lib/number.md) the recordCount

**Sample**

```javascript
var recordCount = foundset.search();
//var recordCount = foundset.search(false,false); //to extend foundset
```

### search(clearLastResults, reduceSearch)

Start the database search and use the results, returns the number of records, make sure you did "find" function first.

Note: Omitted records are automatically excluded when performing a search - meaning that the foundset result by default will not include omitted records.

**Parameters**\
[Boolean](../../js-lib/boolean.md) clearLastResults boolean, clear previous search, default true\
[Boolean](../../js-lib/boolean.md) reduceSearch boolean, reduce (true) or extend (false) previous search results, default true

**Returns**\
[Number](../../js-lib/number.md) the recordCount

**Sample**

```javascript
var recordCount = foundset.search();
//var recordCount = foundset.search(false,false); //to extend foundset
```

### setDataProviderValue(dataprovider, value)

Sets the value based on a specified dataprovider name.

**Parameters**\
[String](../../js-lib/string.md) dataprovider the dataprovider name to set the value for\
[Object](../../js-lib/object.md) value the value to set in the dataprovider

**Returns**\
void

**Sample**

```javascript
controller.setDataProviderValue('contact_name','mycompany');
```

### setDesignMode(designMode)

Sets this form in designmode with param true, false will return to normal browse/edit mode.

**Parameters**\
[Boolean](../../js-lib/boolean.md) designMode sets form in design mode if true, false ends design mode.

**Returns**\
void

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
[Function](../../js-lib/function.md) ondrag onDrag method reference

**Returns**\
void

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
[Function](../../js-lib/function.md) ondrag onDrag method reference\
[Function](../../js-lib/function.md) ondrop onDrop method reference

**Returns**\
void

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
[Function](../../js-lib/function.md) ondrag onDrag method reference\
[Function](../../js-lib/function.md) ondrop onDrop method reference\
[Function](../../js-lib/function.md) onselect onSelect method reference

**Returns**\
void

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
[Function](../../js-lib/function.md) ondrag onDrag method reference\
[Function](../../js-lib/function.md) ondrop onDrop method reference\
[Function](../../js-lib/function.md) onselect onSelect method reference\
[Function](../../js-lib/function.md) onresize onResize method reference

**Returns**\
void

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
[Function](../../js-lib/function.md) ondrag onDrag method reference\
[Function](../../js-lib/function.md) ondrop onDrop method reference\
[Function](../../js-lib/function.md) onselect onSelect method reference\
[Function](../../js-lib/function.md) onresize onResize method reference\
[Function](../../js-lib/function.md) ondblclick onDblClick method reference

**Returns**\
void

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
[Function](../../js-lib/function.md) ondrag onDrag method reference\
[Function](../../js-lib/function.md) ondrop onDrop method reference\
[Function](../../js-lib/function.md) onselect onSelect method reference\
[Function](../../js-lib/function.md) onresize onResize method reference\
[Function](../../js-lib/function.md) ondblclick onDblClick method reference\
[Function](../../js-lib/function.md) onrightclick onRightClick method reference

**Returns**\
void

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

### setSelectedIndex(index)

Sets the current record index of the current foundset.

**Parameters**\
[Number](../../js-lib/number.md) index the index to select

**Returns**\
void

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
[Array](../../js-lib/array.md) arrayOfElements array containing the element references

**Returns**\
void

**Sample**

```javascript
controller.setTabSequence([elements.fld_order_id, elements.fld_order_amount]);
```

### show()

Shows the form (makes the form visible) This function does not affect the form foundset in any way.

**Returns**\
void

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

Shows the form (makes the form visible) This function does not affect the form foundset in any way.

**Parameters**\
[JSWindow](../../application/jswindow.md) window the window in which this form should be shown, given as a window object

**Returns**\
void

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

Shows the form (makes the form visible) This function does not affect the form foundset in any way.

**Parameters**\
[String](../../js-lib/string.md) window the window in which this form should be shown, specified by the name of an existing window

**Returns**\
void

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

### showRecords(foundset)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[JSFoundSet](../../database-manager/jsfoundset.md) foundset the foundset to load before showing the form.

**Returns**\
void

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
[JSFoundSet](../../database-manager/jsfoundset.md) foundset the foundset to load before showing the form.\
[JSWindow](../../application/jswindow.md) window the window in which this form should be shown, given as a window object.

**Returns**\
void

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
[JSFoundSet](../../database-manager/jsfoundset.md) foundset the foundset to load before showing the form.\
[String](../../js-lib/string.md) window the window in which this form should be shown, specified by the name of an existing window.

**Returns**\
void

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
[JSDataSet](../../database-manager/jsdataset.md) pkdataset the pkdataset to load before showing the form.

**Returns**\
void

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
[JSDataSet](../../database-manager/jsdataset.md) pkdataset the pkdataset to load before showing the form.\
[JSWindow](../../application/jswindow.md) window the window in which this form should be shown, given as a window object.

**Returns**\
void

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
[JSDataSet](../../database-manager/jsdataset.md) pkdataset the pkdataset to load before showing the form.\
[String](../../js-lib/string.md) window the window in which this form should be shown, specified by the name of an existing window.

**Returns**\
void

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
[QBSelect](../../database-manager/qbselect.md) query the query to load before showing the form.

**Returns**\
void

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
[QBSelect](../../database-manager/qbselect.md) query the query to load before showing the form.\
[JSWindow](../../application/jswindow.md) window the window in which this form should be shown, given as a window object.

**Returns**\
void

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
[QBSelect](../../database-manager/qbselect.md) query the query to load before showing the form.\
[String](../../js-lib/string.md) window the window in which this form should be shown, specified by the name of an existing window.

**Returns**\
void

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
[UUID](../../application/uuid.md) UUIDpk the UUIDpk to load before showing the form.

**Returns**\
void

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
[UUID](../../application/uuid.md) UUIDpk the UUIDpk to load before showing the form.\
[JSWindow](../../application/jswindow.md) window the window in which this form should be shown, given as a window object.

**Returns**\
void

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
[UUID](../../application/uuid.md) UUIDpk the UUIDpk to load before showing the form.\
[String](../../js-lib/string.md) window the window in which this form should be shown, specified by the name of an existing window.

**Returns**\
void

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

### showRecords(singleNumber\_pk)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[Number](../../js-lib/number.md) singleNumber\_pk the singleNumber\_pk to load before showing the form.

**Returns**\
void

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

### showRecords(singleNumber\_pk, window)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[Number](../../js-lib/number.md) singleNumber\_pk the singleNumber\_pk to load before showing the form.\
[JSWindow](../../application/jswindow.md) window the window in which this form should be shown, given as a window object

**Returns**\
void

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

### showRecords(singleNumber\_pk, window)

Load data into the form and shows the form, is a shortcut for the functions 'loadRecords' and 'show'.

**Parameters**\
[Number](../../js-lib/number.md) singleNumber\_pk the singleNumber\_pk to load before showing the form.\
[String](../../js-lib/string.md) window the window in which this form should be shown, specified by the name of an existing window.

**Returns**\
void

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
[String](../../js-lib/string.md) query the query to load before showing the form.

**Returns**\
void

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
[String](../../js-lib/string.md) query the query to load before showing the form.\
[JSWindow](../../application/jswindow.md) window the window in which this form should be shown, given as a window object

**Returns**\
void

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
[String](../../js-lib/string.md) query the query to load before showing the form.\
[Array](../../js-lib/array.md) argumentsArray the array of arguments for the query

**Returns**\
void

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
[String](../../js-lib/string.md) query the query to load before showing the form.\
[Array](../../js-lib/array.md) argumentsArray the array of arguments for the query\
[JSWindow](../../application/jswindow.md) window the window in which this form should be shown, given as a window object

**Returns**\
void

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
[String](../../js-lib/string.md) query the query to load before showing the form.\
[Array](../../js-lib/array.md) argumentsArray the array of arguments for the query\
[String](../../js-lib/string.md) window the window in which this form should be shown, specified by the name of an existing window.

**Returns**\
void

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
[String](../../js-lib/string.md) query the query to load before showing the form.\
[String](../../js-lib/string.md) window the window in which this form should be shown, specified by the name of an existing window.

**Returns**\
void

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
