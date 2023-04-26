# JSEvent

## Constants Summary

| Type                          | Name                                          | Summary                                                           |
| ----------------------------- | --------------------------------------------- | ----------------------------------------------------------------- |
| [String](../js-lib/string.md) | [ACTION](jsevent.md#ACTION)                   | Constant returned by JSEvent..                                    |
| [String](../js-lib/string.md) | [DATACHANGE](jsevent.md#DATACHANGE)           | Constant returned by JSEvent..                                    |
| [String](../js-lib/string.md) | [DOUBLECLICK](jsevent.md#DOUBLECLICK)         | Constant returned by JSEvent..                                    |
| [String](../js-lib/string.md) | [FOCUSGAINED](jsevent.md#FOCUSGAINED)         | Constant returned by JSEvent..                                    |
| [String](../js-lib/string.md) | [FOCUSLOST](jsevent.md#FOCUSLOST)             | Constant returned by JSEvent..                                    |
| [String](../js-lib/string.md) | [FORM](jsevent.md#FORM)                       | Constant returned by JSEvent..                                    |
| [Number](../js-lib/number.md) | [MODIFIER\_ALT](jsevent.md#MODIFIER\_ALT)     | Constant for the ALT modifier that can be returned by JSEvent..   |
| [Number](../js-lib/number.md) | [MODIFIER\_CTRL](jsevent.md#MODIFIER\_CTRL)   | Constant for the CTRL modifier that can be returned by JSEvent..  |
| [Number](../js-lib/number.md) | [MODIFIER\_META](jsevent.md#MODIFIER\_META)   | Constant for the META modifier that can be returned by JSEvent..  |
| [Number](../js-lib/number.md) | [MODIFIER\_SHIFT](jsevent.md#MODIFIER\_SHIFT) | Constant for the SHIFT modifier that can be returned by JSEvent.. |
| [String](../js-lib/string.md) | [NONE](jsevent.md#NONE)                       | Constant returned by JSEvent..                                    |
| [String](../js-lib/string.md) | [RIGHTCLICK](jsevent.md#RIGHTCLICK)           | Constant returned by JSEvent..                                    |

## Property Summary

| Type                          | Name                    | Summary                                                                                                            |
| ----------------------------- | ----------------------- | ------------------------------------------------------------------------------------------------------------------ |
| [Object](../js-lib/object.md) | [data](jsevent.md#data) | A data object that specific events can set, a user can set data back to the system for events that supports this.. |

## Methods Summary

| Type                          | Name                                          | Summary                                                                                       |
| ----------------------------- | --------------------------------------------- | --------------------------------------------------------------------------------------------- |
| [String](../js-lib/string.md) | [getElementName()](jsevent.md#getelementname) | returns the name of the element, can be null if the form was the source of the event..        |
| [String](../js-lib/string.md) | [getFormName()](jsevent.md#getformname)       | returns the name of the form the element was placed on..                                      |
| [Number](../js-lib/number.md) | [getModifiers()](jsevent.md#getmodifiers)     | Returns the modifiers of the event, see JSEvent..                                             |
| [String](../js-lib/string.md) | [getName()](jsevent.md#getname)               | Returns the name of the event which was triggered.                                            |
| [Object](../js-lib/object.md) | [getSource()](jsevent.md#getsource)           | returns the source component/element of the event..                                           |
| [Date](../js-lib/date.md)     | [getTimestamp()](jsevent.md#gettimestamp)     | Returns the time the event occurred..                                                         |
| [String](../js-lib/string.md) | [getType()](jsevent.md#gettype)               | returns the event type see the JSEvents constants what it can return..                        |
| [Number](../js-lib/number.md) | [getX()](jsevent.md#getx)                     | Returns the x position of the event, relative to the component that fired it, if applicable.. |
| [Number](../js-lib/number.md) | [getY()](jsevent.md#gety)                     | Returns the y position of the event, relative to the component that fired it, if applicable.. |

## Constants Details

### ACTION

Constant returned by JSEvent.getType() in a method that is attached to an onAction event.

**Returns**\
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

**Sample**

```javascript
if (event.getType() == JSEvent.FORM) 
{
	// its a form event or command
}
```

### MODIFIER\_ALT

Constant for the ALT modifier that can be returned by JSEvent.getModifiers();

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
//test if the SHIFT modifier is used.
if (event.getModifiers() & JSEvent.MODIFIER_SHIFT)
{
	//do shift action
}
```

### MODIFIER\_CTRL

Constant for the CTRL modifier that can be returned by JSEvent.getModifiers();

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
//test if the SHIFT modifier is used.
if (event.getModifiers() & JSEvent.MODIFIER_SHIFT)
{
	//do shift action
}
```

### MODIFIER\_META

Constant for the META modifier that can be returned by JSEvent.getModifiers();

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
//test if the SHIFT modifier is used.
if (event.getModifiers() & JSEvent.MODIFIER_SHIFT)
{
	//do shift action
}
```

### MODIFIER\_SHIFT

Constant for the SHIFT modifier that can be returned by JSEvent.getModifiers();

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
//test if the SHIFT modifier is used.
if (event.getModifiers() & JSEvent.MODIFIER_SHIFT)
{
	//do shift action
}
```

### NONE

Constant returned by JSEvent.getType() if the event is not used in a known event or command.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
if (event.getType() == JSEvent.NONE) 
{
	// type is not set.
}
```

### RIGHTCLICK

Constant returned by JSEvent.getType() in a method that is attached to an onRightClick event.

**Returns**\
[String](../js-lib/string.md)

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
[Object](../js-lib/object.md)

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

## Methods Details

### getElementName()

returns the name of the element, can be null if the form was the source of the event.

**Returns**\
[String](../js-lib/string.md) a String representing the element name.

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
[String](../js-lib/string.md) a String representing the form name.

**Sample**

```javascript
forms[event.getFormName()].myFormMethod();
```

### getModifiers()

Returns the modifiers of the event, see JSEvent.MODIFIER\_XXXX for the modifiers that can be returned.

**Returns**\
[Number](../js-lib/number.md) an int which holds the modifiers as a bitset.

**Sample**

```javascript
//test if the SHIFT modifier is used.
if (event.getModifiers() & JSEvent.MODIFIER_SHIFT)
{
	//do shift action
}
```

### getName()

Returns the name of the event which was triggered

**Returns**\
[String](../js-lib/string.md) name of event as string

**Sample**

```javascript
var name = event.getName();
```

### getSource()

returns the source component/element of the event. If it has a name the getElementName() is the name of this component.

**Returns**\
[Object](../js-lib/object.md) an Object representing the source of this event.

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
[Date](../js-lib/date.md) a Date when this event happened.

**Sample**

```javascript
event.getTimestamp();
```

### getType()

returns the event type see the JSEvents constants what it can return. Plugins can create events with there own types.

**Returns**\
[String](../js-lib/string.md) a String representing the type of this event.

**Sample**

```javascript
if (event.getType() == JSEvent.ACTION)
{
	// its an action event.
}
```

### getX()

Returns the x position of the event, relative to the component that fired it, if applicable. For example drag'n'drop events will set the x,y positions.

**Returns**\
[Number](../js-lib/number.md) an int representing the X position.

**Sample**

```javascript
var x = event.getX();
var xPrevious = previousEvent.getX();
var movedXPixels = x -xPrevious;
```

### getY()

Returns the y position of the event, relative to the component that fired it, if applicable. For example drag'n'drop events will set the x,y positions.

**Returns**\
[Number](../js-lib/number.md) an int representing the Y position.

**Sample**

```javascript
var y = event.getY();
var yPrevious = previousEvent.getY();
var movedYPixels = y -yPrevious;
```
