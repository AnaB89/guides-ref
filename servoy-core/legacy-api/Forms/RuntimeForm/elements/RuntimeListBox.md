#  RuntimeListBox

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## **Extends**
    RuntimeComponent

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../../../JSLib/String.md) | [bgcolor](RuntimeListBox.md#bgcolor)                   | Gets or sets the background color of a field..                                    |
| [String](../../../JSLib/String.md) | [border](RuntimeListBox.md#border)                   | Gets or sets the border attribute(s) of a specified element..                                    |
| [Boolean](../../../JSLib/Boolean.md) | [enabled](RuntimeListBox.md#enabled)                   | Gets or sets the enabled state of a specified field, also known as "grayed"..                                    |
| [String](../../../JSLib/String.md) | [fgcolor](RuntimeListBox.md#fgcolor)                   | Gets or sets the foreground color of a field..                                    |
| [String](../../../JSLib/String.md) | [font](RuntimeListBox.md#font)                   | Gets or sets the font name, style, and size of an element..                                    |
| [Boolean](../../../JSLib/Boolean.md) | [readOnly](RuntimeListBox.md#readOnly)                   | Gets or sets the editable/read-only state of a field; true - read-only; false - editable; ! - the editable/read-only state is inverted (the opposite)..                                    |
| [String](../../../JSLib/String.md) | [titleText](RuntimeListBox.md#titleText)                   | Gets or sets the title text..                                    |
| [String](../../../JSLib/String.md) | [toolTipText](RuntimeListBox.md#toolTipText)                   | Gets or sets the tool tip text of an element; text displays when the mouse cursor hovers over an element..                                    |
| [Boolean](../../../JSLib/Boolean.md) | [transparent](RuntimeListBox.md#transparent)                   | Gets or sets the transparency of an element; true - transparent; false - not transparent..                                    |
| [Boolean](../../../JSLib/Boolean.md) | [visible](RuntimeListBox.md#visible)                   | Gets or sets the visibility of an element; true - visible; false - not visible; ! - the visibility state is inverted (the opposite)..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [addStyleClass(styleName)](RuntimeListBox.md#addstyleclass-stylename)                   | Adds a style to the styleClass property..                                    |
| [Number](../../../JSLib/Number.md) | [getAbsoluteFormLocationY()](RuntimeListBox.md#getabsoluteformlocationy)                   | Returns the absolute form (designed) Y location..                                    |
| [Object](../../../JSLib/Object.md) | [getClientProperty(key)](RuntimeListBox.md#getclientproperty-key)                   | Gets the specified client property for the element based on a key..                                    |
| [String](../../../JSLib/String.md) | [getDataProviderID()](RuntimeListBox.md#getdataproviderid)                   | Get the data provider this UI element (display) is showing..                                    |
| [Object](../../../JSLib/Object.md) | [getDesignProperties()](RuntimeListBox.md#getdesignproperties)                   | Get the design-time properties of an element..                                    |
| [Object](../../../JSLib/Object.md) | [getDesignTimeProperty(key)](RuntimeListBox.md#getdesigntimeproperty-key)                   | Get a design-time property of an element..                                    |
| [String](../../../JSLib/String.md) | [getElementType()](RuntimeListBox.md#getelementtype)                   | Returns the type of a specified element..                                    |
| [String](../../../JSLib/String.md) | [getFormName()](RuntimeListBox.md#getformname)                   | Returns the name of the form..                                    |
| [Number](../../../JSLib/Number.md) | [getHeight()](RuntimeListBox.md#getheight)                   | Returns the height of the current element..                                    |
| [Array](../../../JSLib/Array.md) | [getLabelForElementNames()](RuntimeListBox.md#getlabelforelementnames)                   | Returns an Array of label element names that has this field filled in as the labelFor..                                    |
| [Number](../../../JSLib/Number.md) | [getLocationX()](RuntimeListBox.md#getlocationx)                   | Returns the x location of the current element..                                    |
| [Number](../../../JSLib/Number.md) | [getLocationY()](RuntimeListBox.md#getlocationy)                   | Returns the y location of the current element..                                    |
| [String](../../../JSLib/String.md) | [getName()](RuntimeListBox.md#getname)                   | Returns the name of an element..                                    |
| [Number](../../../JSLib/Number.md) | [getScrollX()](RuntimeListBox.md#getscrollx)                   | Returns the x scroll location of specified element - only for an element where height of element is less than the height of element content..                                    |
| [Number](../../../JSLib/Number.md) | [getScrollY()](RuntimeListBox.md#getscrolly)                   | Returns the y scroll location of specified element - only for an element where height of element is less than the height of element content..                                    |
| [Array](../../../JSLib/Array.md) | [getSelectedElements()](RuntimeListBox.md#getselectedelements)                   | Gets the selected values (real values from valuelist) as array..                                    |
| [String](../../../JSLib/String.md) | [getValueListName()](RuntimeListBox.md#getvaluelistname)                   | Returns the current valuelist name for the specified field; returns NULL if no valuelist..                                    |
| [Number](../../../JSLib/Number.md) | [getWidth()](RuntimeListBox.md#getwidth)                   | Returns the width of the current element..                                    |
|void | [hasStyleClass(styleName)](RuntimeListBox.md#hasstyleclass-stylename)                   | Check if an element already have a style from the styleClass property..                                    |
|void | [putClientProperty(key, value)](RuntimeListBox.md#putclientproperty-key-value)                   | Sets the value for the specified element client property key..                                    |
|void | [removeStyleClass(styleName)](RuntimeListBox.md#removestyleclass-stylename)                   | Removes a style from the styleClass property..                                    |
|void | [requestFocus()](RuntimeListBox.md#requestfocus)                   | Request the focus in this element..                                    |
|void | [requestFocus(mustExecuteOnFocusGainedMethod)](RuntimeListBox.md#requestfocus-mustexecuteonfocusgainedmethod)                   | Request the focus in this element..                                    |
|void | [setLocation(x, y)](RuntimeListBox.md#setlocation-x-y)                   | Sets the location of an element..                                    |
|void | [setScroll(x, y)](RuntimeListBox.md#setscroll-x-y)                   | Sets the scroll location of an element..                                    |
|void | [setSize(width, height)](RuntimeListBox.md#setsize-width-height)                   | Sets the size of an element..                                    |
|void | [setValueListItems(value)](RuntimeListBox.md#setvaluelistitems-value)                   | Sets the display/real values to the custom valuelist of the element (if element has custom valuelist)..                                    |

## Properties Details

### bgcolor

Gets or sets the background color of a field. The color has to be set using the hexadecimal RGB value as used in HTML.
It only returns it's correct value if it was explicitly set.

**Returns**\
[String](../../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//sets the border type to "LineBorder"
//sets a 1 px line width for the bottom and left side of the border
//sets the hexadecimal color of the border to "#ccffcc"
%%elementName%%.border = 'LineBorder,1,#ccffcc';
```
### enabled

Gets or sets the enabled state of a specified field, also known as "grayed".
true - enabled; false - not enabled; ! - the enabled state is inverted (the opposite).

NOTE: A disabled element cannot be selected by clicking the element (or by pressing the TAB key even if this option is supported by the operating system).

NOTE: A label or button element will not disable if the "displayType" design time property for a field is set to HTML_AREA.

NOTE: The disabled "grayed" color is dependent on the LAF set in the Servoy Client Application Preferences. For more information see Preferences: Look And Feel in the Servoy Developer User's Guide.

**Returns**\
[Boolean](../../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
%%elementName%%.font = 'Tahoma,1,11';
```
### readOnly

Gets or sets the editable/read-only state of a field; true - read-only; false - editable; ! - the editable/read-only state is inverted (the opposite). 

NOTE: A field set as read-only can be selected by clicking (or pressing the TAB key if this option is supported by the operating system) and the field data can be copied.

**Returns**\
[Boolean](../../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

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
[String](../../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var titleText = %%elementName%%.titleText;
```
### toolTipText

Gets or sets the tool tip text of an element; text displays when the mouse cursor hovers over an element. 

NOTE: HTML should be used for multi-line tooltips; you can also use any valid HTML tags to format tooltip text.

**Returns**\
[String](../../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
NGClient

**Sample**

```javascript
%%elementName%%.addStyleClass('redbg');
```
### getAbsoluteFormLocationY()

Returns the absolute form (designed) Y location.


**Returns**\
[Number](../../../JSLib/Number.md) The y location of the form in pixels.

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var property = %%elementName%%.getClientProperty('ToolTipText');
```
### getDataProviderID()

Get the data provider this UI element (display) is showing.


**Returns**\
[String](../../../JSLib/String.md) The data provider as String.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
%%elementName%%.getDataProviderID();
```
### getDesignProperties()

Get the design-time properties of an element.


**Returns**\
[Object](../../../JSLib/Object.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var prop = forms.orders.elements.mylabel.getDesignTimeProperty('myprop')
```
### getElementType()

Returns the type of a specified element.


**Returns**\
[String](../../../JSLib/String.md) The display type of the element as String.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var et = %%elementName%%.getElementType();
```
### getFormName()

Returns the name of the form. (may be empty string as well)


**Returns**\
[String](../../../JSLib/String.md) The name of the form.

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var ht = %%elementName%%.getHeight();
```
### getLabelForElementNames()

Returns an Array of label element names that has this field filled in as the labelFor.


**Returns**\
[Array](../../../JSLib/Array.md) An array with element names.

**Supported Clients**\
SmartClient,WebClient,NGClient

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

//returns the X and Y coordinates
var x = forms.company.elements.faxBtn.getLocationX();
var y = forms.company.elements.faxBtn.getLocationY();

//sets the new location 10 px to the right; 10 px down from the current location
forms.company.elements.faxBtn.setLocation(x+10,y+10);


**Returns**\
[Number](../../../JSLib/Number.md) The x location of the element in pixels.

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var y =  %%elementName%%.getLocationY();
```
### getName()

Returns the name of an element. (may be null as well)


**Returns**\
[String](../../../JSLib/String.md) The name of the element.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var name = %%elementName%%.getName();
```
### getScrollX()

Returns the x scroll location of specified element - only for an element where height of element is less than the height of element content.

NOTE: getScrollX() can be used with getScrollY() to set the scroll location of an element using the setScroll function. For Example:

//returns the X and Y scroll coordinates
var x = forms.company.elements.portal50.getScrollX();
var y = forms.company.elements.portal50.getScrollY();

//sets the new scroll location
forms.company.elements.portal50.setScroll(x+10,y+10);


**Returns**\
[Number](../../../JSLib/Number.md) The x scroll location in pixels.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var x = %%elementName%%.getScrollX();
```
### getScrollY()

Returns the y scroll location of specified element - only for an element where height of element is less than the height of element content.

NOTE: getScrollY() can be used with getScrollX() to set the scroll location of an element using the setScroll function. For Example:

//returns the X and Y scroll coordinates
var x = forms.company.elements.portal50.getScrollX();
var y = forms.company.elements.portal50.getScrollY();

//sets the new scroll location
forms.company.elements.portal50.setScroll(x+10,y+10);


**Returns**\
[Number](../../../JSLib/Number.md) The y scroll location in pixels.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var y = %%elementName%%.getScrollY();
```
### getSelectedElements()

Gets the selected values (real values from valuelist) as array. The form element should have a dataProviderID assigned in order for this to work.


**Returns**\
[Array](../../../JSLib/Array.md) array with selected values

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var values = %%elementName%%.getSelectedElements();
```
### getValueListName()

Returns the current valuelist name for the specified field; returns NULL if no valuelist.


**Returns**\
[String](../../../JSLib/String.md) The valuelist name.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var name = %%elementName%%.getValueListName();
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

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
NGClient

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

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
NGClient

**Sample**

```javascript
%%elementName%%.removeStyleClass('redbg');
```
### requestFocus()

Request the focus in this element. (Focus is also a text cursor on text components).


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//request the focus in this %%elementName%% (focus is also a text cursor on text components)
%%elementName%%.requestFocus();
```
### requestFocus(mustExecuteOnFocusGainedMethod)

Request the focus in this element. (Focus is also a text cursor on text components).

**Parameters**\
[Boolean](../../../JSLib/Boolean.md) mustExecuteOnFocusGainedMethod If true will execute onFocusGained method, else will not; default value is true.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//request the focus in this %%elementName%% (focus is also a text cursor on text components), skip on focus gained method call
%%elementName%%.requestFocus(false);
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

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
%%elementName%%.setLocation(200,200);
```
### setScroll(x, y)

Sets the scroll location of an element. It takes as input the X (horizontal) and Y (vertical) coordinates - starting from the TOP LEFT side of the screen - only for an element where the height of the element is greater than the height of element content

NOTE: getScrollX() can be used with getScrollY() to return the current scroll location of an element; then use the X and Y coordinates with the setScroll function to set a new scroll location. For Example:

//returns the X and Y coordinates
var x = forms.company.elements.portal50.getScrollX();
var y = forms.company.elements.portal50.getScrollY();

//sets the new location
forms.company.elements.portal50.setScroll(x+10,y+10);

**Parameters**\
[Number](../../../JSLib/Number.md) x the X coordinate of the portal scroll location in pixels\
[Number](../../../JSLib/Number.md) y the Y coordinate of the portal scroll location in pixels

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
%%elementName%%.setScroll(200,200);
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

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
%%elementName%%.setSize(20,30);
```
### setValueListItems(value)

Sets the display/real values to the custom valuelist of the element (if element has custom valuelist).
This does not effect the value list with same name list on other elements or value lists at application level.

Should receive a dataset parameter, first column is for display values, second column (optional) is for real values.

NOTE: if you modify values for checkbox/radio field, note that having one value in valuelist is a special case, so switching between one value and 0/multiple values after form is created may have side effects

**Parameters**\
[Object](../../../JSLib/Object.md) value first column is display value, second column is real value

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var dataset = databaseManager.createEmptyDataSet(0,new Array('display_values','optional_real_values'));
dataset.addRow(['aa',1]);
dataset.addRow(['bb',2]);
dataset.addRow(['cc',3]);
// %%elementName%% should have a valuelist attached
%%elementName%%.setValueListItems(dataset);
```

