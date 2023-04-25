Welcome to the svycanvas wiki!

This wiki provides comprehensive documentation for using the **svycanvas** web-component, which allows you to create and display an interactive canvas within Servoy's NGClient.

# Getting Started
First import the component using one of the release [binaries](https://github.com/Servoy/svycanvas/releases) or via Servoy's Web Package Manager.

If you would like to see the component in an example install the included solution [svyCanvasExample.servoy](https://github.com/Servoy/svycanvas/releases).

# Example Usage
First add the component to a form by dragging it into the form using the Palette Wizard.  It should be under Canvas (Canvas).

# API Documentation 

## Event Handlers
### onClick
Returns the item ID and object selected.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
String| id | ID of selected object if it has one. | Optional
Object| object | returns object selected.  | Required

### onLongPress
Returns the item ID and object selected.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
String| id | ID of selected object if it has one. | Optional
Object| object | returns object selected.  | Required

### onModified
When canvas is modified execute this handler.

### onReady
Fires when canvas has completed initial rendering

## API Methods

### addObject
Add an object to canvas

### copySelectedObject
Copies selected object on canvas

### updateObject
Update an object

### removeObject
Remove an object

### clearCanvas
Clear the canvas

### startAnimate
Start animations

### stopAnimate
Stop animations

### getSelectedObject
Return selected object

### setSelectedObject
Select an object on the canvas

### saveCanvas
Return current canvas as JSON String

### loadCanvas
Draw a canvas using JSON String

### saveAsImage
Return current canvas as an Image

### bringToFront
Bring selected element to top of canvas

### rotate
Rotate the entire canvas and it's objects

### ZoomOnPoint
Zoom on a particular point.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Number| x | X coordinate | Required
Number| y | Y coordinate | Required
Number| zoomLevel | How far to zoom (0+)  | Required

## Component Properties

Type | Name | Summary | Required
--- |--- | --- | ---
Array<canvasObjects> | canvasObjects | An array of canvas objects to be display | Optional
Object | canvasOptions | Options for the canvas | Optional
Number | gridSize | The grid size to use | Required if you are showing the grid.
String | showGrid | Whether or not to show a grid on the canvas. | Optional
String | snapToGrid | Whether or not to try and snap objects to a grid.  | Optional

## canvasOptions 
Type | Name | Summary | Required
--- |--- | --- | ---
Boolean | selectable | Allow objects to be selected | optional
Boolean | skipTargetFind | disable selection of all objects | optional
Boolean | hasRotatingPoint | disable rotation for objects | optional
Boolean | renderOnAddRemove | Performance setting | optional
Boolean | skipOffscreen | Hide drawing elements off-screen | optional
Boolean | animationSpeed | Speed to run animations | optional

## canvasObject 
Type | Name | Summary | Required
--- |--- | --- | ---
String | objectType | Type of object (Circle,Rectangle,Triangle,Image,Text,Group) | required
array<Objects> | objects | An array of objects, used if objectType is 'Group | optional
Color | fill | Color fill (default none) | optional
String | opacity | Opacity of object (default 1.0) | optional
Number | width | Width of object (default 0) | optional
Number | height | Height of object (default 0) | optional
Number | radius | Radius of object (default 0) | optional
Number | left | Left position of object from x-axis | optional
Number | top | Top position of object from y-axis | optional
Number | rx | rx position of object from x-axis | optional
Number | ry | ry position of object from y-axis | optional
Color | stroke | Stroke color of an object | optional
String | id | Identifier for object ( if not filled the object cannot be used with handler events) | optional
Number | scaleX | Scale of object for width (default 1.0) | optional
Number | scaleY | Scale of object for height (default 1.0) | optional
String | text | Text of object, only applies if objectType is 'Text' | optional
String | textAlign | Alignment of text object, only applies if objectType is 'Text' (default left) | optional
String | fontSize | Font size of text, only applies if objectType is 'Text' | optional
String | fontFamily | Font family, only applies if objectType is 'Text' | optional
Number | angle | Angle of object | optional
String | mediaName | Use an image or media with object, only applies if objectType is 'Image'| optional
String | spriteName | Use an sprite with object, only applies if objectType is 'Image'| optional
Number | spriteWidth | Sprite width, only applies if objectType is 'Image'| optional
Number | spriteHeight | Sprite height, only applies if objectType is 'Image'| optional
Number | spriteIndex | Sprite index, only applies if objectType is 'Image'| optional
Number | frameTime | Sprite frametime, only applies if objectType is 'Image'| optional
Boolean | selectable | Allows an element to be selected and manipulated (default true) | optional
Boolean | custom_data | Add additional data to an object  | optional

