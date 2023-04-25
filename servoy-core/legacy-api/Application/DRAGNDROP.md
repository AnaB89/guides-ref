#  DRAGNDROP

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [COPY](DRAGNDROP.md#COPY)                   | Constant for copy drag operation..                                    |
| [String](../JSLib/String.md) | [MIME_TYPE_SERVOY](DRAGNDROP.md#MIME_TYPE_SERVOY)                   | Constant used as mime type for servoy objects..                                    |
| [String](../JSLib/String.md) | [MIME_TYPE_SERVOY_RECORD](DRAGNDROP.md#MIME_TYPE_SERVOY_RECORD)                   | Constant used as mime type for servoy record objects..                                    |
| [Number](../JSLib/Number.md) | [MOVE](DRAGNDROP.md#MOVE)                   | Constant for move drag operation..                                    |
| [Number](../JSLib/Number.md) | [NONE](DRAGNDROP.md#NONE)                   | Constant for no drag operation..                                    |

## Constants Details

### COPY

Constant for copy drag operation.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
function startDrag(event)
{
	if(event.getElementName() == "copy")
		return DRAGNDROP.COPY;
	else if(event.getElementName() == "move")
		return DRAGNDROP.MOVE

	return DRAGNDROP.NONE;
}
```
### MIME_TYPE_SERVOY

Constant used as mime type for servoy objects.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (event.dataMimeType == DRAGNDROP.MIME_TYPE_SERVOY || event.dataMimeType == DRAGNDROP.MIME_TYPE_SERVOY_RECORD) {
	application.output("Dropping is allowed" );
	return true;
} else {
	application.output("Dropping is not allowed" );
	return false;
}
```
### MIME_TYPE_SERVOY_RECORD

Constant used as mime type for servoy record objects.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (event.dataMimeType == DRAGNDROP.MIME_TYPE_SERVOY || event.dataMimeType == DRAGNDROP.MIME_TYPE_SERVOY_RECORD) {
	application.output("Dropping is allowed" );
	return true;
} else {
	application.output("Dropping is not allowed" );
	return false;
}
```
### MOVE

Constant for move drag operation.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
function startDrag(event)
{
	if(event.getElementName() == "copy")
		return DRAGNDROP.COPY;
	else if(event.getElementName() == "move")
		return DRAGNDROP.MOVE

	return DRAGNDROP.NONE;
}
```
### NONE

Constant for no drag operation.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
function startDrag(event)
{
	if(event.getElementName() == "copy")
		return DRAGNDROP.COPY;
	else if(event.getElementName() == "move")
		return DRAGNDROP.MOVE

	return DRAGNDROP.NONE;
}
```

