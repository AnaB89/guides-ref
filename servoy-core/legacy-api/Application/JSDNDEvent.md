#  JSDNDEvent

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [String](../JSLib/String.md) | [ACTION](JSDNDEvent.md#ACTION)                   | Constant returned by JSEvent..                                    |
| [String](../JSLib/String.md) | [DATACHANGE](JSDNDEvent.md#DATACHANGE)                   | Constant returned by JSEvent..                                    |
| [String](../JSLib/String.md) | [DOUBLECLICK](JSDNDEvent.md#DOUBLECLICK)                   | Constant returned by JSEvent..                                    |
| [String](../JSLib/String.md) | [FOCUSGAINED](JSDNDEvent.md#FOCUSGAINED)                   | Constant returned by JSEvent..                                    |
| [String](../JSLib/String.md) | [FOCUSLOST](JSDNDEvent.md#FOCUSLOST)                   | Constant returned by JSEvent..                                    |
| [String](../JSLib/String.md) | [FORM](JSDNDEvent.md#FORM)                   | Constant returned by JSEvent..                                    |
| [Number](../JSLib/Number.md) | [MODIFIER_ALT](JSDNDEvent.md#MODIFIER_ALT)                   | Constant for the ALT modifier that can be returned by JSDNDEvent..                                    |
| [Number](../JSLib/Number.md) | [MODIFIER_CTRL](JSDNDEvent.md#MODIFIER_CTRL)                   | Constant for the CTRL modifier that can be returned by JSDNDEvent..                                    |
| [Number](../JSLib/Number.md) | [MODIFIER_META](JSDNDEvent.md#MODIFIER_META)                   | Constant for the META modifier that can be returned by JSDNDEvent..                                    |
| [Number](../JSLib/Number.md) | [MODIFIER_SHIFT](JSDNDEvent.md#MODIFIER_SHIFT)                   | Constant for the SHIFT modifier that can be returned by JSDNDEvent..                                    |
| [String](../JSLib/String.md) | [NONE](JSDNDEvent.md#NONE)                   | Constant returned by JSEvent..                                    |
| [String](../JSLib/String.md) | [ONDRAG](JSDNDEvent.md#ONDRAG)                   | Constant returned by JSDNDEvent..                                    |
| [String](../JSLib/String.md) | [ONDRAGEND](JSDNDEvent.md#ONDRAGEND)                   | Constant returned by JSDNDEvent..                                    |
| [String](../JSLib/String.md) | [ONDRAGOVER](JSDNDEvent.md#ONDRAGOVER)                   | Constant returned by JSDNDEvent..                                    |
| [String](../JSLib/String.md) | [ONDROP](JSDNDEvent.md#ONDROP)                   | Constant returned by JSDNDEvent..                                    |
| [String](../JSLib/String.md) | [RIGHTCLICK](JSDNDEvent.md#RIGHTCLICK)                   | Constant returned by JSEvent..                                    |

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Object](../JSLib/Object.md) | [data](JSDNDEvent.md#data)                   | A data object that specific events can set, a user can set data back to the system for events that supports this..                                    |
| [String](../JSLib/String.md) | [dataMimeType](JSDNDEvent.md#dataMimeType)                   | The event data mime type..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [getDragResult()](JSDNDEvent.md#getdragresult)                   | Returns the result of the drag action..                                    |
| [String](../JSLib/String.md) | [getElementName()](JSDNDEvent.md#getelementname)                   | returns the name of the element, can be null if the form was the source of the event..                                    |
| [String](../JSLib/String.md) | [getFormName()](JSDNDEvent.md#getformname)                   | returns the name of the form the element was placed on..                                    |
| [Number](../JSLib/Number.md) | [getModifiers()](JSDNDEvent.md#getmodifiers)                   | Returns the modifiers of the event, see JSDNDEvent..                                    |
| [String](../JSLib/String.md) | [getName()](JSDNDEvent.md#getname)                   | Returns the name of the event which was triggered.                                    |
| [JSRecord](../Database%20Manager/JSRecord.md) | [getRecord()](JSDNDEvent.md#getrecord)                   | Returns the record of the event..                                    |
| [Object](../JSLib/Object.md) | [getSource()](JSDNDEvent.md#getsource)                   | returns the source component/element of the event..                                    |
| [Date](../JSLib/Date.md) | [getTimestamp()](JSDNDEvent.md#gettimestamp)                   | Returns the time the event occurred..                                    |
| [String](../JSLib/String.md) | [getType()](JSDNDEvent.md#gettype)                   | returns the dnd event type see the JSDNDEvents constants what it can return..                                    |
| [Number](../JSLib/Number.md) | [getX()](JSDNDEvent.md#getx)                   | Returns the x position of the event, relative to the component that fired it, if applicable..                                    |
| [Number](../JSLib/Number.md) | [getY()](JSDNDEvent.md#gety)                   | Returns the y position of the event, relative to the component that fired it, if applicable..                                    |

## Constants Details

### ACTION

Constant returned by JSEvent.getType() in a method that is attached to an onAction event.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (event.getType() == JSEvent.ACTION) 
{
	// its an action event.
}
```
### DATACHANGE

Constant returned by JSEvent.getType() in a method that is attached to an onDataChange event.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (event.getType() == JSEvent.DATACHANGE) 
{
	// its a data change event
}
```
### DOUBLECLICK

Constant returned by JSEvent.getType() in a method that is attached to an onDoubleClick event.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (event.getType() == JSEvent.DOUBLECLICK) 
{
	// its a double click event.
}
```
### FOCUSGAINED

Constant returned by JSEvent.getType() in a method that is attached to an onFocusGained or the forms onElementFocusGained event.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (event.getType() == JSEvent.FOCUSGAINED) 
{
	// its a focus gained event.
}
```
### FOCUSLOST

Constant returned by JSEvent.getType() in a method that is attached to an onFocusLost or the forms onElementFocusLost event.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (event.getType() == JSEvent.FOCUSLOST) 
{
	// its a focus lost event.
}
```
### FORM

Constant returned by JSEvent.getType() in a method that is attached to a form event (like onShow) or command (like onDeleteRecord)

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (event.getType() == JSEvent.FORM) 
{
	// its a form event or command
}
```
### MODIFIER_ALT

Constant for the ALT modifier that can be returned by JSDNDEvent.getModifiers();

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//test if the SHIFT modifier is used.
if (event.getModifiers() & JSDNDEvent.MODIFIER_SHIFT)
{
	//do shift action
}
```
### MODIFIER_CTRL

Constant for the CTRL modifier that can be returned by JSDNDEvent.getModifiers();

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//test if the SHIFT modifier is used.
if (event.getModifiers() & JSDNDEvent.MODIFIER_SHIFT)
{
	//do shift action
}
```
### MODIFIER_META

Constant for the META modifier that can be returned by JSDNDEvent.getModifiers();

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//test if the SHIFT modifier is used.
if (event.getModifiers() & JSDNDEvent.MODIFIER_SHIFT)
{
	//do shift action
}
```
### MODIFIER_SHIFT

Constant for the SHIFT modifier that can be returned by JSDNDEvent.getModifiers();

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//test if the SHIFT modifier is used.
if (event.getModifiers() & JSDNDEvent.MODIFIER_SHIFT)
{
	//do shift action
}
```
### NONE

Constant returned by JSEvent.getType() if the event is not used in a known event or command.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (event.getType() == JSEvent.NONE) 
{
	// type is not set.
}
```
### ONDRAG

Constant returned by JSDNDEvent.getType() in a method that is attached to an onDrag event.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (event.getType() == JSDNDEvent.ONDRAG)
{
	// its an ondrag event
	if (event.getElementName() == 'todragelement')
		return DRAGNDROP.COPY
}
```
### ONDRAGEND

Constant returned by JSDNDEvent.getType() in a method that is attached to an onDragEnd event.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (event.getType() == JSDNDEvent.ONDRAGEND)
{
	// its an on drag end event.
	// return true if the drop has been completed successfully
	return event.isDropSuccess();
}
```
### ONDRAGOVER

Constant returned by JSDNDEvent.getType() in a method that is attached to an onDragOver event.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (event.getType() == JSDNDEvent.ONDRAGOVER)
{
	// its an on drag over event.
	// return true if it over the right element.
	return event.getElementName() == 'candroponelement';
}
```
### ONDROP

Constant returned by JSDNDEvent.getType() in a method that is attached to an onDrop event.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (event.getType() == JSDNDEvent.ONDROP)
{
	// its a on drop event.
	var element = elements[event.getElementName()];
	// do drop on element
	return true;
}
```
### RIGHTCLICK

Constant returned by JSEvent.getType() in a method that is attached to an onRightClick event.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (event.getType() == JSEvent.RIGHTCLICK) 
{
	// its a right click event.
}
```

## Properties Details

### data

A data object that specific events can set, a user can set data back to the system for events that supports this.

**Returns**\
[Object](../JSLib/Object.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// A client design method that handles ondrag
if (event.getType() == JSEvent.ONDRAG)
{
     // the data is the selected elements array
     var elements = event.data;
     // only start a client design drag when there is 1 element
     if (elements.length == 1)
     {
     	return true;
     }
}

// code for a data drag method
event.data = "drag me!";
return DRAGNDROP.COPY;

// code for a data drop method
var data = event.data;
elements[event.getElementName()].setText(data);
return true;
```
### dataMimeType

The event data mime type.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// only accept drag if data is a servoy record
function onDragOver(event)
{
	if(event.dataMimeType.indexOf("application/x-servoy-record-object") == 0) return true;
	else return false;
}
```

## Methods Details

### getDragResult()

Returns the result of the drag action.


**Returns**\
[Number](../JSLib/Number.md) a DRAGNDROP constant, representing the result of the drag action

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
function onDragEnd(event)
{
	var dragResult = event.getDragResult();
	if(dragResult == DRAGNDROP.NONE)
	{
		// the drag was canceled
	}
	else if(dragResult == DRAGNDROP.COPY)
	{
		// the drag ended with a copy action
	}
	else if(dragResult == DRAGNDROP.MOVE)
	{
		// the drag ended with a move action
	}
}
```
### getElementName()

returns the name of the element, can be null if the form was the source of the event.


**Returns**\
[String](../JSLib/String.md) a String representing the element name.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (event.getElementName() == 'myElement')
{
    elements[event.getElementName()].bgcolor = '#ff0000';
}
```
### getFormName()

returns the name of the form the element was placed on.


**Returns**\
[String](../JSLib/String.md) a String representing the form name.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
forms[event.getFormName()].myFormMethod();
```
### getModifiers()

Returns the modifiers of the event, see JSDNDEvent.MODIFIER_XXXX for the modifiers that can be returned.


**Returns**\
[Number](../JSLib/Number.md) an int which holds the modifiers as a bitset.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//test if the SHIFT modifier is used.
if (event.getModifiers() & JSDNDEvent.MODIFIER_SHIFT)
{
	//do shift action
}
```
### getName()

Returns the name of the event which was triggered


**Returns**\
[String](../JSLib/String.md) name of event as string

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var name = event.getName();
```
### getRecord()

Returns the record of the event.


**Returns**\
[JSRecord](../Database%20Manager/JSRecord.md) Record of the event

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
event.Record();
```
### getSource()

returns the source component/element of the event.
If it has a name the getElementName() is the name of this component.


**Returns**\
[Object](../JSLib/Object.md) an Object representing the source of this event.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// cast to runtime text field (change to anoter kind of type if you know the type)
/** @type {RuntimeTextField} */
var source = event.getSource();
var sourceDataProvider = source.getDataProviderID();
```
### getTimestamp()

Returns the time the event occurred.


**Returns**\
[Date](../JSLib/Date.md) a Date when this event happened.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
event.getTimestamp();
```
### getType()

returns the dnd event type see the JSDNDEvents constants what it can return.


**Returns**\
[String](../JSLib/String.md) a String representing the type of this event.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (event.getType() == JSDNDEvent.ONDROP)
{
	// it's a drop
}
```
### getX()

Returns the x position of the event, relative to the component that fired it, if applicable.
For example drag'n'drop events will set the x,y positions.


**Returns**\
[Number](../JSLib/Number.md) an int representing the X position.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var x = event.getX();
var xPrevious = previousEvent.getX();
var movedXPixels = x -xPrevious;
```
### getY()

Returns the y position of the event, relative to the component that fired it, if applicable.
For example drag'n'drop events will set the x,y positions.


**Returns**\
[Number](../JSLib/Number.md) an int representing the Y position.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var y = event.getY();
var yPrevious = previousEvent.getY();
var movedYPixels = y -yPrevious;
```

