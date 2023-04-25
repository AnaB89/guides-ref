# API Documentation 2

### Classes

[Lookup](API-Documentation-new2.md#lookup)

### Functions

[createLookup(dataSource)](API-Documentation-new2.md#createlookup-datasource-lookup) ⇒ [`Lookup`](API-Documentation-new2.md#lookup)

Creates a lookup object which can be used to show a pop-up form

[createQueryLookup(qbSelect, \[dsName\], \[overrideData\])](API-Documentation-new2.md#createquerylookup-qbselect-dsname-overridedata-lookup) ⇒ [`Lookup`](API-Documentation-new2.md#lookup)

Creates a read only, in-memory datasource from the given query and creates a Lookup for that

[createValueListLookup(valuelistName, \[titleText\])](API-Documentation-new2.md#createvaluelistlookup-valuelistname-titletext-lookup) ⇒ [`Lookup`](API-Documentation-new2.md#lookup)

Creates a lookup object from a valuelist which can be used to show a pop-up form or a modal window

NOTE: Valuelist cannot be based on a database relation or a global method. Custom Valuelists can show up to **500** items in lookup.

### Lookup

* [Lookup](API-Documentation-new2.md#Lookup)
  * [.addField(dataProvider)](API-Documentation-new2.md#lookup.addfield-dataprovider-lookupfield) ⇒ [`LookupField`](API-Documentation-new2.md#new\_LookupField\_new)
  * [.addParam(param)](API-Documentation-new2.md#lookup.addparam-param)
  * [.addSelectedRecord(record)](API-Documentation-new2.md#lookup.addselectedrecord-record)
  * [.clearParams()](API-Documentation-new2.md#lookup.clearparams)
  * [.clearSelectedRecords()](API-Documentation-new2.md#lookup.clearselectedrecords)
  * [.createPopUp(callback, \[initialValue\])](API-Documentation-new2.md#lookup.createpopup-callback-initialvalue-plugins.window.formpopup) ⇒ `plugins.window.FormPopup`
  * [.createWindow(\[x\], \[y\], \[width\], \[height\], \[jsWindowType\])](API-Documentation-new2.md#lookup.createwindow-x-y-width-height-jswindowtype-jswindow) ⇒ `JSWindow`
  * [.getDataSource()](API-Documentation-new2.md#lookup.getdatasource-string) ⇒ `String`
  * [.getField(index)](API-Documentation-new2.md#lookup.getfield-index-lookupfield) ⇒ [`LookupField`](API-Documentation-new2.md#new\_LookupField\_new)
  * [.getFieldCount()](API-Documentation-new2.md#lookup.getfieldcount-number) ⇒ `Number`
  * [.getFoundSet()](API-Documentation-new2.md#lookup.getfoundset-jsfoundset) ⇒ `JSFoundSet`
  * [.getLookupDataProvider()](API-Documentation-new2.md#lookup.getlookupdataprovider-string) ⇒ `String`
  * [.getLookupForm()](API-Documentation-new2.md#lookup.getlookupform-runtimeform-.less-than-abstractlookup-greater-than) ⇒ `[ 'RuntimeForm' ].<AbstractLookup>`
  * [.getParams()](API-Documentation-new2.md#lookup.getparams-array) ⇒ `Array`
  * [.getSelectedRecords()](API-Documentation-new2.md#lookup.getselectedrecords-array-.less-than-jsrecord-greater-than) ⇒ `[ 'Array' ].<JSRecord>`
  * [.getSelectedValues()](API-Documentation-new2.md#lookup.getselectedvalues-array-.less-than-jsrecord-greater-than) ⇒ `[ 'Array' ].<JSRecord>`
  * [.removeField(index)](API-Documentation-new2.md#lookup.removefield-index)
  * [.removeParam(index)](API-Documentation-new2.md#lookup.removeparam-index)
  * [.removeSelectedRecord(record)](API-Documentation-new2.md#lookup.removeselectedrecord-record)
  * [.setLookupDataProvider(dataProvider)](API-Documentation-new2.md#lookup.setlookupdataprovider-dataprovider)
  * [.setLookupForm(lookupForm)](API-Documentation-new2.md#lookup.setlookupform-lookupform)
  * [.setMultiSelect(multiSelect)](API-Documentation-new2.md#lookup.setmultiselect-multiselect-lookup) ⇒ [`Lookup`](API-Documentation-new2.md#Lookup)
  * [.setSelectedPks(pks)](API-Documentation-new2.md#lookup.setselectedpks-pks)
  * [.setSelectedRecords(records)](API-Documentation-new2.md#lookup.setselectedrecords-records)
  * [.setSelectedValues(values)](API-Documentation-new2.md#lookup.setselectedvalues-values)
  * [.showModalWindow(\[callback\], \[x\], \[y\], \[width\], \[height\], \[initialValue\])](API-Documentation-new2.md#lookup.showmodalwindow-callback-x-y-width-height-initialvalue-array.less-than-jsrecord-greater-than) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`
  * [.showPopUp(callback, target, \[width\], \[height\], \[initialValue\])](API-Documentation-new2.md#lookup.showpopup-callback-target-width-height-initialvalue)
  * [.showWindow(win, \[callback\], \[initialValue\])](API-Documentation-new2.md#lookup.showwindow-win-callback-initialvalue-array.less-than-jsrecord-greater-than-or-array.less-than) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`
  * [new Lookup(datasource)](API-Documentation-new2.md#new-lookup-datasource)

***

#### lookup.addField(dataProvider) ⇒ [`LookupField`](API-Documentation-new2.md#new\_LookupField\_new)

Adds a field to the lookup object

| Param        | Type     |
| ------------ | -------- |
| dataProvider | `String` |

**Example**

```js
var lookupObj = scopes.svyLookup.createLookup(datasources.db.example_data.products.getDataSource());

lookupObj.addField('productname').setTitleText('Product');
lookupObj.addField('products_to_suppliers.companyname').setTitleText('Supplier');
lookupObj.addField('unitprice')
	.setSearchable(false)
	.setTitleText('Price')
	.setFormat('#,###.00')
```

***

#### lookup.addParam(param)

Add a params to be added into the onSelect callback arguments

| Param | Type     |
| ----- | -------- |
| param | `Object` |

**Example**

```js
// create lookup object
var lookupObj = scopes.svyLookup.createLookup(datasources.db.example_data.products.getDataSource());
lookupObj.setLookupDataProvider("productname");

// custom param, define to which dataprovider the lookup result should be assigned
lookupObj.addParam({resultDataProvider: "productfk"});
lookupObj.showPopUp(onSelect, elements.productfk);

function onSelect(records, values, lookup) {
	if (values && values.length) {
		var resultDataProvider = lookup.getParams()[0].resultDataProvider;
		foundset[resultDataProvider] = values[0];
	}
}
```

***

#### lookup.addSelectedRecord(record)

Adds the given record to the list of selected records

| Param  | Type       |
| ------ | ---------- |
| record | `JSRecord` |

***

#### lookup.clearParams()

Clear the params

***

#### lookup.clearSelectedRecords()

Clears the selection of this Lookup

***

#### lookup.createPopUp(callback, \[initialValue]) ⇒ `plugins.window.FormPopup`

Creates and returns a Popup Form to be used to show the lookup

| Param           | Type       | Description                                                                                                                             |
| --------------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| callback        | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| \[initialValue] | `String`   | And initial value to show in the search                                                                                                 |

***

#### lookup.createWindow(\[x], \[y], \[width], \[height], \[jsWindowType]) ⇒ `JSWindow`

**Returns**: `JSWindow` - returns a JSWindow which can be used to show the lookup in it using lookup.showWindow(window)

| Param           | Type     | Description                                                                     |
| --------------- | -------- | ------------------------------------------------------------------------------- |
| \[x]            | `Number` |                                                                                 |
| \[y]            | `Number` |                                                                                 |
| \[width]        | `Number` | The width of the pop-up. Optional. Default is component width                   |
| \[height]       | `Number` | The height of the pop-up. Optional. Default is form height.                     |
| \[jsWindowType] | `Number` | Type of window; should be an option of JSWindow, Default JSWindow.MODAL\_DIALOG |

***

#### lookup.getDataSource() ⇒ `String`

Gets the data source for this Lookup object

***

#### lookup.getField(index) ⇒ [`LookupField`](API-Documentation-new2.md#new\_LookupField\_new)

Gets the field at the specified index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

***

#### lookup.getFieldCount() ⇒ `Number`

Gets the number of fields in the lookup object

***

#### lookup.getFoundSet() ⇒ `JSFoundSet`

Gets the foundset for this Lookup object.

***

#### lookup.getLookupDataProvider() ⇒ `String`

Gets the lookup dataprovider

***

#### lookup.getLookupForm() ⇒ `[ 'RuntimeForm' ].<AbstractLookup>`

Returns the Lookup form instance used

***

#### lookup.getParams() ⇒ `Array`

**Example**

```js
// create lookup object
var lookupObj = scopes.svyLookup.createLookup(datasources.db.example_data.products.getDataSource());
lookupObj.setLookupDataProvider("productname");

// custom param, define to which dataprovider the lookup result should be assigned
lookupObj.addParam({resultDataProvider: "productfk"});
lookupObj.showPopUp(onSelect, elements.productfk);

function onSelect(records, values, lookup) {
	if (values && values.length) {
		var resultDataProvider = lookup.getParams()[0].resultDataProvider;
		foundset[resultDataProvider] = values[0];
	}
}
```

***

#### lookup.getSelectedRecords() ⇒ `[ 'Array' ].<JSRecord>`

Returns the selected records for the lookup object Can be used to know which records have been previously selected by the user for this lookup

***

#### lookup.getSelectedValues() ⇒ `[ 'Array' ].<JSRecord>`

Returns the selected values based on the lookupDataProvider based on the lookupFormProvider. Can be used to know which values have been previously selected by the user for this lookup.

throws an exception if the lookupDataProvider has not been set

***

#### lookup.removeField(index)

Removes a field at the specified index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

***

#### lookup.removeParam(index)

Removes a param at the specified index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

***

#### lookup.removeSelectedRecord(record)

Removes the given record from the list of selected records

| Param  | Type       |
| ------ | ---------- |
| record | `JSRecord` |

***

#### lookup.setLookupDataProvider(dataProvider)

Sets the lookup dataprovider Has to be a dataprovider or a related dataprovider of the lookup dataSource Setting the lookup dataprovider will return the selected dataprovider values in the lookup callback

| Param        | Type     |
| ------------ | -------- |
| dataProvider | `String` |

**Example**

```js
var lookupObj = scopes.svyLookup.createLookup(datasources.db.example_data.products.getDataSource());
// set the lookup dataprovider to productid
lookupObj.setLookupDataProvider("productid");

// add fields
lookupObj.addField('productname').setTitleText('Product');
lookupObj.addField('products_to_suppliers.companyname').setTitleText('Supplier');
lookupObj.addField('unitprice')
	.setSearchable(false)
	.setTitleText('Price')
	.setFormat('#,###.00')
		
// show pop-up
lookupObj.showPopUp(onSelect, elements.setProduct, controller.getFormWidth()/2, 412);

//because i have set the lookupDataProvider as productid values contains the selected productid (if any selected)
function onSelect(record, values, lookup){
  if (values && values.length) {
	  foundset.productid = values[0];
  }
}
```

***

#### lookup.setLookupForm(lookupForm)

Sets the lookup form used as template for the lookup popup/dialog The lookup form must extend the abstract form AbstractLookup

| Param      | Type                                 |
| ---------- | ------------------------------------ |
| lookupForm | `[ 'RuntimeForm' ].<AbstractLookup>` |

**Example**

```js
var lookupObj = scopes.svyLookup.createLookup(datasources.db.example_data.products.getDataSource());
// lookup template with NG Table
lookupObj.setLookupForm(forms.svyLookupNGTable);

var lookupObjMulti = scopes.svyLookup.createLookup(datasources.db.example_data.products.getDataSource());
lookupObjMulti.setMultiSelect(true);
// lookup template with NG Table
lookupObjMulti.setLookupForm(forms.svyLookupNGTableMulti);
```

***

#### lookup.setMultiSelect(multiSelect) ⇒ [`Lookup`](API-Documentation-new2.md#lookup)

Allows this Lookup to multi select records The lookup form used will be changed when the instance set does not match the multi select setting

| Param       | Type      |
| ----------- | --------- |
| multiSelect | `Boolean` |

***

#### lookup.setSelectedPks(pks)

Sets the selected records of this Lookup from the given primary keys Can be used to restore the user's selection from a previous user's session

| Param | Type              |
| ----- | ----------------- |
| pks   | `[ 'Array' ].<*>` |

***

#### lookup.setSelectedRecords(records)

Sets the selected records of this Lookup Can be used to restore the user's selection from a previous user's session

| Param   | Type                     |
| ------- | ------------------------ |
| records | `[ 'Array' ].<JSRecord>` |

***

#### lookup.setSelectedValues(values)

| Param  | Type              |
| ------ | ----------------- |
| values | `[ 'Array' ].<*>` |

***

#### lookup.showModalWindow(\[callback], \[x], \[y], \[width], \[height], \[initialValue]) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`

Shows the lookup in a modal Window

**Returns**: `Array.<JSRecord>` | `Array.<(String|Date|Number)>` - returns the selected records; if the lookupDataprovider has been set instead it returns the lookupDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection

| Param           | Type       | Description                                                                                                                             |
| --------------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| \[callback]     | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| \[x]            | `Number`   |                                                                                                                                         |
| \[y]            | `Number`   |                                                                                                                                         |
| \[width]        | `Number`   | The width of the lookup. Optional. Default is same as target component                                                                  |
| \[height]       | `Number`   | The height of the lookup. Optional. Default is implementation-specifc.                                                                  |
| \[initialValue] | `String`   | And initial value to show in the search                                                                                                 |

***

#### lookup.showPopUp(callback, target, \[width], \[height], \[initialValue])

Shows the lookup as a Popup Form

| Param           | Type               | Description                                                                                                                             |
| --------------- | ------------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| callback        | `function`         | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| target          | `RuntimeComponent` | The component to show relative to                                                                                                       |
| \[width]        | `Number`           | The width of the lookup. Optional. Default is same as target component                                                                  |
| \[height]       | `Number`           | The height of the lookup. Optional. Default is implementation-specifc.                                                                  |
| \[initialValue] | `String`           | And initial value to show in the search                                                                                                 |

***

#### lookup.showWindow(win, \[callback], \[initialValue]) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`

Shows the lookup in a Window

**Returns**: `Array.<JSRecord>` | `Array.<(String|Date|Number)>` - returns the selected records; if the lookupDataprovider has been set instead it returns the lookupDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection

| Param           | Type       | Description                                                                                                                             |
| --------------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| win             | `JSWindow` | the JSWindow object to show                                                                                                             |
| \[callback]     | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| \[initialValue] | `String`   | And initial value to show in the search                                                                                                 |

***

#### new Lookup(datasource)

| Param      | Type                     |
| ---------- | ------------------------ |
| datasource | `String` \| `JSFoundSet` |

***

### createLookup(dataSource) ⇒ [`Lookup`](API-Documentation-new2.md#lookup)

Creates a lookup object which can be used to show a pop-up form

| Param      | Type                                   | Description               |
| ---------- | -------------------------------------- | ------------------------- |
| dataSource | `String` \| `JSFoundSet` \| `JSRecord` | The data source to lookup |

**Example**

```js
function onActionAddProducts(event) {
	var lookupObj = scopes.svyLookup.createLookup(datasources.db.example_data.products.getDataSource());

 // allow multi-selection
	lookupObj.setMultiSelect(true);
	
	// add searchable fields 
	lookupObj.addField('productname').setTitleText('Product');
	lookupObj.addField('products_to_suppliers.companyname').setTitleText('Supplier');
	lookupObj.addField('unitprice')
		.setSearchable(false)
		.setTitleText('Price')
		.setFormat('#,###.00')
	
	// show pop-up
	lookupObj.showPopUp(onSelect, elements.btnNewProduct, controller.getFormWidth()/2, 412);
}

// lookup callback. Add products into current order 
function onSelect(records, values, lookup){
	if(records){
		records.forEach(function(rec){
			
			if(foundset.selectRecord(foundset.orderid,rec.productid)) {
				// increase quantity if product already in order
				foundset.quantity = foundset.quantity + 1;
			} else {
				// create a new order line for each product selected in lookup
				var newRec = foundset.getRecord(foundset.newRecord())
				newRec.discount = 0;
				newRec.quantity = 1;
				newRec.unitprice = rec.unitprice;
				newRec.productid = rec.productid;
			}
		})
	 }
}
```

***

### createQueryLookup(qbSelect, \[dsName], \[overrideData]) ⇒ [`Lookup`](API-Documentation-new2.md#lookup)

Creates a read only, in-memory datasource from the given query and creates a Lookup for that

| Param           | Type       | Description                                                                                                                                                                            |
| --------------- | ---------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| qbSelect        | `QBSelect` | the query                                                                                                                                                                              |
| \[dsName]       | `String`   | the name of the datasource in case it should be reused                                                                                                                                 |
| \[overrideData] | `Boolean`  | when true, the datasource with the given name is filled again from the given query, when false, an existing datasource with the same datasource name would be reused; default is false |

**Example**

```js
  //distinct query for the value
  var qbSelect = datasources.db.example_data.order_details.createSelect();
  qbSelect.result.add(qbSelect.joins.order_details_to_products.columns.productname, "productname");
  qbSelect.result.add(qbSelect.columns.productid, "productid");
  qbSelect.result.distinct = true;
  qbSelect.sort.add(qbSelect.joins.order_details_to_products.columns.productname);

  //create lookup and set form provider
  var lookupObj = scopes.svyLookup.createQueryLookup(qbSelect, 'ordered_products');
  
  //set proper header title for field
  var lookupField = lookupObj .getField(0);
  lookupField.setTitleText("Product");
  
  // show the lookup
  lookupObj.showPopUp(onSelect, elements.productid);

  // handle selection
  function onSelect(records, values, lookup) {
	    var selectedLookupValues = records.length ? records[0].productid : null;
  }
```

***

### createValueListLookup(valuelistName, \[titleText]) ⇒ [`Lookup`](API-Documentation-new2.md#lookup)

Creates a lookup object from a valuelist which can be used to show a pop-up form or a modal window

NOTE: Valuelist cannot be based on a database relation or a global method. Custom Valuelists can show up to **500** items in lookup.

| Param         | Type                         | Description                                                                                                                                                                                                                                                                                 |
| ------------- | ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| valuelistName | `String`                     |                                                                                                                                                                                                                                                                                             |
| \[titleText]  | `String` \| `Array.<String>` | Sets the display text for the valuelist field(s). Default is 'Value' or the column names; TODO should i allow to override the valuelist displayvalue, realvalue dataproviders. Could be handy because the lookup returns the record and the user has no clue about displayvalue/realvalue ? |

**Example**

```js
// create the lookup using the valuelist productsTable
var lookupObj = scopes.svyLookup.createValueListLookup("productsTable", "Product");

// show the lookup
lookupObj .showPopUp(onSelect, elements.productid);

// handle selection
function onSelect(records, values, lookup) {
	 var selectedLookupValues = values.length ? values[0] : null;
}
```

***
