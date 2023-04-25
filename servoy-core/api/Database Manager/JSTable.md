#  JSTable


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSColumn](./JSColumn.md) | [getColumn(name)](JSTable.md#getcolumn-name)                   | Returns a JSColumn for the named column (or column dataproviderID)..                                    |
| [Array](../JSLib/Array.md) | [getColumnNames()](JSTable.md#getcolumnnames)                   | Returns an array containing the names of all table columns..                                    |
| [String](../JSLib/String.md) | [getDataSource()](JSTable.md#getdatasource)                   | Returns the table data source uri..                                    |
| [String](../JSLib/String.md) | [getQuotedSQLName()](JSTable.md#getquotedsqlname)                   | Returns a quoted version of the table name, if necessary, as defined by the actual database used..                                    |
| [Array](../JSLib/Array.md) | [getRowIdentifierColumnNames()](JSTable.md#getrowidentifiercolumnnames)                   | Returns an array containing the names of the identifier (PK) column(s)..                                    |
| [String](../JSLib/String.md) | [getSQLName()](JSTable.md#getsqlname)                   | Returns the table name as defined in the database..                                    |
| [String](../JSLib/String.md) | [getServerName()](JSTable.md#getservername)                   | Returns the Servoy server name..                                    |
| [Boolean](../JSLib/Boolean.md) | [isMetadataTable()](JSTable.md#ismetadatatable)                   | Returns whether table was flagged as metadata table..                                    |

## Methods Details

### getColumn(name)

Returns a JSColumn for the named column (or column dataproviderID).

**Parameters**\
[String](../JSLib/String.md) name The name of the column to return the value from.

**Returns**\
[JSColumn](./JSColumn.md) JSColumn column.


**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var jsColumn = jsTable.getColumn('campaign_name')
```
### getColumnNames()

Returns an array containing the names of all table columns.
If the table is in mem, then the internal rowid column name is not returned.


**Returns**\
[Array](../JSLib/Array.md) String array of column names.


**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var columnNames = jsTable.getColumnNames()
```
### getDataSource()

Returns the table data source uri.


**Returns**\
[String](../JSLib/String.md) String datasource uri.


**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var dataSource = jsTable.getDataSource()
```
### getQuotedSQLName()

Returns a quoted version of the table name, if necessary, as defined by the actual database used.


**Returns**\
[String](../JSLib/String.md) String table name, quoted if needed.


**Sample**

```javascript
//use with the raw SQL plugin:
//if the table name contains characters that are illegal in sql, the table name will be quoted
var jsTable = databaseManager.getTable('udm', 'campaigns')
var quotedTableName = jsTable.getQuotedSQLName()
plugins.rawSQL.executeSQL('udm',  quotedTableName,  'select * from ' + quotedTableName + ' where is_active = ?', [1])
```
### getRowIdentifierColumnNames()

Returns an array containing the names of the identifier (PK) column(s).
 Please note that if the table is in mem, then the internal rowid column name is also returned.


**Returns**\
[Array](../JSLib/Array.md) String array of row identifier column names.


**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var identifierColumnNames = jsTable.getRowIdentifierColumnNames()
```
### getSQLName()

Returns the table name as defined in the database.


**Returns**\
[String](../JSLib/String.md) String table sql name.


**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var tableNameForQuery = jsTable.getSQLName()
```
### getServerName()

Returns the Servoy server name.


**Returns**\
[String](../JSLib/String.md) String server name.


**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var serverName = jsTable.getServerName()
```
### isMetadataTable()

Returns whether table was flagged as metadata table.


**Returns**\
[Boolean](../JSLib/Boolean.md) boolean is metadata


**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var isMetaDataTable = jsTable.isMetadataTable()
```

