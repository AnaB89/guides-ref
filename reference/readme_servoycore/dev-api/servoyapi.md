# ServoyApi

## Methods Summary

| Type                                         | Name                                                                                                                 | Summary                                                                                                                                                                          |
| -------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Boolean](js-lib/boolean.md)                 | [addFoundSetFilterParam(foundset, query, filterName)](servoyapi.md#addfoundsetfilterparam-foundset-query-filtername) | Add a filter parameter that is permanent per user session to limit a specified foundset of records..                                                                             |
| [Object](js-lib/object.md)                   | [copyObject(value)](servoyapi.md#copyobject-value)                                                                   | Can be used to deep copy a custom value..                                                                                                                                        |
| [JSDataSet](database-manager/jsdataset.md)   | [getDataSetByQuery(query, max\_returned\_rows)](servoyapi.md#getdatasetbyquery-query-max\_returned\_rows)            | Performs a sql query with a query builder object..                                                                                                                               |
| [Array](js-lib/array.md)                     | [getDatasourcePKs(datasource)](servoyapi.md#getdatasourcepks-datasource)                                             | This will generate a list of primary keys names for the given data source..                                                                                                      |
| [String](js-lib/string.md)                   | [getMediaUrl(bytes)](servoyapi.md#getmediaurl-bytes)                                                                 | This will generate a url from a byte array so that the client can get the bytes from that url..                                                                                  |
| [QBSelect](database-manager/qbselect.md)     | [getQuerySelect(dataSource)](servoyapi.md#getqueryselect-datasource)                                                 | Get select query for dataSource.                                                                                                                                                 |
| [JSFoundSet](database-manager/jsfoundset.md) | [getViewFoundSet(name, query)](servoyapi.md#getviewfoundset-name-query)                                              | .                                                                                                                                                                                |
| [Boolean](js-lib/boolean.md)                 | [hideForm(formName)](servoyapi.md#hideform-formname)                                                                 | Hide a form directly on the server for instance when a tab will change on the client, so it won't need to do a round trip for hiding the form through the browser's component..  |
| [Boolean](js-lib/boolean.md)                 | [showForm(nameOrUUID)](servoyapi.md#showform-nameoruuid)                                                             | Show a form directly on the server for instance when a tab will change on the client, so it won't need to do a round trip for showing the form through the browser's component.. |
| [Boolean](js-lib/boolean.md)                 | [showForm(nameOrUUID, relationName)](servoyapi.md#showform-nameoruuid-relationname)                                  | Show a form directly on the server for instance when a tab will change on the client, so it won't need to do a round trip for showing the form through the browser's component.. |

## Methods Details

### addFoundSetFilterParam(foundset, query, filterName)

Add a filter parameter that is permanent per user session to limit a specified foundset of records. This is similar as calling foundset.js\_addFoundSetFilterParam, but the main difference is that this works also on related foundsets.

**Parameters**\
[JSFoundSet](database-manager/jsfoundset.md) foundset The foundset to add the filter param/query to\
[QBSelect](database-manager/qbselect.md) query The query repesenting the filter\
[String](js-lib/string.md) filterName a name given to this foundset filter

**Returns**\
[Boolean](js-lib/boolean.md)

**Sample**

```javascript
```

### copyObject(value)

Can be used to deep copy a custom value.

**Parameters**\
[Object](js-lib/object.md) value the value to be copied

**Returns**\
[Object](js-lib/object.md) a copy of the value object, the same as constructing the object in javascript from scratch

**Sample**

```javascript
var eventSourceCopy = servoyApi.copyObject(eventSource);
```

### getDataSetByQuery(query, max\_returned\_rows)

Performs a sql query with a query builder object. Will throw an exception if anything did go wrong when executing the query. Will use any data filter defined on table.

**Parameters**\
[QBSelect](database-manager/qbselect.md) query QBSelect query.\
[Number](js-lib/number.md) max\_returned\_rows The maximum number of rows returned by the query.

**Returns**\
[JSDataSet](database-manager/jsdataset.md) The JSDataSet containing the results of the query.

**Sample**

```javascript
var dataset = servoyApi.getDataSetByQuery(qbselect, 10);
```

### getDatasourcePKs(datasource)

This will generate a list of primary keys names for the given data source.

**Parameters**\
[String](js-lib/string.md) datasource the data source

**Returns**\
[Array](js-lib/array.md) a list of primary key names

**Sample**

```javascript
var pkNames = servoyApi.getDatasourcePKs(datasource);
```

### getMediaUrl(bytes)

This will generate a url from a byte array so that the client can get the bytes from that url.

**Parameters**\
[Array](js-lib/array.md) bytes The value where an url should be created for

**Returns**\
[String](js-lib/string.md) the url where the bytes can be downloaded from

**Sample**

```javascript
var url = servoyApi.getMediaUrl(bytes);
```

### getQuerySelect(dataSource)

Get select query for dataSource

**Parameters**\
[String](js-lib/string.md) dataSource the dataSource

**Returns**\
[QBSelect](database-manager/qbselect.md) QB select for the dataSource

**Sample**

```javascript
```

### getViewFoundSet(name, query)

**Parameters**\
[String](js-lib/string.md) name ;\
[QBSelect](database-manager/qbselect.md) query ;

**Returns**\
[JSFoundSet](database-manager/jsfoundset.md)

**Sample**

```javascript
```

### hideForm(formName)

Hide a form directly on the server for instance when a tab will change on the client, so it won't need to do a round trip for hiding the form through the browser's component.

**Parameters**\
[Object](js-lib/object.md) formName the form to hide

**Returns**\
[Boolean](js-lib/boolean.md) true if the form was hidden

**Sample**

```javascript
servoyApi.hideForm(formToHideName)
```

### showForm(nameOrUUID)

Show a form directly on the server for instance when a tab will change on the client, so it won't need to do a round trip for showing the form through the browser's component.

**Parameters**\
[String](js-lib/string.md) nameOrUUID the form to show

**Returns**\
[Boolean](js-lib/boolean.md) true if the form was marked as visible

**Sample**

```javascript
servoyApi.showForm(formToHideName)
```

### showForm(nameOrUUID, relationName)

Show a form directly on the server for instance when a tab will change on the client, so it won't need to do a round trip for showing the form through the browser's component.

**Parameters**\
[String](js-lib/string.md) nameOrUUID the form to show\
[String](js-lib/string.md) relationName the parent container

**Returns**\
[Boolean](js-lib/boolean.md) true if the form was marked as visible

**Sample**

```javascript
servoyApi.showForm(formToHideName)
```
