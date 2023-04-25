#  WsContents


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Array](../../JSLib/Array.md) | [bytes](WsContents.md#bytes)                   | Get contents bytes..                                    |
| [String](../../JSLib/String.md) | [contentType](WsContents.md#contentType)                   | Get contents content type..                                    |
| [String](../../JSLib/String.md) | [fieldName](WsContents.md#fieldName)                   | Get contents field name..                                    |
| [String](../../JSLib/String.md) | [name](WsContents.md#name)                   | Get contents name..                                    |
| [Number](../../JSLib/Number.md) | [size](WsContents.md#size)                   | Get contents size..                                    |
| [String](../../JSLib/String.md) | [string](WsContents.md#string)                   | Get contents as string..                                    |

## Properties Details

### bytes

Get contents bytes.

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
var request = plugins.rest_ws.getRequest();
var contents = request.getContents();
if (contents.length > 0) {
   var bytes = contents[0].getBytes();
}
```
### contentType

Get contents content type.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var request = plugins.rest_ws.getRequest();
var contents = request.getContents();
if (contents.length > 0) {
   var contentType = contents[0].getContentType();
}
```
### fieldName

Get contents field name.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var request = plugins.rest_ws.getRequest();
var contents = request.getContents();
if (contents.length > 0) {
   var fieldName = contents[0].getFieldName();
}
```
### name

Get contents name.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var request = plugins.rest_ws.getRequest();
var contents = request.getContents();
if (contents.length > 0) {
   var name = contents[0].getName();
}
```
### size

Get contents size.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var request = plugins.rest_ws.getRequest();
var contents = request.getContents();
if (contents.length > 0) {
   var size = contents[0].getSize();
}
```
### string

Get contents as string.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var request = plugins.rest_ws.getRequest();
var contents = request.getContents();
if (contents.length > 0) {
   var string = contents[0].getString('UTF-8');
}
```

