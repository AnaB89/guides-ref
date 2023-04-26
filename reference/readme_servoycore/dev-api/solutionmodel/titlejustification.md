# TITLEJUSTIFICATION

## Constants Summary

| Type                          | Name                                       | Summary                                                                                                                                                     |
| ----------------------------- | ------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Number](../js-lib/number.md) | [CENTER](titlejustification.md#CENTER)     | Position title text in the center of the border line..                                                                                                      |
| [Number](../js-lib/number.md) | [DEFAULT](titlejustification.md#DEFAULT)   | Default justification for the title text.                                                                                                                   |
| [Number](../js-lib/number.md) | [LEADING](titlejustification.md#LEADING)   | Position title text at the left side of the border line for left to right orientation, at the right side of the border line for right to left orientation.. |
| [Number](../js-lib/number.md) | [LEFT](titlejustification.md#LEFT)         | Position title text at the left side of the border line..                                                                                                   |
| [Number](../js-lib/number.md) | [RIGHT](titlejustification.md#RIGHT)       | Position title text at the right side of the border line..                                                                                                  |
| [Number](../js-lib/number.md) | [TRAILING](titlejustification.md#TRAILING) | Position title text at the right side of the border line for left to right orientation, at the left side of the border line for right to left orientation.. |

## Constants Details

### CENTER

Position title text in the center of the border line.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.CENTER,SM_TITLEPOSITION.TOP);
```

### DEFAULT

Default justification for the title text

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.DEFAULT,SM_TITLEPOSITION.TOP);
```

### LEADING

Position title text at the left side of the border line for left to right orientation, at the right side of the border line for right to left orientation.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.LEADING,SM_TITLEPOSITION.TOP);
```

### LEFT

Position title text at the left side of the border line.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.LEFT,SM_TITLEPOSITION.TOP);
```

### RIGHT

Position title text at the right side of the border line.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.RIGHT,SM_TITLEPOSITION.TOP);
```

### TRAILING

Position title text at the right side of the border line for left to right orientation, at the left side of the border line for right to left orientation.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.TRAILING,SM_TITLEPOSITION.TOP);
```
