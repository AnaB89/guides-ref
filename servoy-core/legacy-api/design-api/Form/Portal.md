#  Portal

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](../../JSLib/Number.md) | [anchors](Portal.md#anchors)                   | Enables a component to stick to a specific side of form and/or to  grow or shrink when a window is resized..                                    |
| [String](../../JSLib/String.md) | [background](Portal.md#background)                   | The background color of the component..                                    |
| [String](../../JSLib/String.md) | [borderType](Portal.md#borderType)                   | The type, color and style of border of the component..                                    |
| [CSSPosition](../../Application/CSSPosition.md) | [cssPosition](Portal.md#cssPosition)                   | Thecss position of the component..                                    |
| [Object](../../JSLib/Object.md) | [designTimeProperties](Portal.md#designTimeProperties)                   | Property to get and add design-time properties for a component..                                    |
| [Boolean](../../JSLib/Boolean.md) | [enabled](Portal.md#enabled)                   | The enable state of the component, default true..                                    |
| [Number](../../JSLib/Number.md) | [formIndex](Portal.md#formIndex)                   | Form index returns the z-index of the form element..                                    |
| [String](../../JSLib/String.md) | [initialSort](Portal.md#initialSort)                   | The default sort order for the rows displayed in the portal..                                    |
| [String](../../JSLib/String.md) | [intercellSpacing](Portal.md#intercellSpacing)                   | The additional spacing between cell rows..                                    |
| [String](../../JSLib/String.md) | [location](Portal.md#location)                   | The x and y position of the component, in pixels, separated by a comma..                                    |
| [Boolean](../../JSLib/Boolean.md) | [multiLine](Portal.md#multiLine)                   | When set, portal rows can have a custom layout of fields, buttons, etc..                                    |
| [String](../../JSLib/String.md) | [name](Portal.md#name)                   | The name of the component..                                    |
| [Boolean](../../JSLib/Boolean.md) | [ngReadOnlyMode](Portal.md#ngReadOnlyMode)                   | .                                    |
| [Number](../../JSLib/Number.md) | [printSliding](Portal.md#printSliding)                   | Enables an element to resize based on its content and/or move when printing..                                    |
| [Boolean](../../JSLib/Boolean.md) | [printable](Portal.md#printable)                   | Flag that tells if the component should be printed or not when the form is printed..                                    |
| [String](../../JSLib/String.md) | [relationName](Portal.md#relationName)                   | The name of the relationship between the table related to the currently active  form and the table you want to show data from in the portal..                                    |
| [Boolean](../../JSLib/Boolean.md) | [reorderable](Portal.md#reorderable)                   | When set, the portal rows can be re-ordered by dragging the column headers..                                    |
| [Boolean](../../JSLib/Boolean.md) | [resizable](Portal.md#resizable)                   | When set the portal rows can be resized by users..                                    |
| [String](../../JSLib/String.md) | [rowBGColorCalculation](Portal.md#rowBGColorCalculation)                   | The calculation dataprovider (such as servoy_row_bgcolor) used to add background color and highlight selected or alternate portal rows..                                    |
| [Number](../../JSLib/Number.md) | [rowHeight](Portal.md#rowHeight)                   | The height of each row in pixels..                                    |
| [Number](../../JSLib/Number.md) | [scrollbars](Portal.md#scrollbars)                   | Scrollbar options for the vertical and horizontal scrollbars..                                    |
| [Boolean](../../JSLib/Boolean.md) | [showHorizontalLines](Portal.md#showHorizontalLines)                   | When set, the portal displays horizontal lines between the rows..                                    |
| [Boolean](../../JSLib/Boolean.md) | [showVerticalLines](Portal.md#showVerticalLines)                   | When set the portal displays vertical lines between the columns..                                    |
| [String](../../JSLib/String.md) | [size](Portal.md#size)                   | The width and height (in pixels), separated by a comma..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sortable](Portal.md#sortable)                   | When set, users can sort the contents of the portal by clicking on the column headings..                                    |
| [String](../../JSLib/String.md) | [styleClass](Portal.md#styleClass)                   | The name of the style class that should be applied to this component..                                    |
| [Number](../../JSLib/Number.md) | [tabSeq](Portal.md#tabSeq)                   | An index that specifies the position of the component in the tab sequence..                                    |
| [Boolean](../../JSLib/Boolean.md) | [transparent](Portal.md#transparent)                   | Flag that tells if the component is transparent or not..                                    |
| [Boolean](../../JSLib/Boolean.md) | [visible](Portal.md#visible)                   | The visible property of the component, default true..                                    |

## Events Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [void](../../void.md) | [onDrag()](Portal.md#ondrag)                   | The method that is triggered when (non Design Mode) dragging occurs..                                    |
| [void](../../void.md) | [onDragEnd()](Portal.md#ondragend)                   | The method that is triggered when (non Design Mode) dragging end occurs..                                    |
| [void](../../void.md) | [onDragOver()](Portal.md#ondragover)                   | The method that is triggered when (non Design Mode) dragging over a component occurs..                                    |
| [void](../../void.md) | [onDrop()](Portal.md#ondrop)                   | The method that is triggered when (non Design Mode) dropping occurs..                                    |
| [void](../../void.md) | [onRender()](Portal.md#onrender)                   | The method that is executed when the component is rendered..                                    |

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

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### background

The background color of the component.

**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### borderType

The type, color and style of border of the component.

**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### cssPosition

Thecss position of the component.

**Returns**\
[CSSPosition](../../Application/CSSPosition.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### designTimeProperties

Property to get and add design-time properties for a component.

**Returns**\
[Object](../../JSLib/Object.md) map of the design-time properties

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### enabled

The enable state of the component, default true.

**Returns**\
[Boolean](../../JSLib/Boolean.md) enabled state

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### initialSort

The default sort order for the rows displayed in the portal.

**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### intercellSpacing

The additional spacing between cell rows. Is composed from the horizontal spacing
and the vertical spacing.

**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### location

The x and y position of the component, in pixels, separated by a comma.

**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### multiLine

When set, portal rows can have a custom layout of fields, buttons, etc. displayed for each
matching row (rather than the default "grid").

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### name

The name of the component. Through this name it can also accessed in methods.
Must be a valid javascript name. (no - in the name or start with number)

**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### ngReadOnlyMode



**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### printSliding

Enables an element to resize based on its content and/or move when printing.
The component can move horizontally or vertically and can grow or shrink in
height and width, based on its content and the content of neighboring
components.

**Returns**\
[Number](../../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript

```
### printable

Flag that tells if the component should be printed or not when the form is printed.

By default components are printable.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript

```
### relationName

The name of the relationship between the table related to the currently active 
form and the table you want to show data from in the portal.

**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### reorderable

When set, the portal rows can be re-ordered by dragging the column headers.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### resizable

When set the portal rows can be resized by users.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### rowBGColorCalculation

The calculation dataprovider (such as servoy_row_bgcolor) used to add background
color and highlight selected or alternate portal rows.

NOTE: This property has been deprecated and is kept visible for legacy purposes. Use CSS Row Styling & onRender event instead.

**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### rowHeight

The height of each row in pixels. If 0 or not set, the height defaults to 10.

**Returns**\
[Number](../../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### scrollbars

Scrollbar options for the vertical and horizontal scrollbars. Each of the
vertical and horizontal scrollbars can be configured to display all the time,
to display only when needed or to never display.

**Returns**\
[Number](../../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### showHorizontalLines

When set, the portal displays horizontal lines between the rows.

NOTE:
In a multi-line portal, a horizontal line is only displayed
in the selected row; to display a horizontal line in all rows, add a
line to the portal.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### showVerticalLines

When set the portal displays vertical lines between the columns.

NOTE:
In a multi-line portal, a vertical line is only displayed
in the selected row; to display a vertical line in all rows, add
a line to the portal.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### size

The width and height (in pixels), separated by a comma.

**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### sortable

When set, users can sort the contents of the portal by clicking on the column headings.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### transparent

Flag that tells if the component is transparent or not.

The default value is "false", that is the components
are not transparent.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### visible

The visible property of the component, default true.

**Returns**\
[Boolean](../../JSLib/Boolean.md) visible property

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```

