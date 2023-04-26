# ELEMENT\_TYPES

## Constants Summary

| Type                          | Name                                                           | Summary                                                   |
| ----------------------------- | -------------------------------------------------------------- | --------------------------------------------------------- |
| [String](../js-lib/string.md) | [ACCORDIONPANEL](element\_types.md#ACCORDIONPANEL)             | Constant representing a accordionpanel element..          |
| [String](../js-lib/string.md) | [BUTTON](element\_types.md#BUTTON)                             | Constant representing an element of the Button type..     |
| [String](../js-lib/string.md) | [CALENDAR](element\_types.md#CALENDAR)                         | Constant representing an element of the Calendar type..   |
| [String](../js-lib/string.md) | [CHECK](element\_types.md#CHECK)                               | Constant representing an element of the Check type..      |
| [String](../js-lib/string.md) | [COMBOBOX](element\_types.md#COMBOBOX)                         | Constant representing a combobox element..                |
| [String](../js-lib/string.md) | [FORM](element\_types.md#FORM)                                 | Constant representing a form element..                    |
| [String](../js-lib/string.md) | [GROUP](element\_types.md#GROUP)                               | Constant representing a Group of elements..               |
| [String](../js-lib/string.md) | [HTML\_AREA](element\_types.md#HTML\_AREA)                     | Constant representing a html area element..               |
| [String](../js-lib/string.md) | [IMAGE\_MEDIA](element\_types.md#IMAGE\_MEDIA)                 | Constant representing an element of the ImageMedia type.. |
| [String](../js-lib/string.md) | [LABEL](element\_types.md#LABEL)                               | Constant representing an element of the Label type..      |
| [String](../js-lib/string.md) | [LISTBOX](element\_types.md#LISTBOX)                           | Constant representing a listbox element..                 |
| [String](../js-lib/string.md) | [MULTISELECT\_LISTBOX](element\_types.md#MULTISELECT\_LISTBOX) | Constant representing a multi selection listbox element.. |
| [String](../js-lib/string.md) | [PASSWORD](element\_types.md#PASSWORD)                         | Constant representing an element of the Password type..   |
| [String](../js-lib/string.md) | [PORTAL](element\_types.md#PORTAL)                             | Constant representing an element of the Portal type..     |
| [String](../js-lib/string.md) | [RADIOS](element\_types.md#RADIOS)                             | Constant representing an element of the Radios type..     |
| [String](../js-lib/string.md) | [RECTANGLE](element\_types.md#RECTANGLE)                       | Constant representing a rectangle element..               |
| [String](../js-lib/string.md) | [RTF\_AREA](element\_types.md#RTF\_AREA)                       | Constant representing a rtf area of element..             |
| [String](../js-lib/string.md) | [SPINNER](element\_types.md#SPINNER)                           | Constant representing a spinner element..                 |
| [String](../js-lib/string.md) | [SPLITPANE](element\_types.md#SPLITPANE)                       | Constant representing a splitpane element..               |
| [String](../js-lib/string.md) | [TABPANEL](element\_types.md#TABPANEL)                         | Constant representing an element of the Tabpanel type..   |
| [String](../js-lib/string.md) | [TEXT\_AREA](element\_types.md#TEXT\_AREA)                     | Constant representing an element of the TextArea type..   |
| [String](../js-lib/string.md) | [TEXT\_FIELD](element\_types.md#TEXT\_FIELD)                   | Constant representing an element of the TextField type..  |
| [String](../js-lib/string.md) | [TYPE\_AHEAD](element\_types.md#TYPE\_AHEAD)                   | Constant representing a typeahead element..               |

## Constants Details

### ACCORDIONPANEL

Constant representing a accordionpanel element.

**Returns**\
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

**Sample**

```javascript
//the return value for an element type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.GROUP)
{
     // element is a group element
}
```

### HTML\_AREA

Constant representing a html area element.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
//the return value for an element of the TextField type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.HTML_AREA)
{
     // element is a HTML textarea
}
```

### IMAGE\_MEDIA

Constant representing an element of the ImageMedia type.

**Returns**\
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

**Sample**

```javascript
//the return value for an element of the ListBox type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.LISTBOX)
{
     // element is a LISTBOX element
}
```

### MULTISELECT\_LISTBOX

Constant representing a multi selection listbox element.

**Returns**\
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

**Sample**

```javascript
//the return value for an element of the TextField type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.RECTANGLE)
{
     // element is a rectangle element
}
```

### RTF\_AREA

Constant representing a rtf area of element.

**Returns**\
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

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
[String](../js-lib/string.md)

**Sample**

```javascript
//the return value for an element of the Tabpanel type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.TABPANEL)
{
     // element is a Tabpanel component
}
```

### TEXT\_AREA

Constant representing an element of the TextArea type.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
//the return value for an element of the TextArea type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.TEXT_AREA)
{
     // element is a TextArea field
}
```

### TEXT\_FIELD

Constant representing an element of the TextField type.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
//the return value for an element of the TextField type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.TEXT_FIELD)
{
     // element is a text field
}
```

### TYPE\_AHEAD

Constant representing a typeahead element.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
//the return value for an element of the TextField type, as returned by the following code
var etype = elements.elementName.getElementType();
if (etype == ELEMENT_TYPES.TYPE_AHEAD)
{
     // element is a type ahead element
}
```
