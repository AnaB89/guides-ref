#  JSEvent

## **Supported Clients**

    SmartClient
    WebClient
    NGClient
    MobileClient

## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [String](../JSLib/String.md) | [ACTION](JSEvent.md#ACTION)                   | Constant returned by JSEvent..                                    |
| [String](../JSLib/String.md) | [DATACHANGE](JSEvent.md#DATACHANGE)                   | Constant returned by JSEvent..                                    |
| [String](../JSLib/String.md) | [DOUBLECLICK](JSEvent.md#DOUBLECLICK)                   | Constant returned by JSEvent..                                    |
| [String](../JSLib/String.md) | [FOCUSGAINED](JSEvent.md#FOCUSGAINED)                   | Constant returned by JSEvent..                                    |
| [String](../JSLib/String.md) | [FOCUSLOST](JSEvent.md#FOCUSLOST)                   | Constant returned by JSEvent..                                    |
| [String](../JSLib/String.md) | [FORM](JSEvent.md#FORM)                   | Constant returned by JSEvent..                                    |
| [Number](../JSLib/Number.md) | [MODIFIER_ALT](JSEvent.md#MODIFIER_ALT)                   | Constant for the ALT modifier that can be returned by JSEvent..                                    |
| [Number](../JSLib/Number.md) | [MODIFIER_CTRL](JSEvent.md#MODIFIER_CTRL)                   | Constant for the CTRL modifier that can be returned by JSEvent..                                    |
| [Number](../JSLib/Number.md) | [MODIFIER_META](JSEvent.md#MODIFIER_META)                   | Constant for the META modifier that can be returned by JSEvent..                                    |
| [Number](../JSLib/Number.md) | [MODIFIER_SHIFT](JSEvent.md#MODIFIER_SHIFT)                   | Constant for the SHIFT modifier that can be returned by JSEvent..                                    |
| [String](../JSLib/String.md) | [NONE](JSEvent.md#NONE)                   | Constant returned by JSEvent..                                    |
| [String](../JSLib/String.md) | [RIGHTCLICK](JSEvent.md#RIGHTCLICK)                   | Constant returned by JSEvent..                                    |

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Object](../JSLib/Object.md) | [data](JSEvent.md#data)                   | A data object that specific events can set, a user can set data back to the system for events that supports this..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [getElementName()](JSEvent.md#getelementname)                   | returns the name of the element, can be null if the form was the source of the event..                                    |
| [String](../JSLib/String.md) | [getFormName()](JSEvent.md#getformname)                   | returns the name of the form the element was placed on..                                    |
| [Number](../JSLib/Number.md) | [getModifiers()](JSEvent.md#getmodifiers)                   | Returns the modifiers of the event, see JSEvent..                                    |
| [String](../JSLib/String.md) | [getName()](JSEvent.md#getname)                   | Returns the name of the event which was triggered.                                    |
| [Object](../JSLib/Object.md) | [getSource()](JSEvent.md#getsource)                   | returns the source component/element of the event..                                    |
| [Date](../JSLib/Date.md) | [getTimestamp()](JSEvent.md#gettimestamp)                   | Returns the time the event occurred..                                    |
| [String](../JSLib/String.md) | [getType()](JSEvent.md#gettype)                   | returns the event type see the JSEvents constants what it can return..                                    |
| [Number](../JSLib/Number.md) | [getX()](JSEvent.md#getx)                   | Returns the x position of the event, relative to the component that fired it, if applicable..                                    |
| [Number](../JSLib/Number.md) | [getY()](JSEvent.md#gety)                   | Returns the y position of the event, relative to the component that fired it, if applicable..                                    |

## Constants Details

### ACTION

Constant returned by JSEvent.getType() in a method that is attached to an onAction event.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

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
SmartClient,WebClient,NGClient,MobileClient

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
SmartClient,WebClient,NGClient,MobileClient

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
SmartClient,WebClient,NGClient,MobileClient

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
SmartClient,WebClient,NGClient,MobileClient

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
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
if (event.getType() == JSEvent.FORM) 
{
	// its a form event or command
}
```
### MODIFIER_ALT

Constant for the ALT modifier that can be returned by JSEvent.getModifiers();

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
//test if the SHIFT modifier is used.
if (event.getModifiers() & JSEvent.MODIFIER_SHIFT)
{
	//do shift action
}
```
### MODIFIER_CTRL

Constant for the CTRL modifier that can be returned by JSEvent.getModifiers();

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
//test if the SHIFT modifier is used.
if (event.getModifiers() & JSEvent.MODIFIER_SHIFT)
{
	//do shift action
}
```
### MODIFIER_META

Constant for the META modifier that can be returned by JSEvent.getModifiers();

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
//test if the SHIFT modifier is used.
if (event.getModifiers() & JSEvent.MODIFIER_SHIFT)
{
	//do shift action
}
```
### MODIFIER_SHIFT

Constant for the SHIFT modifier that can be returned by JSEvent.getModifiers();

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

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
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

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
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

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
SmartClient,WebClient,NGClient,MobileClient

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
[String](../JSLib/String.md) a String representing the element name.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

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
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
forms[event.getFormName()].myFormMethod();
```
### getModifiers()

Returns the modifiers of the event, see JSEvent.MODIFIER_XXXX for the modifiers that can be returned.


**Returns**\
[Number](../JSLib/Number.md) an int which holds the modifiers as a bitset.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

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
[String](../JSLib/String.md) name of event as string

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var name = event.getName();
```
### getSource()

returns the source component/element of the event.
If it has a name the getElementName() is the name of this component.


**Returns**\
[Object](../JSLib/Object.md) an Object representing the source of this event.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

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
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
event.getTimestamp();
```
### getType()

returns the event type see the JSEvents constants what it can return.
Plugins can create events with there own types.


**Returns**\
[String](../JSLib/String.md) a String representing the type of this event.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
if (event.getType() == JSEvent.ACTION)
{
	// its an action event.
}
```
### getX()

Returns the x position of the event, relative to the component that fired it, if applicable.
For example drag'n'drop events will set the x,y positions.


**Returns**\
[Number](../JSLib/Number.md) an int representing the X position.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

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
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var y = event.getY();
var yPrevious = previousEvent.getY();
var movedYPixels = y -yPrevious;
```

