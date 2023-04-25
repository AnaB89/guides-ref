## Classes

<dl>
<dt><a href="#Lookup">Lookup</a></dt>
<dd></dd>
</dl>

## Functions

<dl>
<dt><a href="#createLookup">createLookup(dataSource)</a> ⇒ <code><a href="#Lookup">Lookup</a></code></dt>
<dd><p>Creates a lookup object which can be used to show a pop-up form</p>
</dd>
<dt><a href="#createQueryLookup">createQueryLookup(qbSelect, [dsName], [overrideData])</a> ⇒ <code><a href="#Lookup">Lookup</a></code></dt>
<dd><p>Creates a read only, in-memory datasource from the given query and creates a Lookup for that</p>
</dd>
<dt><a href="#createValueListLookup">createValueListLookup(valuelistName, [titleText])</a> ⇒ <code><a href="#Lookup">Lookup</a></code></dt>
<dd><p>Creates a lookup object from a valuelist which can be used to show a pop-up form or a modal window</p>
<p>NOTE: Valuelist cannot be based on a database relation or a global method.
Custom Valuelists can show up to <strong>500</strong> items in lookup.</p>
</dd>
</dl>

<a name="Lookup"></a>

## Lookup


* [Lookup](#Lookup)
    * [.addField(dataProvider)](#Lookup+addField) ⇒ [<code>LookupField</code>](#new_LookupField_new)
    * [.addParam(param)](#Lookup+addParam)
    * [.addSelectedRecord(record)](#Lookup+addSelectedRecord)
    * [.clearParams()](#Lookup+clearParams)
    * [.clearSelectedRecords()](#Lookup+clearSelectedRecords)
    * [.createPopUp(callback, [initialValue])](#Lookup+createPopUp) ⇒ <code>plugins.window.FormPopup</code>
    * [.createWindow([x], [y], [width], [height], [jsWindowType])](#Lookup+createWindow) ⇒ <code>JSWindow</code>
    * [.getDataSource()](#Lookup+getDataSource) ⇒ <code>String</code>
    * [.getField(index)](#Lookup+getField) ⇒ [<code>LookupField</code>](#new_LookupField_new)
    * [.getFieldCount()](#Lookup+getFieldCount) ⇒ <code>Number</code>
    * [.getFoundSet()](#Lookup+getFoundSet) ⇒ <code>JSFoundSet</code>
    * [.getLookupDataProvider()](#Lookup+getLookupDataProvider) ⇒ <code>String</code>
    * [.getLookupForm()](#Lookup+getLookupForm) ⇒ <code>[ &#x27;RuntimeForm&#x27; ].&lt;AbstractLookup&gt;</code>
    * [.getParams()](#Lookup+getParams) ⇒ <code>Array</code>
    * [.getSelectedRecords()](#Lookup+getSelectedRecords) ⇒ <code>[ &#x27;Array&#x27; ].&lt;JSRecord&gt;</code>
    * [.getSelectedValues()](#Lookup+getSelectedValues) ⇒ <code>[ &#x27;Array&#x27; ].&lt;JSRecord&gt;</code>
    * [.removeField(index)](#Lookup+removeField)
    * [.removeParam(index)](#Lookup+removeParam)
    * [.removeSelectedRecord(record)](#Lookup+removeSelectedRecord)
    * [.setLookupDataProvider(dataProvider)](#Lookup+setLookupDataProvider)
    * [.setLookupForm(lookupForm)](#Lookup+setLookupForm)
    * [.setMultiSelect(multiSelect)](#Lookup+setMultiSelect) ⇒ [<code>Lookup</code>](#Lookup)
    * [.setSelectedPks(pks)](#Lookup+setSelectedPks)
    * [.setSelectedRecords(records)](#Lookup+setSelectedRecords)
    * [.setSelectedValues(values)](#Lookup+setSelectedValues)
    * [.showModalWindow([callback], [x], [y], [width], [height], [initialValue])](#Lookup+showModalWindow) ⇒ <code>Array.&lt;JSRecord&gt;</code> \| <code>Array.&lt;(String\|Date\|Number)&gt;</code>
    * [.showPopUp(callback, target, [width], [height], [initialValue])](#Lookup+showPopUp)
    * [.showWindow(win, [callback], [initialValue])](#Lookup+showWindow) ⇒ <code>Array.&lt;JSRecord&gt;</code> \| <code>Array.&lt;(String\|Date\|Number)&gt;</code>
    * [new Lookup(datasource)](#new_Lookup_new)


* * *

<a name="Lookup+addField"></a>

### lookup.addField(dataProvider) ⇒ [<code>LookupField</code>](#new_LookupField_new)
Adds a field to the lookup object



| Param | Type |
| --- | --- |
| dataProvider | <code>String</code> | 

**Example**  
```js
<pre>
var lookupObj = scopes.svyLookup.createLookup(datasources.db.example_data.products.getDataSource());

lookupObj.addField('productname').setTitleText('Product');
lookupObj.addField('products_to_suppliers.companyname').setTitleText('Supplier');
lookupObj.addField('unitprice')
	.setSearchable(false)
	.setTitleText('Price')
	.setFormat('#,###.00')
</pre>
```

* * *

<a name="Lookup+addParam"></a>

### lookup.addParam(param)
Add a params to be added into the onSelect callback arguments



| Param | Type |
| --- | --- |
| param | <code>Object</code> | 

**Example**  
```js
<pre>
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
</pre>
```

* * *

<a name="Lookup+addSelectedRecord"></a>

### lookup.addSelectedRecord(record)
Adds the given record to the list of selected records



| Param | Type |
| --- | --- |
| record | <code>JSRecord</code> | 


* * *

<a name="Lookup+clearParams"></a>

### lookup.clearParams()
Clear the params



* * *

<a name="Lookup+clearSelectedRecords"></a>

### lookup.clearSelectedRecords()
Clears the selection of this Lookup



* * *

<a name="Lookup+createPopUp"></a>

### lookup.createPopUp(callback, [initialValue]) ⇒ <code>plugins.window.FormPopup</code>
Creates and returns a Popup Form to be used to show the lookup



| Param | Type | Description |
| --- | --- | --- |
| callback | <code>function</code> | The function that will be called when a selection is made; the callback returns the following arguments: {Array<JSRecord>} record, {Array<String|Date|Number>} lookupValue , {Lookup} lookup |
| [initialValue] | <code>String</code> | And initial value to show in the search |


* * *

<a name="Lookup+createWindow"></a>

### lookup.createWindow([x], [y], [width], [height], [jsWindowType]) ⇒ <code>JSWindow</code>
**Returns**: <code>JSWindow</code> - returns a JSWindow which can be used to show the lookup in it using lookup.showWindow(window)  


| Param | Type | Description |
| --- | --- | --- |
| [x] | <code>Number</code> |  |
| [y] | <code>Number</code> |  |
| [width] | <code>Number</code> | The width of the pop-up. Optional. Default is component width |
| [height] | <code>Number</code> | The height of the pop-up. Optional. Default is form height. |
| [jsWindowType] | <code>Number</code> | Type of window; should be an option of JSWindow, Default JSWindow.MODAL_DIALOG |


* * *

<a name="Lookup+getDataSource"></a>

### lookup.getDataSource() ⇒ <code>String</code>
Gets the data source for this Lookup object



* * *

<a name="Lookup+getField"></a>

### lookup.getField(index) ⇒ [<code>LookupField</code>](#new_LookupField_new)
Gets the field at the specified index



| Param | Type |
| --- | --- |
| index | <code>Number</code> | 


* * *

<a name="Lookup+getFieldCount"></a>

### lookup.getFieldCount() ⇒ <code>Number</code>
Gets the number of fields in the lookup object



* * *

<a name="Lookup+getFoundSet"></a>

### lookup.getFoundSet() ⇒ <code>JSFoundSet</code>
Gets the foundset for this Lookup object.



* * *

<a name="Lookup+getLookupDataProvider"></a>

### lookup.getLookupDataProvider() ⇒ <code>String</code>
Gets the lookup dataprovider



* * *

<a name="Lookup+getLookupForm"></a>

### lookup.getLookupForm() ⇒ <code>[ &#x27;RuntimeForm&#x27; ].&lt;AbstractLookup&gt;</code>
Returns the Lookup form instance used



* * *

<a name="Lookup+getParams"></a>

### lookup.getParams() ⇒ <code>Array</code>

**Example**  
```js
<pre>
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
</pre>
```

* * *

<a name="Lookup+getSelectedRecords"></a>

### lookup.getSelectedRecords() ⇒ <code>[ &#x27;Array&#x27; ].&lt;JSRecord&gt;</code>
Returns the selected records for the lookup object
Can be used to know which records have been previously selected by the user for this lookup



* * *

<a name="Lookup+getSelectedValues"></a>

### lookup.getSelectedValues() ⇒ <code>[ &#x27;Array&#x27; ].&lt;JSRecord&gt;</code>
Returns the selected values based on the lookupDataProvider based on the lookupFormProvider.
Can be used to know which values have been previously selected by the user for this lookup.

 throws an exception if the lookupDataProvider has not been set



* * *

<a name="Lookup+removeField"></a>

### lookup.removeField(index)
Removes a field at the specified index



| Param | Type |
| --- | --- |
| index | <code>Number</code> | 


* * *

<a name="Lookup+removeParam"></a>

### lookup.removeParam(index)
Removes a param at the specified index



| Param | Type |
| --- | --- |
| index | <code>Number</code> | 


* * *

<a name="Lookup+removeSelectedRecord"></a>

### lookup.removeSelectedRecord(record)
Removes the given record from the list of selected records



| Param | Type |
| --- | --- |
| record | <code>JSRecord</code> | 


* * *

<a name="Lookup+setLookupDataProvider"></a>

### lookup.setLookupDataProvider(dataProvider)
Sets the lookup dataprovider
Has to be a dataprovider or a related dataprovider of the lookup dataSource
Setting the lookup dataprovider will return the selected dataprovider values in the lookup callback



| Param | Type |
| --- | --- |
| dataProvider | <code>String</code> | 

**Example**  
```js
<pre> 
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
</pre>
```

* * *

<a name="Lookup+setLookupForm"></a>

### lookup.setLookupForm(lookupForm)
Sets the lookup form used as template for the lookup popup/dialog
The lookup form must extend the abstract form AbstractLookup



| Param | Type |
| --- | --- |
| lookupForm | <code>[ &#x27;RuntimeForm&#x27; ].&lt;AbstractLookup&gt;</code> | 

**Example**  
```js
<pre>
var lookupObj = scopes.svyLookup.createLookup(datasources.db.example_data.products.getDataSource());
// lookup template with NG Table
lookupObj.setLookupForm(forms.svyLookupNGTable);

var lookupObjMulti = scopes.svyLookup.createLookup(datasources.db.example_data.products.getDataSource());
lookupObjMulti.setMultiSelect(true);
// lookup template with NG Table
lookupObjMulti.setLookupForm(forms.svyLookupNGTableMulti);
</pre>
```

* * *

<a name="Lookup+setMultiSelect"></a>

### lookup.setMultiSelect(multiSelect) ⇒ [<code>Lookup</code>](#Lookup)
Allows this Lookup to multi select records
The lookup form used will be changed when the instance set does not match the multi select setting



| Param | Type |
| --- | --- |
| multiSelect | <code>Boolean</code> | 


* * *

<a name="Lookup+setSelectedPks"></a>

### lookup.setSelectedPks(pks)
Sets the selected records of this Lookup from the given primary keys
Can be used to restore the user's selection from a previous user's session



| Param | Type |
| --- | --- |
| pks | <code>[ &#x27;Array&#x27; ].&lt;\*&gt;</code> | 


* * *

<a name="Lookup+setSelectedRecords"></a>

### lookup.setSelectedRecords(records)
Sets the selected records of this Lookup
Can be used to restore the user's selection from a previous user's session



| Param | Type |
| --- | --- |
| records | <code>[ &#x27;Array&#x27; ].&lt;JSRecord&gt;</code> | 


* * *

<a name="Lookup+setSelectedValues"></a>

### lookup.setSelectedValues(values)


| Param | Type |
| --- | --- |
| values | <code>[ &#x27;Array&#x27; ].&lt;\*&gt;</code> | 


* * *

<a name="Lookup+showModalWindow"></a>

### lookup.showModalWindow([callback], [x], [y], [width], [height], [initialValue]) ⇒ <code>Array.&lt;JSRecord&gt;</code> \| <code>Array.&lt;(String\|Date\|Number)&gt;</code>
Shows the lookup in a modal Window

**Returns**: <code>Array.&lt;JSRecord&gt;</code> \| <code>Array.&lt;(String\|Date\|Number)&gt;</code> - returns the selected records; if the lookupDataprovider has been set instead it returns the lookupDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection  


| Param | Type | Description |
| --- | --- | --- |
| [callback] | <code>function</code> | The function that will be called when a selection is made; the callback returns the following arguments: {Array<JSRecord>} record, {Array<String|Date|Number>} lookupValue , {Lookup} lookup |
| [x] | <code>Number</code> |  |
| [y] | <code>Number</code> |  |
| [width] | <code>Number</code> | The width of the lookup. Optional. Default is same as target component |
| [height] | <code>Number</code> | The height of the lookup. Optional. Default is implementation-specifc. |
| [initialValue] | <code>String</code> | And initial value to show in the search |


* * *

<a name="Lookup+showPopUp"></a>

### lookup.showPopUp(callback, target, [width], [height], [initialValue])
Shows the lookup as a Popup Form



| Param | Type | Description |
| --- | --- | --- |
| callback | <code>function</code> | The function that will be called when a selection is made; the callback returns the following arguments: {Array<JSRecord>} record, {Array<String|Date|Number>} lookupValue , {Lookup} lookup |
| target | <code>RuntimeComponent</code> | The component to show relative to |
| [width] | <code>Number</code> | The width of the lookup. Optional. Default is same as target component |
| [height] | <code>Number</code> | The height of the lookup. Optional. Default is implementation-specifc. |
| [initialValue] | <code>String</code> | And initial value to show in the search |


* * *

<a name="Lookup+showWindow"></a>

### lookup.showWindow(win, [callback], [initialValue]) ⇒ <code>Array.&lt;JSRecord&gt;</code> \| <code>Array.&lt;(String\|Date\|Number)&gt;</code>
Shows the lookup in a Window

**Returns**: <code>Array.&lt;JSRecord&gt;</code> \| <code>Array.&lt;(String\|Date\|Number)&gt;</code> - returns the selected records; if the lookupDataprovider has been set instead it returns the lookupDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection  


| Param | Type | Description |
| --- | --- | --- |
| win | <code>JSWindow</code> | the JSWindow object to show |
| [callback] | <code>function</code> | The function that will be called when a selection is made; the callback returns the following arguments: {Array<JSRecord>} record, {Array<String|Date|Number>} lookupValue , {Lookup} lookup |
| [initialValue] | <code>String</code> | And initial value to show in the search |


* * *

<a name="new_Lookup_new"></a>

### new Lookup(datasource)


| Param | Type |
| --- | --- |
| datasource | <code>String</code> \| <code>JSFoundSet</code> | 


* * *

<a name="createLookup"></a>

## createLookup(dataSource) ⇒ [<code>Lookup</code>](#Lookup)
Creates a lookup object which can be used to show a pop-up form



| Param | Type | Description |
| --- | --- | --- |
| dataSource | <code>String</code> \| <code>JSFoundSet</code> \| <code>JSRecord</code> | The data source to lookup |

**Example**  
```js
<pre>
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

</pre>
```

* * *

<a name="createQueryLookup"></a>

## createQueryLookup(qbSelect, [dsName], [overrideData]) ⇒ [<code>Lookup</code>](#Lookup)
Creates a read only, in-memory datasource from the given query and creates a Lookup for that



| Param | Type | Description |
| --- | --- | --- |
| qbSelect | <code>QBSelect</code> | the query |
| [dsName] | <code>String</code> | the name of the datasource in case it should be reused |
| [overrideData] | <code>Boolean</code> | when true, the datasource with the given name is filled again from the given query, when false, an existing datasource with the same datasource name would be reused; default is false |

**Example**  
```js
<pre>
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
  }</pre>
```

* * *

<a name="createValueListLookup"></a>

## createValueListLookup(valuelistName, [titleText]) ⇒ [<code>Lookup</code>](#Lookup)
Creates a lookup object from a valuelist which can be used to show a pop-up form or a modal window

NOTE: Valuelist cannot be based on a database relation or a global method.
Custom Valuelists can show up to **500** items in lookup.



| Param | Type | Description |
| --- | --- | --- |
| valuelistName | <code>String</code> |  |
| [titleText] | <code>String</code> \| <code>Array.&lt;String&gt;</code> | Sets the display text for the valuelist field(s). Default is 'Value' or the column names; TODO should i allow to override the valuelist displayvalue, realvalue dataproviders. Could be handy because the lookup returns the record and the user has no clue about displayvalue/realvalue ? |

**Example**  
```js
<pre>
// create the lookup using the valuelist productsTable
var lookupObj = scopes.svyLookup.createValueListLookup("productsTable", "Product");

// show the lookup
lookupObj .showPopUp(onSelect, elements.productid);

// handle selection
function onSelect(records, values, lookup) {
	 var selectedLookupValues = values.length ? values[0] : null;
}
</pre>
```

* * *

