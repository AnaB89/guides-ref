#  JSMedia


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Array](../JSLib/Array.md) | [bytes](JSMedia.md#bytes)                   | A byte array holding the content of the Media object..                                    |
| [String](../JSLib/String.md) | [mimeType](JSMedia.md#mimeType)                   | The MIME type of the Media object..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [getAsString()](JSMedia.md#getasstring)                   | Returns this media's bytes a a String converting it with the UTF-8 Charset..                                    |
| [String](../JSLib/String.md) | [getName()](JSMedia.md#getname)                   | The name of the Media object..                                    |
| [UUID](../Application/UUID.md) | [getUUID()](JSMedia.md#getuuid)                   | Returns the UUID of this media.                                    |
|void | [setAsString(string)](JSMedia.md#setasstring-string)                   | Sets the bytes of this media to the give String that is converted to bytes using the UTF-8 Charset..                                    |

## Properties Details

### bytes

A byte array holding the content of the Media object.

**Returns**\
[Array](../JSLib/Array.md) 


**Sample**

```javascript
var ballBytes = plugins.file.readFile('d:/ball.jpg');
var mapBytes = plugins.file.readFile('d:/map.png');
var ballImage = solutionModel.newMedia('ball.jpg', ballBytes);
application.output('original image name: ' + ballImage.getName());
ballImage.bytes = mapBytes;
ballImage.mimeType = 'image/png';
application.output('image name after change: ' + ballImage.getName()); // The name remains unchanged. Only the content (bytes) are changed.
application.output('image mime type: ' + ballImage.mimeType);
application.output('image size: ' + ballImage.bytes.length);
```
### mimeType

The MIME type of the Media object.

Some examples are: 'image/jpg', 'image/png', etc.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var ballBytes = plugins.file.readFile('d:/ball.jpg');
var mapBytes = plugins.file.readFile('d:/map.png');
var ballImage = solutionModel.newMedia('ball.jpg', ballBytes);
application.output('original image name: ' + ballImage.getName());
ballImage.bytes = mapBytes;
ballImage.mimeType = 'image/png';
application.output('image name after change: ' + ballImage.getName()); // The name remains unchanged. Only the content (bytes) are changed.
application.output('image mime type: ' + ballImage.mimeType);
application.output('image size: ' + ballImage.bytes.length);
```

## Methods Details

### getAsString()

Returns this media's bytes a a String converting it with the UTF-8 Charset.
Returns null if it couldn't convert it or the bytes where null.


**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### getName()

The name of the Media object.


**Returns**\
[String](../JSLib/String.md) A String holding the name of this Media object.


**Sample**

```javascript
var ballBytes = plugins.file.readFile('d:/ball.jpg');
var mapBytes = plugins.file.readFile('d:/map.png');
var ballImage = solutionModel.newMedia('ball.jpg', ballBytes);
application.output('original image name: ' + ballImage.getName());
ballImage.bytes = mapBytes;
ballImage.mimeType = 'image/png';
application.output('image name after change: ' + ballImage.getName()); // The name remains unchanged. Only the content (bytes) are changed.
application.output('image mime type: ' + ballImage.mimeType);
application.output('image size: ' + ballImage.bytes.length);
```
### getUUID()

Returns the UUID of this media


**Returns**\
[UUID](../Application/UUID.md) 


**Sample**

```javascript
var ballImg = plugins.file.readFile('d:/ball.jpg');
application.output(ballImg.getUUID().toString());
```
### setAsString(string)

Sets the bytes of this media to the give String that is converted to bytes using the UTF-8 Charset.

**Parameters**\
[String](../JSLib/String.md) string  ;

**Returns**\
void 


**Sample**

```javascript

```

