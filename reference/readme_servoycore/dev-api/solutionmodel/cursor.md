# CURSOR

## Constants Summary

| Type                          | Name                                         | Summary                                                         |
| ----------------------------- | -------------------------------------------- | --------------------------------------------------------------- |
| [Number](../js-lib/number.md) | [DEFAULT\_CURSOR](cursor.md#DEFAULT\_CURSOR) | Constant used for setting the roll over cursor for components.. |
| [Number](../js-lib/number.md) | [HAND\_CURSOR](cursor.md#HAND\_CURSOR)       | Constant used for setting the roll over cursor for components.. |

## Constants Details

### DEFAULT\_CURSOR

Constant used for setting the roll over cursor for components. Use this for setting the roll over cursor to the default (dependent on the OS and the L\&F).

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var label = form.newLabel('Move the mouse over me', 10, 10, 200, 200);
label.rolloverCursor = SM_CURSOR.DEFAULT_CURSOR;
```

### HAND\_CURSOR

Constant used for setting the roll over cursor for components. Use this for setting the roll over cursor to a hand.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var label = form.newLabel('Move the mouse over me', 10, 10, 200, 200);
label.rolloverCursor = SM_CURSOR.HAND_CURSOR;
```
