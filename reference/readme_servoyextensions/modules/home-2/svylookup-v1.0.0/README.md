# svyLookup v1

### Reference Guides

* [**API Documentation v1.0.0**](api-documentation-v1.0.0.md)
* [**Base Form svyLookupTable v1.0.0**](base-form-svylookuptable.md)
* [**Base Form AbstractLookup v1.0.0**](base-form-abstractlookup-v1.0.0.md)

### Overview

The svyLookup module provides a UX pattern for quickly finding and returning a record. It is similar to a type-ahead field, but allows for an extended UI, searching and data-binding.

This module provides an out-of-the-box grid implementation, but is also extensible to allow for other UI types

This [**quick screencast**](https://www.screencast.com/t/fxtRsOho) shows the example

### Example

![Example Look-Up](../../../../../extensions/modules/svyLookup/screenshots/lookup.png)

### Example Usage

It takes just a few lines of code to configure and show a robust lookup component. The selected record can be handled in a callback.

#### Show Lookup

```
       // create lookup object
	var lookupObj = scopes.svyLookup.createLookup(datasources.db.example_data.products.getDataSource());
	
	// add fields
	
	// related data is supported
	lookupObj.addField('products_to_categories.categoryname').setTitleText('Category');
	lookupObj.addField('productname').setTitleText('Product');
	lookupObj.addField('products_to_suppliers.companyname').setTitleText('Supplier');
	
	// Valuelists and non-searchable fields supported
	lookupObj.addField('discontinued')
		.setTitleText('Available')
		.setSearchable(false)
		.setvalueListName('product_availability');
	
	// formatted, non-searchable field example
	lookupObj.addField('unitprice')
		.setSearchable(false)
		.setTitleText('Price')
		.setFormat('#,###.00')
	
	// show pop-up
	var component = elements.productID;
	var initialValue = application.getValueListDisplayValue(elements.productID.getValueListName(),selectedProductID);
	lookupObj.showPopUp(onSelect,component,null,null,initialValue);
```

#### Handle selection in callback

```
	function onSelect(record){
		if(record){
			selectedProductID = record.productid
		}
	}
```
