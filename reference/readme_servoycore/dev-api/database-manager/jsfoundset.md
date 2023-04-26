# JSFoundSet

## Property Summary

| Type                            | Name                                               | Summary                                           |
| ------------------------------- | -------------------------------------------------- | ------------------------------------------------- |
| [Array](../js-lib/array.md)     | [alldataproviders](jsfoundset.md#alldataproviders) | Get all dataproviders of the foundset..           |
| [Boolean](../js-lib/boolean.md) | [multiSelect](jsfoundset.md#multiSelect)           | Get or set the multiSelect flag of the foundset.. |

## Methods Summary

| Type                            | Name                                                                                                                                 | Summary                                                                                                                                                                                        |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Boolean](../js-lib/boolean.md) | [addFoundSetFilterParam(query)](jsfoundset.md#addfoundsetfilterparam-query)                                                          | Add a filter parameter that is permanent per user session to limit a specified foundset of records..                                                                                           |
| [Boolean](../js-lib/boolean.md) | [addFoundSetFilterParam(query, name)](jsfoundset.md#addfoundsetfilterparam-query-name)                                               | Add a filter parameter that is permanent per user session to limit a specified foundset of records..                                                                                           |
| [Boolean](../js-lib/boolean.md) | [addFoundSetFilterParam(dataprovider, operator, value)](jsfoundset.md#addfoundsetfilterparam-dataprovider-operator-value)            | Add a filter parameter that is permanent per user session to limit a specified foundset of records..                                                                                           |
| [Boolean](../js-lib/boolean.md) | [addFoundSetFilterParam(dataprovider, operator, value, name)](jsfoundset.md#addfoundsetfilterparam-dataprovider-operator-value-name) | Add a filter parameter that is permanent per user session to limit a specified foundset of records..                                                                                           |
| void                            | [clear()](jsfoundset.md#clear)                                                                                                       | Clear the foundset..                                                                                                                                                                           |
| [JSRecord](jsrecord.md)         | [createRecord()](jsfoundset.md#createrecord)                                                                                         | Create a new record on top of the foundset and change selection to it..                                                                                                                        |
| [JSRecord](jsrecord.md)         | [createRecord(onTop)](jsfoundset.md#createrecord-ontop)                                                                              | Create a new record in the foundset..                                                                                                                                                          |
| [JSRecord](jsrecord.md)         | [createRecord(onTop, changeSelection)](jsfoundset.md#createrecord-ontop-changeselection)                                             | Create a new record in the foundset..                                                                                                                                                          |
| [JSRecord](jsrecord.md)         | [createRecord(index)](jsfoundset.md#createrecord-index)                                                                              | Create a new record in the foundset and change selection to it at specified index..                                                                                                            |
| [JSRecord](jsrecord.md)         | [createRecord(index, changeSelection)](jsfoundset.md#createrecord-index-changeselection)                                             | Create a new record in the foundset..                                                                                                                                                          |
| [Boolean](../js-lib/boolean.md) | [deleteAllRecords()](jsfoundset.md#deleteallrecords)                                                                                 | Delete all records in foundset, resulting in empty foundset..                                                                                                                                  |
| [Boolean](../js-lib/boolean.md) | [deleteRecord()](jsfoundset.md#deleterecord)                                                                                         | Delete currently selected record(s)..                                                                                                                                                          |
| [Boolean](../js-lib/boolean.md) | [deleteRecord(record)](jsfoundset.md#deleterecord-record)                                                                            | Delete record from foundset..                                                                                                                                                                  |
| [Boolean](../js-lib/boolean.md) | [deleteRecord(index)](jsfoundset.md#deleterecord-index)                                                                              | Delete record with the given index..                                                                                                                                                           |
| [Boolean](../js-lib/boolean.md) | [dispose()](jsfoundset.md#dispose)                                                                                                   | Dispose a foundset from memory when foundset is no longer needed..                                                                                                                             |
| [JSFoundSet](jsfoundset.md)     | [duplicateFoundSet()](jsfoundset.md#duplicatefoundset)                                                                               | Get a duplicate of the foundset..                                                                                                                                                              |
| [Number](../js-lib/number.md)   | [duplicateRecord()](jsfoundset.md#duplicaterecord)                                                                                   | Duplicate current record, change selection to new record, place on top..                                                                                                                       |
| [Number](../js-lib/number.md)   | [duplicateRecord(onTop)](jsfoundset.md#duplicaterecord-ontop)                                                                        | Duplicate selected record, change selection to new record..                                                                                                                                    |
| [Number](../js-lib/number.md)   | [duplicateRecord(onTop, changeSelection)](jsfoundset.md#duplicaterecord-ontop-changeselection)                                       | Duplicate selected record..                                                                                                                                                                    |
| [Number](../js-lib/number.md)   | [duplicateRecord(index)](jsfoundset.md#duplicaterecord-index)                                                                        | Duplicate record at index in the foundset, change selection to new record, place on top..                                                                                                      |
| [Number](../js-lib/number.md)   | [duplicateRecord(index, onTop)](jsfoundset.md#duplicaterecord-index-ontop)                                                           | Duplicate record at index in the foundset, change selection to new record..                                                                                                                    |
| [Number](../js-lib/number.md)   | [duplicateRecord(index, onTop, changeSelection)](jsfoundset.md#duplicaterecord-index-ontop-changeselection)                          | Duplicate record at index in the foundset..                                                                                                                                                    |
| [Number](../js-lib/number.md)   | [duplicateRecord(index, location)](jsfoundset.md#duplicaterecord-index-location)                                                     | Duplicate record at index in the foundset, change selection to new record..                                                                                                                    |
| [Number](../js-lib/number.md)   | [duplicateRecord(index, location, changeSelection)](jsfoundset.md#duplicaterecord-index-location-changeselection)                    | Duplicate record at index in the foundset..                                                                                                                                                    |
| [Boolean](../js-lib/boolean.md) | [find()](jsfoundset.md#find)                                                                                                         | Set the foundset in find mode..                                                                                                                                                                |
| [Object](../js-lib/object.md)   | [forEach(callback)](jsfoundset.md#foreach-callback)                                                                                  | Iterates over the records of a foundset taking into account inserts and deletes that may happen at the same time..                                                                             |
| [Object](../js-lib/object.md)   | [forEach(callback, thisObject)](jsfoundset.md#foreach-callback-thisobject)                                                           | Iterates over the records of a foundset taking into account inserts and deletes that may happen at the same time..                                                                             |
| [String](../js-lib/string.md)   | [getCurrentSort()](jsfoundset.md#getcurrentsort)                                                                                     | Get the current sort columns..                                                                                                                                                                 |
| [Object](../js-lib/object.md)   | [getDataProviderValue(dataProviderID)](jsfoundset.md#getdataprovidervalue-dataproviderid)                                            | Get a value based on a dataprovider name..                                                                                                                                                     |
| [String](../js-lib/string.md)   | [getDataSource()](jsfoundset.md#getdatasource)                                                                                       | Get the datasource used..                                                                                                                                                                      |
| [Array](../js-lib/array.md)     | [getFoundSetFilterParams()](jsfoundset.md#getfoundsetfilterparams)                                                                   | Get the list of previously defined foundset filters..                                                                                                                                          |
| [Array](../js-lib/array.md)     | [getFoundSetFilterParams(filterName)](jsfoundset.md#getfoundsetfilterparams-filtername)                                              | Get a previously defined foundset filter, using its given name..                                                                                                                               |
| [String](../js-lib/string.md)   | [getName()](jsfoundset.md#getname)                                                                                                   | Get foundset name..                                                                                                                                                                            |
| [JSDataSet](jsdataset.md)       | [getOmittedPKs()](jsfoundset.md#getomittedpks)                                                                                       | Returns a JSDataSet with the PKs omitted on this foundset If no PKs have been omitted, an empty JSDataSet will be returned.                                                                    |
| [Array](../js-lib/array.md)     | [getParentRecords()](jsfoundset.md#getparentrecords)                                                                                 | Gets the parent records when called on a related foundset..                                                                                                                                    |
| [QBSelect](qbselect.md)         | [getQuery()](jsfoundset.md#getquery)                                                                                                 | Get the query that the foundset is currently using (as a clone; modifying this QBSelect will not automatically change the foundset)..                                                          |
| [QBSelect](qbselect.md)         | [getQuery(includeFilters)](jsfoundset.md#getquery-includefilters)                                                                    | Get the query that the foundset is currently using (as a clone; modifying this QBSelect will not automatically change the foundset)..                                                          |
| [JSRecord](jsrecord.md)         | [getRecord(index)](jsfoundset.md#getrecord-index)                                                                                    | Get the record object at the given index..                                                                                                                                                     |
| [Number](../js-lib/number.md)   | [getRecordIndex(record)](jsfoundset.md#getrecordindex-record)                                                                        | Get the record index..                                                                                                                                                                         |
| [String](../js-lib/string.md)   | [getRelationName()](jsfoundset.md#getrelationname)                                                                                   | Gets the relation name (null if not a related foundset)..                                                                                                                                      |
| [Number](../js-lib/number.md)   | [getSelectedIndex()](jsfoundset.md#getselectedindex)                                                                                 | Get the current record index of the foundset..                                                                                                                                                 |
| [Array](../js-lib/array.md)     | [getSelectedIndexes()](jsfoundset.md#getselectedindexes)                                                                             | Get the indexes of the selected records..                                                                                                                                                      |
| [JSRecord](jsrecord.md)         | [getSelectedRecord()](jsfoundset.md#getselectedrecord)                                                                               | Get the selected record..                                                                                                                                                                      |
| [Array](../js-lib/array.md)     | [getSelectedRecords()](jsfoundset.md#getselectedrecords)                                                                             | Get the selected records..                                                                                                                                                                     |
| [Number](../js-lib/number.md)   | [getSize()](jsfoundset.md#getsize)                                                                                                   | Get the number of records in this foundset..                                                                                                                                                   |
| [Boolean](../js-lib/boolean.md) | [hasConditions()](jsfoundset.md#hasconditions)                                                                                       | Check wether the foundset has any conditions from a previous find action..                                                                                                                     |
| void                            | [invertRecords()](jsfoundset.md#invertrecords)                                                                                       | Invert the foundset against all rows of the current table..                                                                                                                                    |
| [Boolean](../js-lib/boolean.md) | [isInFind()](jsfoundset.md#isinfind)                                                                                                 | Check if this foundset is in find mode..                                                                                                                                                       |
| [Boolean](../js-lib/boolean.md) | [loadAllRecords()](jsfoundset.md#loadallrecords)                                                                                     | Loads all accessible records from the datasource into the foundset..                                                                                                                           |
| [Boolean](../js-lib/boolean.md) | [loadOmittedRecords()](jsfoundset.md#loadomittedrecords)                                                                             | Loads the records that are currently omitted as a foundset..                                                                                                                                   |
| [Boolean](../js-lib/boolean.md) | [loadRecords()](jsfoundset.md#loadrecords)                                                                                           | Reloads all last (related) records again, if, for example, after search in tabpanel..                                                                                                          |
| [Boolean](../js-lib/boolean.md) | [loadRecords(foundset)](jsfoundset.md#loadrecords-foundset)                                                                          | Copies foundset data from another foundset..                                                                                                                                                   |
| [Boolean](../js-lib/boolean.md) | [loadRecords(dataset)](jsfoundset.md#loadrecords-dataset)                                                                            | Loads a primary key dataset, will remove related sort..                                                                                                                                        |
| [Boolean](../js-lib/boolean.md) | [loadRecords(querybuilder)](jsfoundset.md#loadrecords-querybuilder)                                                                  | Loads records into form foundset based on a query builder object (also known as 'Form by query')..                                                                                             |
| [Boolean](../js-lib/boolean.md) | [loadRecords(uuidpk)](jsfoundset.md#loadrecords-uuidpk)                                                                              | Loads a single record by primary key, will remove related sort..                                                                                                                               |
| [Boolean](../js-lib/boolean.md) | [loadRecords(numberpk)](jsfoundset.md#loadrecords-numberpk)                                                                          | Loads a single record by primary key, will remove related sort..                                                                                                                               |
| [Boolean](../js-lib/boolean.md) | [loadRecords(queryString)](jsfoundset.md#loadrecords-querystring)                                                                    | Loads records into form foundset based on a query (also known as 'Form by query')..                                                                                                            |
| [Boolean](../js-lib/boolean.md) | [loadRecords(queryString, argumentsArray)](jsfoundset.md#loadrecords-querystring-argumentsarray)                                     | Loads records into form foundset based on a query (also known as 'Form by query')..                                                                                                            |
| [Number](../js-lib/number.md)   | [newRecord()](jsfoundset.md#newrecord)                                                                                               | Create a new record on top of the foundset and change selection to it..                                                                                                                        |
| [Number](../js-lib/number.md)   | [newRecord(onTop)](jsfoundset.md#newrecord-ontop)                                                                                    | Create a new record in the foundset and change selection to it..                                                                                                                               |
| [Number](../js-lib/number.md)   | [newRecord(onTop, changeSelection)](jsfoundset.md#newrecord-ontop-changeselection)                                                   | Create a new record in the foundset..                                                                                                                                                          |
| [Number](../js-lib/number.md)   | [newRecord(index)](jsfoundset.md#newrecord-index)                                                                                    | Create a new record in the foundset and change selection to it..                                                                                                                               |
| [Number](../js-lib/number.md)   | [newRecord(index, changeSelection)](jsfoundset.md#newrecord-index-changeselection)                                                   | Create a new record in the foundset..                                                                                                                                                          |
| [Boolean](../js-lib/boolean.md) | [omitRecord()](jsfoundset.md#omitrecord)                                                                                             | Omit selected record(s) (add it to omit records list), to be shown with loadOmittedRecords..                                                                                                   |
| [Boolean](../js-lib/boolean.md) | [omitRecord(index)](jsfoundset.md#omitrecord-index)                                                                                  | Omit record under the given index (add it to omit records list), to be shown with loadOmittedRecords..                                                                                         |
| void                            | [reloadWithFilters()](jsfoundset.md#reloadwithfilters)                                                                               | Reloads all last records again with the filters applied..                                                                                                                                      |
| void                            | [relookup()](jsfoundset.md#relookup)                                                                                                 | Perform a relookup for the currently selected records Lookups are defined in the dataprovider (columns) auto-enter setting and are normally performed over a relation upon record creation..   |
| void                            | [relookup(index)](jsfoundset.md#relookup-index)                                                                                      | Perform a relookup for the record under the given index Lookups are defined in the dataprovider (columns) auto-enter setting and are normally performed over a relation upon record creation.. |
| [Boolean](../js-lib/boolean.md) | [removeFoundSetFilterParam(name)](jsfoundset.md#removefoundsetfilterparam-name)                                                      | Remove a named foundset filter..                                                                                                                                                               |
| [Number](../js-lib/number.md)   | [search()](jsfoundset.md#search)                                                                                                     | Start the database search and use the results, returns the number of records, make sure you did "find" function first..                                                                        |
| [Number](../js-lib/number.md)   | [search(clearLastResults)](jsfoundset.md#search-clearlastresults)                                                                    | Start the database search and use the results, returns the number of records, make sure you did "find" function first..                                                                        |
| [Number](../js-lib/number.md)   | [search(clearLastResults, reduceSearch)](jsfoundset.md#search-clearlastresults-reducesearch)                                         | Start the database search and use the results, returns the number of records, make sure you did "find" function first..                                                                        |
| [Boolean](../js-lib/boolean.md) | [selectRecord(pkid1, pkid2, pkidn)](jsfoundset.md#selectrecord-pkid1-pkid2-pkidn)                                                    | Select the record based on pk data..                                                                                                                                                           |
| void                            | [setDataProviderValue(dataProviderID, value)](jsfoundset.md#setdataprovidervalue-dataproviderid-value)                               | Set a value based on a dataprovider name..                                                                                                                                                     |
| void                            | [setSelectedIndex(index)](jsfoundset.md#setselectedindex-index)                                                                      | Set the current record index..                                                                                                                                                                 |
| void                            | [setSelectedIndexes(indexes)](jsfoundset.md#setselectedindexes-indexes)                                                              | Set the selected records indexes..                                                                                                                                                             |
| void                            | [sort(sortString)](jsfoundset.md#sort-sortstring)                                                                                    | Sorts the foundset based on the given sort string..                                                                                                                                            |
| void                            | [sort(sortString, defer)](jsfoundset.md#sort-sortstring-defer)                                                                       | Sorts the foundset based on the given sort string..                                                                                                                                            |
| void                            | [sort(recordComparisonFunction)](jsfoundset.md#sort-recordcomparisonfunction)                                                        | Sorts the foundset based on the given record comparator function..                                                                                                                             |
| [JSFoundSet](jsfoundset.md)     | [unrelate()](jsfoundset.md#unrelate)                                                                                                 | Create a new unrelated foundset that is a copy of the current foundset..                                                                                                                       |

## Properties Details

### alldataproviders

Get all dataproviders of the foundset.

**Returns**\
[Array](../js-lib/array.md)

**Sample**

```javascript
var dataprovidersNames = alldataproviders;
application.output("This foundset has " + dataprovidersNames.length + " data providers.")
for (var i=0; i<dataprovidersNames.length; i++)
	application.output(dataprovidersNames[i]);
```

### multiSelect

Get or set the multiSelect flag of the foundset.

**Returns**\
[Boolean](../js-lib/boolean.md)

**Sample**

```javascript
// allow user to select multiple rows.
foundset.multiSelect = true;
```

## Methods Details

### addFoundSetFilterParam(query)

Add a filter parameter that is permanent per user session to limit a specified foundset of records.

Filters on tables touched in the query will not be applied to the query filter. For example, when a table filter exists on the order\_details table, a query filter with a join from orders to order\_details will be applied to the foundset, but the filter condition on the orders\_details table will not be included.

Use clear(), reloadWithFilters(), loadRecords() or loadAllRecords() to make the filter effective. Multiple filters can be added to the same dataprovider, they will all be applied.

**Parameters**\
[QBSelect](qbselect.md) query condition to filter on.

**Returns**\
[Boolean](../js-lib/boolean.md) true if adding the filter succeeded, false otherwise.

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(
   query.or.add(
            query.columns.shipcity.eq('Amersfoort'))
   .add(    query.columns.shipcity.eq('Amsterdam')));

var success = foundset.addFoundSetFilterParam(query, 'cityFilter'); // possible to add multiple
// Named filters can be removed using foundset.removeFoundSetFilterParam(filterName)

foundset.loadAllRecords(); // to make param(s) effective
```

### addFoundSetFilterParam(query, name)

Add a filter parameter that is permanent per user session to limit a specified foundset of records.

Filters on tables touched in the query will not be applied to the query filter. For example, when a table filter exists on the order\_details table, a query filter with a join from orders to order\_details will be applied to the foundset, but the filter condition on the orders\_details table will not be included.

Use clear(), reloadWithFilters(), loadRecords() or loadAllRecords() to make the filter effective. The filter is removed again using removeFoundSetFilterParam(name).

The table of the query has to be the same as the foundset table.

**Parameters**\
[QBSelect](qbselect.md) query condition to filter on.\
[Object](../js-lib/object.md) name String name, used to remove the filter again.

**Returns**\
[Boolean](../js-lib/boolean.md) true if adding the filter succeeded, false otherwise.

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(
   query.or.add(
            query.columns.shipcity.eq('Amersfoort'))
   .add(    query.columns.shipcity.eq('Amsterdam')));

var success = foundset.addFoundSetFilterParam(query, 'cityFilter'); // possible to add multiple
// Named filters can be removed using foundset.removeFoundSetFilterParam(filterName)

foundset.loadAllRecords(); // to make param(s) effective
```

### addFoundSetFilterParam(dataprovider, operator, value)

Add a filter parameter that is permanent per user session to limit a specified foundset of records. Use clear(), reloadWithFilters(), loadRecords() or loadAllRecords() to make the filter effective. Multiple filters can be added to the same dataprovider, they will all be applied.

**Parameters**\
[String](../js-lib/string.md) dataprovider String column to filter on.\
[String](../js-lib/string.md) operator String operator: =, <, >, >=, <=, !=, (NOT) LIKE, (NOT) IN, (NOT) BETWEEN and IS (NOT) NULL optionally augmented with modifiers "#" (ignore case) or "^||" (or-is-null), prefix with "sql:" to allow the value to be interpreted as a custom query.\
[Object](../js-lib/object.md) value Object filter value (for in array and between an array with 2 elements)

**Returns**\
[Boolean](../js-lib/boolean.md) true if adding the filter succeeded, false otherwise.

**Sample**

```javascript
var success = foundset.addFoundSetFilterParam('customerid', '=', 'BLONP', 'custFilter');//possible to add multiple
// Named filters can be removed using foundset.removeFoundSetFilterParam(filterName)

// you can use modifiers in the operator as well, filter on companies where companyname is null or equals-ignore-case 'servoy'
var ok = foundset.addFoundSetFilterParam('companyname', '#^||=', 'servoy')

// Filters with in-conditions can be used with arrays or with custom queries:
success = foundset.addFoundSetFilterParam("productcode", "in", [120, 144, 200]);
success = foundset.addFoundSetFilterParam("city", "in", ["London", "Paris"]);
// use "sql:in" in stead of "in" to allow the value to be interpreted as a custom query
success = foundset.addFoundSetFilterParam("countrycode", "sql:in", "select country code from countries where region in ('Europe', 'Asia')");

foundset.loadAllRecords();//to make param(s) effective

// see https://wiki.servoy.com/display/DOCS/Using+Table+Filters
```

### addFoundSetFilterParam(dataprovider, operator, value, name)

Add a filter parameter that is permanent per user session to limit a specified foundset of records. Use clear(), reloadWithFilters(), loadRecords() or loadAllRecords() to make the filter effective. The filter is removed again using removeFoundSetFilterParam(name).

**Parameters**\
[String](../js-lib/string.md) dataprovider String column to filter on.\
[String](../js-lib/string.md) operator String operator: =, <, >, >=, <=, !=, (NOT) LIKE, (NOT) IN, (NOT) BETWEEN and IS (NOT) NULL optionally augmented with modifiers "#" (ignore case) or "^||" (or-is-null), prefix with "sql:" to allow the value to be interpreted as a custom query.\
[Object](../js-lib/object.md) value Object filter value (for in array and between an array with 2 elements)\
[String](../js-lib/string.md) name String name, used to remove the filter again.

**Returns**\
[Boolean](../js-lib/boolean.md) true if adding the filter succeeded, false otherwise.

**Sample**

```javascript
var success = foundset.addFoundSetFilterParam('customerid', '=', 'BLONP', 'custFilter');//possible to add multiple
// Named filters can be removed using foundset.removeFoundSetFilterParam(filterName)

// you can use modifiers in the operator as well, filter on companies where companyname is null or equals-ignore-case 'servoy'
var ok = foundset.addFoundSetFilterParam('companyname', '#^||=', 'servoy')

// Filters with in-conditions can be used with arrays or with custom queries:
success = foundset.addFoundSetFilterParam("productcode", "in", [120, 144, 200]);
success = foundset.addFoundSetFilterParam("city", "in", ["London", "Paris"]);
// use "sql:in" in stead of "in" to allow the value to be interpreted as a custom query
success = foundset.addFoundSetFilterParam("countrycode", "sql:in", "select country code from countries where region in ('Europe', 'Asia')");

foundset.loadAllRecords();//to make param(s) effective

// see https://wiki.servoy.com/display/DOCS/Using+Table+Filters
```

### clear()

Clear the foundset.

**Returns**\
void

**Sample**

```javascript
//Clear the foundset, including searches that may be on it
foundset.clear();
```

### createRecord()

Create a new record on top of the foundset and change selection to it. Returns the new record or null if record was not created.

**Returns**\
[JSRecord](jsrecord.md) IJSRecord the new record

**Sample**

```javascript
var rec = foundset.createRecord(); // add as first record
```

### createRecord(onTop)

Create a new record in the foundset. Returns the new record or null if the record can't be made.

**Parameters**\
[Boolean](../js-lib/boolean.md) onTop when true the new record is added as the topmost record.

**Returns**\
[JSRecord](jsrecord.md) IJSRecord of new record.

**Sample**

```javascript
var rec = foundset.createRecord(false); // add as last record, do change selection
```

### createRecord(onTop, changeSelection)

Create a new record in the foundset. Returns the new record or null if the record can't be made.

**Parameters**\
[Boolean](../js-lib/boolean.md) onTop when true the new record is added as the topmost record; when false the record is added to the end, if all records are loaded, otherwise it will be added to the top\
[Boolean](../js-lib/boolean.md) changeSelection when true the selection is changed to the new record.

**Returns**\
[JSRecord](jsrecord.md) IJSRecord of new record.

**Sample**

```javascript
var rec = foundset.createRecord(false, false); // add as last record, do not change selection
```

### createRecord(index)

Create a new record in the foundset and change selection to it at specified index. Returns the new record or null if the record can't be made.

**Parameters**\
[Number](../js-lib/number.md) index the new record is added at specified index (1-based).

**Returns**\
[JSRecord](jsrecord.md) IJSRecord of new record.

**Sample**

```javascript
var rec = foundset.createRecord(1); // add as first record, do change selection
```

### createRecord(index, changeSelection)

Create a new record in the foundset. Returns the new record or null if the record can't be made.

**Parameters**\
[Number](../js-lib/number.md) index the new record is added at specified index (1-based).\
[Boolean](../js-lib/boolean.md) changeSelection when true the selection is changed to the new record.

**Returns**\
[JSRecord](jsrecord.md) IJSRecord of new record.

**Sample**

```javascript
var rec = foundset.createRecord(1, false); // add as first record, do not change selection
```

### deleteAllRecords()

Delete all records in foundset, resulting in empty foundset.

**Returns**\
[Boolean](../js-lib/boolean.md) boolean true if all records could be deleted.

**Sample**

```javascript
var success = foundset.deleteAllRecords();
```

### deleteRecord()

Delete currently selected record(s). If the foundset is in multiselect mode, all selected records are deleted.

**Returns**\
[Boolean](../js-lib/boolean.md) boolean true if all records could be deleted.

**Sample**

```javascript
var success = foundset.deleteRecord();
//can return false incase of related foundset having records and orphans records are not allowed by the relation
```

### deleteRecord(record)

Delete record from foundset.

**Parameters**\
[JSRecord](jsrecord.md) record The record to delete from the foundset.

**Returns**\
[Boolean](../js-lib/boolean.md) boolean true if record could be deleted.

**Sample**

```javascript
var success = foundset.deleteRecord(rec);
//can return false incase of related foundset having records and orphans records are not allowed by the relation
```

### deleteRecord(index)

Delete record with the given index.

**Parameters**\
[Number](../js-lib/number.md) index The index of the record to delete.

**Returns**\
[Boolean](../js-lib/boolean.md) boolean true if record could be deleted.

**Sample**

```javascript
var success = foundset.deleteRecord(4);
//can return false incase of related foundset having records and orphans records are not allowed by the relation
```

### dispose()

Dispose a foundset from memory when foundset is no longer needed. Should be used to destroy separate foundsets (is an optimization for memory management). A related foundset or a foundset which is linked to visible forms/components cannot be disposed. Returns whether foundset was disposed or not.

**Returns**\
[Boolean](../js-lib/boolean.md) boolean foundset was disposed

**Sample**

```javascript
foundset.dispose();
```

### duplicateFoundSet()

Get a duplicate of the foundset. This is a full copy of the foundset (cached pks,records, relation, filters, search criteria, omitted records, selection).

**Returns**\
[JSFoundSet](jsfoundset.md) foundset duplicate.

**Sample**

```javascript
var dupFoundset = foundset.duplicateFoundSet();
foundset.find();
//search some fields
var count = foundset.search();
if (count == 0)
{
	plugins.dialogs.showWarningDialog('Alert', 'No records found','OK');
	foundset.loadRecords(dupFoundset);
}
```

### duplicateRecord()

Duplicate current record, change selection to new record, place on top.

**Returns**\
[Number](../js-lib/number.md) 0 if record was not created or the record index if it was created.

**Sample**

```javascript
foundset.duplicateRecord();
foundset.duplicateRecord(false); //duplicate the current record, adds at bottom
foundset.duplicateRecord(1,2); //duplicate the first record as second record
//duplicates the record (record index 3), adds on top and selects the record
foundset.duplicateRecord(3,true,true);
```

### duplicateRecord(onTop)

Duplicate selected record, change selection to new record.

**Parameters**\
[Boolean](../js-lib/boolean.md) onTop when true the new record is added as the topmost record.

**Returns**\
[Number](../js-lib/number.md) 0 if record was not created or the record index if it was created.

**Sample**

```javascript
foundset.duplicateRecord();
foundset.duplicateRecord(false); //duplicate the current record, adds at bottom
foundset.duplicateRecord(1,2); //duplicate the first record as second record
//duplicates the record (record index 3), adds on top and selects the record
foundset.duplicateRecord(3,true,true);
```

### duplicateRecord(onTop, changeSelection)

Duplicate selected record.

**Parameters**\
[Boolean](../js-lib/boolean.md) onTop when true the new record is added as the topmost record.\
[Boolean](../js-lib/boolean.md) changeSelection when true the selection is changed to the duplicated record.

**Returns**\
[Number](../js-lib/number.md) 0 if record was not created or the record index if it was created.

**Sample**

```javascript
foundset.duplicateRecord();
foundset.duplicateRecord(false); //duplicate the current record, adds at bottom
foundset.duplicateRecord(1,2); //duplicate the first record as second record
//duplicates the record (record index 3), adds on top and selects the record
foundset.duplicateRecord(3,true,true);
```

### duplicateRecord(index)

Duplicate record at index in the foundset, change selection to new record, place on top.

**Parameters**\
[Number](../js-lib/number.md) index The index of the record to duplicate; defaults to currently selected index. Ignored if first given parameter is a boolean value.

**Returns**\
[Number](../js-lib/number.md) 0 if record was not created or the record index if it was created.

**Sample**

```javascript
foundset.duplicateRecord();
foundset.duplicateRecord(false); //duplicate the current record, adds at bottom
foundset.duplicateRecord(1,2); //duplicate the first record as second record
//duplicates the record (record index 3), adds on top and selects the record
foundset.duplicateRecord(3,true,true);
```

### duplicateRecord(index, onTop)

Duplicate record at index in the foundset, change selection to new record.

**Parameters**\
[Number](../js-lib/number.md) index The index of the record to duplicate; defaults to currently selected index. Ignored if first given parameter is a boolean value.\
[Boolean](../js-lib/boolean.md) onTop when true the new record is added as the topmost record.

**Returns**\
[Number](../js-lib/number.md) 0 if record was not created or the record index if it was created.

**Sample**

```javascript
foundset.duplicateRecord();
foundset.duplicateRecord(false); //duplicate the current record, adds at bottom
foundset.duplicateRecord(1,2); //duplicate the first record as second record
//duplicates the record (record index 3), adds on top and selects the record
foundset.duplicateRecord(3,true,true);
```

### duplicateRecord(index, onTop, changeSelection)

Duplicate record at index in the foundset.

**Parameters**\
[Number](../js-lib/number.md) index The index of the record to duplicate; defaults to currently selected index. Ignored if first given parameter is a boolean value.\
[Boolean](../js-lib/boolean.md) onTop when true the new record is added as the topmost record.\
[Boolean](../js-lib/boolean.md) changeSelection when true the selection is changed to the duplicated record.

**Returns**\
[Number](../js-lib/number.md) 0 if record was not created or the record index if it was created.

**Sample**

```javascript
foundset.duplicateRecord();
foundset.duplicateRecord(false); //duplicate the current record, adds at bottom
foundset.duplicateRecord(1,2); //duplicate the first record as second record
//duplicates the record (record index 3), adds on top and selects the record
foundset.duplicateRecord(3,true,true);
```

### duplicateRecord(index, location)

Duplicate record at index in the foundset, change selection to new record.

**Parameters**\
[Number](../js-lib/number.md) index The index of the record to duplicate; defaults to currently selected index. Ignored if first given parameter is a boolean value.\
[Number](../js-lib/number.md) location the new record is added at specified index

**Returns**\
[Number](../js-lib/number.md) 0 if record was not created or the record index if it was created.

**Sample**

```javascript
foundset.duplicateRecord();
foundset.duplicateRecord(false); //duplicate the current record, adds at bottom
foundset.duplicateRecord(1,2); //duplicate the first record as second record
//duplicates the record (record index 3), adds on top and selects the record
foundset.duplicateRecord(3,true,true);
```

### duplicateRecord(index, location, changeSelection)

Duplicate record at index in the foundset.

**Parameters**\
[Number](../js-lib/number.md) index The index of the record to duplicate; defaults to currently selected index. Ignored if first given parameter is a boolean value.\
[Number](../js-lib/number.md) location the new record is added at specified index\
[Boolean](../js-lib/boolean.md) changeSelection when true the selection is changed to the duplicated record.

**Returns**\
[Number](../js-lib/number.md) 0 if record was not created or the record index if it was created.

**Sample**

```javascript
foundset.duplicateRecord();
foundset.duplicateRecord(false); //duplicate the current record, adds at bottom
foundset.duplicateRecord(1,2); //duplicate the first record as second record
//duplicates the record (record index 3), adds on top and selects the record
foundset.duplicateRecord(3,true,true);
```

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
[Boolean](../js-lib/boolean.md) true if the foundset is now in find mode, false otherwise.

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

### forEach(callback)

Iterates over the records of a foundset taking into account inserts and deletes that may happen at the same time. It will dynamically load all records in the foundset (using Servoy lazy loading mechanism). If callback function returns a non null value the traversal will be stopped and that value is returned. If no value is returned all records of the foundset will be traversed. Foundset modifications( like sort, omit...) cannot be performed in the callback function. If foundset is modified an exception will be thrown. This exception will also happen if a refresh happens because of a rollback call for records on this datasource when iterating. When an exception is thrown from the callback function, the iteraion over the foundset will be stopped.

**Parameters**\
[Function](../js-lib/function.md) callback The callback function to be called for each loaded record in the foundset. Can receive three parameters: the record to be processed, the index of the record in the foundset, and the foundset that is traversed.

**Returns**\
[Object](../js-lib/object.md) Object the return value of the callback

**Sample**

```javascript
foundset.forEach(function(record,recordIndex,foundset) {
 	//handle the record here
 });
```

### forEach(callback, thisObject)

Iterates over the records of a foundset taking into account inserts and deletes that may happen at the same time. It will dynamically load all records in the foundset (using Servoy lazy loading mechanism). If callback function returns a non null value the traversal will be stopped and that value is returned. If no value is returned all records of the foundset will be traversed. Foundset modifications( like sort, omit...) cannot be performed in the callback function. If foundset is modified an exception will be thrown. This exception will also happen if a refresh happens because of a rollback call for records on this datasource when iterating. When an exception is thrown from the callback function, the iteraion over the foundset will be stopped.

**Parameters**\
[Function](../js-lib/function.md) callback The callback function to be called for each loaded record in the foundset. Can receive three parameters: the record to be processed, the index of the record in the foundset, and the foundset that is traversed.\
[Object](../js-lib/object.md) thisObject What the this object should be in the callback function (default it is the foundset)

**Returns**\
[Object](../js-lib/object.md) Object the return value of the callback

**Sample**

```javascript
foundset.forEach(function(record,recordIndex,foundset) {
 	//handle the record here
 });
```

### getCurrentSort()

Get the current sort columns.

**Returns**\
[String](../js-lib/string.md) String sort columns

**Sample**

```javascript
//reverse the current sort

//the original sort "companyName asc, companyContact desc"
//the inversed sort "companyName desc, companyContact asc"
var foundsetSort = foundset.getCurrentSort()
var sortColumns = foundsetSort.split(',')
var newFoundsetSort = ''
for(var i=0; i<sortColumns.length; i++)
{
	var currentSort = sortColumns[i]
	var sortType = currentSort.substring(currentSort.length-3)
	if(sortType.equalsIgnoreCase('asc'))
	{
		newFoundsetSort += currentSort.replace(' asc', ' desc')
	}
	else
	{
		newFoundsetSort += currentSort.replace(' desc', ' asc')
	}
	if(i != sortColumns.length - 1)
	{
		newFoundsetSort += ','
	}
}
foundset.sort(newFoundsetSort)
```

### getDataProviderValue(dataProviderID)

Get a value based on a dataprovider name.

**Parameters**\
[String](../js-lib/string.md) dataProviderID data provider name

**Returns**\
[Object](../js-lib/object.md) Object value

**Sample**

```javascript
var val = foundset.getDataProviderValue('contact_name');
```

### getDataSource()

Get the datasource used. The datasource is an url that describes the data source.

**Returns**\
[String](../js-lib/string.md) String data source.

**Sample**

```javascript
var dataSource = foundset.getDataSource();
```

### getFoundSetFilterParams()

Get the list of previously defined foundset filters.

For column-based table filters, a row of 5 fields per filter are returned. The "columns" of a row from this array are: tablename, dataprovider, operator, value, filtername

For query-based filters, a row of 2 fields per filter are returned. The "columns" of a row from this array are: query, filtername

**Returns**\
[Array](../js-lib/array.md) Array of filter definitions.

**Sample**

```javascript
var params = foundset.getFoundSetFilterParams()
for (var i = 0; params != null && i < params.length; i++)
{
 if (params[i].length() == 5) {
		application.output('FoundSet filter on table ' + params[i][0] + ': '+ params[i][1] + ' '+params[i][2] + ' '+params[i][3] + (params[i][4] == null ? ' [no name]' : ' ['+params[i][4]+']'))
	}
 if (params[i].length() == 2) {
		application.output('FoundSet filter with query ' + params[i][0]+ ': ' + (params[i][1] == null ? ' [no name]' : ' ['+params[i][1]+']'))
	}
}
```

### getFoundSetFilterParams(filterName)

Get a previously defined foundset filter, using its given name. The result is an array of: \[ tableName, dataprovider, operator, value, name ]

**Parameters**\
[String](../js-lib/string.md) filterName name of the filter to retrieve.

**Returns**\
[Array](../js-lib/array.md) Array of filter definitions.

**Sample**

```javascript
var params = foundset.getFoundSetFilterParams()
for (var i = 0; params != null && i < params.length; i++)
{
	application.output('FoundSet filter on table ' + params[i][0]+ ': '+ params[i][1]+ ' '+params[i][2]+ ' '+params[i][3] +(params[i][4] == null ? ' [no name]' : ' ['+params[i][4]+']'))
}
```

### getName()

Get foundset name. If foundset is not named foundset or related foundset will return null.

**Returns**\
[String](../js-lib/string.md) name.

**Sample**

```javascript
var name = foundset.getName()
```

### getOmittedPKs()

Returns a JSDataSet with the PKs omitted on this foundset If no PKs have been omitted, an empty JSDataSet will be returned

**Returns**\
[JSDataSet](jsdataset.md) a JSDataSet

**Sample**

```javascript
foundset.getOmittedPKs();
```

### getParentRecords()

Gets the parent records when called on a related foundset. (empty array if not a related foundset) Depending on the cardinality of the relation, this method returns either 1 or more records. This can be useful when creating a new record in an empty related foundset and some data from the parent record(s) is needed.

Be aware that if datasources.xxx.getFoundset() is called multiple times on the same datasource it creates multiple foundset instances then the related foundset can have multiple references to the same parent record but in different foundsets. (different instances of the record for the same row in the database) In that case, this method will return the record from the first foundset.

**Returns**\
[Array](../js-lib/array.md) an array of records

**Sample**

```javascript
var parents = relatedFoundset.getParentRecords();
```

### getQuery()

Get the query that the foundset is currently using (as a clone; modifying this QBSelect will not automatically change the foundset). When the foundset is in find mode, the find conditions are included in the resulting query. So the query that would be used when just calling search() (or search(true,true)) is returned. Note that foundset filters are optionally included and table filters are not included in the query.

**Returns**\
[QBSelect](qbselect.md) query.

**Sample**

```javascript
var q = foundset.getQuery()
q.where.add(q.columns.x.eq(100))
foundset.loadRecords(q);
```

### getQuery(includeFilters)

Get the query that the foundset is currently using (as a clone; modifying this QBSelect will not automatically change the foundset). When the foundset is in find mode, the find conditions are included in the resulting query. So the query that would be used when just calling search() (or search(true,true)) is returned. Note that foundset filters are optionally included and table filters are not included in the query.

**Parameters**\
[Boolean](../js-lib/boolean.md) includeFilters include the foundset filters, default true.

**Returns**\
[QBSelect](qbselect.md) query.

**Sample**

```javascript
var q = foundset.getQuery()
q.where.add(q.columns.x.eq(100))
foundset.loadRecords(q);
```

### getRecord(index)

Get the record object at the given index. Argument "index" is 1 based (so first record is 1).

**Parameters**\
[Number](../js-lib/number.md) index record index (1 based).

**Returns**\
[JSRecord](jsrecord.md) Record record.

**Sample**

```javascript
var record = foundset.getRecord(index);
```

### getRecordIndex(record)

Get the record index. Will return -1 if the record can't be found.

**Parameters**\
[JSRecord](jsrecord.md) record Record

**Returns**\
[Number](../js-lib/number.md) int index.

**Sample**

```javascript
var index = foundset.getRecordIndex(record);
```

### getRelationName()

Gets the relation name (null if not a related foundset).

**Returns**\
[String](../js-lib/string.md) String relation name when related.

**Sample**

```javascript
var relName = foundset.getRelationName();
```

### getSelectedIndex()

Get the current record index of the foundset.

**Returns**\
[Number](../js-lib/number.md) int current index (1-based)

**Sample**

```javascript
//gets the current record index in the current foundset
var current = foundset.getSelectedIndex();
//sets the next record in the foundset
foundset.setSelectedIndex(current+1);
```

### getSelectedIndexes()

Get the indexes of the selected records. When the founset is in multiSelect mode (see property multiSelect), a selection can consist of more than one index.

**Returns**\
[Array](../js-lib/array.md) Array current indexes (1-based)

**Sample**

```javascript
// modify selection to the first selected item and the following row only
var current = foundset.getSelectedIndexes();
if (current.length > 1)
{
	var newSelection = new Array();
	newSelection[0] = current[0]; // first current selection
	newSelection[1] = current[0] + 1; // and the next row
	foundset.setSelectedIndexes(newSelection);
}
```

### getSelectedRecord()

Get the selected record.

**Returns**\
[JSRecord](jsrecord.md) Record record.

**Sample**

```javascript
var selectedRecord = foundset.getSelectedRecord();
```

### getSelectedRecords()

Get the selected records. When the founset is in multiSelect mode (see property multiSelect), selection can be a more than 1 record.

**Returns**\
[Array](../js-lib/array.md) Array current records.

**Sample**

```javascript
var selectedRecords = foundset.getSelectedRecords();
```

### getSize()

Get the number of records in this foundset. This is the number of records loaded, note that when looping over a foundset, size() may increase as more records are loaded.

**Returns**\
[Number](../js-lib/number.md) int current size.

**Sample**

```javascript
var nrRecords = foundset.getSize()

// to loop over foundset, recalculate size for each record
for (var i = 1; i <= foundset.getSize(); i++)
{
	var rec = foundset.getRecord(i);
}
```

### hasConditions()

Check wether the foundset has any conditions from a previous find action.

**Returns**\
[Boolean](../js-lib/boolean.md) wether the foundset has find-conditions

**Sample**

```javascript
if (foundset.hasConditions())
{
		// foundset had find actions
}
```

### invertRecords()

Invert the foundset against all rows of the current table. All records that are not in the foundset will become the current foundset.

**Returns**\
void

**Sample**

```javascript
foundset.invertRecords();
```

### isInFind()

Check if this foundset is in find mode.

**Returns**\
[Boolean](../js-lib/boolean.md) boolean is in find mode.

**Sample**

```javascript
//Returns true when find was called on this foundset and search has not been called yet
foundset.isInFind();
```

### loadAllRecords()

Loads all accessible records from the datasource into the foundset. Filters on the foundset are applied.

Before loading the records, all unsaved records will be saved in the database. If this fails (due to validation failures or sql errors) or is not allowed (autosave off), records will not be loaded,

**Returns**\
[Boolean](../js-lib/boolean.md) true if records are loaded, false otherwise.

**Sample**

```javascript
foundset.loadAllRecords();
```

### loadOmittedRecords()

Loads the records that are currently omitted as a foundset.

Before loading the omitted records, all unsaved records will be saved in the database. If this fails (due to validation failures or sql errors) or is not allowed (autosave off), omitted records will not be loaded,

**Returns**\
[Boolean](../js-lib/boolean.md) true if records are loaded, false otherwise.

**Sample**

```javascript
foundset.loadOmittedRecords();
```

### loadRecords()

Reloads all last (related) records again, if, for example, after search in tabpanel. When in find mode, this will reload the records from before the find() call.

**Returns**\
[Boolean](../js-lib/boolean.md) true if successful

**Sample**

```javascript
//to reload all last (related) records again, if for example when searched in tabpanel
 foundset.loadRecords();
```

### loadRecords(foundset)

Copies foundset data from another foundset. This will alter the foundset state to the state of the foundset that is given. If you really just want to use the given foundset on the form itself, then you need to use controller.loadRecords(foundset) that will change the instance of the foundset that is used for this form. Not just update an existing forms foundset.

If you copy over a relation into this foundset, then this foundset will not be a related foundset, it will not automatically update its state of records are updated or added that belong to that relation. It will only be a snapshot of that related foundsets state.

Foundset filter params are copied over from the original/source foundset and are merged with the existing filters on this foundset. So if the original foundset had filters and the given foundset has filters then the resulting foundset will have all the filters of both, If you don't want this and you really want only the state of the given foundset, use controller.loadRecords(fs) instead of foundset.loadRecords(fs)

**Parameters**\
[JSFoundSet](jsfoundset.md) foundset The foundset to load records from

**Returns**\
[Boolean](../js-lib/boolean.md) true if successful

**Sample**

```javascript
//Copies foundset data from another foundset
foundset.loadRecords(fs);
```

### loadRecords(dataset)

Loads a primary key dataset, will remove related sort. Tries to preserve selection based on primary key, otherwise first record is selected.

**Parameters**\
[JSDataSet](jsdataset.md) dataset pkdataset

**Returns**\
[Boolean](../js-lib/boolean.md) true if successful

**Sample**

```javascript
// loads a primary key dataset, will remove related sort!
//var dataset = databaseManager.getDataSetByQuery(...);
// dataset must match the table primary key columns (alphabetically ordered)
foundset.loadRecords(dataset);
```

### loadRecords(querybuilder)

Loads records into form foundset based on a query builder object (also known as 'Form by query'). When the foundset is in find mode, the find states are discarded, the foundset will go out of find mode and the foundset will be loaded using the query. If the foundset is related, the relation-condition will be added to the query. Tries to preserve selection based on primary key, otherwise first record is selected.

**Parameters**\
[QBSelect](qbselect.md) querybuilder the query builder

**Returns**\
[Boolean](../js-lib/boolean.md) true if successful

**Sample**

```javascript
foundset.loadRecords(qbselect);
```

### loadRecords(uuidpk)

Loads a single record by primary key, will remove related sort.

NOTE: This function will return true if the foundset was altered/changed. It is up to the developer to check for the presence of actual data using getSize().

**Parameters**\
[UUID](../application/uuid.md) uuidpk single-column pk value

**Returns**\
[Boolean](../js-lib/boolean.md) true if successful

**Sample**

```javascript
//Loads a single record by primary key, will remove related sort!
foundset.loadRecords(application.getUUID('6b5e2f5d-047e-45b3-80ee-3a32267b1f20'));
```

### loadRecords(numberpk)

Loads a single record by primary key, will remove related sort.

NOTE: This function will return true if the foundset was altered/changed. It is up to the developer to check for the presence of actual data using getSize().

**Parameters**\
[Number](../js-lib/number.md) numberpk single-column pk value

**Returns**\
[Boolean](../js-lib/boolean.md) true if successful

**Sample**

```javascript
//Loads a single record by primary key, will remove related sort!
foundset.loadRecords(123);
```

### loadRecords(queryString)

Loads records into form foundset based on a query (also known as 'Form by query'). The query must be a valid sql select. If the foundset is related this function is not allowed. Tries to preserve selection based on primary key, otherwise first record is selected.

see foundset.loadRecords(QBSelect).

When possible, the foundset will be loaded with the given query. This is not always possible because the foundset needs to manipulate the query when adding conditions and joins. In that case the query will be wrapped: select pk from tab where pk = (queryString) The result is the same, except for the ordering in the queryString which will be ignored.

The query will be wrapped when one of the following is true:

* you have no order-by clause
* you have no from keyword
* your query is not fully qualified on the main table
* you have a group-by, having, join or union keyword

**Parameters**\
[String](../js-lib/string.md) queryString select statement

**Returns**\
[Boolean](../js-lib/boolean.md) true if successful

**Sample**

```javascript
//loads records in to the foundset based on a query (also known as 'Form by query')
foundset.loadRecords(sqlstring);
```

### loadRecords(queryString, argumentsArray)

Loads records into form foundset based on a query (also known as 'Form by query'). The query must be a valid sql select. If the foundset is related this function is not allowed. Tries to preserve selection based on primary key, otherwise first record is selected.

see foundset.loadRecords(QBSelect).

When possible, the foundset will be loaded with the given query. This is not always possible because the foundset needs to manipulate the query when adding conditions and joins. In that case the query will be wrapped: select pk from tab where pk = (queryString) The result is the same, except for the ordering in the queryString which will be ignored.

The query will be wrapped when one of the following is true:

* you have no order-by clause
* you have no from keyword
* your query is not fully qualified on the main table
* you have a group-by, having, join or union keyword

**Parameters**\
[String](../js-lib/string.md) queryString select statement\
[Array](../js-lib/array.md) argumentsArray arguments to query

**Returns**\
[Boolean](../js-lib/boolean.md) true if successful

**Sample**

```javascript
//loads records in to the foundset based on a query (also known as 'Form by query')
foundset.loadRecords(sqlstring,parameters);
```

### newRecord()

Create a new record on top of the foundset and change selection to it. Returns -1 if the record can't be made.

**Returns**\
[Number](../js-lib/number.md) int index of new record.

**Sample**

```javascript
// foreign key data is only filled in for equals (=) relation items
var idx = foundset.newRecord(false); // add as last record
// foundset.newRecord(); // adds as first record
// foundset.newRecord(2); //adds as second record
if (idx >= 0) // returned index is -1 in case of failure
{
	foundset.some_column = "some text";
	application.output("added on position " + idx);
	// when adding at the end of the foundset, the returned index
	// corresponds with the size of the foundset
}
```

### newRecord(onTop)

Create a new record in the foundset and change selection to it. Returns -1 if the record can't be made.

**Parameters**\
[Boolean](../js-lib/boolean.md) onTop when true the new record is added as the topmost record.

**Returns**\
[Number](../js-lib/number.md) int index of new record.

**Sample**

```javascript
// foreign key data is only filled in for equals (=) relation items
var idx = foundset.newRecord(false); // add as last record
// foundset.newRecord(); // adds as first record
// foundset.newRecord(2); //adds as second record
if (idx >= 0) // returned index is -1 in case of failure
{
	foundset.some_column = "some text";
	application.output("added on position " + idx);
	// when adding at the end of the foundset, the returned index
	// corresponds with the size of the foundset
}
```

### newRecord(onTop, changeSelection)

Create a new record in the foundset. Returns -1 if the record can't be made.

**Parameters**\
[Boolean](../js-lib/boolean.md) onTop when true the new record is added as the topmost record; when false the record is added to the end, if all records are loaded, otherwise it will be added to the top\
[Boolean](../js-lib/boolean.md) changeSelection when true the selection is changed to the new record.

**Returns**\
[Number](../js-lib/number.md) int index of new record.

**Sample**

```javascript
// foreign key data is only filled in for equals (=) relation items
var idx = foundset.newRecord(false); // add as last record
// foundset.newRecord(); // adds as first record
// foundset.newRecord(2); //adds as second record
if (idx >= 0) // returned index is -1 in case of failure
{
	foundset.some_column = "some text";
	application.output("added on position " + idx);
	// when adding at the end of the foundset, the returned index
	// corresponds with the size of the foundset
}
```

### newRecord(index)

Create a new record in the foundset and change selection to it. Returns -1 if the record can't be made.

**Parameters**\
[Number](../js-lib/number.md) index the new record is added at specified index.

**Returns**\
[Number](../js-lib/number.md) int index of new record.

**Sample**

```javascript
// foreign key data is only filled in for equals (=) relation items
var idx = foundset.newRecord(false); // add as last record
// foundset.newRecord(); // adds as first record
// foundset.newRecord(2); //adds as second record
if (idx >= 0) // returned index is -1 in case of failure
{
	foundset.some_column = "some text";
	application.output("added on position " + idx);
	// when adding at the end of the foundset, the returned index
	// corresponds with the size of the foundset
}
```

### newRecord(index, changeSelection)

Create a new record in the foundset. Returns -1 if the record can't be made.

**Parameters**\
[Number](../js-lib/number.md) index the new record is added at specified index.\
[Boolean](../js-lib/boolean.md) changeSelection when true the selection is changed to the new record.

**Returns**\
[Number](../js-lib/number.md) int index of new record.

**Sample**

```javascript
// foreign key data is only filled in for equals (=) relation items
var idx = foundset.newRecord(false); // add as last record
// foundset.newRecord(); // adds as first record
// foundset.newRecord(2); //adds as second record
if (idx >= 0) // returned index is -1 in case of failure
{
	foundset.some_column = "some text";
	application.output("added on position " + idx);
	// when adding at the end of the foundset, the returned index
	// corresponds with the size of the foundset
}
```

### omitRecord()

Omit selected record(s) (add it to omit records list), to be shown with loadOmittedRecords. T his operation returns false only when foundset is in bad state (table not accessible or not having a valid selected record) or the record is in an edit state and can't be saved (autosave is false).

Note: The omitted records list is discarded when these functions are executed: loadAllRecords, loadRecords(dataset), loadRecords(sqlstring), invertRecords()

**Returns**\
[Boolean](../js-lib/boolean.md) boolean true if all selected record(s) could be omitted.

**Sample**

```javascript
var success = foundset.omitRecord();
```

### omitRecord(index)

Omit record under the given index (add it to omit records list), to be shown with loadOmittedRecords. If index is null it behaves just like omitRecord(). This operation returns false when index is invalid (should be between 1 and foundset size) or foundset is in bad state (its table not accessible) or the record is in an edit state and can't be saved (autosave is false). Any retrievable record can be ommitted.

Note: The omitted records list is discarded when these functions are executed: loadAllRecords, loadRecords(dataset), loadRecords(sqlstring), invertRecords()

**Parameters**\
[Number](../js-lib/number.md) index The index of the record to omit, starting with 1 .

**Returns**\
[Boolean](../js-lib/boolean.md) boolean true if all records could be omitted.

**Sample**

```javascript
var success = foundset.omitRecord();
```

### reloadWithFilters()

Reloads all last records again with the filters applied.

**Returns**\
void

**Sample**

```javascript
foundset.reloadWithFilters();
```

### relookup()

Perform a relookup for the currently selected records Lookups are defined in the dataprovider (columns) auto-enter setting and are normally performed over a relation upon record creation.

**Returns**\
void

**Sample**

```javascript
foundset.relookup(1);
```

### relookup(index)

Perform a relookup for the record under the given index Lookups are defined in the dataprovider (columns) auto-enter setting and are normally performed over a relation upon record creation.

**Parameters**\
[Number](../js-lib/number.md) index record index (1-based)

**Returns**\
void

**Sample**

```javascript
foundset.relookup(1);
```

### removeFoundSetFilterParam(name)

Remove a named foundset filter. Use clear(), reloadWithFilters(), loadRecords() or loadAllRecords() to make the filter effective.

**Parameters**\
[String](../js-lib/string.md) name String filter name.

**Returns**\
[Boolean](../js-lib/boolean.md) true if removing the filter succeeded, false otherwise.

**Sample**

```javascript
var success = foundset.removeFoundSetFilterParam('custFilter');// removes all filters with this name
foundset.loadAllRecords();//to make param(s) effective
```

### search()

Start the database search and use the results, returns the number of records, make sure you did "find" function first. Clear results from previous searches.

Note: Omitted records are automatically excluded when performing a search - meaning that the foundset result by default will not include omitted records.

**Returns**\
[Number](../js-lib/number.md) the recordCount

**Sample**

```javascript
var recordCount = foundset.search();
//var recordCount = foundset.search(false,false); //to extend foundset
```

### search(clearLastResults)

Start the database search and use the results, returns the number of records, make sure you did "find" function first. Reduce results from previous searches.

Note: Omitted records are automatically excluded when performing a search - meaning that the foundset result by default will not include omitted records.

**Parameters**\
[Boolean](../js-lib/boolean.md) clearLastResults boolean, clear previous search, default true

**Returns**\
[Number](../js-lib/number.md) the recordCount

**Sample**

```javascript
var recordCount = foundset.search();
//var recordCount = foundset.search(false,false); //to extend foundset
```

### search(clearLastResults, reduceSearch)

Start the database search and use the results, returns the number of records, make sure you did "find" function first.

Note: Omitted records are automatically excluded when performing a search - meaning that the foundset result by default will not include omitted records.

**Parameters**\
[Boolean](../js-lib/boolean.md) clearLastResults boolean, clear previous search, default true\
[Boolean](../js-lib/boolean.md) reduceSearch boolean, reduce (true) or extend (false) previous search results, default true

**Returns**\
[Number](../js-lib/number.md) the recordCount

**Sample**

```javascript
var recordCount = foundset.search();
//var recordCount = foundset.search(false,false); //to extend foundset
```

### selectRecord(pkid1, pkid2, pkidn)

Select the record based on pk data. Note that if the foundset has not loaded the record with the pk, selectrecord will fail.

In case of a table with a composite key, the pk sequence must match the alphabetical ordering of the pk column names.

**Parameters**\
[Object](../js-lib/object.md) pkid1 primary key\
[Object](../js-lib/object.md) pkid2 second primary key (in case of composite primary key)\
[Object](../js-lib/object.md) pkidn nth primary key

**Returns**\
[Boolean](../js-lib/boolean.md) true if succeeded.

**Sample**

```javascript
foundset.selectRecord(pkid1,pkid2,pkidn);//pks must be alphabetically set! It is also possible to use an array as parameter.
```

### setDataProviderValue(dataProviderID, value)

Set a value based on a dataprovider name.

**Parameters**\
[String](../js-lib/string.md) dataProviderID data provider name\
[Object](../js-lib/object.md) value value to set

**Returns**\
void

**Sample**

```javascript
foundset.setDataProviderValue('contact_name','mycompany');
```

### setSelectedIndex(index)

Set the current record index.

**Parameters**\
[Number](../js-lib/number.md) index index to set (1-based)

**Returns**\
void

**Sample**

```javascript
//gets the current record index in the current foundset
var current = foundset.getSelectedIndex();
//sets the next record in the foundset
foundset.setSelectedIndex(current+1);
```

### setSelectedIndexes(indexes)

Set the selected records indexes.

**Parameters**\
[Array](../js-lib/array.md) indexes An array with indexes to set.

**Returns**\
void

**Sample**

```javascript
// modify selection to the first selected item and the following row only
var current = foundset.getSelectedIndexes();
if (current.length > 1)
{
	var newSelection = new Array();
	newSelection[0] = current[0]; // first current selection
	newSelection[1] = current[0] + 1; // and the next row
	foundset.setSelectedIndexes(newSelection);
}
```

### sort(sortString)

Sorts the foundset based on the given sort string. Tries to preserve selection based on primary key. If first record is selected or cannot select old record it will select first record after sort. TIP: You can use the Copy button in the developer Select Sorting Fields dialog to get the needed syntax string for the desired sort fields/order.

**Parameters**\
[String](../js-lib/string.md) sortString the specified columns (and sort order)

**Returns**\
void

**Sample**

```javascript
foundset.sort('columnA desc,columnB asc');
```

### sort(sortString, defer)

Sorts the foundset based on the given sort string. Tries to preserve selection based on primary key. If first record is selected or cannot select old record it will select first record after sort. TIP: You can use the Copy button in the developer Select Sorting Fields dialog to get the needed syntax string for the desired sort fields/order.

**Parameters**\
[String](../js-lib/string.md) sortString the specified columns (and sort order)\
[Boolean](../js-lib/boolean.md) defer when true, the "sortString" will be just stored, without performing a query on the database (the actual sorting will be deferred until the next data loading action).

**Returns**\
void

**Sample**

```javascript
foundset.sort('columnA desc,columnB asc');
```

### sort(recordComparisonFunction)

Sorts the foundset based on the given record comparator function. Tries to preserve selection based on primary key. If first record is selected or cannot select old record it will select first record after sort. The comparator function is called to compare two records, that are passed as arguments, and it will return -1/0/1 if the first record is less/equal/greater then the second record.

The function based sorting does not work with printing. It is just a temporary in-memory sort.

NOTE: starting with 7.2 release this function doesn't save the data anymore

**Parameters**\
[Function](../js-lib/function.md) recordComparisonFunction record comparator function

**Returns**\
void

**Sample**

```javascript
foundset.sort(mySortFunction);

function mySortFunction(r1, r2)
{
	var o = 0;
	if(r1.id < r2.id)
	{
		o = -1;
	}
	else if(r1.id > r2.id)
	{
		o = 1;
	}
	return o;
}
```

### unrelate()

Create a new unrelated foundset that is a copy of the current foundset. If the current foundset is not related, no copy will made.

**Returns**\
[JSFoundSet](jsfoundset.md) FoundSet unrelated foundset.

**Sample**

```javascript
foundset.unrelate();
```
