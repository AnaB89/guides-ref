# JSTableFilter

## Property Summary

| Type                          | Name                                      | Summary                   |
| ----------------------------- | ----------------------------------------- | ------------------------- |
| [String](../js-lib/string.md) | [serverName](jstablefilter.md#serverName) | Returns the server name.. |
| [String](../js-lib/string.md) | [tableName](jstablefilter.md#tableName)   | Returns the table name..  |

## Methods Summary

| Type                              | Name                                                             | Summary                      |
| --------------------------------- | ---------------------------------------------------------------- | ---------------------------- |
| [JSTableFilter](jstablefilter.md) | [dataBroadcast(boolean)](jstablefilter.md#databroadcast-boolean) | Set the dataBroadcast flag.. |

## Properties Details

### serverName

Returns the server name.

**Returns**\
[String](../js-lib/string.md) String server name.

**Sample**

```javascript
var filter = databaseManager.createTableFilterParam('admin', 'messages', 'messagesid', '>', 10)
var serverName = filter.serverName // admin
```

### tableName

Returns the table name.

**Returns**\
[String](../js-lib/string.md) String table name.

**Sample**

```javascript
var filter = databaseManager.createTableFilterParam('admin', 'messages', 'messagesid', '>', 10)
var tableName = filter.tableName // messages
```

## Methods Details

### dataBroadcast(boolean)

Set the dataBroadcast flag.

When the dataBroadcast flag is set, this filter will be used server-side to reduce databroadcast events for clients having a databroadcast filter set for the same column with a different value.

Note that the dataBroadcast flag is \*only\* supported for simple filters, only for operator 'in' or '='.

**Parameters**\
[Boolean](../js-lib/boolean.md)

**Returns**\
[JSTableFilter](jstablefilter.md) filter.

**Sample**

```javascript
var filter = databaseManager.createTableFilterParam('example', 'orders', 'clusterid', '=', 10).dataBroadcast(true)
```
