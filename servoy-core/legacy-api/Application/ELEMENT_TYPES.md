#  ELEMENT_TYPES

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [String](../JSLib/String.md) | [ACCORDIONPANEL](ELEMENT_TYPES.md#ACCORDIONPANEL)                   | Constant representing a accordionpanel element..                                    |
| [String](../JSLib/String.md) | [BUTTON](ELEMENT_TYPES.md#BUTTON)                   | Constant representing an element of the Button type..                                    |
| [String](../JSLib/String.md) | [CALENDAR](ELEMENT_TYPES.md#CALENDAR)                   | Constant representing an element of the Calendar type..                                    |
| [String](../JSLib/String.md) | [CHECK](ELEMENT_TYPES.md#CHECK)                   | Constant representing an element of the Check type..                                    |
| [String](../JSLib/String.md) | [COMBOBOX](ELEMENT_TYPES.md#COMBOBOX)                   | Constant representing a combobox element..                                    |
| [String](../JSLib/String.md) | [FORM](ELEMENT_TYPES.md#FORM)                   | Constant representing a form element..                                    |
| [String](../JSLib/String.md) | [GROUP](ELEMENT_TYPES.md#GROUP)                   | Constant representing a Group of elements..                                    |
| [String](../JSLib/String.md) | [HTML_AREA](ELEMENT_TYPES.md#HTML_AREA)                   | Constant representing a html area element..                                    |
| [String](../JSLib/String.md) | [IMAGE_MEDIA](ELEMENT_TYPES.md#IMAGE_MEDIA)                   | Constant representing an element of the ImageMedia type..                                    |
| [String](../JSLib/String.md) | [LABEL](ELEMENT_TYPES.md#LABEL)                   | Constant representing an element of the Label type..                                    |
| [String](../JSLib/String.md) | [LISTBOX](ELEMENT_TYPES.md#LISTBOX)                   | Constant representing a listbox element..                                    |
| [String](../JSLib/String.md) | [MULTISELECT_LISTBOX](ELEMENT_TYPES.md#MULTISELECT_LISTBOX)                   | Constant representing a multi selection listbox element..                                    |
| [String](../JSLib/String.md) | [PASSWORD](ELEMENT_TYPES.md#PASSWORD)                   | Constant representing an element of the Password type..                                    |
| [String](../JSLib/String.md) | [PORTAL](ELEMENT_TYPES.md#PORTAL)                   | Constant representing an element of the Portal type..                                    |
| [String](../JSLib/String.md) | [RADIOS](ELEMENT_TYPES.md#RADIOS)                   | Constant representing an element of the Radios type..                                    |
| [String](../JSLib/String.md) | [RECTANGLE](ELEMENT_TYPES.md#RECTANGLE)                   | Constant representing a rectangle element..                                    |
| [String](../JSLib/String.md) | [RTF_AREA](ELEMENT_TYPES.md#RTF_AREA)                   | Constant representing a rtf area of element..                                    |
| [String](../JSLib/String.md) | [SPINNER](ELEMENT_TYPES.md#SPINNER)                   | Constant representing a spinner element..                                    |
| [String](../JSLib/String.md) | [SPLITPANE](ELEMENT_TYPES.md#SPLITPANE)                   | Constant representing a splitpane element..                                    |
| [String](../JSLib/String.md) | [TABPANEL](ELEMENT_TYPES.md#TABPANEL)                   | Constant representing an element of the Tabpanel type..                                    |
| [String](../JSLib/String.md) | [TEXT_AREA](ELEMENT_TYPES.md#TEXT_AREA)                   | Constant representing an element of the TextArea type..                                    |
| [String](../JSLib/String.md) | [TEXT_FIELD](ELEMENT_TYPES.md#TEXT_FIELD)                   | Constant representing an element of the TextField type..                                    |
| [String](../JSLib/String.md) | [TYPE_AHEAD](ELEMENT_TYPES.md#TYPE_AHEAD)                   | Constant representing a typeahead element..                                    |

## Constants Details

### ACCORDIONPANEL

Constant representing a accordionpanel element.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.ACCORDIONPANEL)
{
     // element is a accordion panel element
}
```
### BUTTON

Constant representing an element of the Button type.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the Button type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.BUTTON)
{
     // element is a Button component
}
```
### CALENDAR

Constant representing an element of the Calendar type.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the Calendar type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.CALENDAR)
{
     // element is a Calendar field
}
```
### CHECK

Constant representing an element of the Check type.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the Check type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.CHECK)
{
     // element is a Check(box) field
}
```
### COMBOBOX

Constant representing a combobox element.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the TextField type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.COMBOBOX)
{
     // element is a COMBOBOX element
}
```
### FORM

Constant representing a form element.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the Form type, as returned by the following code
var renderElementType = event.getRenderable().getElementType();
if (renderElementType == ELEMENT_TYPES.FORM)
{
     // element is a type form element
}
```
### GROUP

Constant representing a Group of elements.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.GROUP)
{
     // element is a group element
}
```
### HTML_AREA

Constant representing a html area element.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the TextField type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.HTML_AREA)
{
     // element is a HTML textarea
}
```
### IMAGE_MEDIA

Constant representing an element of the ImageMedia type.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the ImageMedia type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.IMAGE_MEDIA)
{
     // element is a Image Media field
}
```
### LABEL

Constant representing an element of the Label type.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the Label type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.LABEL)
{
     // element is a Label component
}
```
### LISTBOX

Constant representing a listbox element.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the ListBox type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.LISTBOX)
{
     // element is a LISTBOX element
}
```
### MULTISELECT_LISTBOX

Constant representing a multi selection listbox element.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the TextField type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.MULTISELECT_LISTBOX)
{
     // element is a MULTISELECT_LISTBOX element
}
```
### PASSWORD

Constant representing an element of the Password type.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the Password type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.PASSWORD)
{
     // element is a Password component
}
```
### PORTAL

Constant representing an element of the Portal type.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the Portal type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.PORTAL)
{
     // element is a Portal component
}
```
### RADIOS

Constant representing an element of the Radios type.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the Radios type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.RADIOS)
{
     // element is a Radios field.
}
```
### RECTANGLE

Constant representing a rectangle element.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the TextField type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.RECTANGLE)
{
     // element is a rectangle element
}
```
### RTF_AREA

Constant representing a rtf area of element.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the TextField type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.RTF_AREA)
{
     // element is a RTF textarea.
}
```
### SPINNER

Constant representing a spinner element.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the Spinner type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.SPINNER)
{
     // element is a SPINNER element
}
```
### SPLITPANE

Constant representing a splitpane element.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.SPLITPANE)
{
     // element is a splitpane element
}
```
### TABPANEL

Constant representing an element of the Tabpanel type.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the Tabpanel type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.TABPANEL)
{
     // element is a Tabpanel component
}
```
### TEXT_AREA

Constant representing an element of the TextArea type.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the TextArea type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.TEXT_AREA)
{
     // element is a TextArea field
}
```
### TEXT_FIELD

Constant representing an element of the TextField type.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the TextField type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.TEXT_FIELD)
{
     // element is a text field
}
```
### TYPE_AHEAD

Constant representing a typeahead element.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//the return value for an element of the TextField type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.TYPE_AHEAD)
{
     // element is a type ahead element
}
```

