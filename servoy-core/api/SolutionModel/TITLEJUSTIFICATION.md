#  TITLEJUSTIFICATION


## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [CENTER](TITLEJUSTIFICATION.md#CENTER)                   | Position title text in the center of the border line..                                    |
| [Number](../JSLib/Number.md) | [DEFAULT](TITLEJUSTIFICATION.md#DEFAULT)                   | Default justification for the title text.                                    |
| [Number](../JSLib/Number.md) | [LEADING](TITLEJUSTIFICATION.md#LEADING)                   | Position title text at the left side of the border line  for left to right orientation, at the right side of the   border line for right to left orientation..                                    |
| [Number](../JSLib/Number.md) | [LEFT](TITLEJUSTIFICATION.md#LEFT)                   | Position title text at the left side of the border line..                                    |
| [Number](../JSLib/Number.md) | [RIGHT](TITLEJUSTIFICATION.md#RIGHT)                   | Position title text at the right side of the border line..                                    |
| [Number](../JSLib/Number.md) | [TRAILING](TITLEJUSTIFICATION.md#TRAILING)                   | Position title text at the right side of the border line  for left to right orientation, at the left side of the   border line for right to left orientation..                                    |

## Constants Details

### CENTER

Position title text in the center of the border line.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.CENTER,SM_TITLEPOSITION.TOP);
```
### DEFAULT

Default justification for the title text

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.DEFAULT,SM_TITLEPOSITION.TOP);
```
### LEADING

Position title text at the left side of the border line
 for left to right orientation, at the right side of the 
 border line for right to left orientation.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.LEADING,SM_TITLEPOSITION.TOP);
```
### LEFT

Position title text at the left side of the border line.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.LEFT,SM_TITLEPOSITION.TOP);
```
### RIGHT

Position title text at the right side of the border line.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.RIGHT,SM_TITLEPOSITION.TOP);
```
### TRAILING

Position title text at the right side of the border line
 for left to right orientation, at the left side of the 
 border line for right to left orientation.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.TRAILING,SM_TITLEPOSITION.TOP);
```

