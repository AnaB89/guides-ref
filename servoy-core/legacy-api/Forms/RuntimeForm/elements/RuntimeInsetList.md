#  RuntimeInsetList

## **Supported Clients**

    NGClient
    MobileClient

## **Extends**
    RuntimeComponent

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../../../JSLib/String.md) | [bgcolor](RuntimeInsetList.md#bgcolor)                   | Gets or sets the background color of a field..                                    |
| [String](../../../JSLib/String.md) | [border](RuntimeInsetList.md#border)                   | Gets or sets the border attribute(s) of a specified element..                                    |
| [Boolean](../../../JSLib/Boolean.md) | [enabled](RuntimeInsetList.md#enabled)                   | Gets or sets the enabled state of a specified field, also known as "grayed"..                                    |
| [String](../../../JSLib/String.md) | [fgcolor](RuntimeInsetList.md#fgcolor)                   | Gets or sets the foreground color of a field..                                    |
| [String](../../../JSLib/String.md) | [font](RuntimeInsetList.md#font)                   | Gets or sets the font name, style, and size of an element..                                    |
| [Boolean](../../../JSLib/Boolean.md) | [readOnly](RuntimeInsetList.md#readOnly)                   | Gets or sets the editable/read-only state of a field; true - read-only; false - editable; ! - the editable/read-only state is inverted (the opposite)..                                    |
| [String](../../../JSLib/String.md) | [toolTipText](RuntimeInsetList.md#toolTipText)                   | Gets or sets the tool tip text of an element; text displays when the mouse cursor hovers over an element..                                    |
| [Boolean](../../../JSLib/Boolean.md) | [transparent](RuntimeInsetList.md#transparent)                   | Gets or sets the transparency of an element; true - transparent; false - not transparent..                                    |
| [Boolean](../../../JSLib/Boolean.md) | [visible](RuntimeInsetList.md#visible)                   | Gets or sets the visibility of an element; true - visible; false - not visible; ! - the visibility state is inverted (the opposite)..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [addStyleClass(styleName)](RuntimeInsetList.md#addstyleclass-stylename)                   | Adds a style to the styleClass property..                                    |
|void | [deleteRecord()](RuntimeInsetList.md#deleterecord)                   | Deletes the currently selected portal row in the foundset of the specified portal..                                    |
|void | [duplicateRecord()](RuntimeInsetList.md#duplicaterecord)                   | Duplicates the currently selected portal row in the foundset of the specified portal..                                    |
|void | [duplicateRecord(addOnTop)](RuntimeInsetList.md#duplicaterecord-addontop)                   | Duplicates the currently selected portal row in the foundset of the specified portal..                                    |
| [Number](../../../JSLib/Number.md) | [getAbsoluteFormLocationY()](RuntimeInsetList.md#getabsoluteformlocationy)                   | Returns the absolute form (designed) Y location..                                    |
| [Object](../../../JSLib/Object.md) | [getClientProperty(key)](RuntimeInsetList.md#getclientproperty-key)                   | Gets the specified client property for the element based on a key..                                    |
| [Object](../../../JSLib/Object.md) | [getDesignProperties()](RuntimeInsetList.md#getdesignproperties)                   | Get the design-time properties of an element..                                    |
| [Object](../../../JSLib/Object.md) | [getDesignTimeProperty(key)](RuntimeInsetList.md#getdesigntimeproperty-key)                   | Get a design-time property of an element..                                    |
| [String](../../../JSLib/String.md) | [getElementType()](RuntimeInsetList.md#getelementtype)                   | Returns the type of a specified element..                                    |
| [String](../../../JSLib/String.md) | [getFormName()](RuntimeInsetList.md#getformname)                   | Returns the name of the form..                                    |
| [Number](../../../JSLib/Number.md) | [getHeight()](RuntimeInsetList.md#getheight)                   | Returns the height of the current element..                                    |
| [Number](../../../JSLib/Number.md) | [getLocationX()](RuntimeInsetList.md#getlocationx)                   | Returns the x location of the current element..                                    |
| [Number](../../../JSLib/Number.md) | [getLocationY()](RuntimeInsetList.md#getlocationy)                   | Returns the y location of the current element..                                    |
| [String](../../../JSLib/String.md) | [getName()](RuntimeInsetList.md#getname)                   | Returns the name of an element..                                    |
| [Number](../../../JSLib/Number.md) | [getScrollX()](RuntimeInsetList.md#getscrollx)                   | Returns the x scroll location of specified element - only for an element where height of element is less than the height of element content..                                    |
| [Number](../../../JSLib/Number.md) | [getScrollY()](RuntimeInsetList.md#getscrolly)                   | Returns the y scroll location of specified element - only for an element where height of element is less than the height of element content..                                    |
| [Number](../../../JSLib/Number.md) | [getSelectedIndex()](RuntimeInsetList.md#getselectedindex)                   | Gets the selected record index in the current cached foundset in the specified portal..                                    |
| [String](../../../JSLib/String.md) | [getSortColumns()](RuntimeInsetList.md#getsortcolumns)                   | Returns the sort columns names of the current portal (as comma separated string)..                                    |
| [Number](../../../JSLib/Number.md) | [getWidth()](RuntimeInsetList.md#getwidth)                   | Returns the width of the current element..                                    |
|void | [hasStyleClass(styleName)](RuntimeInsetList.md#hasstyleclass-stylename)                   | Check if an element already have a style from the styleClass property..                                    |
|void | [newRecord()](RuntimeInsetList.md#newrecord)                   | Creates a new portal row in the foundset of the specified portal..                                    |
|void | [newRecord(addOnTop)](RuntimeInsetList.md#newrecord-addontop)                   | Creates a new portal row in the foundset of the specified portal..                                    |
|void | [putClientProperty(key, value)](RuntimeInsetList.md#putclientproperty-key-value)                   | Sets the value for the specified element client property key..                                    |
|void | [removeStyleClass(styleName)](RuntimeInsetList.md#removestyleclass-stylename)                   | Removes a style from the styleClass property..                                    |
|void | [setLocation(x, y)](RuntimeInsetList.md#setlocation-x-y)                   | Sets the location of an element..                                    |
|void | [setScroll(x, y)](RuntimeInsetList.md#setscroll-x-y)                   | Sets the scroll location of an element..                                    |
|void | [setSelectedIndex(index)](RuntimeInsetList.md#setselectedindex-index)                   | Sets the selected record index in the current cached foundset in the specified portal..                                    |
|void | [setSize(width, height)](RuntimeInsetList.md#setsize-width-height)                   | Sets the size of an element..                                    |

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
SmartClient,WebClient,NGClient,MobileClient

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
SmartClient,WebClient,NGClient,MobileClient

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
### deleteRecord()

Deletes the currently selected portal row in the foundset of the specified portal.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
%%elementName%%.deleteRecord();
```
### duplicateRecord()

Duplicates the currently selected portal row in the foundset of the specified portal.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// adds the duplicated record on top
%%elementName%%.duplicateRecord();

adds the duplicated record as the topmost record of the foundset
```
### duplicateRecord(addOnTop)

Duplicates the currently selected portal row in the foundset of the specified portal.

**Parameters**\
[Boolean](../../../JSLib/Boolean.md) addOnTop add on top (default true)
adds the duplicated record to the foundset

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// adds the duplicated record on top
%%elementName%%.duplicateRecord(true);
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
SmartClient,WebClient,NGClient,MobileClient

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
### getSelectedIndex()

Gets the selected record index in the current cached foundset in the specified portal.


**Returns**\
[Number](../../../JSLib/Number.md) The selected index (integer).

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//gets the selected record index in the foundset
var current = %%elementName%%.getSelectedIndex();

//sets the next record index in the foundset
%%elementName%%.setSelectedIndex(current+1);
```
### getSortColumns()

Returns the sort columns names of the current portal (as comma separated string).


**Returns**\
[String](../../../JSLib/String.md) array with column names

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var w = %%elementName%%.getSortColumns();
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
### newRecord()

Creates a new portal row in the foundset of the specified portal.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// foreign key data is only filled in for equals (=) relation items 
%%elementName%%.newRecord();
```
### newRecord(addOnTop)

Creates a new portal row in the foundset of the specified portal.

**Parameters**\
[Boolean](../../../JSLib/Boolean.md) addOnTop adds the new portal record as the topmost row of the foundset, default value is true

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// foreign key data is only filled in for equals (=) relation items 
//adds the new record on top
%%elementName%%.newRecord(true);
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
### setSelectedIndex(index)

Sets the selected record index in the current cached foundset in the specified portal.

**Parameters**\
[Number](../../../JSLib/Number.md) index the specified record index

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//gets the selected record index in the foundset
var current = %%elementName%%.getSelectedIndex();

//sets the next record index in the foundset
%%elementName%%.setSelectedIndex(current+1);
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

