# DBDataSourceServer

## Methods Summary

| Type                                                | Name                                                                     | Summary                                                                                                                                                       |
| --------------------------------------------------- | ------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [JSConnectionDefinition](jsconnectiondefinition.md) | [defineClientConnection()](dbdatasourceserver.md#defineclientconnection) | Define a client connection for this server, you can configure this DB Server to create connections for this client that are configured by this JSConnection.. |
| [DBDataSourceServer](dbdatasourceserver.md)         | [getDataModelCloneFrom()](dbdatasourceserver.md#getdatamodelclonefrom)   | Get the server where this server is a data model clone from..                                                                                                 |
| [String](../js-lib/string.md)                       | [getServerName()](dbdatasourceserver.md#getservername)                   | Get the server name..                                                                                                                                         |
| [Array](../js-lib/array.md)                         | [getTableNames()](dbdatasourceserver.md#gettablenames)                   | Returns an array with the names of all tables of this server..                                                                                                |

## Methods Details

### defineClientConnection()

Define a client connection for this server, you can configure this DB Server to create connections for this client that are configured by this JSConnection. All interaction with the database will go over a connection coming from a specific client pool with that is created for tihs client. Things like username,password or connection properties can be adjusted.

**Returns**\
[JSConnectionDefinition](jsconnectiondefinition.md) DBDataSourceServer server

**Sample**

```javascript
var conncetionDefinition = datasources.db.example_data.defineClientConnection().setProperty('key', 'value').create();
```

### getDataModelCloneFrom()

Get the server where this server is a data model clone from.

**Returns**\
[DBDataSourceServer](dbdatasourceserver.md) DBDataSourceServer server

**Sample**

```javascript
datasources.db.example_data.getDataModelCloneFrom().getServerName()
```

### getServerName()

Get the server name.

**Returns**\
[String](../js-lib/string.md) String server name

**Sample**

```javascript
datasources.db.example_data.getServerName() // returns 'example_data'
```

### getTableNames()

Returns an array with the names of all tables of this server.

**Returns**\
[Array](../js-lib/array.md) String\[] server table names;

**Sample**

```javascript
datasources.db.example_data.getTableNames()
```
