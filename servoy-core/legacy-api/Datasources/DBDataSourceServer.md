#  DBDataSourceServer

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSConnectionDefinition](./JSConnectionDefinition.md) | [defineClientConnection()](DBDataSourceServer.md#defineclientconnection)                   | Define a client connection for this server, you can configure this DB Server to create connections for this client that are configured by this JSConnection..                                    |
| [DBDataSourceServer](./DBDataSourceServer.md) | [getDataModelCloneFrom()](DBDataSourceServer.md#getdatamodelclonefrom)                   | Get the server where this server is a data model clone from..                                    |
| [String](../JSLib/String.md) | [getServerName()](DBDataSourceServer.md#getservername)                   | Get the server name..                                    |
| [Array](../JSLib/Array.md) | [getTableNames()](DBDataSourceServer.md#gettablenames)                   | Returns an array with the names of all tables of this server..                                    |

## Methods Details

### defineClientConnection()

Define a client connection for this server, you can configure this DB Server to create connections for this client that are configured by this JSConnection.
All interaction with the database will go over a connection coming from a specific client pool with that is created for tihs client.
Things like username,password or connection properties can be adjusted.


**Returns**\
[JSConnectionDefinition](./JSConnectionDefinition.md) DBDataSourceServer server

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var conncetionDefinition = datasources.db.example_data.defineClientConnection().setProperty('key', 'value').create();
```
### getDataModelCloneFrom()

Get the server where this server is a data model clone from.


**Returns**\
[DBDataSourceServer](./DBDataSourceServer.md) DBDataSourceServer server

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
datasources.db.example_data.getDataModelCloneFrom().getServerName()
```
### getServerName()

Get the server name.


**Returns**\
[String](../JSLib/String.md) String server name

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
datasources.db.example_data.getServerName() // returns 'example_data'
```
### getTableNames()

Returns an array with the names of all tables of this server.


**Returns**\
[Array](../JSLib/Array.md) String[] server table names;

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
datasources.db.example_data.getTableNames()
```

