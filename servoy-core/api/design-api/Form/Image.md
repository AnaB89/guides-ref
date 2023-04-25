#  Image


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](../../JSLib/Number.md) | [anchors](Image.md#anchors)                   | Enables a component to stick to a specific side of form and/or to  grow or shrink when a window is resized..                                    |
| [String](../../JSLib/String.md) | [background](Image.md#background)                   | The background color of the component..                                    |
| [String](../../JSLib/String.md) | [borderType](Image.md#borderType)                   | The type, color and style of border of the component..                                    |
| [String](../../JSLib/String.md) | [comment](Image.md#comment)                   | .                                    |
| [CSSPosition](../../Application/CSSPosition.md) | [cssPosition](Image.md#cssPosition)                   | Thecss position of the component..                                    |
| [String](../../JSLib/String.md) | [dataProvider](Image.md#dataProvider)                   | The dataprovider of the component..                                    |
| [Object](../../JSLib/Object.md) | [designTimeProperties](Image.md#designTimeProperties)                   | Property to get and add design-time properties for a component..                                    |
| [Boolean](../../JSLib/Boolean.md) | [displaysTags](Image.md#displaysTags)                   | Flag that enables or disables merging of data inside components using tags (placeholders)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [enabled](Image.md#enabled)                   | The enable state of the component, default true..                                    |
| [String](../../JSLib/String.md) | [fontType](Image.md#fontType)                   | The font type of the component..                                    |
| [String](../../JSLib/String.md) | [foreground](Image.md#foreground)                   | The foreground color of the component..                                    |
| [Number](../../JSLib/Number.md) | [formIndex](Image.md#formIndex)                   | Form index returns the z-index of the form element..                                    |
| [String](../../JSLib/String.md) | [format](Image.md#format)                   | The format that should be applied when displaying data(using dataProviderID) in the label/button..                                    |
| [Number](../../JSLib/Number.md) | [horizontalAlignment](Image.md#horizontalAlignment)                   | Horizontal alignment of the text inside the component..                                    |
| [Number](../../JSLib/Number.md) | [imageMedia](Image.md#imageMedia)                   | The image Media object that should be displayed inside the component..                                    |
| [String](../../JSLib/String.md) | [labelFor](Image.md#labelFor)                   | Some components can be set to be labels of other components..                                    |
| [String](../../JSLib/String.md) | [location](Image.md#location)                   | The x and y position of the component, in pixels, separated by a comma..                                    |
| [String](../../JSLib/String.md) | [margin](Image.md#margin)                   | The margins of the component..                                    |
| [Number](../../JSLib/Number.md) | [mediaOptions](Image.md#mediaOptions)                   | Options to scale the image Media object that is displayed inside the component..                                    |
| [String](../../JSLib/String.md) | [mnemonic](Image.md#mnemonic)                   | The keyboard shortcut that activates this component..                                    |
| [String](../../JSLib/String.md) | [name](Image.md#name)                   | The name of the component..                                    |
| [Number](../../JSLib/Number.md) | [rolloverCursor](Image.md#rolloverCursor)                   | The cursor that is shown as the mouse is rolled over the component..                                    |
| [Number](../../JSLib/Number.md) | [rolloverImageMedia](Image.md#rolloverImageMedia)                   | The roll over image Media object used..                                    |
| [Boolean](../../JSLib/Boolean.md) | [showClick](Image.md#showClick)                   | When set, the element will show the clicked state when selected..                                    |
| [Boolean](../../JSLib/Boolean.md) | [showFocus](Image.md#showFocus)                   | When set the text of an element will showfocus when selected..                                    |
| [String](../../JSLib/String.md) | [size](Image.md#size)                   | The width and height (in pixels), separated by a comma..                                    |
| [String](../../JSLib/String.md) | [styleClass](Image.md#styleClass)                   | The name of the style class that should be applied to this component..                                    |
| [Number](../../JSLib/Number.md) | [tabSeq](Image.md#tabSeq)                   | An index that specifies the position of the component in the tab sequence..                                    |
| [String](../../JSLib/String.md) | [text](Image.md#text)                   | The text that is displayed inside the component..                                    |
| [Number](../../JSLib/Number.md) | [textRotation](Image.md#textRotation)                   | The rotation of the element..                                    |
| [String](../../JSLib/String.md) | [toolTipText](Image.md#toolTipText)                   | The text displayed when hovering over the component with a mouse cursor..                                    |
| [Boolean](../../JSLib/Boolean.md) | [transparent](Image.md#transparent)                   | Flag that tells if the component is transparent or not..                                    |
| [Number](../../JSLib/Number.md) | [verticalAlignment](Image.md#verticalAlignment)                   | The vertical alignment of the text inside the component..                                    |
| [Boolean](../../JSLib/Boolean.md) | [visible](Image.md#visible)                   | The visible property of the component, default true..                                    |

## Events Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [void](../../void.md) | [onAction()](Image.md#onaction)                   | .                                    |
| [void](../../void.md) | [onDoubleClick(event)](Image.md#ondoubleclick-event)                   | The method that is executed when the component is double clicked..                                    |
| [void](../../void.md) | [onRightClick(event)](Image.md#onrightclick-event)                   | The method that is executed when the component is right clicked..                                    |

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

The format that should be applied when displaying data(using dataProviderID) in the label/button.
Some examples are "#%", "dd-MM-yyyy", "MM-dd-yyyy", etc.

**Returns**\
[String](../../JSLib/String.md) 


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
### imageMedia

The image Media object that should be displayed inside the component.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript

```
### labelFor

Some components can be set to be labels of other components. This is useful in
two situations. In table view mode it is used for constructing the header of the
table. In record view mode, by setting mnemonics on the label, keyboard shortcuts
can be used to set the focus to fields.

**Returns**\
[String](../../JSLib/String.md) 


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
### mediaOptions

Options to scale the image Media object that is displayed inside the component.
Can be set to one or a combination of CROP, REDUCE, ENLARGE and KEEPASPECT.

REDUCE will scale down the image if the component is smaller than the image.
REDUCE combined with KEEPASPECT will reduce the image, but keep its aspect ratio.
This is useful when the component has other proportions than the image.

ENLARGE will scale up the image if the component is larger than the image.
ENLARGE combined with KEEPASPECT will scale up the image while keeping its aspect ratio.

CROP will leave the image at its original size. If the component is smaller than
the image this will result in only a part of the image showing up.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript

```
### mnemonic

The keyboard shortcut that activates this component. A letter must be specified,
and the actual shortcut will be combination of ALT + the specified letter.

This property can be used in two ways. Normally the keyboard shortcut activates
the onClick event of the component. But if the "labelFor" property is set for the
component, then the keyboard shortcut will move the focus to the component whose
label this component is.

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
### rolloverCursor

The cursor that is shown as the mouse is rolled over the component.
Possible options are DEFAULT and HAND. Note that roll over cursor is not supported in Smart client for list view and tableview forms.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript

```
### rolloverImageMedia

The roll over image Media object used. It will only work if a property image is also used.
When the mouse is moved over the component, this image Media will be displayed.
When the mouse is moved out of the component, whatever text or image was being initially
displayed will be restored. Note that roll over image is not supported in Smart client for list view and tableview forms.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript

```
### showClick

When set, the element will show the clicked state when selected.
Applies to labels and buttons and images only.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript

```
### showFocus

When set the text of an element will showfocus when selected.
Applies to labels and buttons only.
The text property for the element MUST be filled in first.

NOTE: The TAB key may also be used to select the element, depending
on the operating system being used and the selected LAF.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


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
### text

The text that is displayed inside the component.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript

```
### textRotation

The rotation of the element. You can choose 0, 90, 180, or 270 and the label is rotated accordingly.
This property also applies to buttons and images.

**Returns**\
[Number](../../JSLib/Number.md) 


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
### verticalAlignment

The vertical alignment of the text inside the component. Can be one of
TOP, CENTER or BOTTOM.

Note that this property does not refer to the vertical alignment of the
component inside the form.

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

