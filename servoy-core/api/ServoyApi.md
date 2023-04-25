#  ServoyApi


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](JSLib/Boolean.md) | [addFoundSetFilterParam(foundset, query, filterName)](ServoyApi.md#addfoundsetfilterparam-foundset-query-filtername)                   | Add a filter parameter that is permanent per user session to limit a specified foundset of records..                                    |
| [Object](JSLib/Object.md) | [copyObject(value)](ServoyApi.md#copyobject-value)                   | Can be used to deep copy a custom value..                                    |
| [JSDataSet](Database%20Manager/JSDataSet.md) | [getDataSetByQuery(query, max_returned_rows)](ServoyApi.md#getdatasetbyquery-query-max_returned_rows)                   | Performs a sql query with a query builder object..                                    |
| [Array](JSLib/Array.md) | [getDatasourcePKs(datasource)](ServoyApi.md#getdatasourcepks-datasource)                   | This will generate a list of primary keys names for the given data source..                                    |
| [String](JSLib/String.md) | [getMediaUrl(bytes)](ServoyApi.md#getmediaurl-bytes)                   | This will generate a url from a byte array so that the client can get the bytes from that url..                                    |
| [QBSelect](Database%20Manager/QBSelect.md) | [getQuerySelect(dataSource)](ServoyApi.md#getqueryselect-datasource)                   | Get select query for dataSource.                                    |
| [JSFoundSet](Database%20Manager/JSFoundSet.md) | [getViewFoundSet(name, query)](ServoyApi.md#getviewfoundset-name-query)                   | .                                    |
| [Boolean](JSLib/Boolean.md) | [hideForm(formName)](ServoyApi.md#hideform-formname)                   | Hide a form directly on the server for instance when a tab will change on the client, so it won't need to do a round trip for hiding the form through the browser's component..                                    |
| [Boolean](JSLib/Boolean.md) | [showForm(nameOrUUID)](ServoyApi.md#showform-nameoruuid)                   | Show a form directly on the server for instance when a tab will change on the client, so it won't need to do a round trip for showing the form through the browser's component..                                    |
| [Boolean](JSLib/Boolean.md) | [showForm(nameOrUUID, relationName)](ServoyApi.md#showform-nameoruuid-relationname)                   | Show a form directly on the server for instance when a tab will change on the client, so it won't need to do a round trip for showing the form through the browser's component..                                    |

## Methods Details

### addFoundSetFilterParam(foundset, query, filterName)

Add a filter parameter that is permanent per user session to limit a specified foundset of records.
This is similar as calling foundset.js_addFoundSetFilterParam, but the main difference is that this
works also on related foundsets.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset The foundset to add the filter param/query to\
[QBSelect](Database%20Manager/QBSelect.md) query The query repesenting the filter\
[String](JSLib/String.md) filterName a name given to this foundset filter

**Returns**\
[Boolean](JSLib/Boolean.md) 


**Sample**

```javascript

```
### copyObject(value)

Can be used to deep copy a custom value.

**Parameters**\
[Object](JSLib/Object.md) value the value to be copied

**Returns**\
[Object](JSLib/Object.md) a copy of the value object, the same as constructing the object in javascript from scratch


**Sample**

```javascript
var eventSourceCopy = servoyApi.copyObject(eventSource);
```
### getDataSetByQuery(query, max_returned_rows)

Performs a sql query with a query builder object.
Will throw an exception if anything did go wrong when executing the query.
Will use any data filter defined on table.

**Parameters**\
[QBSelect](Database%20Manager/QBSelect.md) query QBSelect query.\
[Number](JSLib/Number.md) max_returned_rows The maximum number of rows returned by the query.

**Returns**\
[JSDataSet](Database%20Manager/JSDataSet.md) The JSDataSet containing the results of the query.


**Sample**

```javascript
var dataset = servoyApi.getDataSetByQuery(qbselect, 10);
```
### getDatasourcePKs(datasource)

This will generate a list of primary keys names for the given data source.

**Parameters**\
[String](JSLib/String.md) datasource the data source

**Returns**\
[Array](JSLib/Array.md) a list of primary key names


**Sample**

```javascript
var pkNames = servoyApi.getDatasourcePKs(datasource);
```
### getMediaUrl(bytes)

This will generate a url from a byte array so that the client can get the bytes from that url.

**Parameters**\
[Array](JSLib/Array.md) bytes The value where an url should be created for

**Returns**\
[String](JSLib/String.md) the url where the bytes can be downloaded from


**Sample**

```javascript
var url = servoyApi.getMediaUrl(bytes);
```
### getQuerySelect(dataSource)

Get select query for dataSource

**Parameters**\
[String](JSLib/String.md) dataSource the dataSource

**Returns**\
[QBSelect](Database%20Manager/QBSelect.md) QB select for the dataSource


**Sample**

```javascript

```
### getViewFoundSet(name, query)



**Parameters**\
[String](JSLib/String.md) name  ;\
[QBSelect](Database%20Manager/QBSelect.md) query  ;

**Returns**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) 


**Sample**

```javascript

```
### hideForm(formName)

Hide a form directly on the server for instance when a tab will change on the client, so it won't need to do a round trip
for hiding the form through the browser's component.

**Parameters**\
[Object](JSLib/Object.md) formName the form to hide

**Returns**\
[Boolean](JSLib/Boolean.md) true if the form was hidden


**Sample**

```javascript
servoyApi.hideForm(formToHideName)
```
### showForm(nameOrUUID)

Show a form directly on the server for instance when a tab will change on the client, so it won't need to do a round trip
for showing the form through the browser's component.

**Parameters**\
[String](JSLib/String.md) nameOrUUID the form to show

**Returns**\
[Boolean](JSLib/Boolean.md) true if the form was marked as visible


**Sample**

```javascript
servoyApi.showForm(formToHideName)
```
### showForm(nameOrUUID, relationName)

Show a form directly on the server for instance when a tab will change on the client, so it won't need to do a round trip
for showing the form through the browser's component.

**Parameters**\
[String](JSLib/String.md) nameOrUUID the form to show\
[String](JSLib/String.md) relationName the parent container

**Returns**\
[Boolean](JSLib/Boolean.md) true if the form was marked as visible


**Sample**

```javascript
servoyApi.showForm(formToHideName)
```

