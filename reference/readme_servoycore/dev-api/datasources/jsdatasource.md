# JSDataSource

## Methods Summary

| Type                                            | Name                                                                | Summary                                                                                                                                                      |
| ----------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [QBSelect](../database-manager/qbselect.md)     | [createSelect()](jsdatasource.md#createselect)                      | Create a query builder for a data source..                                                                                                                   |
| [QBSelect](../database-manager/qbselect.md)     | [createSelect(tableAlias)](jsdatasource.md#createselect-tablealias) | Create a query builder for a data source with given table alias..                                                                                            |
| [Array](../js-lib/array.md)                     | [getColumnNames()](jsdatasource.md#getcolumnnames)                  | Get the column names of a datasource..                                                                                                                       |
| [String](../js-lib/string.md)                   | [getDataSource()](jsdatasource.md#getdatasource)                    | Get the datasource string..                                                                                                                                  |
| [JSFoundSet](../database-manager/jsfoundset.md) | [getFoundSet()](jsdatasource.md#getfoundset)                        | Returns a foundset object for a specified datasource or server and tablename..                                                                               |
| [JSFoundSet](../database-manager/jsfoundset.md) | [getFoundSet(name)](jsdatasource.md#getfoundset-name)               | An existing foundset under that name will be returned, or created if there is a definition (there is a form with a named foundset property with that name).. |
| [JSRecord](../database-manager/jsrecord.md)     | [getRecord(pk)](jsdatasource.md#getrecord-pk)                       | Get a single record from a datasource..                                                                                                                      |
| [JSTable](../database-manager/jstable.md)       | [getTable()](jsdatasource.md#gettable)                              | Get the table of a datasource..                                                                                                                              |
| [JSFoundSet](../database-manager/jsfoundset.md) | [loadRecords(dataSet)](jsdatasource.md#loadrecords-dataset)         | get a new foundset containing records based on a dataset of pks..                                                                                            |
| [JSFoundSet](../database-manager/jsfoundset.md) | [loadRecords(qbSelect)](jsdatasource.md#loadrecords-qbselect)       | get a new foundset containing records based on a QBSelect query..                                                                                            |
| [JSFoundSet](../database-manager/jsfoundset.md) | [loadRecords(query)](jsdatasource.md#loadrecords-query)             | get a new foundset containing records based on an SQL query string..                                                                                         |
| [JSFoundSet](../database-manager/jsfoundset.md) | [loadRecords(query, args)](jsdatasource.md#loadrecords-query-args)  | get a new foundset containing records based on an SQL query string with parameters..                                                                         |

## Methods Details

### createSelect()

Create a query builder for a data source.

**Returns**\
[QBSelect](../database-manager/qbselect.md) query builder

**Sample**

```javascript
var q = datasources.db.example_data.book_nodes.createSelect()
 q.result.addPk()
 q.where.add(q.columns.label_text.not.isin(null))
 datasources.db.example_data.book_nodes.getFoundSet().loadRecords(q)
```

### createSelect(tableAlias)

Create a query builder for a data source with given table alias. The alias can be used inside custom queries to bind to the outer table.

**Parameters**\
[String](../js-lib/string.md) tableAlias the table alias to use

**Returns**\
[QBSelect](../database-manager/qbselect.md) query builder

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
[Array](../js-lib/array.md) String\[] column names

**Sample**

```javascript
```

### getDataSource()

Get the datasource string.

**Returns**\
[String](../js-lib/string.md) String datasource

**Sample**

```javascript
datasources.db.example_data.orders.getDataSource() // returns 'db:/example_data/orders'
```

### getFoundSet()

Returns a foundset object for a specified datasource or server and tablename. It is important to note that this is a FACTORY method, it constantly creates new foundsets.

**Returns**\
[JSFoundSet](../database-manager/jsfoundset.md) A new JSFoundset for the datasource.

**Sample**

```javascript
var fs = datasources.db.example_data.orders.getFoundSet()
var ridx = fs.newRecord()
var record = fs.getRecord(ridx)
record.emp_name = 'John'
databaseManager.saveData()
```

### getFoundSet(name)

An existing foundset under that name will be returned, or created if there is a definition (there is a form with a named foundset property with that name). If named foundset datasource does not match current datasource will not be returned (will return null instead).

**Parameters**\
[String](../js-lib/string.md) name The named foundset to get for this datasource.

**Returns**\
[JSFoundSet](../database-manager/jsfoundset.md) An existing named foundset for the datasource.

**Sample**

```javascript
var fs = datasources.db.example_data.orders.getFoundSet('myname')
var ridx = fs.newRecord()
var record = fs.getRecord(ridx)
record.emp_name = 'John'
databaseManager.saveData()
```

### getRecord(pk)

Get a single record from a datasource. For the sake of performance, if more records are needed, don't call this method in a loop but try using other methods instead.

**Parameters**\
[Object](../js-lib/object.md) pk The primary key of the record to be retrieved. Can be an array, in case of a composite pk.

**Returns**\
[JSRecord](../database-manager/jsrecord.md) a record

**Sample**

```javascript
var detailsRecord = datasources.db.example_data.order_details.getRecord([10248, 11])
var orderRecord = datasources.db.example_data.orders.getRecord(10248)
var customerRecord = datasources.db.example_data.customers.getRecord('ANATR')
```

### getTable()

Get the table of a datasource.

**Returns**\
[JSTable](../database-manager/jstable.md) JSTable table

**Sample**

```javascript
```

### loadRecords(dataSet)

get a new foundset containing records based on a dataset of pks.

**Parameters**\
[JSDataSet](../database-manager/jsdataset.md) dataSet ;

**Returns**\
[JSFoundSet](../database-manager/jsfoundset.md) a new JSFoundset

**Sample**

```javascript
var fs = datasources.db.example_data.customers.loadRecords(pkDataSet)
```

### loadRecords(qbSelect)

get a new foundset containing records based on a QBSelect query.

**Parameters**\
[QBSelect](../database-manager/qbselect.md) qbSelect a query builder object

**Returns**\
[JSFoundSet](../database-manager/jsfoundset.md) a new JSFoundset

**Sample**

```javascript
var qb = datasources.db.example_data.orders.createSelect();
qb.result.add(qb.columns.orderid);
var fs = datasources.db.example_data.orders.loadRecords(qb);
```

### loadRecords(query)

get a new foundset containing records based on an SQL query string.

**Parameters**\
[String](../js-lib/string.md) query an SQL query

**Returns**\
[JSFoundSet](../database-manager/jsfoundset.md) a new JSFoundset

**Sample**

```javascript
var query = "SELECT * FROM public.orders WHERE customerid = 'ROMEY' ORDER BY orderid ASC";
var fs = datasources.db.example_data.orders.loadRecords(query);
```

### loadRecords(query, args)

get a new foundset containing records based on an SQL query string with parameters.

**Parameters**\
[String](../js-lib/string.md) query an SQL query string with parameter placeholders\
[Array](../js-lib/array.md) args an array of arguments for the query string

**Returns**\
[JSFoundSet](../database-manager/jsfoundset.md) a new JSFoundset

**Sample**

```javascript
var query = "SELECT * FROM public.orders WHERE customerid = ? OR customerid = ? order by orderid asc";
var args = ['ROMEY', 'BERGS'];
var fs = datasources.db.example_data.orders.loadRecords(query, args);
```
