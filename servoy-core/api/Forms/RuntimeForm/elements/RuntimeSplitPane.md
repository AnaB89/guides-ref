#  RuntimeSplitPane


## **Extends**
    RuntimeComponent

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../../../JSLib/String.md) | [bgcolor](RuntimeSplitPane.md#bgcolor)                   | Gets or sets the background color of a field..                                    |
| [String](../../../JSLib/String.md) | [border](RuntimeSplitPane.md#border)                   | Gets or sets the border attribute(s) of a specified element..                                    |
| [Boolean](../../../JSLib/Boolean.md) | [continuousLayout](RuntimeSplitPane.md#continuousLayout)                   | Gets or sets if the components should continuously be redrawn as the divider changes position..                                    |
| [Number](../../../JSLib/Number.md) | [dividerLocation](RuntimeSplitPane.md#dividerLocation)                   | Gets or sets divider location..                                    |
| [Number](../../../JSLib/Number.md) | [dividerSize](RuntimeSplitPane.md#dividerSize)                   | Gets or sets divider size in pixels..                                    |
| [Boolean](../../../JSLib/Boolean.md) | [enabled](RuntimeSplitPane.md#enabled)                   | Gets or sets the enabled state of a specified field, also known as "grayed"..                                    |
| [String](../../../JSLib/String.md) | [fgcolor](RuntimeSplitPane.md#fgcolor)                   | Gets or sets the foreground color of a field..                                    |
| [String](../../../JSLib/String.md) | [font](RuntimeSplitPane.md#font)                   | Gets or sets the font name, style, and size of an element..                                    |
| [Number](../../../JSLib/Number.md) | [leftFormMinSize](RuntimeSplitPane.md#leftFormMinSize)                   | Gets or sets left form minimum size in pixels..                                    |
| [Boolean](../../../JSLib/Boolean.md) | [readOnly](RuntimeSplitPane.md#readOnly)                   | Gets or sets the editable/read-only state of a field; true - read-only; false - editable; ! - the editable/read-only state is inverted (the opposite)..                                    |
| [Number](../../../JSLib/Number.md) | [resizeWeight](RuntimeSplitPane.md#resizeWeight)                   | Specifies how to distribute extra space when the size of the split pane changes..                                    |
| [Number](../../../JSLib/Number.md) | [rightFormMinSize](RuntimeSplitPane.md#rightFormMinSize)                   | Gets or sets right form minimum size in pixels..                                    |
| [String](../../../JSLib/String.md) | [toolTipText](RuntimeSplitPane.md#toolTipText)                   | Gets or sets the tool tip text of an element; text displays when the mouse cursor hovers over an element..                                    |
| [Boolean](../../../JSLib/Boolean.md) | [transparent](RuntimeSplitPane.md#transparent)                   | Gets or sets the transparency of an element; true - transparent; false - not transparent..                                    |
| [Boolean](../../../JSLib/Boolean.md) | [visible](RuntimeSplitPane.md#visible)                   | Gets or sets the visibility of an element; true - visible; false - not visible; ! - the visibility state is inverted (the opposite)..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [addStyleClass(styleName)](RuntimeSplitPane.md#addstyleclass-stylename)                   | Adds a style to the styleClass property..                                    |
| [Number](../../../JSLib/Number.md) | [getAbsoluteFormLocationY()](RuntimeSplitPane.md#getabsoluteformlocationy)                   | Returns the absolute form (designed) Y location..                                    |
| [Object](../../../JSLib/Object.md) | [getClientProperty(key)](RuntimeSplitPane.md#getclientproperty-key)                   | Gets the specified client property for the element based on a key..                                    |
| [Object](../../../JSLib/Object.md) | [getDesignProperties()](RuntimeSplitPane.md#getdesignproperties)                   | Get the design-time properties of an element..                                    |
| [Object](../../../JSLib/Object.md) | [getDesignTimeProperty(key)](RuntimeSplitPane.md#getdesigntimeproperty-key)                   | Get a design-time property of an element..                                    |
| [String](../../../JSLib/String.md) | [getElementType()](RuntimeSplitPane.md#getelementtype)                   | Returns the type of a specified element..                                    |
| [String](../../../JSLib/String.md) | [getFormName()](RuntimeSplitPane.md#getformname)                   | Returns the name of the form..                                    |
| [Number](../../../JSLib/Number.md) | [getHeight()](RuntimeSplitPane.md#getheight)                   | Returns the height of the current element..                                    |
| [RuntimeForm](../../RuntimeForm.md) | [getLeftForm()](RuntimeSplitPane.md#getleftform)                   | Returns the left form of the split pane..                                    |
| [Number](../../../JSLib/Number.md) | [getLocationX()](RuntimeSplitPane.md#getlocationx)                   | Returns the x location of the current element..                                    |
| [Number](../../../JSLib/Number.md) | [getLocationY()](RuntimeSplitPane.md#getlocationy)                   | Returns the y location of the current element..                                    |
| [String](../../../JSLib/String.md) | [getMnemonicAt(i)](RuntimeSplitPane.md#getmnemonicat-i)                   | Returns the mnemonic for a specified tab of a tabpanel..                                    |
| [String](../../../JSLib/String.md) | [getName()](RuntimeSplitPane.md#getname)                   | Returns the name of an element..                                    |
| [RuntimeForm](../../RuntimeForm.md) | [getRightForm()](RuntimeSplitPane.md#getrightform)                   | Returns the right form of the split pane..                                    |
| [Number](../../../JSLib/Number.md) | [getWidth()](RuntimeSplitPane.md#getwidth)                   | Returns the width of the current element..                                    |
|void | [hasStyleClass(styleName)](RuntimeSplitPane.md#hasstyleclass-stylename)                   | Check if an element already have a style from the styleClass property..                                    |
|void | [putClientProperty(key, value)](RuntimeSplitPane.md#putclientproperty-key-value)                   | Sets the value for the specified element client property key..                                    |
|void | [removeStyleClass(styleName)](RuntimeSplitPane.md#removestyleclass-stylename)                   | Removes a style from the styleClass property..                                    |
| [Boolean](../../../JSLib/Boolean.md) | [setLeftForm(form)](RuntimeSplitPane.md#setleftform-form)                   | Set a relationless or related form as left panel..                                    |
| [Boolean](../../../JSLib/Boolean.md) | [setLeftForm(form, relation)](RuntimeSplitPane.md#setleftform-form-relation)                   | Set a relationless or related form as left panel..                                    |
|void | [setLocation(x, y)](RuntimeSplitPane.md#setlocation-x-y)                   | Sets the location of an element..                                    |
|void | [setMnemonicAt(index, text)](RuntimeSplitPane.md#setmnemonicat-index-text)                   | Sets the mnemonic for a specified tab in a tabpanel..                                    |
| [Boolean](../../../JSLib/Boolean.md) | [setRightForm(form)](RuntimeSplitPane.md#setrightform-form)                   | Set a relationless or related form as right panel..                                    |
| [Boolean](../../../JSLib/Boolean.md) | [setRightForm(form, relation)](RuntimeSplitPane.md#setrightform-form-relation)                   | Set a relationless or related form as right panel..                                    |
|void | [setSize(width, height)](RuntimeSplitPane.md#setsize-width-height)                   | Sets the size of an element..                                    |

## Properties Details

### bgcolor

Gets or sets the background color of a field. The color has to be set using the hexadecimal RGB value as used in HTML.
It only returns it's correct value if it was explicitly set.

**Returns**\
[String](../../../JSLib/String.md) 


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

borderType - EmptyBorder, EtchedBorder, BevelBorder, LineBorder, TitleBorder, MatteBorder, SpecialMatteBorder.
size - (numeric value) for: bottom, left, right, top.
color - (hexadecimal value) for: bottom, left, right, top.
dash pattern - (numeric value) for selected side(s).
rounding radius - (numeric value) for selected side(s).

It only returns it's correct value if it was explicitly set.

NOTE: Use the same value(s) and order of attribute(s) from the element design time property "borderType".

**Returns**\
[String](../../../JSLib/String.md) 


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
[Boolean](../../../JSLib/Boolean.md) 


**Sample**

```javascript
%%elementName%%.continuousLayout = true;
```
### dividerLocation

Gets or sets divider location.
If location is less then 1 then the location will be considered at (location * 100) percent of the split pane from left,
otherwise it will represent the pixels from left.

**Returns**\
[Number](../../../JSLib/Number.md) 


**Sample**

```javascript
%%elementName%%.dividerLocation = 0.75;
```
### dividerSize

Gets or sets divider size in pixels.

**Returns**\
[Number](../../../JSLib/Number.md) 


**Sample**

```javascript
%%elementName%%.dividerSize = 10;
```
### enabled

Gets or sets the enabled state of a specified field, also known as "grayed".
true - enabled; false - not enabled; ! - the enabled state is inverted (the opposite).

NOTE: A disabled element cannot be selected by clicking the element (or by pressing the TAB key even if this option is supported by the operating system).

NOTE: A label or button element will not disable if the "displayType" design time property for a field is set to HTML_AREA.

NOTE: The disabled "grayed" color is dependent on the LAF set in the Servoy Client Application Preferences. For more information see Preferences: Look And Feel in the Servoy Developer User's Guide.

**Returns**\
[Boolean](../../../JSLib/Boolean.md) 


**Sample**

```javascript
//gets the enabled state of the field
var currState = %%elementName%%.enabled;

//sets the enabled state of the field
%%elementName%%.enabled = !currentState;
```
### fgcolor

Gets or sets the foreground color of a field. The color has to be set using the hexadecimal RGB value as used in HTML.
It only returns it's correct value if it was explicitly set.

**Returns**\
[String](../../../JSLib/String.md) 


**Sample**

```javascript
//sets the foreground color of the field
%%elementName%%.fgcolor = "#000000";

//gets the foreground color of the field
var c = %%elementName%%.fgcolor;
```
### font

Gets or sets the font name, style, and size of an element. 

font name - the name of the font family.
style - the type of the font. (plain = 0; bold = 1; italic = 2; bold-italic = 3).
size - the size of the font (in points). 

It only returns it's correct value if it was explicitly set.

**Returns**\
[String](../../../JSLib/String.md) 


**Sample**

```javascript
%%elementName%%.font = 'Tahoma,1,11';
```
### leftFormMinSize

Gets or sets left form minimum size in pixels.

**Returns**\
[Number](../../../JSLib/Number.md) 


**Sample**

```javascript
%%elementName%%.leftFormMinSize = 100;
```
### readOnly

Gets or sets the editable/read-only state of a field; true - read-only; false - editable; ! - the editable/read-only state is inverted (the opposite). 

NOTE: A field set as read-only can be selected by clicking (or pressing the TAB key if this option is supported by the operating system) and the field data can be copied.

**Returns**\
[Boolean](../../../JSLib/Boolean.md) 


**Sample**

```javascript
//gets the editable/read-only state of the field
var currentState = %%elementName%%.readOnly;

//sets the editable/read-only state of the field
%%elementName%%.readOnly = !currentState;
```
### resizeWeight

Specifies how to distribute extra space when the size of the split pane changes.
A value of 0, the default, indicates the right/bottom component gets all the extra space (the left/top component acts fixed),
where as a value of 1 specifies the left/top component gets all the extra space (the right/bottom component acts fixed).
Specifically, the left/top component gets (weight * diff) extra space and the right/bottom component gets (1 - weight) * diff extra space

**Returns**\
[Number](../../../JSLib/Number.md) 


**Sample**

```javascript
%%elementName%%.resizeWeight = 0.5;
```
### rightFormMinSize

Gets or sets right form minimum size in pixels.

**Returns**\
[Number](../../../JSLib/Number.md) 


**Sample**

```javascript
%%elementName%%.rightFormMinSize = 100;
```
### toolTipText

Gets or sets the tool tip text of an element; text displays when the mouse cursor hovers over an element. 

NOTE: HTML should be used for multi-line tooltips; you can also use any valid HTML tags to format tooltip text.

**Returns**\
[String](../../../JSLib/String.md) 


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
[Boolean](../../../JSLib/Boolean.md) 


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
[Boolean](../../../JSLib/Boolean.md) 


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
[String](../../../JSLib/String.md) styleName the name of the style class to add

**Returns**\
void 


**Sample**

```javascript
%%elementName%%.addStyleClass('redbg');
```
### getAbsoluteFormLocationY()

Returns the absolute form (designed) Y location.


**Returns**\
[Number](../../../JSLib/Number.md) The y location of the form in pixels.


**Sample**

```javascript
var absolute_y = %%elementName%%.getAbsoluteFormLocationY();
```
### getClientProperty(key)

Gets the specified client property for the element based on a key.

NOTE: Depending on the operating system, a user interface property name may be available.

**Parameters**\
[Object](../../../JSLib/Object.md) key user interface key (depends on operating system)

**Returns**\
[Object](../../../JSLib/Object.md) The value of the property for specified key.


**Sample**

```javascript
var property = %%elementName%%.getClientProperty('ToolTipText');
```
### getDesignProperties()

Get the design-time properties of an element.


**Returns**\
[Object](../../../JSLib/Object.md) 


**Sample**

```javascript
var prop = forms.orders.elements.mylabel.getDesignProperties()
```
### getDesignTimeProperty(key)

Get a design-time property of an element.

**Parameters**\
[String](../../../JSLib/String.md) key the name of the property

**Returns**\
[Object](../../../JSLib/Object.md) 


**Sample**

```javascript
var prop = forms.orders.elements.mylabel.getDesignTimeProperty('myprop')
```
### getElementType()

Returns the type of a specified element.


**Returns**\
[String](../../../JSLib/String.md) The display type of the element as String.


**Sample**

```javascript
var et = %%elementName%%.getElementType();
```
### getFormName()

Returns the name of the form. (may be empty string as well)


**Returns**\
[String](../../../JSLib/String.md) The name of the form.


**Sample**

```javascript
var name = %%elementName%%.getFormName();
```
### getHeight()

Returns the height of the current element. 
NOTE: getHeight() can be used with getWidth() to set the size of an element using the setSize function. For example:

//returns the width (w) and height (h)
var w = forms.company.elements.faxBtn.getWidth();
var h = forms.company.elements.faxBtn.getHeight();

//sets the new size
forms.company.elements.faxBtn.setSize(w,h);

//sets the new size and adds 1 px to both the width and height
forms.company.elements.faxBtn.setSize(w+1,h+1);


**Returns**\
[Number](../../../JSLib/Number.md) The height of the element in pixels.


**Sample**

```javascript
var ht = %%elementName%%.getHeight();
```
### getLeftForm()

Returns the left form of the split pane.


**Returns**\
[RuntimeForm](../../RuntimeForm.md) left form of the split pane


**Sample**

```javascript
var leftForm = %%elementName%%.getLeftForm();
```
### getLocationX()

Returns the x location of the current element. 

NOTE: getLocationX() can be used with getLocationY() to set the location of an element using the setLocation function. For Example:

//returns the X and Y coordinates
var x = forms.company.elements.faxBtn.getLocationX();
var y = forms.company.elements.faxBtn.getLocationY();

//sets the new location 10 px to the right; 10 px down from the current location
forms.company.elements.faxBtn.setLocation(x+10,y+10);


**Returns**\
[Number](../../../JSLib/Number.md) The x location of the element in pixels.


**Sample**

```javascript
var x = %%elementName%%.getLocationX();
```
### getLocationY()

Returns the y location of the current element. The method can only be used in Record view.

NOTE: getLocationY() can be used with getLocationX() to set the location of an element using the setLocation function. For Example:

//returns the X and Y coordinates
var x = forms.company.elements.faxBtn.getLocationX();
var y = forms.company.elements.faxBtn.getLocationY();

//sets the new location 10 px to the right; 10 px down from the current location
forms.company.elements.faxBtn.setLocation(x+10,y+10);


**Returns**\
[Number](../../../JSLib/Number.md) The y location of the element in pixels.


**Sample**

```javascript
var y =  %%elementName%%.getLocationY();
```
### getMnemonicAt(i)

Returns the mnemonic for a specified tab of a tabpanel.

**Parameters**\
[Number](../../../JSLib/Number.md) i The number of the specified tab.

**Returns**\
[String](../../../JSLib/String.md) The mnemonic.


**Sample**

```javascript
var mnemonic = %%elementName%%.getMnemonicAt(3);
```
### getName()

Returns the name of an element. (may be null as well)


**Returns**\
[String](../../../JSLib/String.md) The name of the element.


**Sample**

```javascript
var name = %%elementName%%.getName();
```
### getRightForm()

Returns the right form of the split pane.


**Returns**\
[RuntimeForm](../../RuntimeForm.md) right form of the split pane


**Sample**

```javascript
var rightForm = %%elementName%%.getRightForm();
```
### getWidth()

Returns the width of the current element. 

NOTE: getWidth() can be used with getHeight() to set the size of an element using the setSize function. For Example:

//returns the width (w) and height (h)
var w = forms.company.elements.faxBtn.getWidth();
var h = forms.company.elements.faxBtn.getHeight();

//sets the new size
forms.company.elements.faxBtn.setSize(w,h);

//sets the new size and adds 1 px to both the width and height
forms.company.elements.faxBtn.setSize(w+1,h+1);


**Returns**\
[Number](../../../JSLib/Number.md) The width of the element in pixels.


**Sample**

```javascript
var w = %%elementName%%.getWidth();
```
### hasStyleClass(styleName)

Check if an element already have a style from the styleClass property.

**Parameters**\
[String](../../../JSLib/String.md) styleName the name of the style class to be checked

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
[Object](../../../JSLib/Object.md) key user interface key (depends on operating system)\
[Object](../../../JSLib/Object.md) value a predefined value for the key

**Returns**\
void 


**Sample**

```javascript
%%elementName%%.putClientProperty('ToolTipText','some text');
```
### removeStyleClass(styleName)

Removes a style from the styleClass property. This works only for NGClient where multiple styles are supported.

**Parameters**\
[String](../../../JSLib/String.md) styleName the name of the style class to remove

**Returns**\
void 


**Sample**

```javascript
%%elementName%%.removeStyleClass('redbg');
```
### setLeftForm(form)

Set a relationless or related form as left panel.

**Parameters**\
[Object](../../../JSLib/Object.md) form the specified form or form name you wish to add as left panel

**Returns**\
[Boolean](../../../JSLib/Boolean.md) a boolean value indicating if tab was successfully added


**Sample**

```javascript
%%elementName%%.setLeftForm(forms.orders);
```
### setLeftForm(form, relation)

Set a relationless or related form as left panel.

**Parameters**\
[Object](../../../JSLib/Object.md) form the specified form or form name you wish to add as left panel\
[Object](../../../JSLib/Object.md) relation the relation name or a related foundset or null for relationless

**Returns**\
[Boolean](../../../JSLib/Boolean.md) a boolean value indicating if tab was successfully added


**Sample**

```javascript
%%elementName%%.setLeftForm(forms.orders,'orders_to_order_details');
```
### setLocation(x, y)

Sets the location of an element. It takes as input the X (horizontal) and Y (vertical) coordinates - starting from the TOP LEFT side of the screen.
Please note that location should not be altered at runtime when an element is anchored. Use the solutionModel in such a situation.

NOTE: getLocationX() can be used with getLocationY() to return the current location of an element; then use the X and Y coordinates with the setLocation function to set a new location. For Example:

//returns the X and Y coordinates
var x = forms.company.elements.faxBtn.getLocationX();
var y = forms.company.elements.faxBtn.getLocationY();

//sets the new location 10 px to the right; 10 px down from the current location
forms.company.elements.faxBtn.setLocation(x+10,y+10);

**Parameters**\
[Number](../../../JSLib/Number.md) x the X coordinate of the element in pixels.\
[Number](../../../JSLib/Number.md) y the Y coordinate of the element in pixels.

**Returns**\
void 


**Sample**

```javascript
%%elementName%%.setLocation(200,200);
```
### setMnemonicAt(index, text)

Sets the mnemonic for a specified tab in a tabpanel.

**Parameters**\
[Object](../../../JSLib/Object.md) index the number of the specified tab\
[Object](../../../JSLib/Object.md) text the text to be set for the specified tab

**Returns**\
void 


**Sample**

```javascript
%%elementName%%.setMnemonicAt(3,'a');
```
### setRightForm(form)

Set a relationless or related form as right panel.

**Parameters**\
[Object](../../../JSLib/Object.md) form the specified form or form name you wish to add as right panel

**Returns**\
[Boolean](../../../JSLib/Boolean.md) a boolean value indicating if tab was successfully added


**Sample**

```javascript
%%elementName%%.setRightForm(forms.orders);
```
### setRightForm(form, relation)

Set a relationless or related form as right panel.

**Parameters**\
[Object](../../../JSLib/Object.md) form the specified form or form name you wish to add as right panel\
[Object](../../../JSLib/Object.md) relation the relation name or a related foundset or null for relationless

**Returns**\
[Boolean](../../../JSLib/Boolean.md) a boolean value indicating if tab was successfully added


**Sample**

```javascript
%%elementName%%.setRightForm(forms.orders,'orders_to_order_details');
```
### setSize(width, height)

Sets the size of an element. It takes as input the width and the height. 
Please note that size should not be altered at runtime when an element is anchored. Use the solutionModel in such a situation.

NOTE: getWidth() can be used with getHeight() to set the size of an element using the setSize function. For Example: 

//returns the width (w) and height (h)
var w = forms.company.elements.faxBtn.getWidth();
var h = forms.company.elements.faxBtn.getHeight();

//sets the new size
forms.company.elements.faxBtn.setSize(w,h);

//sets the new size and adds 1 px to both the width and height
forms.company.elements.faxBtn.setSize(w+1,h+1);

**Parameters**\
[Number](../../../JSLib/Number.md) width the width of the element in pixels.\
[Number](../../../JSLib/Number.md) height the height of the element in pixels.

**Returns**\
void 


**Sample**

```javascript
%%elementName%%.setSize(20,30);
```

