#  TITLEPOSITION


## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [ABOVE_BOTTOM](TITLEPOSITION.md#ABOVE_BOTTOM)                   | Title in the middle of the border's bottom line.                                    |
| [Number](../JSLib/Number.md) | [ABOVE_TOP](TITLEPOSITION.md#ABOVE_TOP)                   | Title above the border's top line.                                    |
| [Number](../JSLib/Number.md) | [BELOW_BOTTOM](TITLEPOSITION.md#BELOW_BOTTOM)                   | Title below the border's bottom line.                                    |
| [Number](../JSLib/Number.md) | [BELOW_TOP](TITLEPOSITION.md#BELOW_TOP)                   | Title above the border's bottom line.                                    |
| [Number](../JSLib/Number.md) | [DEFAULT](TITLEPOSITION.md#DEFAULT)                   | Default vertical orientation for the title text.                                    |
| [Number](../JSLib/Number.md) | [TOP](TITLEPOSITION.md#TOP)                   | Title in the middle of the border's top line.                                    |

## Constants Details

### ABOVE_BOTTOM

Title in the middle of the border's bottom line

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.DEFAULT,SM_TITLEPOSITION.ABOVE_BOTTOM);
```
### ABOVE_TOP

Title above the border's top line

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.DEFAULT,SM_TITLEPOSITION.ABOVE_TOP);
```
### BELOW_BOTTOM

Title below the border's bottom line

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.DEFAULT,SM_TITLEPOSITION.BELOW_BOTTOM);
```
### BELOW_TOP

Title above the border's bottom line

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.DEFAULT,SM_TITLEPOSITION.BELOW_TOP);
```
### DEFAULT

Default vertical orientation for the title text

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.DEFAULT,SM_TITLEPOSITION.DEFAULT_POSITION);
```
### TOP

Title in the middle of the border's top line

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.DEFAULT,SM_TITLEPOSITION.TOP);
```

