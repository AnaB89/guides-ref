# DRAGNDROP

## Constants Summary

| Type                          | Name                                                                  | Summary                                                |
| ----------------------------- | --------------------------------------------------------------------- | ------------------------------------------------------ |
| [Number](../js-lib/number.md) | [COPY](dragndrop.md#COPY)                                             | Constant for copy drag operation..                     |
| [String](../js-lib/string.md) | [MIME\_TYPE\_SERVOY](dragndrop.md#MIME\_TYPE\_SERVOY)                 | Constant used as mime type for servoy objects..        |
| [String](../js-lib/string.md) | [MIME\_TYPE\_SERVOY\_RECORD](dragndrop.md#MIME\_TYPE\_SERVOY\_RECORD) | Constant used as mime type for servoy record objects.. |
| [Number](../js-lib/number.md) | [MOVE](dragndrop.md#MOVE)                                             | Constant for move drag operation..                     |
| [Number](../js-lib/number.md) | [NONE](dragndrop.md#NONE)                                             | Constant for no drag operation..                       |

## Constants Details

### COPY

Constant for copy drag operation.

**Returns**\
[Number](../js-lib/number.md)

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

### MIME\_TYPE\_SERVOY

Constant used as mime type for servoy objects.

**Returns**\
[String](../js-lib/string.md)

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

### MIME\_TYPE\_SERVOY\_RECORD

Constant used as mime type for servoy record objects.

**Returns**\
[String](../js-lib/string.md)

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
[Number](../js-lib/number.md)

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
[Number](../js-lib/number.md)

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
