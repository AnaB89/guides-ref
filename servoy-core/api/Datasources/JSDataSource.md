#  JSDataSource


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [QBSelect](../Database%20Manager/QBSelect.md) | [createSelect()](JSDataSource.md#createselect)                   | Create a query builder for a data source..                                    |
| [QBSelect](../Database%20Manager/QBSelect.md) | [createSelect(tableAlias)](JSDataSource.md#createselect-tablealias)                   | Create a query builder for a data source with given table alias..                                    |
| [Array](../JSLib/Array.md) | [getColumnNames()](JSDataSource.md#getcolumnnames)                   | Get the column names of a datasource..                                    |
| [String](../JSLib/String.md) | [getDataSource()](JSDataSource.md#getdatasource)                   | Get the datasource string..                                    |
| [JSFoundSet](../Database%20Manager/JSFoundSet.md) | [getFoundSet()](JSDataSource.md#getfoundset)                   | Returns a foundset object for a specified datasource or server and tablename..                                    |
| [JSFoundSet](../Database%20Manager/JSFoundSet.md) | [getFoundSet(name)](JSDataSource.md#getfoundset-name)                   | An existing foundset under that name will be returned, or created if there is a definition (there is a form with a named foundset property with that name)..                                    |
| [JSRecord](../Database%20Manager/JSRecord.md) | [getRecord(pk)](JSDataSource.md#getrecord-pk)                   | Get a single record from a datasource..                                    |
| [JSTable](../Database%20Manager/JSTable.md) | [getTable()](JSDataSource.md#gettable)                   | Get the table of a datasource..                                    |
| [JSFoundSet](../Database%20Manager/JSFoundSet.md) | [loadRecords(dataSet)](JSDataSource.md#loadrecords-dataset)                   | get a new foundset containing records based on a dataset of pks..                                    |
| [JSFoundSet](../Database%20Manager/JSFoundSet.md) | [loadRecords(qbSelect)](JSDataSource.md#loadrecords-qbselect)                   | get a new foundset containing records based on a QBSelect query..                                    |
| [JSFoundSet](../Database%20Manager/JSFoundSet.md) | [loadRecords(query)](JSDataSource.md#loadrecords-query)                   | get a new foundset containing records based on an SQL query string..                                    |
| [JSFoundSet](../Database%20Manager/JSFoundSet.md) | [loadRecords(query, args)](JSDataSource.md#loadrecords-query-args)                   | get a new foundset containing records based on an SQL query string with parameters..                                    |

## Methods Details

### createSelect()

Create a query builder for a data source.


**Returns**\
[QBSelect](../Database%20Manager/QBSelect.md) query builder


**Sample**

```javascript
var q = datasources.db.example_data.book_nodes.createSelect()
 q.result.addPk()
 q.where.add(q.columns.label_text.not.isin(null))
 datasources.db.example_data.book_nodes.getFoundSet().loadRecords(q)
```
### createSelect(tableAlias)

Create a query builder for a data source with given table alias.
 The alias can be used inside custom queries to bind to the outer table.

**Parameters**\
[String](../JSLib/String.md) tableAlias the table alias to use

**Returns**\
[QBSelect](../Database%20Manager/QBSelect.md) query builder


**Sample**

```javascript
var q = datasources.db.example_data.book_nodes.createSelect('b')
 q.result.addPk()
 q.where.add(q.columns.label_text.isin('select comment_text from book_text t where t.note_text = ? and t.node_id = b.node_id', ['test']))
 datasources.db.example_data.book_nodes.getFoundSet().loadRecords(q)
```
### getColumnNames()

Get the column names of a datasource.


**Returns**\
[Array](../JSLib/Array.md) String[] column names


**Sample**

```javascript

```
### getDataSource()

Get the datasource string.


**Returns**\
[String](../JSLib/String.md) String datasource


**Sample**

```javascript
datasources.db.example_data.orders.getDataSource() // returns 'db:/example_data/orders'
```
### getFoundSet()

Returns a foundset object for a specified datasource or server and tablename.
It is important to note that this is a FACTORY method, it constantly creates new foundsets.


**Returns**\
[JSFoundSet](../Database%20Manager/JSFoundSet.md) A new JSFoundset for the datasource.


**Sample**

```javascript
var fs = datasources.db.example_data.orders.getFoundSet()
var ridx = fs.newRecord()
var record = fs.getRecord(ridx)
record.emp_name = 'John'
databaseManager.saveData()
```
### getFoundSet(name)

An existing foundset under that name will be returned, or created if there is a definition (there is a form with a named foundset property with that name).
If named foundset datasource does not match current datasource will not be returned (will return null instead).

**Parameters**\
[String](../JSLib/String.md) name The named foundset to get  for this datasource.

**Returns**\
[JSFoundSet](../Database%20Manager/JSFoundSet.md) An existing named foundset for the datasource.


**Sample**

```javascript
var fs = datasources.db.example_data.orders.getFoundSet('myname')
var ridx = fs.newRecord()
var record = fs.getRecord(ridx)
record.emp_name = 'John'
databaseManager.saveData()
```
### getRecord(pk)

Get a single record from a datasource.
For the sake of performance, if more records are needed,
don't call this method in a loop but try using other methods instead.

**Parameters**\
[Object](../JSLib/Object.md) pk The primary key of the record to be retrieved. Can be an array, in case of a composite pk.

**Returns**\
[JSRecord](../Database%20Manager/JSRecord.md) a record


**Sample**

```javascript
var detailsRecord = datasources.db.example_data.order_details.getRecord([10248, 11])
var orderRecord = datasources.db.example_data.orders.getRecord(10248)
var customerRecord = datasources.db.example_data.customers.getRecord('ANATR')
```
### getTable()

Get the table of a datasource.


**Returns**\
[JSTable](../Database%20Manager/JSTable.md) JSTable table


**Sample**

```javascript

```
### loadRecords(dataSet)

get a new foundset containing records based on a dataset of pks.

**Parameters**\
[JSDataSet](../Database%20Manager/JSDataSet.md) dataSet  ;

**Returns**\
[JSFoundSet](../Database%20Manager/JSFoundSet.md) a new JSFoundset


**Sample**

```javascript
var fs = datasources.db.example_data.customers.loadRecords(pkDataSet)
```
### loadRecords(qbSelect)

get a new foundset containing records based on a QBSelect query.

**Parameters**\
[QBSelect](../Database%20Manager/QBSelect.md) qbSelect a query builder object

**Returns**\
[JSFoundSet](../Database%20Manager/JSFoundSet.md) a new JSFoundset


**Sample**

```javascript
var qb = datasources.db.example_data.orders.createSelect();
qb.result.add(qb.columns.orderid);
var fs = datasources.db.example_data.orders.loadRecords(qb);
```
### loadRecords(query)

get a new foundset containing records based on an SQL query string.

**Parameters**\
[String](../JSLib/String.md) query an SQL query

**Returns**\
[JSFoundSet](../Database%20Manager/JSFoundSet.md) a new JSFoundset


**Sample**

```javascript
var query = "SELECT * FROM public.orders WHERE customerid = 'ROMEY' ORDER BY orderid ASC";
var fs = datasources.db.example_data.orders.loadRecords(query);
```
### loadRecords(query, args)

get a new foundset containing records based on an SQL query string with parameters.

**Parameters**\
[String](../JSLib/String.md) query an SQL query string with parameter placeholders\
[Array](../JSLib/Array.md) args an array of arguments for the query string

**Returns**\
[JSFoundSet](../Database%20Manager/JSFoundSet.md) a new JSFoundset


**Sample**

```javascript
var query = "SELECT * FROM public.orders WHERE customerid = ? OR customerid = ? order by orderid asc";
var args = ['ROMEY', 'BERGS'];
var fs = datasources.db.example_data.orders.loadRecords(query, args);
```

