#  ViewFoundSet


## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [MONITOR_AGGREGATES](ViewFoundSet.md#MONITOR_AGGREGATES)                   | Constant for the flags in #enableDatabroadcastFor(QBTableClause,int) to listen for changes in columns (selected) of the given datasource in the query that can affect aggregates..                                    |
| [Number](../JSLib/Number.md) | [MONITOR_COLUMNS](ViewFoundSet.md#MONITOR_COLUMNS)                   | Constant for the flags in #enableDatabroadcastFor(QBTableClause,int) to listen also for column changes of the given table/datasource..                                    |
| [Number](../JSLib/Number.md) | [MONITOR_DELETES](ViewFoundSet.md#MONITOR_DELETES)                   | Constant for the flags in #enableDatabroadcastFor(QBTableClause,int) to listen for deletes on the given table/datasource..                                    |
| [Number](../JSLib/Number.md) | [MONITOR_DELETES_FOR_PRIMARY_TABLE](ViewFoundSet.md#MONITOR_DELETES_FOR_PRIMARY_TABLE)                   | Constant for the flags in #enableDatabroadcastFor(QBTableClause,int) to listen for deletes on the given table/datasource which should be the primary/main table of this query..                                    |
| [Number](../JSLib/Number.md) | [MONITOR_INSERT](ViewFoundSet.md#MONITOR_INSERT)                   | Constant for the flags in #enableDatabroadcastFor(QBTableClause,int) to listen for inserts on the given table/datasource..                                    |
| [Number](../JSLib/Number.md) | [MONITOR_JOIN_CONDITIONS](ViewFoundSet.md#MONITOR_JOIN_CONDITIONS)                   | Constant for the flags in #enableDatabroadcastFor(QBTableClause,int) to listen also for column changes of the given table/datasource in the join statement - like order_lines..                                    |
| [Number](../JSLib/Number.md) | [MONITOR_WHERE_CONDITIONS](ViewFoundSet.md#MONITOR_WHERE_CONDITIONS)                   | Constant for the flags in #enableDatabroadcastFor(QBTableClause,int) to listen also for column changes of the given table/datasource that are used in the where statement - like order_lines..                                    |
| [String](../JSLib/String.md) | [VIEW_FOUNDSET](ViewFoundSet.md#VIEW_FOUNDSET)                   | .                                    |

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../JSLib/Boolean.md) | [multiSelect](ViewFoundSet.md#multiSelect)                   | Returns true if this foundset is in multiselect mode and false if it's in single-select mode..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../JSLib/Boolean.md) | [dispose()](ViewFoundSet.md#dispose)                   | Dispose and unregisters a view foundset from memory when is no longer needed..                                    |
| [JSFoundSet](./JSFoundSet.md) | [duplicateFoundSet()](ViewFoundSet.md#duplicatefoundset)                   | Get a duplicate of the viewfoundset..                                    |
|void | [enableDatabroadcastFor(queryTable)](ViewFoundSet.md#enabledatabroadcastfor-querytable)                   | Databroadcast can be enabled per select table of a query, the select table can be the main QBSelect or on of it QBJoins By default this monitors only the column values that are in the result of the QBSelect, you can only enable this default monitoring for a table if for that table also the PK is selected in the results..                                    |
|void | [enableDatabroadcastFor(queryTableclause, flags)](ViewFoundSet.md#enabledatabroadcastfor-querytableclause-flags)                   | Enable the databroadcast for a specific table of the QBSelect or QBJoin with  flags for looking for join or where criteria or deletes/inserts..                                    |
| [Object](../JSLib/Object.md) | [forEach(callback)](ViewFoundSet.md#foreach-callback)                   | Iterates over the records of a foundset taking into account inserts and deletes that may happen at the same time..                                    |
| [Object](../JSLib/Object.md) | [forEach(callback, thisObject)](ViewFoundSet.md#foreach-callback-thisobject)                   | Iterates over the records of a foundset taking into account inserts and deletes that may happen at the same time..                                    |
| [String](../JSLib/String.md) | [getCurrentSort()](ViewFoundSet.md#getcurrentsort)                   | Get the last sort columns that were set using viewfoundset sort api..                                    |
| [String](../JSLib/String.md) | [getDataSource()](ViewFoundSet.md#getdatasource)                   | Returns the datasource (view:name) for this ViewFoundSet..                                    |
| [Array](../JSLib/Array.md) | [getEditedRecords()](ViewFoundSet.md#geteditedrecords)                   | Get the edited records of this view foundset..                                    |
| [Array](../JSLib/Array.md) | [getFailedRecords()](ViewFoundSet.md#getfailedrecords)                   | Get the records which could not be saved..                                    |
| [String](../JSLib/String.md) | [getName()](ViewFoundSet.md#getname)                   | Get foundset name..                                    |
| [QBSelect](./QBSelect.md) | [getQuery()](ViewFoundSet.md#getquery)                   | Get the cloned query that created this ViewFoundSset (modifying this QBSelect will not change the foundset)..                                    |
| [JSRecord](./JSRecord.md) | [getRecord(index)](ViewFoundSet.md#getrecord-index)                   | Get the ViewRecord object at the given index..                                    |
| [Number](../JSLib/Number.md) | [getRecordIndex(record)](ViewFoundSet.md#getrecordindex-record)                   | Get the record index..                                    |
| [Number](../JSLib/Number.md) | [getSelectedIndex()](ViewFoundSet.md#getselectedindex)                   | Get the current record index of the viewfoundset..                                    |
| [Array](../JSLib/Array.md) | [getSelectedIndexes()](ViewFoundSet.md#getselectedindexes)                   | Get the indexes of the selected records..                                    |
| [JSRecord](./JSRecord.md) | [getSelectedRecord()](ViewFoundSet.md#getselectedrecord)                   | .                                    |
| [Array](../JSLib/Array.md) | [getSelectedRecords()](ViewFoundSet.md#getselectedrecords)                   | Get the selected records..                                    |
| [Number](../JSLib/Number.md) | [getSize()](ViewFoundSet.md#getsize)                   | Get the number of records in this viewfoundset..                                    |
| [Boolean](../JSLib/Boolean.md) | [hasRecordChanges()](ViewFoundSet.md#hasrecordchanges)                   | Check whether the foundset has record changes..                                    |
| [Boolean](../JSLib/Boolean.md) | [hasRecords()](ViewFoundSet.md#hasrecords)                   | Returns true if the viewfoundset has records..                                    |
|void | [loadAllRecords()](ViewFoundSet.md#loadallrecords)                   | This will reload the current set of ViewRecords in this foundset, resetting the chunk size back to the start (default 200)..                                    |
|void | [revertEditedRecords()](ViewFoundSet.md#reverteditedrecords)                   | Revert changes of all unsaved view records of the view foundset..                                    |
|void | [revertEditedRecords(rec)](ViewFoundSet.md#reverteditedrecords-rec)                   | Revert changes of the provided view records..                                    |
| [Boolean](../JSLib/Boolean.md) | [save()](ViewFoundSet.md#save)                   | Saves all records in the view foundset that have changes..                                    |
| [Boolean](../JSLib/Boolean.md) | [save(record)](ViewFoundSet.md#save-record)                   | Saved a specific record of this foundset..                                    |
|void | [setSelectedIndex(index)](ViewFoundSet.md#setselectedindex-index)                   | Set the current record index..                                    |
|void | [setSelectedIndexes(indexes)](ViewFoundSet.md#setselectedindexes-indexes)                   | Set the selected records indexes..                                    |
|void | [sort(sortString)](ViewFoundSet.md#sort-sortstring)                   | Sorts the foundset based on the given sort string..                                    |
|void | [sort(sortString, defer)](ViewFoundSet.md#sort-sortstring-defer)                   | Sorts the foundset based on the given sort string..                                    |
|void | [sort(recordComparisonFunction)](ViewFoundSet.md#sort-recordcomparisonfunction)                   | Sorts the foundset based on the given record comparator function..                                    |
| [JSRecordMarkers](./JSRecordMarkers.md) | [validate(record)](ViewFoundSet.md#validate-record)                   | Validates the given record, it runs first the method that is attached to the entity event "onValidate"..                                    |
| [JSRecordMarkers](./JSRecordMarkers.md) | [validate(record, customObject)](ViewFoundSet.md#validate-record-customobject)                   | Validates the given record, it runs first the method that is attached to the entity event "onValidate"..                                    |

## Constants Details

### MONITOR_AGGREGATES

Constant for the flags in #enableDatabroadcastFor(QBTableClause,int) to listen for changes in
columns (selected) of the given datasource in the query that can affect aggregates. This means that when
there are deletes, inserts or updates on columns selected from that datasource, a full re-query will
happen to refresh the aggregates.

IMPORTANT: in general, this flag should be set on (possible multiple) datasources from the query that
have group by on their columns, and the columns don't contain the pk, or that have the actual aggregates
on their columns (because all those could influence the value of aggregates).

For example (ignoring the fact that in a real-life situation these fields might not change), a view
foundset based on this query:

SELECT orders.customerid, orders.orderdate, SUM(order_details.unitprice) FROM orders
   LEFT OUTER JOIN order_details ON orders.orderid = order_details.orderid
   GROUP BY orders.customerid, orders.orderdate
	  ORDER BY orders.customerid asc, orders.orderdate desc

will want to enable databroadcast flag MONITOR_AGGREGATES on both "orders" (because if "orderdate" or
"customerid" - that are used in GROUP BY - change/are corrected on a row, that row could move from one
group to the other, affecting the SUM(order_details.unitprice) for the groups involved) and "order_details"
(because if "unitprice" changes/is corrected, the aggregate will be affected).

But if the above query would also select the orders.odersid (and also group by that) then the orders row
that you select for that sum will always be unique and only #MONITOR_COLUMNS has to be used for
those - if needed.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```
### MONITOR_COLUMNS

Constant for the flags in #enableDatabroadcastFor(QBTableClause,int) to listen also for column
changes of the given table/datasource. This is used by default if you just use enableDatabroadcastFor()
without flags. If you use the one with the flags you need to give this one if you just want to listen to
column changes that are in the result for a given datasource and pk.

This constants needs to have the pk's selected for the given datasource (should be in the results).

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```
### MONITOR_DELETES

Constant for the flags in #enableDatabroadcastFor(QBTableClause,int) to listen for deletes on the
given table/datasource. This will always result in a full query to detect changes whenever an delete on
that table happens.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```
### MONITOR_DELETES_FOR_PRIMARY_TABLE

Constant for the flags in #enableDatabroadcastFor(QBTableClause,int) to listen for deletes on the
given table/datasource which should be the primary/main table of this query. If a delete comes in for this
table, then we will only remove the records from the ViewFoundSet that do have this primary key in its
value. So no need to do a full query. So this will only work if the query shows order_lines for the
order_lines table, not for the products table that is joined to get the product_name. Only 1 of the 2
monitors for deletes should be registered for a table/datasource.

This constants needs to have the pk's selected for the given datasource (should be in the results)

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```
### MONITOR_INSERT

Constant for the flags in #enableDatabroadcastFor(QBTableClause,int) to listen for inserts on the
given table/datasource. This will always result in a full query to detect changes whenever an insert on
that table happens.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```
### MONITOR_JOIN_CONDITIONS

Constant for the flags in #enableDatabroadcastFor(QBTableClause,int) to listen also for column
changes of the given table/datasource in the join statement - like order_lines.productid that has a join
to orders and is displaying the productname. If a change in such a join condition (like
order_lines.productid in the sample above) is seen then the query will be fired again to detect changes.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```
### MONITOR_WHERE_CONDITIONS

Constant for the flags in #enableDatabroadcastFor(QBTableClause,int) to listen also for column
changes of the given table/datasource that are used in the where statement - like
order_lines.unit_price > 100. If a change is seen on that datasource on such a column used in the where
a full query will be fired again to detect changes.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```
### VIEW_FOUNDSET



**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```

## Properties Details

### multiSelect

Returns true if this foundset is in multiselect mode and false if it's in single-select mode.

**Returns**\
[Boolean](../JSLib/Boolean.md) true if this foundset is in multiselect mode and false if it's in single-select mode.


**Sample**

```javascript

```

## Methods Details

### dispose()

Dispose and unregisters a view foundset from memory when is no longer needed.
Returns whether foundset was disposed.
If linked to visible form or component, view foundset cannot be disposed.

Normally ViewFoundSets are not hold on to by the system, so if you only use this inside a method it will be disposed by itself.
This method is then just helps by also calling clear()

For ViewFoundSets that are also registered  by using true as the last argument in the call: databaseMananager.getViewFoundSet(name, query, boolean register)
are hold on to by the system and Forms can use it for there foundset. Calling dispose on those will remove it from the system, so it is not usable anymore in forms.


**Returns**\
[Boolean](../JSLib/Boolean.md) boolean foundset was disposed


**Sample**

```javascript
vfs.dispose();
```
### duplicateFoundSet()

Get a duplicate of the viewfoundset. This is a full copy of the view foundset.


**Returns**\
[JSFoundSet](./JSFoundSet.md) foundset duplicate.


**Sample**

```javascript
var dupFoundset = foundset.duplicateFoundSet();
```
### enableDatabroadcastFor(queryTable)

Databroadcast can be enabled per select table of a query, the select table can be the main QBSelect or on of it QBJoins
By default this monitors only the column values that are in the result of the QBSelect, you can only enable this default monitoring for a table if for that table also the PK is selected in the results.

you can use #enableDatabroadcastFor(QBTableClause,int) to specify what should be monitored more besides pure column values per pk.
Those have impact on performance because for the most part if we see a hit then a full query is done to see if there are changes.

**Parameters**\
[QBTableClause](./QBTableClause.md) queryTable The QBSelect or QBJoin of a full query where this foundset should listen for data changes.

**Returns**\
void 


**Sample**

```javascript
var select = datasources.db.example_data.order_details.createSelect();
 var join = select.joins.add("db:/example_data/products");
 join.on.add(select.columns.productid.eq(join.columns.productid));
 select.result.add(); // add columns of the select or join
 var vf = databaseManager.getViewFoundSet("myorders",select)
 vf.enableDatabroadcastFor(select);
 vf.enableDatabroadcastFor(join);
```
### enableDatabroadcastFor(queryTableclause, flags)

Enable the databroadcast for a specific table of the QBSelect or QBJoin with  flags for looking for join or where criteria or deletes/inserts.
These  flags can be a performance hit because the query needs to be executed again to see if there are any changes.
For certain flags #MONITOR_COLUMNS and #MONITOR_DELETES_FOR_PRIMARY_TABLE the pk for that table must be in the results.

**Parameters**\
[QBTableClause](./QBTableClause.md) queryTableclause The QBSelect or QBJoin of a full query where this foundset should listen for data changes.\
[Number](../JSLib/Number.md) flags One or more of the ViewFoundSet.XXX flags added to each other.

**Returns**\
void 


**Sample**

```javascript
var select = datasources.db.example_data.order_details.createSelect();
 var join = select.joins.add("db:/example_data/products");
 join.on.add(select.columns.productid.eq(join.columns.productid));
 select.result.add(); // add columns of the select or join
 var vf = databaseManager.getViewFoundSet("myorders",select)
 // monitor for the main table the join conditions (orders->product, when product id changes in the orders table) and requery the table on insert events, delete directly the record if a pk delete happens.
 vf.enableDatabroadcastFor(select, ViewFoundSet.MONITOR_JOIN_CONDITIONS | ViewFoundSet.MONITOR_INSERT | ViewFoundSet.MONITOR_DELETES_FOR_PRIMARY_TABLE);
 vf.enableDatabroadcastFor(join);
```
### forEach(callback)

Iterates over the records of a foundset taking into account inserts and deletes that may happen at the same time.
It will dynamically load all records in the foundset (using Servoy lazy loading mechanism). If callback function returns a non null value the traversal will be stopped and that value is returned.
If no value is returned all records of the foundset will be traversed. Foundset modifications( like sort, omit...) cannot be performed in the callback function.
If foundset is modified an exception will be thrown. This exception will also happen if a refresh happens because of a rollback call for records on this datasource when iterating.
When an exception is thrown from the callback function, the iteraion over the foundset will be stopped.

**Parameters**\
[Function](../JSLib/Function.md) callback The callback function to be called for each loaded record in the foundset. Can receive three parameters: the record to be processed, the index of the record in the foundset, and the foundset that is traversed.

**Returns**\
[Object](../JSLib/Object.md) Object the return value of the callback


**Sample**

```javascript
foundset.forEach(function(record,recordIndex,foundset) {
 	//handle the record here
 });
```
### forEach(callback, thisObject)

Iterates over the records of a foundset taking into account inserts and deletes that may happen at the same time.
It will dynamically load all records in the foundset (using Servoy lazy loading mechanism). If callback function returns a non null value the traversal will be stopped and that value is returned.
If no value is returned all records of the foundset will be traversed. Foundset modifications( like sort, omit...) cannot be performed in the callback function.
If foundset is modified an exception will be thrown. This exception will also happen if a refresh happens because of a rollback call for records on this datasource when iterating.
When an exception is thrown from the callback function, the iteraion over the foundset will be stopped.

**Parameters**\
[Function](../JSLib/Function.md) callback The callback function to be called for each loaded record in the foundset. Can receive three parameters: the record to be processed, the index of the record in the foundset, and the foundset that is traversed.\
[Object](../JSLib/Object.md) thisObject What the this object should be in the callback function (default it is the foundset)

**Returns**\
[Object](../JSLib/Object.md) Object the return value of the callback


**Sample**

```javascript
foundset.forEach(function(record,recordIndex,foundset) {
 	//handle the record here
 });
```
### getCurrentSort()

Get the last sort columns that were set using viewfoundset sort api.s


**Returns**\
[String](../JSLib/String.md) String sort columns


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
### getDataSource()

Returns the datasource (view:name) for this ViewFoundSet.


**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
solutionModel.getForm("x").dataSource  = viewFoundSet.getDataSource();
```
### getEditedRecords()

Get the edited records of this view foundset.


**Returns**\
[Array](../JSLib/Array.md) an array of edited records


**Sample**

```javascript
var editedRecords = foundset.getEditedRecords();
for (var i = 0; i < editedRecords.length; i++)
{
   application.output(editedRecords[i]);
}
```
### getFailedRecords()

Get the records which could not be saved.


**Returns**\
[Array](../JSLib/Array.md) an array of failed records


**Sample**

```javascript

```
### getName()

Get foundset name. If foundset is not named foundset will return null.


**Returns**\
[String](../JSLib/String.md) name.


**Sample**

```javascript
var name = foundset.getName()
```
### getQuery()

Get the cloned query that created this ViewFoundSset (modifying this QBSelect will not change the foundset).
The ViewFoundSets main query can't be altered after creation; you need to make a new ViewFoundSet for that (it can have the same datasource name).


**Returns**\
[QBSelect](./QBSelect.md) query.


**Sample**

```javascript
var q = foundset.getQuery()
q.where.add(q.columns.x.eq(100))
var newVF = databaseManager.getViewFoundset("name", q);
```
### getRecord(index)

Get the ViewRecord object at the given index.
Argument "index" is 1 based (so first record is 1).

**Parameters**\
[Number](../JSLib/Number.md) index record index (1 based).

**Returns**\
[JSRecord](./JSRecord.md) ViewRecord record.


**Sample**

```javascript
var record = vfs.getRecord(index);
```
### getRecordIndex(record)

Get the record index. Will return -1 if the record can't be found.

**Parameters**\
[JSRecord](./JSRecord.md) record Record

**Returns**\
[Number](../JSLib/Number.md) int index.


**Sample**

```javascript
var index = foundset.getRecordIndex(record);
```
### getSelectedIndex()

Get the current record index of the viewfoundset.


**Returns**\
[Number](../JSLib/Number.md) int current index (1-based)


**Sample**

```javascript
//gets the current record index in the current viewfoundset
var current = foundset.getSelectedIndex();
//sets the next record in the viewfoundset
foundset.setSelectedIndex(current+1);
```
### getSelectedIndexes()

Get the indexes of the selected records.
When the viewfounset is in multiSelect mode (see property multiSelect), a selection can consist of more than one index.


**Returns**\
[Array](../JSLib/Array.md) Array current indexes (1-based)


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




**Returns**\
[JSRecord](./JSRecord.md) 


**Sample**

```javascript

```
### getSelectedRecords()

Get the selected records.
When the viewfounset is in multiSelect mode (see property multiSelect), selection can be a more than 1 record.


**Returns**\
[Array](../JSLib/Array.md) Array current records.


**Sample**

```javascript
var selectedRecords = foundset.getSelectedRecords();
```
### getSize()

Get the number of records in this viewfoundset.
This is the number of records loaded, note that when looping over a foundset, size() may
increase as more records are loaded.


**Returns**\
[Number](../JSLib/Number.md) int current size.


**Sample**

```javascript
var nrRecords = vfs.getSize()

// to loop over foundset, recalculate size for each record
for (var i = 1; i <= foundset.getSize(); i++)
{
	var rec = vfs.getRecord(i);
}
```
### hasRecordChanges()

Check whether the foundset has record changes.


**Returns**\
[Boolean](../JSLib/Boolean.md) true if the foundset has any edited records, false otherwise


**Sample**

```javascript

```
### hasRecords()

Returns true if the viewfoundset has records.


**Returns**\
[Boolean](../JSLib/Boolean.md) true if the viewfoundset has records.


**Sample**

```javascript

```
### loadAllRecords()

This will reload the current set of ViewRecords in this foundset, resetting the chunk size back to the start (default 200).
All edited records will be discarded! So this can be seen as a full clean up of this ViewFoundSet.


**Returns**\
void 


**Sample**

```javascript

```
### revertEditedRecords()

Revert changes of all unsaved view records of the view foundset.


**Returns**\
void 


**Sample**

```javascript

```
### revertEditedRecords(rec)

Revert changes of the provided view records.

**Parameters**\
[Array](../JSLib/Array.md) rec an array of view records

**Returns**\
void 


**Sample**

```javascript

```
### save()

Saves all records in the view foundset that have changes.
You can only save columns from a table if the pks of that table are also selected by the view foundset's query.


**Returns**\
[Boolean](../JSLib/Boolean.md) true if the save was successfull, false if not and then the record will hav the exception set.


**Sample**

```javascript

```
### save(record)

Saved a specific record of this foundset.
You can only save columns from a table if also the pk is selected of that table

**Parameters**\
[JSRecord](./JSRecord.md) record  ;

**Returns**\
[Boolean](../JSLib/Boolean.md) true if the save was successfull, false if not and then the record will hav the exception set.


**Sample**

```javascript

```
### setSelectedIndex(index)

Set the current record index.

**Parameters**\
[Number](../JSLib/Number.md) index index to set (1-based)

**Returns**\
void 


**Sample**

```javascript

```
### setSelectedIndexes(indexes)

Set the selected records indexes.

**Parameters**\
[Array](../JSLib/Array.md) indexes An array with indexes to set.

**Returns**\
void 


**Sample**

```javascript

```
### sort(sortString)

Sorts the foundset based on the given sort string.
Column in sort string must already exist in ViewFoundset.

**Parameters**\
[String](../JSLib/String.md) sortString the specified columns (and sort order)

**Returns**\
void 


**Sample**

```javascript
foundset.sort('columnA desc,columnB asc');
```
### sort(sortString, defer)

Sorts the foundset based on the given sort string.
Column in sort string must already exist in ViewFoundset.

**Parameters**\
[String](../JSLib/String.md) sortString the specified columns (and sort order)\
[Boolean](../JSLib/Boolean.md) defer when true, the "sortString" will be just stored, without performing a query on the database (the actual sorting will be deferred until the next data loading action).

**Returns**\
void 


**Sample**

```javascript
foundset.sort('columnA desc,columnB asc');
```
### sort(recordComparisonFunction)

Sorts the foundset based on the given record comparator function.
Tries to preserve selection based on primary key. If first record is selected or cannot select old record it will select first record after sort.
The comparator function is called to compare
two records, that are passed as arguments, and
it will return -1/0/1 if the first record is less/equal/greater
then the second record.

The function based sorting does not work with printing.
It is just a temporary in-memory sort.

NOTE: starting with 7.2 release this function doesn't save the data anymore

**Parameters**\
[Function](../JSLib/Function.md) recordComparisonFunction record comparator function

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
### validate(record)

Validates the given record, it runs first the method that is attached to the entity event "onValidate".
Those methods do get a parameter JSRecordMarkers where the problems can be reported against.
All columns are then also null/empty checked and if they are and the Column is marked as "not null" an error will be
added with the message key "servoy.record.error.null.not.allowed" for that column.

An extra state object can be given that will also be passed around if you want to have more state in the validation objects
(like giving some ui state so the entity methods know where you come from)

It will return a JSRecordMarkers when the record had validation problems

**Parameters**\
[JSRecord](./JSRecord.md) record  ;

**Returns**\
[JSRecordMarkers](./JSRecordMarkers.md) Returns a JSRecordMarkers if the record has validation problems


**Sample**

```javascript

```
### validate(record, customObject)

Validates the given record, it runs first the method that is attached to the entity event "onValidate".
Those methods do get a parameter JSRecordMarkers where the problems can be reported against.
All columns are then also null/empty checked and if they are and the Column is marked as "not null" an error will be
added with the message key "servoy.record.error.null.not.allowed" for that column.

An extra state object can be given that will also be passed around if you want to have more state in the validation objects
(like giving some ui state so the entity methods know where you come from)

It will return a JSRecordMarkers when the record had validation problems

**Parameters**\
[JSRecord](./JSRecord.md) record The ViewRecord to validate\
[Object](../JSLib/Object.md) customObject An extra customObject to give to the validate method.

**Returns**\
[JSRecordMarkers](./JSRecordMarkers.md) 


**Sample**

```javascript

```

