#  TabPanel


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](../../JSLib/Number.md) | [anchors](TabPanel.md#anchors)                   | Enables a component to stick to a specific side of form and/or to  grow or shrink when a window is resized..                                    |
| [String](../../JSLib/String.md) | [background](TabPanel.md#background)                   | The background color of the component..                                    |
| [String](../../JSLib/String.md) | [borderType](TabPanel.md#borderType)                   | The type, color and style of border of the component..                                    |
| [String](../../JSLib/String.md) | [comment](TabPanel.md#comment)                   | .                                    |
| [CSSPosition](../../Application/CSSPosition.md) | [cssPosition](TabPanel.md#cssPosition)                   | Thecss position of the component..                                    |
| [Object](../../JSLib/Object.md) | [designTimeProperties](TabPanel.md#designTimeProperties)                   | Property to get and add design-time properties for a component..                                    |
| [Boolean](../../JSLib/Boolean.md) | [enabled](TabPanel.md#enabled)                   | The enable state of the component, default true..                                    |
| [String](../../JSLib/String.md) | [fontType](TabPanel.md#fontType)                   | The font type of the component..                                    |
| [String](../../JSLib/String.md) | [foreground](TabPanel.md#foreground)                   | The foreground color of the component..                                    |
| [Number](../../JSLib/Number.md) | [formIndex](TabPanel.md#formIndex)                   | Form index returns the z-index of the form element..                                    |
| [Number](../../JSLib/Number.md) | [horizontalAlignment](TabPanel.md#horizontalAlignment)                   | The horizontal alignment of the tabpanel..                                    |
| [String](../../JSLib/String.md) | [location](TabPanel.md#location)                   | The x and y position of the component, in pixels, separated by a comma..                                    |
| [String](../../JSLib/String.md) | [name](TabPanel.md#name)                   | The name of the component..                                    |
| [Boolean](../../JSLib/Boolean.md) | [scrollTabs](TabPanel.md#scrollTabs)                   | Flag that tells how to arrange the tabs if they don't fit on a single line..                                    |
| [String](../../JSLib/String.md) | [size](TabPanel.md#size)                   | The width and height (in pixels), separated by a comma..                                    |
| [String](../../JSLib/String.md) | [styleClass](TabPanel.md#styleClass)                   | The name of the style class that should be applied to this component..                                    |
| [Number](../../JSLib/Number.md) | [tabOrientation](TabPanel.md#tabOrientation)                   | The position of the tabs related to the tab panel..                                    |
| [Number](../../JSLib/Number.md) | [tabSeq](TabPanel.md#tabSeq)                   | An index that specifies the position of the component in the tab sequence..                                    |
| [Boolean](../../JSLib/Boolean.md) | [transparent](TabPanel.md#transparent)                   | Flag that tells if the component is transparent or not..                                    |
| [Boolean](../../JSLib/Boolean.md) | [visible](TabPanel.md#visible)                   | The visible property of the component, default true..                                    |

## Events Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [void](../../void.md) | [onChange(previousIndex, event)](TabPanel.md#onchange-previousindex-event)                   | Method to be executed when the selected tab is changed in the tab panel or divider position is changed in split pane..                                    |

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
### designTimeProperties

Property to get and add design-time properties for a component.

**Returns**\
[Object](../../JSLib/Object.md) map of the design-time properties


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
### horizontalAlignment

The horizontal alignment of the tabpanel.

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
### name

The name of the component. Through this name it can also accessed in methods.
Must be a valid javascript name. (no - in the name or start with number)

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript

```
### scrollTabs

Flag that tells how to arrange the tabs if they don't fit on a single line.
If this flag is set, then the tabs will stay on a single line, but there will
be the possibility to scroll them to the left and to the right. If this flag
is not set, then the tabs will be arranged on multiple lines.

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
### tabOrientation

The position of the tabs related to the tab panel. Can be one of TOP, RIGHT, BOTTOM, LEFT,
HIDE, SPLIT_HORIZONTAL, SPLIT_VERTICAL, ACCORDION_PANEL. The HIDE option makes the tabs invisible, SPLIT_HORIZONTAL
makes the tab panel horizontal split pane, SPLIT_VERTICAL makes the tab panel vertical split pane, ACCORDION_PANEL turns
the tab panel into an accordion.

**Returns**\
[Number](../../JSLib/Number.md) 


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
### transparent

Flag that tells if the component is transparent or not.

The default value is "false", that is the components
are not transparent.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


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

