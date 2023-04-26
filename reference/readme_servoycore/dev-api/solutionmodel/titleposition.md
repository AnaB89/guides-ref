# TITLEPOSITION

## Constants Summary

| Type                          | Name                                            | Summary                                          |
| ----------------------------- | ----------------------------------------------- | ------------------------------------------------ |
| [Number](../js-lib/number.md) | [ABOVE\_BOTTOM](titleposition.md#ABOVE\_BOTTOM) | Title in the middle of the border's bottom line. |
| [Number](../js-lib/number.md) | [ABOVE\_TOP](titleposition.md#ABOVE\_TOP)       | Title above the border's top line.               |
| [Number](../js-lib/number.md) | [BELOW\_BOTTOM](titleposition.md#BELOW\_BOTTOM) | Title below the border's bottom line.            |
| [Number](../js-lib/number.md) | [BELOW\_TOP](titleposition.md#BELOW\_TOP)       | Title above the border's bottom line.            |
| [Number](../js-lib/number.md) | [DEFAULT](titleposition.md#DEFAULT)             | Default vertical orientation for the title text. |
| [Number](../js-lib/number.md) | [TOP](titleposition.md#TOP)                     | Title in the middle of the border's top line.    |

## Constants Details

### ABOVE\_BOTTOM

Title in the middle of the border's bottom line

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.DEFAULT,SM_TITLEPOSITION.ABOVE_BOTTOM);
```

### ABOVE\_TOP

Title above the border's top line

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.DEFAULT,SM_TITLEPOSITION.ABOVE_TOP);
```

### BELOW\_BOTTOM

Title below the border's bottom line

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.DEFAULT,SM_TITLEPOSITION.BELOW_BOTTOM);
```

### BELOW\_TOP

Title above the border's bottom line

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.DEFAULT,SM_TITLEPOSITION.BELOW_TOP);
```

### DEFAULT

Default vertical orientation for the title text

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.DEFAULT,SM_TITLEPOSITION.DEFAULT_POSITION);
```

### TOP

Title in the middle of the border's top line

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createTitledBorder('Test',null,'#ff0000',SM_TITLEJUSTIFICATION.DEFAULT,SM_TITLEPOSITION.TOP);
```
