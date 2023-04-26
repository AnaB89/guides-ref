# FONTSTYLE

## Constants Summary

| Type                          | Name                                      | Summary                      |
| ----------------------------- | ----------------------------------------- | ---------------------------- |
| [Number](../js-lib/number.md) | [BOLD](fontstyle.md#BOLD)                 | Bold font style..            |
| [Number](../js-lib/number.md) | [BOLD\_ITALIC](fontstyle.md#BOLD\_ITALIC) | Bold and italic font style.. |
| [Number](../js-lib/number.md) | [ITALIC](fontstyle.md#ITALIC)             | Italic font style..          |
| [Number](../js-lib/number.md) | [PLAIN](fontstyle.md#PLAIN)               | Plain(normal) font style..   |

## Constants Details

### BOLD

Bold font style.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
var component = form.getComponent("someComponent")
component.fontType = solutionModel.createFont('Arial',SM_FONTSTYLE.BOLD,12);
```

### BOLD\_ITALIC

Bold and italic font style.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
var component = form.getComponent("someComponent")
component.fontType = solutionModel.createFont('Arial',SM_FONTSTYLE.BOLD_ITALIC,20);
```

### ITALIC

Italic font style.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
var component = form.getComponent("someComponent")
component.fontType = solutionModel.createFont('Arial',SM_FONTSTYLE.ITALIC,14);
```

### PLAIN

Plain(normal) font style.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
var component = form.getComponent("someComponent")
component.fontType = solutionModel.createFont('Arial',SM_FONTSTYLE.PLAIN,10);
```
