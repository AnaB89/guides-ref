# RuntimeSplitPane

## **Extends**

```
RuntimeComponent
```

## Property Summary

| Type                                  | Name                                                     | Summary                                                                                                                                                 |
| ------------------------------------- | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [String](../../../js-lib/string.md)   | [bgcolor](runtimesplitpane.md#bgcolor)                   | Gets or sets the background color of a field..                                                                                                          |
| [String](../../../js-lib/string.md)   | [border](runtimesplitpane.md#border)                     | Gets or sets the border attribute(s) of a specified element..                                                                                           |
| [Boolean](../../../js-lib/boolean.md) | [continuousLayout](runtimesplitpane.md#continuousLayout) | Gets or sets if the components should continuously be redrawn as the divider changes position..                                                         |
| [Number](../../../js-lib/number.md)   | [dividerLocation](runtimesplitpane.md#dividerLocation)   | Gets or sets divider location..                                                                                                                         |
| [Number](../../../js-lib/number.md)   | [dividerSize](runtimesplitpane.md#dividerSize)           | Gets or sets divider size in pixels..                                                                                                                   |
| [Boolean](../../../js-lib/boolean.md) | [enabled](runtimesplitpane.md#enabled)                   | Gets or sets the enabled state of a specified field, also known as "grayed"..                                                                           |
| [String](../../../js-lib/string.md)   | [fgcolor](runtimesplitpane.md#fgcolor)                   | Gets or sets the foreground color of a field..                                                                                                          |
| [String](../../../js-lib/string.md)   | [font](runtimesplitpane.md#font)                         | Gets or sets the font name, style, and size of an element..                                                                                             |
| [Number](../../../js-lib/number.md)   | [leftFormMinSize](runtimesplitpane.md#leftFormMinSize)   | Gets or sets left form minimum size in pixels..                                                                                                         |
| [Boolean](../../../js-lib/boolean.md) | [readOnly](runtimesplitpane.md#readOnly)                 | Gets or sets the editable/read-only state of a field; true - read-only; false - editable; ! - the editable/read-only state is inverted (the opposite).. |
| [Number](../../../js-lib/number.md)   | [resizeWeight](runtimesplitpane.md#resizeWeight)         | Specifies how to distribute extra space when the size of the split pane changes..                                                                       |
| [Number](../../../js-lib/number.md)   | [rightFormMinSize](runtimesplitpane.md#rightFormMinSize) | Gets or sets right form minimum size in pixels..                                                                                                        |
| [String](../../../js-lib/string.md)   | [toolTipText](runtimesplitpane.md#toolTipText)           | Gets or sets the tool tip text of an element; text displays when the mouse cursor hovers over an element..                                              |
| [Boolean](../../../js-lib/boolean.md) | [transparent](runtimesplitpane.md#transparent)           | Gets or sets the transparency of an element; true - transparent; false - not transparent..                                                              |
| [Boolean](../../../js-lib/boolean.md) | [visible](runtimesplitpane.md#visible)                   | Gets or sets the visibility of an element; true - visible; false - not visible; ! - the visibility state is inverted (the opposite)..                   |

## Methods Summary

| Type                                  | Name                                                                             | Summary                                                                 |
| ------------------------------------- | -------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| void                                  | [addStyleClass(styleName)](runtimesplitpane.md#addstyleclass-stylename)          | Adds a style to the styleClass property..                               |
| [Number](../../../js-lib/number.md)   | [getAbsoluteFormLocationY()](runtimesplitpane.md#getabsoluteformlocationy)       | Returns the absolute form (designed) Y location..                       |
| [Object](../../../js-lib/object.md)   | [getClientProperty(key)](runtimesplitpane.md#getclientproperty-key)              | Gets the specified client property for the element based on a key..     |
| [Object](../../../js-lib/object.md)   | [getDesignProperties()](runtimesplitpane.md#getdesignproperties)                 | Get the design-time properties of an element..                          |
| [Object](../../../js-lib/object.md)   | [getDesignTimeProperty(key)](runtimesplitpane.md#getdesigntimeproperty-key)      | Get a design-time property of an element..                              |
| [String](../../../js-lib/string.md)   | [getElementType()](runtimesplitpane.md#getelementtype)                           | Returns the type of a specified element..                               |
| [String](../../../js-lib/string.md)   | [getFormName()](runtimesplitpane.md#getformname)                                 | Returns the name of the form..                                          |
| [Number](../../../js-lib/number.md)   | [getHeight()](runtimesplitpane.md#getheight)                                     | Returns the height of the current element..                             |
| [RuntimeForm](../)                    | [getLeftForm()](runtimesplitpane.md#getleftform)                                 | Returns the left form of the split pane..                               |
| [Number](../../../js-lib/number.md)   | [getLocationX()](runtimesplitpane.md#getlocationx)                               | Returns the x location of the current element..                         |
| [Number](../../../js-lib/number.md)   | [getLocationY()](runtimesplitpane.md#getlocationy)                               | Returns the y location of the current element..                         |
| [String](../../../js-lib/string.md)   | [getMnemonicAt(i)](runtimesplitpane.md#getmnemonicat-i)                          | Returns the mnemonic for a specified tab of a tabpanel..                |
| [String](../../../js-lib/string.md)   | [getName()](runtimesplitpane.md#getname)                                         | Returns the name of an element..                                        |
| [RuntimeForm](../)                    | [getRightForm()](runtimesplitpane.md#getrightform)                               | Returns the right form of the split pane..                              |
| [Number](../../../js-lib/number.md)   | [getWidth()](runtimesplitpane.md#getwidth)                                       | Returns the width of the current element..                              |
| void                                  | [hasStyleClass(styleName)](runtimesplitpane.md#hasstyleclass-stylename)          | Check if an element already have a style from the styleClass property.. |
| void                                  | [putClientProperty(key, value)](runtimesplitpane.md#putclientproperty-key-value) | Sets the value for the specified element client property key..          |
| void                                  | [removeStyleClass(styleName)](runtimesplitpane.md#removestyleclass-stylename)    | Removes a style from the styleClass property..                          |
| [Boolean](../../../js-lib/boolean.md) | [setLeftForm(form)](runtimesplitpane.md#setleftform-form)                        | Set a relationless or related form as left panel..                      |
| [Boolean](../../../js-lib/boolean.md) | [setLeftForm(form, relation)](runtimesplitpane.md#setleftform-form-relation)     | Set a relationless or related form as left panel..                      |
| void                                  | [setLocation(x, y)](runtimesplitpane.md#setlocation-x-y)                         | Sets the location of an element..                                       |
| void                                  | [setMnemonicAt(index, text)](runtimesplitpane.md#setmnemonicat-index-text)       | Sets the mnemonic for a specified tab in a tabpanel..                   |
| [Boolean](../../../js-lib/boolean.md) | [setRightForm(form)](runtimesplitpane.md#setrightform-form)                      | Set a relationless or related form as right panel..                     |
| [Boolean](../../../js-lib/boolean.md) | [setRightForm(form, relation)](runtimesplitpane.md#setrightform-form-relation)   | Set a relationless or related form as right panel..                     |
| void                                  | [setSize(width, height)](runtimesplitpane.md#setsize-width-height)               | Sets the size of an element..                                           |

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

### continuousLayout

Gets or sets if the components should continuously be redrawn as the divider changes position.

**Returns**\
[Boolean](../../../js-lib/boolean.md)

**Sample**

```javascript
%%elementName%%.continuousLayout = true;
```

### dividerLocation

Gets or sets divider location. If location is less then 1 then the location will be considered at (location \* 100) percent of the split pane from left, otherwise it will represent the pixels from left.

**Returns**\
[Number](../../../js-lib/number.md)

**Sample**

```javascript
%%elementName%%.dividerLocation = 0.75;
```

### dividerSize

Gets or sets divider size in pixels.

**Returns**\
[Number](../../../js-lib/number.md)

**Sample**

```javascript
%%elementName%%.dividerSize = 10;
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

### leftFormMinSize

Gets or sets left form minimum size in pixels.

**Returns**\
[Number](../../../js-lib/number.md)

**Sample**

```javascript
%%elementName%%.leftFormMinSize = 100;
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

### resizeWeight

Specifies how to distribute extra space when the size of the split pane changes. A value of 0, the default, indicates the right/bottom component gets all the extra space (the left/top component acts fixed), where as a value of 1 specifies the left/top component gets all the extra space (the right/bottom component acts fixed). Specifically, the left/top component gets (weight \* diff) extra space and the right/bottom component gets (1 - weight) \* diff extra space

**Returns**\
[Number](../../../js-lib/number.md)

**Sample**

```javascript
%%elementName%%.resizeWeight = 0.5;
```

### rightFormMinSize

Gets or sets right form minimum size in pixels.

**Returns**\
[Number](../../../js-lib/number.md)

**Sample**

```javascript
%%elementName%%.rightFormMinSize = 100;
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

### getLeftForm()

Returns the left form of the split pane.

**Returns**\
[RuntimeForm](../) left form of the split pane

**Sample**

```javascript
var leftForm = %%elementName%%.getLeftForm();
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

### getMnemonicAt(i)

Returns the mnemonic for a specified tab of a tabpanel.

**Parameters**\
[Number](../../../js-lib/number.md) i The number of the specified tab.

**Returns**\
[String](../../../js-lib/string.md) The mnemonic.

**Sample**

```javascript
var mnemonic = %%elementName%%.getMnemonicAt(3);
```

### getName()

Returns the name of an element. (may be null as well)

**Returns**\
[String](../../../js-lib/string.md) The name of the element.

**Sample**

```javascript
var name = %%elementName%%.getName();
```

### getRightForm()

Returns the right form of the split pane.

**Returns**\
[RuntimeForm](../) right form of the split pane

**Sample**

```javascript
var rightForm = %%elementName%%.getRightForm();
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

### setLeftForm(form)

Set a relationless or related form as left panel.

**Parameters**\
[Object](../../../js-lib/object.md) form the specified form or form name you wish to add as left panel

**Returns**\
[Boolean](../../../js-lib/boolean.md) a boolean value indicating if tab was successfully added

**Sample**

```javascript
%%elementName%%.setLeftForm(forms.orders);
```

### setLeftForm(form, relation)

Set a relationless or related form as left panel.

**Parameters**\
[Object](../../../js-lib/object.md) form the specified form or form name you wish to add as left panel\
[Object](../../../js-lib/object.md) relation the relation name or a related foundset or null for relationless

**Returns**\
[Boolean](../../../js-lib/boolean.md) a boolean value indicating if tab was successfully added

**Sample**

```javascript
%%elementName%%.setLeftForm(forms.orders,'orders_to_order_details');
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

### setMnemonicAt(index, text)

Sets the mnemonic for a specified tab in a tabpanel.

**Parameters**\
[Object](../../../js-lib/object.md) index the number of the specified tab\
[Object](../../../js-lib/object.md) text the text to be set for the specified tab

**Returns**\
void

**Sample**

```javascript
%%elementName%%.setMnemonicAt(3,'a');
```

### setRightForm(form)

Set a relationless or related form as right panel.

**Parameters**\
[Object](../../../js-lib/object.md) form the specified form or form name you wish to add as right panel

**Returns**\
[Boolean](../../../js-lib/boolean.md) a boolean value indicating if tab was successfully added

**Sample**

```javascript
%%elementName%%.setRightForm(forms.orders);
```

### setRightForm(form, relation)

Set a relationless or related form as right panel.

**Parameters**\
[Object](../../../js-lib/object.md) form the specified form or form name you wish to add as right panel\
[Object](../../../js-lib/object.md) relation the relation name or a related foundset or null for relationless

**Returns**\
[Boolean](../../../js-lib/boolean.md) a boolean value indicating if tab was successfully added

**Sample**

```javascript
%%elementName%%.setRightForm(forms.orders,'orders_to_order_details');
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
