# UNITS

## Constants Summary

| Type                          | Name                      | Summary                   |
| ----------------------------- | ------------------------- | ------------------------- |
| [Number](../js-lib/number.md) | [INCH](units.md#INCH)     | Inch length unit..        |
| [Number](../js-lib/number.md) | [MM](units.md#MM)         | Millimeters length unit.. |
| [Number](../js-lib/number.md) | [PIXELS](units.md#PIXELS) | Pixels length unit..      |

## Constants Details

### INCH

Inch length unit.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.defaultPageFormat = solutionModel.createPageFormat(8.5,11,1,1,1,1,SM_ORIENTATION.PORTRAIT,SM_UNITS.INCH);
```

### MM

Millimeters length unit.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.defaultPageFormat = solutionModel.createPageFormat(215,279,25,25,25,25,SM_ORIENTATION.PORTRAIT,SM_UNITS.MM);
```

### PIXELS

Pixels length unit.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.defaultPageFormat = solutionModel.createPageFormat(612,792,72,72,72,72,SM_ORIENTATION.PORTRAIT,SM_UNITS.PIXELS);
```
