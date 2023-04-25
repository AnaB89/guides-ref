#  Rectangle


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](../../JSLib/Number.md) | [anchors](Rectangle.md#anchors)                   | Enables a component to stick to a specific side of form and/or to  grow or shrink when a window is resized..                                    |
| [String](../../JSLib/String.md) | [background](Rectangle.md#background)                   | The background color of the component..                                    |
| [String](../../JSLib/String.md) | [borderType](Rectangle.md#borderType)                   | The type, color and style of border of the component..                                    |
| [CSSPosition](../../Application/CSSPosition.md) | [cssPosition](Rectangle.md#cssPosition)                   | Thecss position of the component..                                    |
| [Object](../../JSLib/Object.md) | [designTimeProperties](Rectangle.md#designTimeProperties)                   | Property to get and add design-time properties for a component..                                    |
| [Boolean](../../JSLib/Boolean.md) | [enabled](Rectangle.md#enabled)                   | The enable state of the component, default true..                                    |
| [String](../../JSLib/String.md) | [foreground](Rectangle.md#foreground)                   | The foreground color of the component..                                    |
| [Number](../../JSLib/Number.md) | [formIndex](Rectangle.md#formIndex)                   | Form index returns the z-index of the form element..                                    |
| [Number](../../JSLib/Number.md) | [lineSize](Rectangle.md#lineSize)                   | The width of the line used for drawing the rectangle..                                    |
| [String](../../JSLib/String.md) | [location](Rectangle.md#location)                   | The x and y position of the component, in pixels, separated by a comma..                                    |
| [String](../../JSLib/String.md) | [name](Rectangle.md#name)                   | The name of the component..                                    |
| [Number](../../JSLib/Number.md) | [roundedRadius](Rectangle.md#roundedRadius)                   | The rounding radius in pixels..                                    |
| [Number](../../JSLib/Number.md) | [shapeType](Rectangle.md#shapeType)                   | The type of the shape..                                    |
| [String](../../JSLib/String.md) | [size](Rectangle.md#size)                   | The width and height (in pixels), separated by a comma..                                    |
| [Boolean](../../JSLib/Boolean.md) | [transparent](Rectangle.md#transparent)                   | Flag that tells if the component is transparent or not..                                    |
| [Boolean](../../JSLib/Boolean.md) | [visible](Rectangle.md#visible)                   | The visible property of the component, default true..                                    |

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
### lineSize

The width of the line used for drawing the rectangle.

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
### roundedRadius

The rounding radius in pixels.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript

```
### shapeType

The type of the shape. The type can be BORDER_PANEL, RECTANGLE, ROUNDED_RECTANGLE or OVAL.

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

