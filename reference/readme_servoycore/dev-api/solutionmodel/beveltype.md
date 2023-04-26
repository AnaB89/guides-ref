# BEVELTYPE

## Constants Summary

| Type                          | Name                            | Summary                     |
| ----------------------------- | ------------------------------- | --------------------------- |
| [Number](../js-lib/number.md) | [LOWERED](beveltype.md#LOWERED) | Lowered bevel border type.. |
| [Number](../js-lib/number.md) | [RAISED](beveltype.md#RAISED)   | Raised bevel border type..  |

## Constants Details

### LOWERED

Lowered bevel border type.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createBevelBorder(SM_BEVELTYPE.LOWERED, '#ff0000', '#00ff00','#f0000f', '#0000ff');
```

### RAISED

Raised bevel border type.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createBevelBorder(SM_BEVELTYPE.RAISED, '#ff0000', '#00ff00','#f0000f', '#0000ff');
```
