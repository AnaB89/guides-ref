#  PRINTSLIDING

## **Supported Clients**

    SmartClient
    WebClient

## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [ALLOW_MOVE_X](PRINTSLIDING.md#ALLOW_MOVE_X)                   | Constant to be used when specifiying the print sliding for components..                                    |
| [Number](../JSLib/Number.md) | [ALLOW_MOVE_Y](PRINTSLIDING.md#ALLOW_MOVE_Y)                   | Constant to be used when specifiying the print sliding for components..                                    |
| [Number](../JSLib/Number.md) | [GROW_HEIGHT](PRINTSLIDING.md#GROW_HEIGHT)                   | Constant to be used when specifiying the print sliding for components..                                    |
| [Number](../JSLib/Number.md) | [GROW_WIDTH](PRINTSLIDING.md#GROW_WIDTH)                   | Constant to be used when specifiying the print sliding for components..                                    |
| [Number](../JSLib/Number.md) | [NO_SLIDING](PRINTSLIDING.md#NO_SLIDING)                   | Constant to be used when specifiying the print sliding for components..                                    |
| [Number](../JSLib/Number.md) | [SHRINK_HEIGHT](PRINTSLIDING.md#SHRINK_HEIGHT)                   | Constant to be used when specifiying the print sliding for components..                                    |
| [Number](../JSLib/Number.md) | [SHRINK_WIDTH](PRINTSLIDING.md#SHRINK_WIDTH)                   | Constant to be used when specifiying the print sliding for components..                                    |

## Constants Details

### ALLOW_MOVE_X

Constant to be used when specifiying the print sliding for components.
The component will move horizontally to align with its left neighbor,
if that left neighbor moves or increases/decreases its size.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
var form = solutionModel.newForm('printForm', 'db:/example_data/parent_table', null, false, 400, 300);
var growHorizLabel = form.newLabel('Grow horizontal -- long text', 10, 30, 30, 20);
growHorizLabel.printSliding = SM_PRINT_SLIDING.GROW_WIDTH;
growHorizLabel.background = 'blue';
var moveHorizRightLabel = form.newLabel('Move horizontal right', 50, 30, 100, 20);
moveHorizRightLabel.printSliding = SM_PRINT_SLIDING.ALLOW_MOVE_X;
moveHorizRightLabel.background = 'pink';
var shrinkHorizLabel = form.newLabel('Short', 10, 50, 100, 20);
shrinkHorizLabel.printSliding = SM_PRINT_SLIDING.SHRINK_WIDTH;
shrinkHorizLabel.background = 'green';
var moveHorizLeftLabel = form.newLabel('Move horizontal left', 100, 50, 150, 20);
moveHorizLeftLabel.printSliding = SM_PRINT_SLIDING.ALLOW_MOVE_X;
moveHorizLeftLabel.background = 'magenta';
forms['printForm'].controller.showPrintPreview();
```
### ALLOW_MOVE_Y

Constant to be used when specifiying the print sliding for components.
The component will move vertically to align with its top neighbor,
if that neighbor moves or increases/decreases its size.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
var form = solutionModel.newForm('printForm', 'db:/example_data/parent_table', null, false, 400, 300);
var growVertLabel = form.newLabel('Grow vertical', 10, 70, 100, 5);
growVertLabel.printSliding = SM_PRINT_SLIDING.GROW_HEIGHT;
growVertLabel.background = 'orange';
var moveVertDownLabel = form.newLabel('Move vertical down', 10, 75, 100, 20);
moveVertDownLabel.printSliding = SM_PRINT_SLIDING.ALLOW_MOVE_Y;
moveVertDownLabel.background = 'cyan';
var shrinkVertLabel = form.newLabel('Shrink vertical', 10, 110, 100, 40);
shrinkVertLabel.printSliding = SM_PRINT_SLIDING.SHRINK_HEIGHT;
shrinkVertLabel.background = 'yellow';
var moveVertUpLabel = form.newLabel('Move vertical up', 10, 160, 100, 20);
moveVertUpLabel.printSliding = SM_PRINT_SLIDING.ALLOW_MOVE_Y;
moveVertUpLabel.background = 'purple';
forms['printForm'].controller.showPrintPreview();
```
### GROW_HEIGHT

Constant to be used when specifiying the print sliding for components.
The component will increase its height to adapt its content, if
the content is too large.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
var form = solutionModel.newForm('printForm', 'db:/example_data/parent_table', null, false, 400, 300);
var growVertLabel = form.newLabel('Grow vertical', 10, 70, 100, 5);
growVertLabel.printSliding = SM_PRINT_SLIDING.GROW_HEIGHT;
growVertLabel.background = 'orange';
forms['printForm'].controller.showPrintPreview();
```
### GROW_WIDTH

Constant to be used when specifiying the print sliding for components.
The component will increase its width to adapt its content, if the 
content is too large.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
var form = solutionModel.newForm('printForm', 'db:/example_data/parent_table', null, false, 400, 300);
var growHorizLabel = form.newLabel('Grow horizontal -- long text', 10, 30, 30, 20);
growHorizLabel.printSliding = SM_PRINT_SLIDING.GROW_WIDTH;
growHorizLabel.background = 'blue';
forms['printForm'].controller.showPrintPreview();
```
### NO_SLIDING

Constant to be used when specifiying the print sliding for components.
Makes the component not slide during printing. The component will
maintain its designtime location and size.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
var form = solutionModel.newForm('printForm', 'db:/example_data/parent_table', null, false, 400, 300);
var noSlidingLabel = form.newLabel('No sliding -- long text', 10, 10, 30, 20);
noSlidingLabel.printSliding = SM_PRINT_SLIDING.NO_SLIDING;
noSlidingLabel.background = 'red';
forms['printForm'].controller.showPrintPreview();
```
### SHRINK_HEIGHT

Constant to be used when specifiying the print sliding for components.
The component will decrease its height to adapt its content, if
the content is too small.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
var form = solutionModel.newForm('printForm', 'db:/example_data/parent_table', null, false, 400, 300);
var shrinkVertLabel = form.newLabel('Shrink vertical', 10, 110, 100, 40);
shrinkVertLabel.printSliding = SM_PRINT_SLIDING.SHRINK_HEIGHT;
shrinkVertLabel.background = 'yellow';
forms['printForm'].controller.showPrintPreview();
```
### SHRINK_WIDTH

Constant to be used when specifiying the print sliding for components.
The component will decrease its width to adapt its content, if the
content is too small.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
var form = solutionModel.newForm('printForm', 'db:/example_data/parent_table', null, false, 400, 300);
var shrinkHorizLabel = form.newLabel('Short', 10, 50, 100, 20);
shrinkHorizLabel.printSliding = SM_PRINT_SLIDING.SHRINK_WIDTH;
shrinkHorizLabel.background = 'green';
forms['printForm'].controller.showPrintPreview();
```

