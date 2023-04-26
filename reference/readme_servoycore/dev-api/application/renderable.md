# Renderable

## Property Summary

| Type                            | Name                                     | Summary                                                                                                                                        |
| ------------------------------- | ---------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| [String](../js-lib/string.md)   | [bgcolor](renderable.md#bgcolor)         | Gets or sets the background color of a field..                                                                                                 |
| [String](../js-lib/string.md)   | [border](renderable.md#border)           | Gets or sets the border attribute(s) of a specified element..                                                                                  |
| [Boolean](../js-lib/boolean.md) | [enabled](renderable.md#enabled)         | Gets or sets the enabled state of a specified field, also known as "grayed"..                                                                  |
| [String](../js-lib/string.md)   | [fgcolor](renderable.md#fgcolor)         | Gets or sets the foreground color of a field..                                                                                                 |
| [String](../js-lib/string.md)   | [font](renderable.md#font)               | Gets or sets the font name, style, and size of an element..                                                                                    |
| [String](../js-lib/string.md)   | [format](renderable.md#format)           | Gets or sets the display formatting of an element for number and text values; does not affect the actual value stored in the database column.. |
| [String](../js-lib/string.md)   | [imageURL](renderable.md#imageURL)       | Gets/Sets the image displayed on a button or label; based on URL..                                                                             |
| [String](../js-lib/string.md)   | [toolTipText](renderable.md#toolTipText) | Gets or sets the tool tip text of an element; text displays when the mouse cursor hovers over an element..                                     |
| [Boolean](../js-lib/boolean.md) | [transparent](renderable.md#transparent) | Gets or sets the transparency of an element; true - transparent; false - not transparent..                                                     |
| [Boolean](../js-lib/boolean.md) | [visible](renderable.md#visible)         | Gets or sets the visibility of an element; true - visible; false - not visible; ! - the visibility state is inverted (the opposite)..          |

## Methods Summary

| Type                          | Name                                                                       | Summary                                                             |
| ----------------------------- | -------------------------------------------------------------------------- | ------------------------------------------------------------------- |
| [Number](../js-lib/number.md) | [getAbsoluteFormLocationY()](renderable.md#getabsoluteformlocationy)       | Returns the absolute form (designed) Y location..                   |
| [Object](../js-lib/object.md) | [getClientProperty(key)](renderable.md#getclientproperty-key)              | Gets the specified client property for the element based on a key.. |
| [String](../js-lib/string.md) | [getDataProviderID()](renderable.md#getdataproviderid)                     | Get the data provider this UI element (display) is showing..        |
| [String](../js-lib/string.md) | [getElementType()](renderable.md#getelementtype)                           | Returns the type of a specified element..                           |
| [Number](../js-lib/number.md) | [getHeight()](renderable.md#getheight)                                     | Returns the height of the current element..                         |
| [Number](../js-lib/number.md) | [getLocationX()](renderable.md#getlocationx)                               | Returns the x location of the current element..                     |
| [Number](../js-lib/number.md) | [getLocationY()](renderable.md#getlocationy)                               | Returns the y location of the current element..                     |
| [String](../js-lib/string.md) | [getName()](renderable.md#getname)                                         | Returns the name of an element..                                    |
| [Number](../js-lib/number.md) | [getWidth()](renderable.md#getwidth)                                       | Returns the width of the current element..                          |
| void                          | [putClientProperty(key, value)](renderable.md#putclientproperty-key-value) | Sets the value for the specified element client property key..      |

## Properties Details

### bgcolor

Gets or sets the background color of a field. The color has to be set using the hexadecimal RGB value as used in HTML. It only returns it's correct value if it was explicitly set.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
//sets the background color of the field
%%elementName%%.bgcolor = "#FFFFFF";
//gets the background color of the field
var c = %%elementName%%.bgcolor;
```

### border

Gets or sets the border attribute(s) of a specified element.

The border attributes:

borderType - EmptyBorder, EtchedBorder, BevelBorder, LineBorder, TitleBorder, MatteBorder, SpecialMatteBorder. size - (numeric value) for: bottom, left, right, top. color - (hexadecimal value) for: bottom, left, right, top. dash pattern - (numeric value) for selected side(s). rounding radius - (numeric value) for selected side(s).

It only returns it's correct value if it was explicitly set.

NOTE: Use the same value(s) and order of attribute(s) from the element design time property "borderType".

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
//sets the border type to "LineBorder"
//sets a 1 px line width for the bottom and left side of the border
//sets the hexadecimal color of the border to "#ccffcc"
%%elementName%%.border = 'LineBorder,1,#ccffcc';
```

### enabled

Gets or sets the enabled state of a specified field, also known as "grayed". true - enabled; false - not enabled; ! - the enabled state is inverted (the opposite).

NOTE: A disabled element cannot be selected by clicking the element (or by pressing the TAB key even if this option is supported by the operating system).

NOTE: A label or button element will not disable if the "displayType" design time property for a field is set to HTML\_AREA.

NOTE: The disabled "grayed" color is dependent on the LAF set in the Servoy Client Application Preferences. For more information see Preferences: Look And Feel in the Servoy Developer User's Guide.

**Returns**\
[Boolean](../js-lib/boolean.md)

**Sample**

```javascript
//gets the enabled state of the field
var currState = %%elementName%%.enabled;

//sets the enabled state of the field
%%elementName%%.enabled = !currentState;
```

### fgcolor

Gets or sets the foreground color of a field. The color has to be set using the hexadecimal RGB value as used in HTML. It only returns it's correct value if it was explicitly set.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
//sets the foreground color of the field
%%elementName%%.fgcolor = "#000000";

//gets the foreground color of the field
var c = %%elementName%%.fgcolor;
```

### font

Gets or sets the font name, style, and size of an element.

font name - the name of the font family. style - the type of the font. (plain = 0; bold = 1; italic = 2; bold-italic = 3). size - the size of the font (in points).

It only returns it's correct value if it was explicitly set.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
%%elementName%%.font = 'Tahoma,1,11';
```

### format

Gets or sets the display formatting of an element for number and text values; does not affect the actual value stored in the database column.

There are different options for the different dataprovider types that are assigned to this field. For Integer fields, there is a display and an edit format, using http://docs.oracle.com/javase/7/docs/api/java/text/DecimalFormat.html and the max (string) length can be set. For Text/String fields, there are options to force uppercase,lowercase or only numbers. Or a mask can be set that restrict the input the pattern chars can be found here: http://docs.oracle.com/javase/7/docs/api/javax/swing/text/MaskFormatter.html A mask can have a placehoder (what is shown when there is no data) and if the data must be stored raw (without literals of the mask). A max text length can also be set to force the max text length input, this doesn't work on mask because that max length is controlled with the mask. For Date fields a display and edit format can be set by using a pattern from here: http://docs.oracle.com/javase/7/docs/api/java/text/SimpleDateFormat.html, you can also say this must behave like a mask (the edit format) A mask only works with when the edit format is exactly that mask (1 char is 1 number/char), because for example MM then only 2 numbers are allowed MMM that displays the month as a string is not supported as a mask. Some examples are "dd-MM-yyyy", "MM-dd-yyyy", etc. The format property is also used to set the UI Converter, this means that you can convert the value object to something else before it gets set into the field, this can also result in a type change of the data. So a string in scripting/db is converted to a integer in the ui, then you have to set an integer format. It only returns it's correct value if it was explicitly set, otherwise null.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
//sets the display formatting of the field
%%elementName%%.format = '###';

//gets the display formatting of the field
var format = %%elementName%%.format;
```

### imageURL

Gets/Sets the image displayed on a button or label; based on URL.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
//dynamically sets an image displayed on a button or label
%%elementName%%.imageURL = "http://www.servoy.com/images/test.gif";

//sets an image from your own image library
%%elementName%%.imageURL = "media:///arrow.gif";

//loads an image (BLOB) from a field in a selected record into HTML
%%elementName%%.imageURL = 'media:///servoy_blobloader?datasource='+controller.getDataSource()+'&dataprovider=image_data&mimetype=image/jpeg&rowid1=2';
```

### toolTipText

Gets or sets the tool tip text of an element; text displays when the mouse cursor hovers over an element.

NOTE: HTML should be used for multi-line tooltips; you can also use any valid HTML tags to format tooltip text.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
//gets the tooltip text of the element
var toolTip = %%elementName%%.toolTipText;

//sets the tooltip text of the element
%%elementName%%.toolTipText = "New tip";
%%elementName%%.toolTipText = "<html>This includes <b>bolded text</b> and <font color='blue'>BLUE</font> text as well.";
```

### transparent

Gets or sets the transparency of an element; true - transparent; false - not transparent.

NOTE: transparency can be inverted using ! operator: elements.elementName.transparent = !elements.elementName.transparent;

NOTE: transparency will be mostly used for background color, a transparent element will receive the background of the element "beneath" it, a non transparent one will use its own background color

**Returns**\
[Boolean](../js-lib/boolean.md)

**Sample**

```javascript
//gets the transparency of the element
var currentState = %%elementName%%.transparent;

//sets the transparency of the element
%%elementName%%.transparent = !currentState;
```

### visible

Gets or sets the visibility of an element; true - visible; false - not visible; ! - the visibility state is inverted (the opposite).

NOTE: The visibility of an element is not persistent; the state of visibility only applies to the current user in his/her current session.

**Returns**\
[Boolean](../js-lib/boolean.md)

**Sample**

```javascript
//sets the element as visible
forms.company.elements.faxBtn.visible = true;

//gets the visibility of the element
var currentState = forms.company.elements.faxBtn.visible;

//sets the element as not visible when the current state is visible
forms.company.elements.faxBtn.visible = !currentState;
```

## Methods Details

### getAbsoluteFormLocationY()

Returns the absolute form (designed) Y location.

**Returns**\
[Number](../js-lib/number.md) The y location of the form in pixels.

**Sample**

```javascript
var absolute_y = %%elementName%%.getAbsoluteFormLocationY();
```

### getClientProperty(key)

Gets the specified client property for the element based on a key.

NOTE: Depending on the operating system, a user interface property name may be available.

**Parameters**\
[Object](../js-lib/object.md) key user interface key (depends on operating system)

**Returns**\
[Object](../js-lib/object.md) The value of the property for specified key.

**Sample**

```javascript
var property = %%elementName%%.getClientProperty('ToolTipText');
```

### getDataProviderID()

Get the data provider this UI element (display) is showing.

**Returns**\
[String](../js-lib/string.md) The data provider as String.

**Sample**

```javascript
%%elementName%%.getDataProviderID();
```

### getElementType()

Returns the type of a specified element.

**Returns**\
[String](../js-lib/string.md) The display type of the element as String.

**Sample**

```javascript
var et = %%elementName%%.getElementType();
```

### getHeight()

Returns the height of the current element. NOTE: getHeight() can be used with getWidth() to set the size of an element using the setSize function. For example:

//returns the width (w) and height (h) var w = forms.company.elements.faxBtn.getWidth(); var h = forms.company.elements.faxBtn.getHeight();

//sets the new size forms.company.elements.faxBtn.setSize(w,h);

//sets the new size and adds 1 px to both the width and height forms.company.elements.faxBtn.setSize(w+1,h+1);

**Returns**\
[Number](../js-lib/number.md) The height of the element in pixels.

**Sample**

```javascript
var ht = %%elementName%%.getHeight();
```

### getLocationX()

Returns the x location of the current element.

NOTE: getLocationX() can be used with getLocationY() to set the location of an element using the setLocation function. For Example:

//returns the X and Y coordinates var x = forms.company.elements.faxBtn.getLocationX(); var y = forms.company.elements.faxBtn.getLocationY();

//sets the new location 10 px to the right; 10 px down from the current location forms.company.elements.faxBtn.setLocation(x+10,y+10);

**Returns**\
[Number](../js-lib/number.md) The x location of the element in pixels.

**Sample**

```javascript
var x = %%elementName%%.getLocationX();
```

### getLocationY()

Returns the y location of the current element. The method can only be used in Record view.

NOTE: getLocationY() can be used with getLocationX() to set the location of an element using the setLocation function. For Example:

//returns the X and Y coordinates var x = forms.company.elements.faxBtn.getLocationX(); var y = forms.company.elements.faxBtn.getLocationY();

//sets the new location 10 px to the right; 10 px down from the current location forms.company.elements.faxBtn.setLocation(x+10,y+10);

**Returns**\
[Number](../js-lib/number.md) The y location of the element in pixels.

**Sample**

```javascript
var y =  %%elementName%%.getLocationY();
```

### getName()

Returns the name of an element. (may be null as well)

**Returns**\
[String](../js-lib/string.md) The name of the element.

**Sample**

```javascript
var name = %%elementName%%.getName();
```

### getWidth()

Returns the width of the current element.

NOTE: getWidth() can be used with getHeight() to set the size of an element using the setSize function. For Example:

//returns the width (w) and height (h) var w = forms.company.elements.faxBtn.getWidth(); var h = forms.company.elements.faxBtn.getHeight();

//sets the new size forms.company.elements.faxBtn.setSize(w,h);

//sets the new size and adds 1 px to both the width and height forms.company.elements.faxBtn.setSize(w+1,h+1);

**Returns**\
[Number](../js-lib/number.md) The width of the element in pixels.

**Sample**

```javascript
var w = %%elementName%%.getWidth();
```

### putClientProperty(key, value)

Sets the value for the specified element client property key.

NOTE: Depending on the operating system, a user interface property name may be available.

**Parameters**\
[Object](../js-lib/object.md) key user interface key (depends on operating system)\
[Object](../js-lib/object.md) value a predefined value for the key

**Returns**\
void

**Sample**

```javascript
%%elementName%%.putClientProperty('ToolTipText','some text');
```
