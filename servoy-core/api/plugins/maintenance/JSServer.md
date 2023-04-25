#  JSServer


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSTableObject](./JSTableObject.md) | [createNewTable(tableName)](JSServer.md#createnewtable-tablename)                   | Creates in this server a new table with the specified name..                                    |
| [Boolean](../../JSLib/Boolean.md) | [dropTable(tableName)](JSServer.md#droptable-tablename)                   | Drops the table with the specified name from this server..                                    |
| [JSTableObject](./JSTableObject.md) | [getTable(tableName)](JSServer.md#gettable-tablename)                   | Returns a JSTable instance corresponding to the table with the specified name from this server..                                    |
| [Array](../../JSLib/Array.md) | [getTableNames()](JSServer.md#gettablenames)                   | Returns an array with the names of all tables in this server..                                    |
| [Boolean](../../JSLib/Boolean.md) | [isValid()](JSServer.md#isvalid)                   | Get valid state for the server..                                    |
|void | [reloadDataModel()](JSServer.md#reloaddatamodel)                   | Reloads the datamodel from the database, if changed externally or via rawSQL plugin..                                    |
| [Boolean](../../JSLib/Boolean.md) | [synchronizeWithDB(table)](JSServer.md#synchronizewithdb-table)                   | Synchronizes a JSTable instance with the database..                                    |

## Methods Details

### createNewTable(tableName)

Creates in this server a new table with the specified name.

**Parameters**\
[String](../../JSLib/String.md) tableName The name of the table to create.

**Returns**\
[JSTableObject](./JSTableObject.md) JSTableObject created table.


**Sample**

```javascript
var server = plugins.maintenance.getServer("example_data");
if (server)
{
	var table = server.createNewTable("new_table");
	if (table) {
		var pk = table.createNewColumn("new_table_id", JSColumn.INTEGER, 0);
		pk.rowIdentifierType = JSColumn.PK_COLUMN;
		if (server.synchronizeWithDB(table))
			application.output("New table created in the database.");
		else
			application.output("New table not created in database.");
	}
	else application.output("New table not created at all.");
}
```
### dropTable(tableName)

Drops the table with the specified name from this server.

**Parameters**\
[String](../../JSLib/String.md) tableName The name of the table to drop.

**Returns**\
[Boolean](../../JSLib/Boolean.md) boolean success.


**Sample**

```javascript
var server = plugins.maintenance.getServer("example_data");
if (server) {
	var result = server.dropTable("new_table");
	if (result)
		application.output("Table dropped.");
	else
		application.output("Table not dropped.");
}
```
### getTable(tableName)

Returns a JSTable instance corresponding to the table with the specified name from this server.

**Parameters**\
[String](../../JSLib/String.md) tableName The name of the table to retrieve.

**Returns**\
[JSTableObject](./JSTableObject.md) JSTableObject table.


**Sample**

```javascript
var server = plugins.maintenance.getServer("example_data");
if (server) {
	var table = server.getTable("employees");
	if (table) {
		var colNames = table.getColumnNames()
		application.output("Table has " + colNames.length + " columns.");
		for (var i=0; i<colNames.length; i++)
			application.output("Column " + i + ": " + colNames[i]);
	}
}
```
### getTableNames()

Returns an array with the names of all tables in this server.


**Returns**\
[Array](../../JSLib/Array.md) Array of String table names.


**Sample**

```javascript
var server = plugins.maintenance.getServer("example_data");
if (server) {
	var tableNames = server.getTableNames();
	application.output("There are " + tableNames.length + " tables.");
	for (var i=0; i<tableNames.length; i++)
		application.output("Table " + i + ": " + tableNames[i]);
}
else {
	plugins.dialogs.showInfoDialog("Attention","Server 'example_data' cannot be found.","OK");
}
```
### isValid()

Get valid state for the server.


**Returns**\
[Boolean](../../JSLib/Boolean.md) boolean valid state.


**Sample**

```javascript
var server = plugins.maintenance.getServer("example_data");
if (!server.isValid()) {
	application.output("Server not valid!");
}
```
### reloadDataModel()

Reloads the datamodel from the database, if changed externally or via rawSQL plugin.

This call is not needed after a call to synchronizeWithDB().


**Returns**\
void 


**Sample**

```javascript
var server = plugins.maintenance.getServer("example_data");
var result = plugins.rawSQL.executeSQL("example_data", null, 'CREATE TABLE raw_table (raw_table_id INTEGER)');
if (result) {
	application.output("Table created through rawSQL plugin.");
	if (server) {
		server.reloadDataModel();
		// All existing JSTableObject/JSColumn object references are invalid now! Use getTable to get new ones.
		var table = server.getTable("raw_table");
		if (table) {
			var colNames = table.getColumnNames()
			application.output("Table has " + colNames.length + " columns.");
			for (var i=0; i<colNames.length; i++)
				application.output("Column " + i + ": " + colNames[i]);
		}
	}
}
else {
	application.output("Raw table creation failed: " + plugins.rawSQL.getException());
}
```
### synchronizeWithDB(table)

Synchronizes a JSTable instance with the database. If columns were added to or removed from the JSTable instance, all these changes will now be persisted to the database.

**Parameters**\
[JSTableObject](./JSTableObject.md) table A JSTableObject instance that should be synchronized.

**Returns**\
[Boolean](../../JSLib/Boolean.md) boolean success.


**Sample**

```javascript
var server = plugins.maintenance.getServer("example_data");
if (server)
{
	var table = server.createNewTable("new_table");
	if (table) {
		var pk = table.createNewColumn("new_table_id", JSColumn.INTEGER, 0);
		pk.rowIdentifierType = JSColumn.PK_COLUMN;
		if (server.synchronizeWithDB(table))
			application.output("New table created in the database.");
		else
			application.output("New table not created in database.");
	}
	else application.output("New table not created at all.");
}
```

