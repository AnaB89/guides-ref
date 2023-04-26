# QUERY\_COLUMN\_TYPES

## Constants Summary

| Type                          | Name                                                             | Summary                     |
| ----------------------------- | ---------------------------------------------------------------- | --------------------------- |
| [String](../js-lib/string.md) | [TYPE\_BIG\_DECIMAL](query\_column\_types.md#TYPE\_BIG\_DECIMAL) | Constant used for casting.. |
| [String](../js-lib/string.md) | [TYPE\_BIG\_INTEGER](query\_column\_types.md#TYPE\_BIG\_INTEGER) | Constant used for casting.. |
| [String](../js-lib/string.md) | [TYPE\_BINARY](query\_column\_types.md#TYPE\_BINARY)             | Constant used for casting.. |
| [String](../js-lib/string.md) | [TYPE\_BLOB](query\_column\_types.md#TYPE\_BLOB)                 | Constant used for casting.. |
| [String](../js-lib/string.md) | [TYPE\_BOOLEAN](query\_column\_types.md#TYPE\_BOOLEAN)           | Constant used for casting.. |
| [String](../js-lib/string.md) | [TYPE\_BYTE](query\_column\_types.md#TYPE\_BYTE)                 | Constant used for casting.. |
| [String](../js-lib/string.md) | [TYPE\_CHARACTER](query\_column\_types.md#TYPE\_CHARACTER)       | Constant used for casting.. |
| [String](../js-lib/string.md) | [TYPE\_CLOB](query\_column\_types.md#TYPE\_CLOB)                 | Constant used for casting.. |
| [String](../js-lib/string.md) | [TYPE\_DATE](query\_column\_types.md#TYPE\_DATE)                 | Constant used for casting.. |
| [String](../js-lib/string.md) | [TYPE\_DOUBLE](query\_column\_types.md#TYPE\_DOUBLE)             | Constant used for casting.. |
| [String](../js-lib/string.md) | [TYPE\_FLOAT](query\_column\_types.md#TYPE\_FLOAT)               | Constant used for casting.. |
| [String](../js-lib/string.md) | [TYPE\_IMAGE](query\_column\_types.md#TYPE\_IMAGE)               | Constant used for casting.. |
| [String](../js-lib/string.md) | [TYPE\_INTEGER](query\_column\_types.md#TYPE\_INTEGER)           | Constant used for casting.. |
| [String](../js-lib/string.md) | [TYPE\_SHORT](query\_column\_types.md#TYPE\_SHORT)               | Constant used for casting.. |
| [String](../js-lib/string.md) | [TYPE\_STRING](query\_column\_types.md#TYPE\_STRING)             | Constant used for casting.. |
| [String](../js-lib/string.md) | [TYPE\_TEXT](query\_column\_types.md#TYPE\_TEXT)                 | Constant used for casting.. |
| [String](../js-lib/string.md) | [TYPE\_TIME](query\_column\_types.md#TYPE\_TIME)                 | Constant used for casting.. |
| [String](../js-lib/string.md) | [TYPE\_TIMESTAMP](query\_column\_types.md#TYPE\_TIMESTAMP)       | Constant used for casting.. |

## Constants Details

### TYPE\_BIG\_DECIMAL

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### TYPE\_BIG\_INTEGER

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### TYPE\_BINARY

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### TYPE\_BLOB

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### TYPE\_BOOLEAN

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### TYPE\_BYTE

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### TYPE\_CHARACTER

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### TYPE\_CLOB

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### TYPE\_DATE

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### TYPE\_DOUBLE

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### TYPE\_FLOAT

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### TYPE\_IMAGE

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### TYPE\_INTEGER

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### TYPE\_SHORT

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### TYPE\_STRING

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### TYPE\_TEXT

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### TYPE\_TIME

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### TYPE\_TIMESTAMP

Constant used for casting.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
