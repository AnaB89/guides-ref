# SCROLLBAR

## Constants Summary

| Type                          | Name                                                                                | Summary                                                                                                            |
| ----------------------------- | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| [Number](../js-lib/number.md) | [HORIZONTAL\_SCROLLBAR\_ALWAYS](scrollbar.md#HORIZONTAL\_SCROLLBAR\_ALWAYS)         | Used to set the horizontal scroll bar policy so that horizontal scrollbars are always displayed..                  |
| [Number](../js-lib/number.md) | [HORIZONTAL\_SCROLLBAR\_AS\_NEEDED](scrollbar.md#HORIZONTAL\_SCROLLBAR\_AS\_NEEDED) | Used to set the horizontal scroll bar policy so that horizontal scrollbars are displayed only when needed..        |
| [Number](../js-lib/number.md) | [HORIZONTAL\_SCROLLBAR\_NEVER](scrollbar.md#HORIZONTAL\_SCROLLBAR\_NEVER)           | Used to set the horizontal scroll bar policy so that horizontal scrollbars are never displayed..                   |
| [Number](../js-lib/number.md) | [SCROLLBARS\_WHEN\_NEEDED](scrollbar.md#SCROLLBARS\_WHEN\_NEEDED)                   | Used to set the horizontal and vertical scroll bar policy so that both scrollbars are displayed only when needed.. |
| [Number](../js-lib/number.md) | [VERTICAL\_SCROLLBAR\_ALWAYS](scrollbar.md#VERTICAL\_SCROLLBAR\_ALWAYS)             | Used to set the vertical scroll bar policy so that vertical scrollbars are always displayed..                      |
| [Number](../js-lib/number.md) | [VERTICAL\_SCROLLBAR\_AS\_NEEDED](scrollbar.md#VERTICAL\_SCROLLBAR\_AS\_NEEDED)     | Used to set the vertical scroll bar policy so that vertical scrollbars are displayed only when needed..            |
| [Number](../js-lib/number.md) | [VERTICAL\_SCROLLBAR\_NEVER](scrollbar.md#VERTICAL\_SCROLLBAR\_NEVER)               | Used to set the vertical scroll bar policy so that vertical scrollbars are never displayed..                       |

## Constants Details

### HORIZONTAL\_SCROLLBAR\_ALWAYS

Used to set the horizontal scroll bar policy so that horizontal scrollbars are always displayed.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var alwaysScrollbars = form.newField('my_table_text', JSField.TEXT_AREA, 230, 10, 100, 100);
alwaysScrollbars.scrollbars = SM_SCROLLBAR.HORIZONTAL_SCROLLBAR_ALWAYS | SM_SCROLLBAR.VERTICAL_SCROLLBAR_ALWAYS;
```

### HORIZONTAL\_SCROLLBAR\_AS\_NEEDED

Used to set the horizontal scroll bar policy so that horizontal scrollbars are displayed only when needed.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var neededScrollbars = form.newField('my_table_text', JSField.TEXT_AREA, 120, 10, 100, 100);
neededScrollbars.scrollbars = SM_SCROLLBAR.HORIZONTAL_SCROLLBAR_AS_NEEDED | SM_SCROLLBAR.VERTICAL_SCROLLBAR_AS_NEEDED;
```

### HORIZONTAL\_SCROLLBAR\_NEVER

Used to set the horizontal scroll bar policy so that horizontal scrollbars are never displayed.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var noScrollbars = form.newField('my_table_text', JSField.TEXT_AREA, 10, 10, 100, 100);
noScrollbars.scrollbars = SM_SCROLLBAR.HORIZONTAL_SCROLLBAR_NEVER | SM_SCROLLBAR.VERTICAL_SCROLLBAR_NEVER;
```

### SCROLLBARS\_WHEN\_NEEDED

Used to set the horizontal and vertical scroll bar policy so that both scrollbars are displayed only when needed.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var neededScrollbars = form.newField('my_table_text', JSField.TEXT_AREA, 120, 10, 100, 100);
// This is the default option, but if you really want you can set it explicitly.
neededScrollbars.scrollbars = SM_SCROLLBAR.SCROLLBARS_WHEN_NEEDED;
```

### VERTICAL\_SCROLLBAR\_ALWAYS

Used to set the vertical scroll bar policy so that vertical scrollbars are always displayed.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var alwaysScrollbars = form.newField('my_table_text', JSField.TEXT_AREA, 230, 10, 100, 100);
alwaysScrollbars.scrollbars = SM_SCROLLBAR.HORIZONTAL_SCROLLBAR_ALWAYS | SM_SCROLLBAR.VERTICAL_SCROLLBAR_ALWAYS;
```

### VERTICAL\_SCROLLBAR\_AS\_NEEDED

Used to set the vertical scroll bar policy so that vertical scrollbars are displayed only when needed.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var neededScrollbars = form.newField('my_table_text', JSField.TEXT_AREA, 120, 10, 100, 100);
neededScrollbars.scrollbars = SM_SCROLLBAR.HORIZONTAL_SCROLLBAR_AS_NEEDED | SM_SCROLLBAR.VERTICAL_SCROLLBAR_AS_NEEDED;
```

### VERTICAL\_SCROLLBAR\_NEVER

Used to set the vertical scroll bar policy so that vertical scrollbars are never displayed.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var noScrollbars = form.newField('my_table_text', JSField.TEXT_AREA, 10, 10, 100, 100);
noScrollbars.scrollbars = SM_SCROLLBAR.HORIZONTAL_SCROLLBAR_NEVER | SM_SCROLLBAR.VERTICAL_SCROLLBAR_NEVER;
```
