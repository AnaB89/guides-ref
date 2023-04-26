# RuntimePassword

## **Extends**

```
RuntimeComponent
```

## Property Summary

| Type                                  | Name                                                  | Summary                                                                                                                                                 |
| ------------------------------------- | ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [String](../../../js-lib/string.md)   | [bgcolor](runtimepassword.md#bgcolor)                 | Gets or sets the background color of a field..                                                                                                          |
| [String](../../../js-lib/string.md)   | [border](runtimepassword.md#border)                   | Gets or sets the border attribute(s) of a specified element..                                                                                           |
| [Boolean](../../../js-lib/boolean.md) | [editable](runtimepassword.md#editable)               | Gets or sets the editable/read-only state of a field; true - editable; false - read-only..                                                              |
| [Boolean](../../../js-lib/boolean.md) | [enabled](runtimepassword.md#enabled)                 | Gets or sets the enabled state of a specified field, also known as "grayed"..                                                                           |
| [String](../../../js-lib/string.md)   | [fgcolor](runtimepassword.md#fgcolor)                 | Gets or sets the foreground color of a field..                                                                                                          |
| [String](../../../js-lib/string.md)   | [font](runtimepassword.md#font)                       | Gets or sets the font name, style, and size of an element..                                                                                             |
| [String](../../../js-lib/string.md)   | [placeholderText](runtimepassword.md#placeholderText) | Gets or sets the placeholder text in a field..                                                                                                          |
| [Boolean](../../../js-lib/boolean.md) | [readOnly](runtimepassword.md#readOnly)               | Gets or sets the editable/read-only state of a field; true - read-only; false - editable; ! - the editable/read-only state is inverted (the opposite).. |
| [String](../../../js-lib/string.md)   | [titleText](runtimepassword.md#titleText)             | Gets or sets the title text..                                                                                                                           |
| [String](../../../js-lib/string.md)   | [toolTipText](runtimepassword.md#toolTipText)         | Gets or sets the tool tip text of an element; text displays when the mouse cursor hovers over an element..                                              |
| [Boolean](../../../js-lib/boolean.md) | [transparent](runtimepassword.md#transparent)         | Gets or sets the transparency of an element; true - transparent; false - not transparent..                                                              |
| [Boolean](../../../js-lib/boolean.md) | [visible](runtimepassword.md#visible)                 | Gets or sets the visibility of an element; true - visible; false - not visible; ! - the visibility state is inverted (the opposite)..                   |

## Methods Summary

| Type                                | Name                                                                                                           | Summary                                                                                 |
| ----------------------------------- | -------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| void                                | [addStyleClass(styleName)](runtimepassword.md#addstyleclass-stylename)                                         | Adds a style to the styleClass property..                                               |
| [Number](../../../js-lib/number.md) | [getAbsoluteFormLocationY()](runtimepassword.md#getabsoluteformlocationy)                                      | Returns the absolute form (designed) Y location..                                       |
| [Object](../../../js-lib/object.md) | [getClientProperty(key)](runtimepassword.md#getclientproperty-key)                                             | Gets the specified client property for the element based on a key..                     |
| [String](../../../js-lib/string.md) | [getDataProviderID()](runtimepassword.md#getdataproviderid)                                                    | Get the data provider this UI element (display) is showing..                            |
| [Object](../../../js-lib/object.md) | [getDesignProperties()](runtimepassword.md#getdesignproperties)                                                | Get the design-time properties of an element..                                          |
| [Object](../../../js-lib/object.md) | [getDesignTimeProperty(key)](runtimepassword.md#getdesigntimeproperty-key)                                     | Get a design-time property of an element..                                              |
| [String](../../../js-lib/string.md) | [getElementType()](runtimepassword.md#getelementtype)                                                          | Returns the type of a specified element..                                               |
| [String](../../../js-lib/string.md) | [getFormName()](runtimepassword.md#getformname)                                                                | Returns the name of the form..                                                          |
| [Number](../../../js-lib/number.md) | [getHeight()](runtimepassword.md#getheight)                                                                    | Returns the height of the current element..                                             |
| [Array](../../../js-lib/array.md)   | [getLabelForElementNames()](runtimepassword.md#getlabelforelementnames)                                        | Returns an Array of label element names that has this field filled in as the labelFor.. |
| [Number](../../../js-lib/number.md) | [getLocationX()](runtimepassword.md#getlocationx)                                                              | Returns the x location of the current element..                                         |
| [Number](../../../js-lib/number.md) | [getLocationY()](runtimepassword.md#getlocationy)                                                              | Returns the y location of the current element..                                         |
| [String](../../../js-lib/string.md) | [getName()](runtimepassword.md#getname)                                                                        | Returns the name of an element..                                                        |
| [Number](../../../js-lib/number.md) | [getWidth()](runtimepassword.md#getwidth)                                                                      | Returns the width of the current element..                                              |
| void                                | [hasStyleClass(styleName)](runtimepassword.md#hasstyleclass-stylename)                                         | Check if an element already have a style from the styleClass property..                 |
| void                                | [putClientProperty(key, value)](runtimepassword.md#putclientproperty-key-value)                                | Sets the value for the specified element client property key..                          |
| void                                | [removeStyleClass(styleName)](runtimepassword.md#removestyleclass-stylename)                                   | Removes a style from the styleClass property..                                          |
| void                                | [requestFocus()](runtimepassword.md#requestfocus)                                                              | Request the focus in this element..                                                     |
| void                                | [requestFocus(mustExecuteOnFocusGainedMethod)](runtimepassword.md#requestfocus-mustexecuteonfocusgainedmethod) | Request the focus in this element..                                                     |
| void                                | [setLocation(x, y)](runtimepassword.md#setlocation-x-y)                                                        | Sets the location of an element..                                                       |
| void                                | [setSize(width, height)](runtimepassword.md#setsize-width-height)                                              | Sets the size of an element..                                                           |

## Properties Details

### bgcolor

Gets or sets the background color of a field. The color has to be set using the hexadecimal RGB value as used in HTML. It only returns it's correct value if it was explicitly set.

**Returns**\
[String](../../../js-lib/string.md)

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
[String](../../../js-lib/string.md)

**Sample**

```javascript
//sets the border type to "LineBorder"
//sets a 1 px line width for the bottom and left side of the border
//sets the hexadecimal color of the border to "#ccffcc"
%%elementName%%.border = 'LineBorder,1,#ccffcc';
```

### editable

Gets or sets the editable/read-only state of a field; true - editable; false - read-only.

NOTE the "!" operator can be used to invert the editable state.

**Returns**\
[Boolean](../../../js-lib/boolean.md)

**Sample**

```javascript
var currentState = %%elementName%%.editable;
%%elementName%%.editable = !currentState;
```

### enabled

Gets or sets the enabled state of a specified field, also known as "grayed". true - enabled; false - not enabled; ! - the enabled state is inverted (the opposite).

NOTE: A disabled element cannot be selected by clicking the element (or by pressing the TAB key even if this option is supported by the operating system).

NOTE: A label or button element will not disable if the "displayType" design time property for a field is set to HTML\_AREA.

NOTE: The disabled "grayed" color is dependent on the LAF set in the Servoy Client Application Preferences. For more information see Preferences: Look And Feel in the Servoy Developer User's Guide.

**Returns**\
[Boolean](../../../js-lib/boolean.md)

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
[String](../../../js-lib/string.md)

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
[String](../../../js-lib/string.md)

**Sample**

```javascript
%%elementName%%.font = 'Tahoma,1,11';
```

### placeholderText

Gets or sets the placeholder text in a field.

**Returns**\
[String](../../../js-lib/string.md)

**Sample**

```javascript
//get the placeholder text
var placeholderText = %%elementName%%.placeholderText;
//set another placeholder
%%elementName%%.placeholderText = 'Search..';
```

### readOnly

Gets or sets the editable/read-only state of a field; true - read-only; false - editable; ! - the editable/read-only state is inverted (the opposite).

NOTE: A field set as read-only can be selected by clicking (or pressing the TAB key if this option is supported by the operating system) and the field data can be copied.

**Returns**\
[Boolean](../../../js-lib/boolean.md)

**Sample**

```javascript
//gets the editable/read-only state of the field
var currentState = %%elementName%%.readOnly;

//sets the editable/read-only state of the field
%%elementName%%.readOnly = !currentState;
```

### titleText

Gets or sets the title text.

**Returns**\
[String](../../../js-lib/string.md)

**Sample**

```javascript
var titleText = %%elementName%%.titleText;
```

### toolTipText

Gets or sets the tool tip text of an element; text displays when the mouse cursor hovers over an element.

NOTE: HTML should be used for multi-line tooltips; you can also use any valid HTML tags to format tooltip text.

**Returns**\
[String](../../../js-lib/string.md)

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
[Boolean](../../../js-lib/boolean.md)

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
[Boolean](../../../js-lib/boolean.md)

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

### addStyleClass(styleName)

Adds a style to the styleClass property. This works only for NGClient where multiple styles are supported.

**Parameters**\
[String](../../../js-lib/string.md) styleName the name of the style class to add

**Returns**\
void

**Sample**

```javascript
%%elementName%%.addStyleClass('redbg');
```

### getAbsoluteFormLocationY()

Returns the absolute form (designed) Y location.

**Returns**\
[Number](../../../js-lib/number.md) The y location of the form in pixels.

**Sample**

```javascript
var absolute_y = %%elementName%%.getAbsoluteFormLocationY();
```

### getClientProperty(key)

Gets the specified client property for the element based on a key.

NOTE: Depending on the operating system, a user interface property name may be available.

**Parameters**\
[Object](../../../js-lib/object.md) key user interface key (depends on operating system)

**Returns**\
[Object](../../../js-lib/object.md) The value of the property for specified key.

**Sample**

```javascript
var property = %%elementName%%.getClientProperty('ToolTipText');
```

### getDataProviderID()

Get the data provider this UI element (display) is showing.

**Returns**\
[String](../../../js-lib/string.md) The data provider as String.

**Sample**

```javascript
%%elementName%%.getDataProviderID();
```

### getDesignProperties()

Get the design-time properties of an element.

**Returns**\
[Object](../../../js-lib/object.md)

**Sample**

```javascript
var prop = forms.orders.elements.mylabel.getDesignProperties()
```

### getDesignTimeProperty(key)

Get a design-time property of an element.

**Parameters**\
[String](../../../js-lib/string.md) key the name of the property

**Returns**\
[Object](../../../js-lib/object.md)

**Sample**

```javascript
var prop = forms.orders.elements.mylabel.getDesignTimeProperty('myprop')
```

### getElementType()

Returns the type of a specified element.

**Returns**\
[String](../../../js-lib/string.md) The display type of the element as String.

**Sample**

```javascript
var et = %%elementName%%.getElementType();
```

### getFormName()

Returns the name of the form. (may be empty string as well)

**Returns**\
[String](../../../js-lib/string.md) The name of the form.

**Sample**

```javascript
var name = %%elementName%%.getFormName();
```

### getHeight()

Returns the height of the current element. NOTE: getHeight() can be used with getWidth() to set the size of an element using the setSize function. For example:

//returns the width (w) and height (h) var w = forms.company.elements.faxBtn.getWidth(); var h = forms.company.elements.faxBtn.getHeight();

//sets the new size forms.company.elements.faxBtn.setSize(w,h);

//sets the new size and adds 1 px to both the width and height forms.company.elements.faxBtn.setSize(w+1,h+1);

**Returns**\
[Number](../../../js-lib/number.md) The height of the element in pixels.

**Sample**

```javascript
var ht = %%elementName%%.getHeight();
```

### getLabelForElementNames()

Returns an Array of label element names that has this field filled in as the labelFor.

**Returns**\
[Array](../../../js-lib/array.md) An array with element names.

**Sample**

```javascript
var array = elements.name_first.getLabelForElementNames();
for (var i = 0; i<array.length; i++)
{
	elements[array[i]].fgcolor = "#ff00ff";
}
```

### getLocationX()

Returns the x location of the current element.

NOTE: getLocationX() can be used with getLocationY() to set the location of an element using the setLocation function. For Example:

//returns the X and Y coordinates var x = forms.company.elements.faxBtn.getLocationX(); var y = forms.company.elements.faxBtn.getLocationY();

//sets the new location 10 px to the right; 10 px down from the current location forms.company.elements.faxBtn.setLocation(x+10,y+10);

**Returns**\
[Number](../../../js-lib/number.md) The x location of the element in pixels.

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
[Number](../../../js-lib/number.md) The y location of the element in pixels.

**Sample**

```javascript
var y =  %%elementName%%.getLocationY();
```

### getName()

Returns the name of an element. (may be null as well)

**Returns**\
[String](../../../js-lib/string.md) The name of the element.

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
[Number](../../../js-lib/number.md) The width of the element in pixels.

**Sample**

```javascript
var w = %%elementName%%.getWidth();
```

### hasStyleClass(styleName)

Check if an element already have a style from the styleClass property.

**Parameters**\
[String](../../../js-lib/string.md) styleName the name of the style class to be checked

**Returns**\
void

**Sample**

```javascript
%%elementName%%.hasStyleClass('redbg');
```

### putClientProperty(key, value)

Sets the value for the specified element client property key.

NOTE: Depending on the operating system, a user interface property name may be available.

**Parameters**\
[Object](../../../js-lib/object.md) key user interface key (depends on operating system)\
[Object](../../../js-lib/object.md) value a predefined value for the key

**Returns**\
void

**Sample**

```javascript
%%elementName%%.putClientProperty('ToolTipText','some text');
```

### removeStyleClass(styleName)

Removes a style from the styleClass property. This works only for NGClient where multiple styles are supported.

**Parameters**\
[String](../../../js-lib/string.md) styleName the name of the style class to remove

**Returns**\
void

**Sample**

```javascript
%%elementName%%.removeStyleClass('redbg');
```

### requestFocus()

Request the focus in this element. (Focus is also a text cursor on text components).

**Returns**\
void

**Sample**

```javascript
//request the focus in this %%elementName%% (focus is also a text cursor on text components)
%%elementName%%.requestFocus();
```

### requestFocus(mustExecuteOnFocusGainedMethod)

Request the focus in this element. (Focus is also a text cursor on text components).

**Parameters**\
[Boolean](../../../js-lib/boolean.md) mustExecuteOnFocusGainedMethod If true will execute onFocusGained method, else will not; default value is true.

**Returns**\
void

**Sample**

```javascript
//request the focus in this %%elementName%% (focus is also a text cursor on text components), skip on focus gained method call
%%elementName%%.requestFocus(false);
```

### setLocation(x, y)

Sets the location of an element. It takes as input the X (horizontal) and Y (vertical) coordinates - starting from the TOP LEFT side of the screen. Please note that location should not be altered at runtime when an element is anchored. Use the solutionModel in such a situation.

NOTE: getLocationX() can be used with getLocationY() to return the current location of an element; then use the X and Y coordinates with the setLocation function to set a new location. For Example:

//returns the X and Y coordinates var x = forms.company.elements.faxBtn.getLocationX(); var y = forms.company.elements.faxBtn.getLocationY();

//sets the new location 10 px to the right; 10 px down from the current location forms.company.elements.faxBtn.setLocation(x+10,y+10);

**Parameters**\
[Number](../../../js-lib/number.md) x the X coordinate of the element in pixels.\
[Number](../../../js-lib/number.md) y the Y coordinate of the element in pixels.

**Returns**\
void

**Sample**

```javascript
%%elementName%%.setLocation(200,200);
```

### setSize(width, height)

Sets the size of an element. It takes as input the width and the height. Please note that size should not be altered at runtime when an element is anchored. Use the solutionModel in such a situation.

NOTE: getWidth() can be used with getHeight() to set the size of an element using the setSize function. For Example:

//returns the width (w) and height (h) var w = forms.company.elements.faxBtn.getWidth(); var h = forms.company.elements.faxBtn.getHeight();

//sets the new size forms.company.elements.faxBtn.setSize(w,h);

//sets the new size and adds 1 px to both the width and height forms.company.elements.faxBtn.setSize(w+1,h+1);

**Parameters**\
[Number](../../../js-lib/number.md) width the width of the element in pixels.\
[Number](../../../js-lib/number.md) height the height of the element in pixels.

**Returns**\
void

**Sample**

```javascript
%%elementName%%.setSize(20,30);
```
