#  RadioButtons


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](../../JSLib/Number.md) | [anchors](RadioButtons.md#anchors)                   | Enables a component to stick to a specific side of form and/or to  grow or shrink when a window is resized..                                    |
| [String](../../JSLib/String.md) | [background](RadioButtons.md#background)                   | The background color of the component..                                    |
| [String](../../JSLib/String.md) | [borderType](RadioButtons.md#borderType)                   | The type, color and style of border of the component..                                    |
| [String](../../JSLib/String.md) | [comment](RadioButtons.md#comment)                   | .                                    |
| [CSSPosition](../../Application/CSSPosition.md) | [cssPosition](RadioButtons.md#cssPosition)                   | Thecss position of the component..                                    |
| [String](../../JSLib/String.md) | [dataProvider](RadioButtons.md#dataProvider)                   | The dataprovider of the component..                                    |
| [Object](../../JSLib/Object.md) | [designTimeProperties](RadioButtons.md#designTimeProperties)                   | Property to get and add design-time properties for a component..                                    |
| [Number](../../JSLib/Number.md) | [displayType](RadioButtons.md#displayType)                   | The type of display used by the field..                                    |
| [Boolean](../../JSLib/Boolean.md) | [displaysTags](RadioButtons.md#displaysTags)                   | Flag that enables or disables merging of data inside components using tags (placeholders)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [editable](RadioButtons.md#editable)                   | Flag that tells if the content of the field can be edited or not..                                    |
| [Boolean](../../JSLib/Boolean.md) | [enabled](RadioButtons.md#enabled)                   | The enable state of the component, default true..                                    |
| [String](../../JSLib/String.md) | [fontType](RadioButtons.md#fontType)                   | The font type of the component..                                    |
| [String](../../JSLib/String.md) | [foreground](RadioButtons.md#foreground)                   | The foreground color of the component..                                    |
| [Number](../../JSLib/Number.md) | [formIndex](RadioButtons.md#formIndex)                   | Form index returns the z-index of the form element..                                    |
| [String](../../JSLib/String.md) | [format](RadioButtons.md#format)                   | The format that should be applied when displaying the data in the component..                                    |
| [Boolean](../../JSLib/Boolean.md) | [horizontal](RadioButtons.md#horizontal)                   | Show the radios as horizontal or vertical set..                                    |
| [Number](../../JSLib/Number.md) | [horizontalAlignment](RadioButtons.md#horizontalAlignment)                   | Horizontal alignment of the text inside the component..                                    |
| [String](../../JSLib/String.md) | [location](RadioButtons.md#location)                   | The x and y position of the component, in pixels, separated by a comma..                                    |
| [String](../../JSLib/String.md) | [margin](RadioButtons.md#margin)                   | The margins of the component..                                    |
| [String](../../JSLib/String.md) | [name](RadioButtons.md#name)                   | The name of the component..                                    |
| [Number](../../JSLib/Number.md) | [scrollbars](RadioButtons.md#scrollbars)                   | Scrollbar options for the vertical and horizontal scrollbars..                                    |
| [String](../../JSLib/String.md) | [size](RadioButtons.md#size)                   | The width and height (in pixels), separated by a comma..                                    |
| [String](../../JSLib/String.md) | [styleClass](RadioButtons.md#styleClass)                   | The name of the style class that should be applied to this component..                                    |
| [Number](../../JSLib/Number.md) | [tabSeq](RadioButtons.md#tabSeq)                   | An index that specifies the position of the component in the tab sequence..                                    |
| [String](../../JSLib/String.md) | [titleText](RadioButtons.md#titleText)                   | Header text to component.                                    |
| [String](../../JSLib/String.md) | [toolTipText](RadioButtons.md#toolTipText)                   | The text displayed when hovering over the component with a mouse cursor..                                    |
| [Boolean](../../JSLib/Boolean.md) | [transparent](RadioButtons.md#transparent)                   | Flag that tells if the component is transparent or not..                                    |
| [Number](../../JSLib/Number.md) | [valuelist](RadioButtons.md#valuelist)                   | The valuelist that is used by this field when displaying data..                                    |
| [Boolean](../../JSLib/Boolean.md) | [visible](RadioButtons.md#visible)                   | The visible property of the component, default true..                                    |

## Events Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [void](../../void.md) | [onAction()](RadioButtons.md#onaction)                   | The method that is executed when the component is clicked..                                    |
| [Boolean](../../JSLib/Boolean.md) | [onDataChange(oldValue, newValue, event)](RadioButtons.md#ondatachange-oldvalue-newvalue-event)                   | Method that is executed when the data in the component is successfully changed..                                    |
| [void](../../void.md) | [onFocusGained(event)](RadioButtons.md#onfocusgained-event)                   | The method that is executed when the component gains focus..                                    |
| [void](../../void.md) | [onFocusLost(event)](RadioButtons.md#onfocuslost-event)                   | The method that is executed when the component looses focus..                                    |
| [void](../../void.md) | [onRightClick(event)](RadioButtons.md#onrightclick-event)                   | The method that is executed when the component is right clicked..                                    |

## Properties Details

### anchors

Enables a component to stick to a specific side of form and/or to 
grow or shrink when a window is resized. 

If opposite anchors are activated then the component with grow or 
shrink with the window. For example if Top and Bottom are activated, 
then the component will grow/shrink when the window is vertically 
resized. If Left and Right are activated then the component
will grow/shrink when the window is horizontally resized. 

If opposite anchors are not activated, then the component will 
keep a constant distance from the sides of the window which
correspond to the activated anchors.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript

```
### background

The background color of the component.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript

```
### borderType

The type, color and style of border of the component.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript

```
### comment



**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript

```
### cssPosition

Thecss position of the component.

**Returns**\
[CSSPosition](../../Application/CSSPosition.md) 


**Sample**

```javascript

```
### dataProvider

The dataprovider of the component.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript

```
### designTimeProperties

Property to get and add design-time properties for a component.

**Returns**\
[Object](../../JSLib/Object.md) map of the design-time properties


**Sample**

```javascript

```
### displayType

The type of display used by the field. Can be one of CALENDAR, CHECKS,
COMBOBOX, HTML_AREA, IMAGE_MEDIA, PASSWORD, RADIOS, RTF_AREA, TEXT_AREA,
TEXT_FIELD, TYPE_AHEAD, LIST_BOX, MULTISELECT_LISTBOX or SPINNER.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript

```
### displaysTags

Flag that enables or disables merging of data inside components using tags (placeholders).
Tags (or placeholders) are words surrounded by %% on each side. There are data tags and
standard tags. Data tags consist in names of dataproviders surrounded by %%. Standard tags
are a set of predefined tags that are made available by the system.

See the "Merging data" section for more details about tags.

The default value of this flag is "false", that is merging of data is disabled by default.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript

```
### editable

Flag that tells if the content of the field can be edited or not.
The default value of this flag is "true", that is the content can be edited.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript

```
### enabled

The enable state of the component, default true.

**Returns**\
[Boolean](../../JSLib/Boolean.md) enabled state


**Sample**

```javascript

```
### fontType

The font type of the component.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript

```
### foreground

The foreground color of the component.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript

```
### formIndex

Form index returns the z-index of the form element. If two elements overlap,
then the element with higher Z index is displayed above the form element with lower Z index.
In case of form inheritance, form index is evaluated in the context (form) where property is defined.
Elements which have child form as context will always be on top of elements which have parent form.
If element is overridden in child form but form index property is still inherited its context is still parent form.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript

```
### format

The format that should be applied when displaying the data in the component.
There are different options for the different dataprovider types that are assigned to this field.
For Integer fields, there is a display and an edit format, using http://docs.oracle.com/javase/7/docs/api/java/text/DecimalFormat.html and the max (string) length can be set.
For Text/String fields, there are options to force uppercase,lowercase or only numbers. Or a mask can be set that restrict the input the pattern chars can be found here: http://docs.oracle.com/javase/7/docs/api/javax/swing/text/MaskFormatter.html
A mask can have a placehoder (what is shown when there is no data) and if the data must be stored raw (without literals of the mask). A max text length can also be set to force
the max text length input, this doesn't work on mask because that max length is controlled with the mask.
For Date fields a display and edit format can be set by using a pattern from here: http://docs.oracle.com/javase/7/docs/api/java/text/SimpleDateFormat.html, you can also say this must behave like a mask (the edit format)
A mask only works with when the edit format is exactly that mask (1 char is 1 number/char), because for example MM then only 2 numbers are allowed MMM that displays the month as a string is not supported as a mask.
Some examples are "dd-MM-yyyy", "MM-dd-yyyy", etc.
The format property is also used to set the UI Converter, this means that you can convert the value object to something else before it gets set into the field, this can also result in a type change of the data. 
So a string in scripting/db is converted to a integer in the ui, then you have to set an integer format. 
This property is applicable only for types: TEXT_FIELD, COMBOBOX, TYPE_AHEAD, CALENDAR and SPINNER.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript

```
### horizontal

Show the radios as horizontal or vertical set.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript

```
### horizontalAlignment

Horizontal alignment of the text inside the component. Can be one of
LEFT, CENTER or RIGHT.

Note that this property does not refer to the horizontal alignment
of the component inside the form.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript

```
### location

The x and y position of the component, in pixels, separated by a comma.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript

```
### margin

The margins of the component. They are specified in this order, 
separated by commas: top, left, bottom, right.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript

```
### name

The name of the component. Through this name it can also accessed in methods.
Must be a valid javascript name. (no - in the name or start with number)

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript

```
### scrollbars

Scrollbar options for the vertical and horizontal scrollbars. Each of the
vertical and horizontal scrollbars can be configured to display all the time,
to display only when needed or to never display.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript

```
### size

The width and height (in pixels), separated by a comma.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript

```
### styleClass

The name of the style class that should be applied to this component.

When defining style classes for specific component types, their names
must be prefixed according to the type of the component. For example 
in order to define a class names 'fancy' for fields, in the style
definition the class must be named 'field.fancy'. If it would be 
intended for labels, then it would be named 'label.fancy'. When specifying
the class name for a component, the prefix is dropped however. Thus the
field or the label will have its styleClass property set to 'fancy' only.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript

```
### tabSeq

An index that specifies the position of the component in the tab sequence. The components 
are put into the tab sequence in increasing order of this property. A value of 0 means
to use the default mechanism of building the tab sequence (based on their location on the form).
A value of -2 means to remove the component from the tab sequence.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript

```
### titleText

Header text to component

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript

```
### toolTipText

The text displayed when hovering over the component with a mouse cursor.

NOTE:
HTML should be used for multi-line tooltips; you can also use any
valid HTML tags to format tooltip text. For example:
<html>This includes<b>bolded text</b> and
<font color='blue'>BLUE</font> text as well.</html>

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript

```
### transparent

Flag that tells if the component is transparent or not.

The default value is "false", that is the components
are not transparent.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript

```
### valuelist

The valuelist that is used by this field when displaying data. Can be used
with fields of type CHECKS, COMBOBOX, RADIOS and TYPE_AHEAD.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript

```
### visible

The visible property of the component, default true.

**Returns**\
[Boolean](../../JSLib/Boolean.md) visible property


**Sample**

```javascript

```

