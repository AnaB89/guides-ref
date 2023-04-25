#  QUERY_COLUMN_TYPES


## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [String](../JSLib/String.md) | [TYPE_BIG_DECIMAL](QUERY_COLUMN_TYPES.md#TYPE_BIG_DECIMAL)                   | Constant used for casting..                                    |
| [String](../JSLib/String.md) | [TYPE_BIG_INTEGER](QUERY_COLUMN_TYPES.md#TYPE_BIG_INTEGER)                   | Constant used for casting..                                    |
| [String](../JSLib/String.md) | [TYPE_BINARY](QUERY_COLUMN_TYPES.md#TYPE_BINARY)                   | Constant used for casting..                                    |
| [String](../JSLib/String.md) | [TYPE_BLOB](QUERY_COLUMN_TYPES.md#TYPE_BLOB)                   | Constant used for casting..                                    |
| [String](../JSLib/String.md) | [TYPE_BOOLEAN](QUERY_COLUMN_TYPES.md#TYPE_BOOLEAN)                   | Constant used for casting..                                    |
| [String](../JSLib/String.md) | [TYPE_BYTE](QUERY_COLUMN_TYPES.md#TYPE_BYTE)                   | Constant used for casting..                                    |
| [String](../JSLib/String.md) | [TYPE_CHARACTER](QUERY_COLUMN_TYPES.md#TYPE_CHARACTER)                   | Constant used for casting..                                    |
| [String](../JSLib/String.md) | [TYPE_CLOB](QUERY_COLUMN_TYPES.md#TYPE_CLOB)                   | Constant used for casting..                                    |
| [String](../JSLib/String.md) | [TYPE_DATE](QUERY_COLUMN_TYPES.md#TYPE_DATE)                   | Constant used for casting..                                    |
| [String](../JSLib/String.md) | [TYPE_DOUBLE](QUERY_COLUMN_TYPES.md#TYPE_DOUBLE)                   | Constant used for casting..                                    |
| [String](../JSLib/String.md) | [TYPE_FLOAT](QUERY_COLUMN_TYPES.md#TYPE_FLOAT)                   | Constant used for casting..                                    |
| [String](../JSLib/String.md) | [TYPE_IMAGE](QUERY_COLUMN_TYPES.md#TYPE_IMAGE)                   | Constant used for casting..                                    |
| [String](../JSLib/String.md) | [TYPE_INTEGER](QUERY_COLUMN_TYPES.md#TYPE_INTEGER)                   | Constant used for casting..                                    |
| [String](../JSLib/String.md) | [TYPE_SHORT](QUERY_COLUMN_TYPES.md#TYPE_SHORT)                   | Constant used for casting..                                    |
| [String](../JSLib/String.md) | [TYPE_STRING](QUERY_COLUMN_TYPES.md#TYPE_STRING)                   | Constant used for casting..                                    |
| [String](../JSLib/String.md) | [TYPE_TEXT](QUERY_COLUMN_TYPES.md#TYPE_TEXT)                   | Constant used for casting..                                    |
| [String](../JSLib/String.md) | [TYPE_TIME](QUERY_COLUMN_TYPES.md#TYPE_TIME)                   | Constant used for casting..                                    |
| [String](../JSLib/String.md) | [TYPE_TIMESTAMP](QUERY_COLUMN_TYPES.md#TYPE_TIMESTAMP)                   | Constant used for casting..                                    |

## Constants Details

### TYPE_BIG_DECIMAL

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### TYPE_BIG_INTEGER

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### TYPE_BINARY

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### TYPE_BLOB

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### TYPE_BOOLEAN

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### TYPE_BYTE

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### TYPE_CHARACTER

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### TYPE_CLOB

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### TYPE_DATE

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### TYPE_DOUBLE

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### TYPE_FLOAT

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### TYPE_IMAGE

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### TYPE_INTEGER

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### TYPE_SHORT

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### TYPE_STRING

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### TYPE_TEXT

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### TYPE_TIME

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### TYPE_TIMESTAMP

Constant used for casting.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

