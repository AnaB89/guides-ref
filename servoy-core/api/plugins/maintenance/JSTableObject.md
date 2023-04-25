#  JSTableObject


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSColumnObject](./JSColumnObject.md) | [createNewColumn(columnName, type, length)](JSTableObject.md#createnewcolumn-columnname-type-length)                   | Creates a new column in this table..                                    |
| [JSColumnObject](./JSColumnObject.md) | [createNewColumn(columnName, type, length, allowNull)](JSTableObject.md#createnewcolumn-columnname-type-length-allownull)                   | Creates a new column in this table..                                    |
| [JSColumnObject](./JSColumnObject.md) | [createNewColumn(columnName, type, length, allowNull, pkColumn)](JSTableObject.md#createnewcolumn-columnname-type-length-allownull-pkcolumn)                   | Creates a new column in this table..                                    |
|void | [deleteColumn(columnName)](JSTableObject.md#deletecolumn-columnname)                   | Deletes the column with the specified name from this table..                                    |
| [JSColumn](../../Database%20Manager/JSColumn.md) | [getColumn(name)](JSTableObject.md#getcolumn-name)                   | Returns a JSColumn for the named column (or column dataproviderID)..                                    |
| [Array](../../JSLib/Array.md) | [getColumnNames()](JSTableObject.md#getcolumnnames)                   | Returns an array containing the names of all table columns..                                    |
| [String](../../JSLib/String.md) | [getDataSource()](JSTableObject.md#getdatasource)                   | Returns the table data source uri..                                    |
| [String](../../JSLib/String.md) | [getQuotedSQLName()](JSTableObject.md#getquotedsqlname)                   | Returns a quoted version of the table name, if necessary, as defined by the actual database used..                                    |
| [Array](../../JSLib/Array.md) | [getRowIdentifierColumnNames()](JSTableObject.md#getrowidentifiercolumnnames)                   | Returns an array containing the names of the identifier (PK) column(s)..                                    |
| [String](../../JSLib/String.md) | [getSQLName()](JSTableObject.md#getsqlname)                   | Returns the table name as defined in the database..                                    |
| [String](../../JSLib/String.md) | [getServerName()](JSTableObject.md#getservername)                   | Returns the Servoy server name..                                    |
| [Boolean](../../JSLib/Boolean.md) | [isMetadataTable()](JSTableObject.md#ismetadatatable)                   | Returns whether table was flagged as metadata table..                                    |

## Methods Details

### createNewColumn(columnName, type, length)

Creates a new column in this table. The name, type and length of the new column must be specified. For specifying the
type of the column, use the JSColumn constants. The column is not actually created in the database until this
table is synchronized with the database using the JSServer.synchronizeWithDB method.

The method returns a JSColumn instance that corresponds to the newly created column. If any error occurs and the column cannot be created, then the method
returns null.

**Parameters**\
[String](../../JSLib/String.md) columnName  ;\
[Number](../../JSLib/Number.md) type  ;\
[Number](../../JSLib/Number.md) length  ;

**Returns**\
[JSColumnObject](./JSColumnObject.md) 


**Sample**

```javascript
var server = plugins.maintenance.getServer("example_data");
if (server)
{
	var table = server.createNewTable("users");
	if (table)
	{
		var pk = table.createNewColumn("id", JSColumn.MEDIA, 16); // can also use (JSColumn.TEXT, 36) for UUIDs
		pk.rowIdentifierType = JSColumn.PK_COLUMN;
		pk.setFlag(JSColumn.UUID_COLUMN, true)
		pk.sequenceType = JSColumn.UUID_GENERATOR
		var c = table.createNewColumn("name", JSColumn.TEXT, 100);
		c.allowNull = false
		table.createNewColumn("age", JSColumn.INTEGER, 0);
		table.createNewColumn("last_login", JSColumn.DATETIME, 0);
		var result = server.synchronizeWithDB(table);
		if (result) application.output("Table successfully created.");
		else application.output("Table not created.");
	}
}
```
### createNewColumn(columnName, type, length, allowNull)

Creates a new column in this table. The name, type and length of the new column must be specified. For specifying the
type of the column, use the JSColumn constants. The column is not actually created in the database until this
table is synchronized with the database using the JSServer.synchronizeWithDB method.

The method returns a JSColumn instance that corresponds to the newly created column. If any error occurs and the column cannot be created, then the method
returns null.

**Parameters**\
[String](../../JSLib/String.md) columnName  ;\
[Number](../../JSLib/Number.md) type  ;\
[Number](../../JSLib/Number.md) length  ;\
[Boolean](../../JSLib/Boolean.md) allowNull  ;

**Returns**\
[JSColumnObject](./JSColumnObject.md) 


**Sample**

```javascript
var server = plugins.maintenance.getServer("example_data");
if (server)
{
	var table = server.createNewTable("users");
	if (table)
	{
		var pk = table.createNewColumn("id", JSColumn.MEDIA, 16); // can also use (JSColumn.TEXT, 36) for UUIDs
		pk.rowIdentifierType = JSColumn.PK_COLUMN;
		pk.setFlag(JSColumn.UUID_COLUMN, true)
		pk.sequenceType = JSColumn.UUID_GENERATOR
		var c = table.createNewColumn("name", JSColumn.TEXT, 100);
		c.allowNull = false
		table.createNewColumn("age", JSColumn.INTEGER, 0);
		table.createNewColumn("last_login", JSColumn.DATETIME, 0);
		var result = server.synchronizeWithDB(table);
		if (result) application.output("Table successfully created.");
		else application.output("Table not created.");
	}
}
```
### createNewColumn(columnName, type, length, allowNull, pkColumn)

Creates a new column in this table. The name, type and length of the new column must be specified. For specifying the
type of the column, use the JSColumn constants. The column is not actually created in the database until this
table is synchronized with the database using the JSServer.synchronizeWithDB method.

The method returns a JSColumn instance that corresponds to the newly created column. If any error occurs and the column cannot be created, then the method
returns null.

**Parameters**\
[String](../../JSLib/String.md) columnName  ;\
[Number](../../JSLib/Number.md) type  ;\
[Number](../../JSLib/Number.md) length  ;\
[Boolean](../../JSLib/Boolean.md) allowNull  ;\
[Boolean](../../JSLib/Boolean.md) pkColumn  ;

**Returns**\
[JSColumnObject](./JSColumnObject.md) 


**Sample**

```javascript
var server = plugins.maintenance.getServer("example_data");
if (server)
{
	var table = server.createNewTable("users");
	if (table)
	{
		var pk = table.createNewColumn("id", JSColumn.MEDIA, 16); // can also use (JSColumn.TEXT, 36) for UUIDs
		pk.rowIdentifierType = JSColumn.PK_COLUMN;
		pk.setFlag(JSColumn.UUID_COLUMN, true)
		pk.sequenceType = JSColumn.UUID_GENERATOR
		var c = table.createNewColumn("name", JSColumn.TEXT, 100);
		c.allowNull = false
		table.createNewColumn("age", JSColumn.INTEGER, 0);
		table.createNewColumn("last_login", JSColumn.DATETIME, 0);
		var result = server.synchronizeWithDB(table);
		if (result) application.output("Table successfully created.");
		else application.output("Table not created.");
	}
}
```
### deleteColumn(columnName)

Deletes the column with the specified name from this table. The column is not actually deleted from the database until this
table is synchronized with the database using the JSServer.synchronizeWithDB method.

**Parameters**\
[String](../../JSLib/String.md) columnName  ;

**Returns**\
void 


**Sample**

```javascript
var server = plugins.maintenance.getServer("example_data");
if (server) {
	var table = server.getTable("users");
	if (table) {
		table.deleteColumn("last_login");
		server.synchronizeWithDB(table);
	}
}
```
### getColumn(name)

Returns a JSColumn for the named column (or column dataproviderID).

**Parameters**\
[String](../../JSLib/String.md) name The name of the column to return the value from.

**Returns**\
[JSColumn](../../Database%20Manager/JSColumn.md) JSColumn column.


**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var jsColumn = jsTable.getColumn('campaign_name')
```
### getColumnNames()

Returns an array containing the names of all table columns.
If the table is in mem, then the internal rowid column name is not returned.


**Returns**\
[Array](../../JSLib/Array.md) String array of column names.


**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var columnNames = jsTable.getColumnNames()
```
### getDataSource()

Returns the table data source uri.


**Returns**\
[String](../../JSLib/String.md) String datasource uri.


**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var dataSource = jsTable.getDataSource()
```
### getQuotedSQLName()

Returns a quoted version of the table name, if necessary, as defined by the actual database used.


**Returns**\
[String](../../JSLib/String.md) String table name, quoted if needed.


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
[Array](../../JSLib/Array.md) String array of row identifier column names.


**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var identifierColumnNames = jsTable.getRowIdentifierColumnNames()
```
### getSQLName()

Returns the table name as defined in the database.


**Returns**\
[String](../../JSLib/String.md) String table sql name.


**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var tableNameForQuery = jsTable.getSQLName()
```
### getServerName()

Returns the Servoy server name.


**Returns**\
[String](../../JSLib/String.md) String server name.


**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var serverName = jsTable.getServerName()
```
### isMetadataTable()

Returns whether table was flagged as metadata table.


**Returns**\
[Boolean](../../JSLib/Boolean.md) boolean is metadata


**Sample**

```javascript
var jsTable = databaseManager.getTable('udm', 'campaigns')
var isMetaDataTable = jsTable.isMetadataTable()
```

