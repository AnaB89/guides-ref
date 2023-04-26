# RuntimeAccordionPanel

## **Extends**

```
RuntimeComponent
```

## Property Summary

| Type                                  | Name                                                | Summary                                                                                                                                                 |
| ------------------------------------- | --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [String](../../../js-lib/string.md)   | [bgcolor](runtimeaccordionpanel.md#bgcolor)         | Gets or sets the background color of a field..                                                                                                          |
| [String](../../../js-lib/string.md)   | [border](runtimeaccordionpanel.md#border)           | Gets or sets the border attribute(s) of a specified element..                                                                                           |
| [Boolean](../../../js-lib/boolean.md) | [enabled](runtimeaccordionpanel.md#enabled)         | Gets or sets the enabled state of a specified field, also known as "grayed"..                                                                           |
| [String](../../../js-lib/string.md)   | [fgcolor](runtimeaccordionpanel.md#fgcolor)         | Gets or sets the foreground color of a field..                                                                                                          |
| [String](../../../js-lib/string.md)   | [font](runtimeaccordionpanel.md#font)               | Gets or sets the font name, style, and size of an element..                                                                                             |
| [Boolean](../../../js-lib/boolean.md) | [readOnly](runtimeaccordionpanel.md#readOnly)       | Gets or sets the editable/read-only state of a field; true - read-only; false - editable; ! - the editable/read-only state is inverted (the opposite).. |
| [Object](../../../js-lib/object.md)   | [tabIndex](runtimeaccordionpanel.md#tabIndex)       | Gets or sets the selected tab index for the specified tabpanel..                                                                                        |
| [String](../../../js-lib/string.md)   | [toolTipText](runtimeaccordionpanel.md#toolTipText) | Gets or sets the tool tip text of an element; text displays when the mouse cursor hovers over an element..                                              |
| [Boolean](../../../js-lib/boolean.md) | [transparent](runtimeaccordionpanel.md#transparent) | Gets or sets the transparency of an element; true - transparent; false - not transparent..                                                              |
| [Boolean](../../../js-lib/boolean.md) | [visible](runtimeaccordionpanel.md#visible)         | Gets or sets the visibility of an element; true - visible; false - not visible; ! - the visibility state is inverted (the opposite)..                   |

## Methods Summary

| Type                                  | Name                                                                                                                                                                                                                       | Summary                                                                                        |
| ------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| void                                  | [addStyleClass(styleName)](runtimeaccordionpanel.md#addstyleclass-stylename)                                                                                                                                               | Adds a style to the styleClass property..                                                      |
| [Boolean](../../../js-lib/boolean.md) | [addTab(form/formname, name, tabText, tooltip, iconURL, fg, bg, relatedfoundset/relationname, index)](runtimeaccordionpanel.md#addtab-form/formname-name-tabtext-tooltip-iconurl-fg-bg-relatedfoundset/relationname-index) | Adds a relationless or related form as a tab in a specified tabpanel..                         |
| [Number](../../../js-lib/number.md)   | [getAbsoluteFormLocationY()](runtimeaccordionpanel.md#getabsoluteformlocationy)                                                                                                                                            | Returns the absolute form (designed) Y location..                                              |
| [Object](../../../js-lib/object.md)   | [getClientProperty(key)](runtimeaccordionpanel.md#getclientproperty-key)                                                                                                                                                   | Gets the specified client property for the element based on a key..                            |
| [Object](../../../js-lib/object.md)   | [getDesignProperties()](runtimeaccordionpanel.md#getdesignproperties)                                                                                                                                                      | Get the design-time properties of an element..                                                 |
| [Object](../../../js-lib/object.md)   | [getDesignTimeProperty(key)](runtimeaccordionpanel.md#getdesigntimeproperty-key)                                                                                                                                           | Get a design-time property of an element..                                                     |
| [String](../../../js-lib/string.md)   | [getElementType()](runtimeaccordionpanel.md#getelementtype)                                                                                                                                                                | Returns the type of a specified element..                                                      |
| [String](../../../js-lib/string.md)   | [getFormName()](runtimeaccordionpanel.md#getformname)                                                                                                                                                                      | Returns the name of the form..                                                                 |
| [Number](../../../js-lib/number.md)   | [getHeight()](runtimeaccordionpanel.md#getheight)                                                                                                                                                                          | Returns the height of the current element..                                                    |
| [Number](../../../js-lib/number.md)   | [getLocationX()](runtimeaccordionpanel.md#getlocationx)                                                                                                                                                                    | Returns the x location of the current element..                                                |
| [Number](../../../js-lib/number.md)   | [getLocationY()](runtimeaccordionpanel.md#getlocationy)                                                                                                                                                                    | Returns the y location of the current element..                                                |
| [Number](../../../js-lib/number.md)   | [getMaxTabIndex()](runtimeaccordionpanel.md#getmaxtabindex)                                                                                                                                                                | Returns the maximum tab index for a specified tabpanel..                                       |
| [String](../../../js-lib/string.md)   | [getMnemonicAt(i)](runtimeaccordionpanel.md#getmnemonicat-i)                                                                                                                                                               | Returns the mnemonic for a specified tab of a tabpanel..                                       |
| [String](../../../js-lib/string.md)   | [getName()](runtimeaccordionpanel.md#getname)                                                                                                                                                                              | Returns the name of an element..                                                               |
| [String](../../../js-lib/string.md)   | [getTabFGColorAt(i)](runtimeaccordionpanel.md#gettabfgcolorat-i)                                                                                                                                                           | Returns the foreground color for a specified tab of a tabpanel..                               |
| [String](../../../js-lib/string.md)   | [getTabFormNameAt(i)](runtimeaccordionpanel.md#gettabformnameat-i)                                                                                                                                                         | Returns the form name for a specified tab of a tabpanel..                                      |
| [String](../../../js-lib/string.md)   | [getTabNameAt(i)](runtimeaccordionpanel.md#gettabnameat-i)                                                                                                                                                                 | Returns the name - the "name" design time property value - for a specified tab of a tabpanel.. |
| [String](../../../js-lib/string.md)   | [getTabRelationNameAt(i)](runtimeaccordionpanel.md#gettabrelationnameat-i)                                                                                                                                                 | Returns the relation name for a specified tab of a tabpanel..                                  |
| [String](../../../js-lib/string.md)   | [getTabTextAt(i)](runtimeaccordionpanel.md#gettabtextat-i)                                                                                                                                                                 | Returns the text for a specified tab of a tabpanel..                                           |
| [Number](../../../js-lib/number.md)   | [getWidth()](runtimeaccordionpanel.md#getwidth)                                                                                                                                                                            | Returns the width of the current element..                                                     |
| void                                  | [hasStyleClass(styleName)](runtimeaccordionpanel.md#hasstyleclass-stylename)                                                                                                                                               | Check if an element already have a style from the styleClass property..                        |
| [Boolean](../../../js-lib/boolean.md) | [isTabEnabledAt(i)](runtimeaccordionpanel.md#istabenabledat-i)                                                                                                                                                             | Returns the enabled status of a specified tab in a tabpanel..                                  |
| void                                  | [putClientProperty(key, value)](runtimeaccordionpanel.md#putclientproperty-key-value)                                                                                                                                      | Sets the value for the specified element client property key..                                 |
| [Boolean](../../../js-lib/boolean.md) | [removeAllTabs()](runtimeaccordionpanel.md#removealltabs)                                                                                                                                                                  | Removes all tabs for a specified tabpanel..                                                    |
| void                                  | [removeStyleClass(styleName)](runtimeaccordionpanel.md#removestyleclass-stylename)                                                                                                                                         | Removes a style from the styleClass property..                                                 |
| [Boolean](../../../js-lib/boolean.md) | [removeTabAt(index)](runtimeaccordionpanel.md#removetabat-index)                                                                                                                                                           | Removes a specified tab in a tabpanel; can be based on a relation or relationless..            |
| void                                  | [setLocation(x, y)](runtimeaccordionpanel.md#setlocation-x-y)                                                                                                                                                              | Sets the location of an element..                                                              |
| void                                  | [setMnemonicAt(index, text)](runtimeaccordionpanel.md#setmnemonicat-index-text)                                                                                                                                            | Sets the mnemonic for a specified tab in a tabpanel..                                          |
| void                                  | [setSize(width, height)](runtimeaccordionpanel.md#setsize-width-height)                                                                                                                                                    | Sets the size of an element..                                                                  |
| void                                  | [setTabEnabledAt(i, b)](runtimeaccordionpanel.md#settabenabledat-i-b)                                                                                                                                                      | Sets the status of a specified tab in a tabpanel..                                             |
| void                                  | [setTabFGColorAt(i, s)](runtimeaccordionpanel.md#settabfgcolorat-i-s)                                                                                                                                                      | Sets the foreground color for a specified tab in a tabpanel..                                  |
| void                                  | [setTabTextAt(index, text)](runtimeaccordionpanel.md#settabtextat-index-text)                                                                                                                                              | Sets the text for a specified tab in a tabpanel..                                              |

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

### tabIndex

Gets or sets the selected tab index for the specified tabpanel. When setting the value either the tab index or the tab name can be used. When getting the value, the tab index (not the name) will be returned all the time.

NOTE: In NGClient tabIndex is updated after form is shown (so onShow of form will have the old index)

**Returns**\
[Object](../../../js-lib/object.md)

**Sample**

```javascript
//gets the selected tab index of the tabpanel
var current = %%elementName%%.tabIndex;

//sets (goes to) the selected tabIndex of the tabpanel
%%elementName%%.tabIndex = current + 1;

//or sets (goes to) the tab with the specified name
%%elementName%%.tabIndex = 'tab_name';
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

### addTab(form/formname, name, tabText, tooltip, iconURL, fg, bg, relatedfoundset/relationname, index)

Adds a relationless or related form as a tab in a specified tabpanel.

**Parameters**\
[Object](../../../js-lib/object.md) form/formname the specified form/form name you wish to add as a tab\
[Object](../../../js-lib/object.md) name the specified name for the tab or NULL (default is null)\
[Object](../../../js-lib/object.md) tabText the specified text for the tab (default is null)\
[Object](../../../js-lib/object.md) tooltip a specified tooltip for the tab (default is null)\
[Object](../../../js-lib/object.md) iconURL a specified icon image or icon URL for the tab (default is null)\
[Object](../../../js-lib/object.md) fg the HTML RGB Hexadecimal foreground color for the tab (default is null)\
[Object](../../../js-lib/object.md) bg the HTML RGB Hexadecimal background color for the tab (default is null)\
[Object](../../../js-lib/object.md) relatedfoundset/relationname the specified name of the related foundset (default is null)\
[Object](../../../js-lib/object.md) index the specified index of a tab, default is -1, will add tab to the end, this index is 0 based

**Returns**\
[Boolean](../../../js-lib/boolean.md) a boolean value indicating if tab was successfully added

**Sample**

```javascript
%%elementName%%.addTab(forms.orders,'ordersTab','Orders',null,null,'#000000','#BBCCEE');
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

### getMaxTabIndex()

Returns the maximum tab index for a specified tabpanel.

**Returns**\
[Number](../../../js-lib/number.md) maximum tab index (number)

**Sample**

```javascript
var max = %%elementName%%.getMaxTabIndex();
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

### getTabFGColorAt(i)

Returns the foreground color for a specified tab of a tabpanel.

**Parameters**\
[Number](../../../js-lib/number.md) i the number of the specified tab

**Returns**\
[String](../../../js-lib/string.md) color as hexadecimal RGB string

**Sample**

```javascript
var color = %%elementName%%.getTabFGColorAt(3);
```

### getTabFormNameAt(i)

Returns the form name for a specified tab of a tabpanel.

**Parameters**\
[Number](../../../js-lib/number.md) i index of the tab

**Returns**\
[String](../../../js-lib/string.md) the name of the form

**Sample**

```javascript
var formName = %%elementName%%.getSelectedTabFormName(3);
```

### getTabNameAt(i)

Returns the name - the "name" design time property value - for a specified tab of a tabpanel.

**Parameters**\
[Number](../../../js-lib/number.md) i The number of the specified tab.

**Returns**\
[String](../../../js-lib/string.md) The tab name

**Sample**

```javascript
var tabName = %%elementName%%.getTabNameAt(3);
```

### getTabRelationNameAt(i)

Returns the relation name for a specified tab of a tabpanel.

**Parameters**\
[Number](../../../js-lib/number.md) i index of the tab

**Returns**\
[String](../../../js-lib/string.md) relation name

**Sample**

```javascript
var relName = %%elementName%%.getTabRelationNameAt(3);
```

### getTabTextAt(i)

Returns the text for a specified tab of a tabpanel.

**Parameters**\
[Number](../../../js-lib/number.md) i The number of the specified tab.

**Returns**\
[String](../../../js-lib/string.md) The tab text.

**Sample**

```javascript
var tabText = %%elementName%%.getTabTextAt(3);
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

### isTabEnabledAt(i)

Returns the enabled status of a specified tab in a tabpanel.

**Parameters**\
[Number](../../../js-lib/number.md) i the number of the specified tab.

**Returns**\
[Boolean](../../../js-lib/boolean.md) True if tab is enabled, false otherwise.

**Sample**

```javascript
var status = %%elementName%%.isTabEnabledAt(3);
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

### removeAllTabs()

Removes all tabs for a specified tabpanel.

**Returns**\
[Boolean](../../../js-lib/boolean.md) a boolean value indicating if tabs were successfully removed

**Sample**

```javascript
%%elementName%%.removeAllTabs();
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

### removeTabAt(index)

Removes a specified tab in a tabpanel; can be based on a relation or relationless.

NOTE: In Servoy 4.x (and higher), the addTab function applies to relationless or related tabs in a tabpanel.

**Parameters**\
[Object](../../../js-lib/object.md) index The index of the tab to remove.

**Returns**\
[Boolean](../../../js-lib/boolean.md) a boolean value indicating if tab was successfully removed

**Sample**

```javascript
%%elementName%%.removeTabAt(3);
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

### setTabEnabledAt(i, b)

Sets the status of a specified tab in a tabpanel.

**Parameters**\
[Number](../../../js-lib/number.md) i the number of the specified tab.\
[Boolean](../../../js-lib/boolean.md) b true if enabled; or false if disabled.

**Returns**\
void

**Sample**

```javascript
%%elementName%%.setTabEnabledAt(3,true);
```

### setTabFGColorAt(i, s)

Sets the foreground color for a specified tab in a tabpanel.

**Parameters**\
[Number](../../../js-lib/number.md) i the number of the specified tab\
[String](../../../js-lib/string.md) s the hexadecimal RGB color value to be set.

**Returns**\
void

**Sample**

```javascript
%%elementName%%.setTabFGColorAt(3,'#000000');
```

### setTabTextAt(index, text)

Sets the text for a specified tab in a tabpanel.

**Parameters**\
[Object](../../../js-lib/object.md) index the number of the specified tab\
[Object](../../../js-lib/object.md) text the text to be set for the specified tab

**Returns**\
void

**Sample**

```javascript
%%elementName%%.setTabTextAt(3,'newTitle');
```
