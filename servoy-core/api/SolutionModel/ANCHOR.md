#  ANCHOR


## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [ALL](ANCHOR.md#ALL)                   | Constant to be used when specifying anchoring for components..                                    |
| [Number](../JSLib/Number.md) | [DEFAULT](ANCHOR.md#DEFAULT)                   | Constant to be used when specifying anchoring for components..                                    |
| [Number](../JSLib/Number.md) | [EAST](ANCHOR.md#EAST)                   | Constant to be used when specifying anchoring for components..                                    |
| [Number](../JSLib/Number.md) | [NORTH](ANCHOR.md#NORTH)                   | Constant to be used when specifying anchoring for components..                                    |
| [Number](../JSLib/Number.md) | [SOUTH](ANCHOR.md#SOUTH)                   | Constant to be used when specifying anchoring for components..                                    |
| [Number](../JSLib/Number.md) | [WEST](ANCHOR.md#WEST)                   | Constant to be used when specifying anchoring for components..                                    |

## Constants Details

### ALL

Constant to be used when specifying anchoring for components.
Makes the component anchored on all sides. This means that
the component will keep a constant distance from all sides
of the window and will grow/shrink as the window is resized.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.newForm('mediaForm', 'db:/example_data/parent_table', null, false, 400, 300);
var strechAllDirectionsLabel = form.newLabel('Strech all directions', 10, 10, 380, 280);
strechAllDirectionsLabel.background = 'red';
strechAllDirectionsLabel.anchors = SM_ANCHOR.ALL;
```
### DEFAULT

Constant to be used when specifying anchoring for components.
It is equivalent to a combination of NORTH and WEST anchoring.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.newForm('mediaForm', 'db:/example_data/parent_table', null, false, 400, 300);
var stickToTopLeftCornerLabel = form.newLabel('Stick to top-left corner', 10, 10, 200, 100);
stickToTopLeftCornerLabel.background = 'orange';
stickToTopLeftCornerLabel.anchors = SM_ANCHOR.DEFAULT;
```
### EAST

Constant to be used when specifying anchoring for components.
Makes the component anchored to the right side of the window,
which means that the component will keep a constant distance
from the right side of the window. If WEST anchoring is also 
enabled, then the component will grow/shrink as the window 
is horizontally resized.

This constant is used also for setting tab orientation on tab panels.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.newForm('mediaForm', 'db:/example_data/parent_table', null, false, 400, 300);
var strechHorizontallyLabel = form.newLabel('Strech horizontally', 10, 10, 380, 140);
strechHorizontallyLabel.background = 'blue';
strechHorizontallyLabel.anchors = SM_ANCHOR.NORTH | SM_ANCHOR.WEST | SM_ANCHOR.EAST;
var stickToBottomRightCornerLabel = form.newLabel('Stick to bottom-right corner', 190, 190, 200, 100);
stickToBottomRightCornerLabel.background = 'pink';
stickToBottomRightCornerLabel.anchors = SM_ANCHOR.SOUTH | SM_ANCHOR.EAST;
```
### NORTH

Constant to be used when specifying anchoring for components.
Makes the component anchored to the top side of the window,
which means that the component will keep a constant distance
from the top side of the window. If SOUTH anchoring is also 
enabled, then the component will grow/shrink as the window 
is vertically resized.

This constant is used also for setting tab orientation on tab panels.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.newForm('mediaForm', 'db:/example_data/parent_table', null, false, 400, 300);
var strechVerticallyLabel = form.newLabel('Strech vertically', 10, 10, 190, 280);
strechVerticallyLabel.background = 'green';
strechVerticallyLabel.anchors = SM_ANCHOR.WEST | SM_ANCHOR.NORTH | SM_ANCHOR.SOUTH;
var stickToTopLeftCornerLabel = form.newLabel('Stick to top-left corner', 10, 10, 200, 100);
stickToTopLeftCornerLabel.background = 'orange';
stickToTopLeftCornerLabel.anchors = SM_ANCHOR.NORTH | SM_ANCHOR.WEST;
```
### SOUTH

Constant to be used when specifying anchoring for components.
Makes the component anchored to the bottom side of the window,
which means that the component will keep a constant distance
from the bottom side of the window. If NORTH anchoring is also 
enabled, then the component will grow/shrink as the window 
is vertically resized.

This constant is used also for setting tab orientation on tab panels.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.newForm('mediaForm', 'db:/example_data/parent_table', null, false, 400, 300);
var strechVerticallyLabel = form.newLabel('Strech vertically', 10, 10, 190, 280);
strechVerticallyLabel.background = 'green';
strechVerticallyLabel.anchors = SM_ANCHOR.WEST | SM_ANCHOR.NORTH | SM_ANCHOR.SOUTH;
var stickToBottomRightCornerLabel = form.newLabel('Stick to bottom-right corner', 190, 190, 200, 100);
stickToBottomRightCornerLabel.background = 'pink';
stickToBottomRightCornerLabel.anchors = SM_ANCHOR.SOUTH | SM_ANCHOR.EAST;
```
### WEST

Constant to be used when specifying anchoring for components.
Makes the component anchored to the left side of the window,
which means that the component will keep a constant distance
from the left side of the window. If EAST anchoring is also 
enabled, then the component will grow/shrink as the window 
is vertically resized.

This constant is used also for setting tab orientation on tab panels.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.newForm('mediaForm', 'db:/example_data/parent_table', null, false, 400, 300);
var strechHorizontallyLabel = form.newLabel('Strech horizontally', 10, 10, 380, 140);
strechHorizontallyLabel.background = 'blue';
strechHorizontallyLabel.anchors = SM_ANCHOR.NORTH | SM_ANCHOR.WEST | SM_ANCHOR.EAST;
var stickToTopLeftCornerLabel = form.newLabel('Stick to top-left corner', 10, 10, 200, 100);
stickToTopLeftCornerLabel.background = 'orange';
stickToTopLeftCornerLabel.anchors = SM_ANCHOR.NORTH | SM_ANCHOR.WEST;
```

