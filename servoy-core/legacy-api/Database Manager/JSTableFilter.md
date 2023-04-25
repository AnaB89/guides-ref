#  JSTableFilter

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [serverName](JSTableFilter.md#serverName)                   | Returns the server name..                                    |
| [String](../JSLib/String.md) | [tableName](JSTableFilter.md#tableName)                   | Returns the table name..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSTableFilter](./JSTableFilter.md) | [dataBroadcast(boolean)](JSTableFilter.md#databroadcast-boolean)                   | Set the dataBroadcast flag..                                    |

## Properties Details

### serverName

Returns the server name.

**Returns**\
[String](../JSLib/String.md) String server name.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var filter = databaseManager.createTableFilterParam('admin', 'messages', 'messagesid', '>', 10)
var serverName = filter.serverName // admin
```
### tableName

Returns the table name.

**Returns**\
[String](../JSLib/String.md) String table name.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var filter = databaseManager.createTableFilterParam('admin', 'messages', 'messagesid', '>', 10)
var tableName = filter.tableName // messages
```

## Methods Details

### dataBroadcast(boolean)

Set the dataBroadcast flag.
<p>
When the dataBroadcast flag is set, this filter will be used server-side to reduce databroadcast events
for clients having a databroadcast filter set for the same column with a different value.
<p>
Note that the dataBroadcast flag is *only* supported for simple filters, only for operator 'in' or '='.

**Parameters**\
[Boolean](../JSLib/Boolean.md) 

**Returns**\
[JSTableFilter](./JSTableFilter.md) filter.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var filter = databaseManager.createTableFilterParam('example', 'orders', 'clusterid', '=', 10).dataBroadcast(true)
```

