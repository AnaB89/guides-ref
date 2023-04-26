# JSTable

## Methods Summary

| Type                            | Name                                                                    | Summary                                                                                            |
| ------------------------------- | ----------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| [JSColumn](jscolumn.md)         | [getColumn(name)](jstable.md#getcolumn-name)                            | Returns a JSColumn for the named column (or column dataproviderID)..                               |
| [Array](../js-lib/array.md)     | [getColumnNames()](jstable.md#getcolumnnames)                           | Returns an array containing the names of all table columns..                                       |
| [String](../js-lib/string.md)   | [getDataSource()](jstable.md#getdatasource)                             | Returns the table data source uri..                                                                |
| [String](../js-lib/string.md)   | [getQuotedSQLName()](jstable.md#getquotedsqlname)                       | Returns a quoted version of the table name, if necessary, as defined by the actual database used.. |
| [Array](../js-lib/array.md)     | [getRowIdentifierColumnNames()](jstable.md#getrowidentifiercolumnnames) | Returns an array containing the names of the identifier (PK) column(s)..                           |
| [String](../js-lib/string.md)   | [getSQLName()](jstable.md#getsqlname)                                   | Returns the table name as defined in the database..                                                |
| [String](../js-lib/string.md)   | [getServerName()](jstable.md#getservername)                             | Returns the Servoy server name..                                                                   |
| [Boolean](../js-lib/boolean.md) | [isMetadataTable()](jstable.md#ismetadatatable)                         | Returns whether table was flagged as metadata table..                                              |

## Methods Details

### getColumn(name)

Returns a JSColumn for the named column (or column dataproviderID).

**Parameters**\
[String](../js-lib/string.md) name The name of the column to return the value from.

**Returns**\
[JSColumn](jscolumn.md) JSColumn column.

**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var jsColumn = jsTable.getColumn('campaign_name')
```

### getColumnNames()

Returns an array containing the names of all table columns. If the table is in mem, then the internal rowid column name is not returned.

**Returns**\
[Array](../js-lib/array.md) String array of column names.

**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var columnNames = jsTable.getColumnNames()
```

### getDataSource()

Returns the table data source uri.

**Returns**\
[String](../js-lib/string.md) String datasource uri.

**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var dataSource = jsTable.getDataSource()
```

### getQuotedSQLName()

Returns a quoted version of the table name, if necessary, as defined by the actual database used.

**Returns**\
[String](../js-lib/string.md) String table name, quoted if needed.

**Sample**

```javascript
//use with the raw SQL plugin:
//if the table name contains characters that are illegal in sql, the table name will be quoted
var jsTable = databaseManager.getTable('udm', 'campaigns')
var quotedTableName = jsTable.getQuotedSQLName()
plugins.rawSQL.executeSQL('udm',  quotedTableName,  'select * from ' + quotedTableName + ' where is_active = ?', [1])
```

### getRowIdentifierColumnNames()

Returns an array containing the names of the identifier (PK) column(s). Please note that if the table is in mem, then the internal rowid column name is also returned.

**Returns**\
[Array](../js-lib/array.md) String array of row identifier column names.

**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var identifierColumnNames = jsTable.getRowIdentifierColumnNames()
```

### getSQLName()

Returns the table name as defined in the database.

**Returns**\
[String](../js-lib/string.md) String table sql name.

**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var tableNameForQuery = jsTable.getSQLName()
```

### getServerName()

Returns the Servoy server name.

**Returns**\
[String](../js-lib/string.md) String server name.

**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var serverName = jsTable.getServerName()
```

### isMetadataTable()

Returns whether table was flagged as metadata table.

**Returns**\
[Boolean](../js-lib/boolean.md) boolean is metadata

**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var isMetaDataTable = jsTable.isMetadataTable()
```
