#  SCROLLBAR

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [HORIZONTAL_SCROLLBAR_ALWAYS](SCROLLBAR.md#HORIZONTAL_SCROLLBAR_ALWAYS)                   | Used to set the horizontal scroll bar policy so that horizontal scrollbars are always displayed..                                    |
| [Number](../JSLib/Number.md) | [HORIZONTAL_SCROLLBAR_AS_NEEDED](SCROLLBAR.md#HORIZONTAL_SCROLLBAR_AS_NEEDED)                   | Used to set the horizontal scroll bar policy so that horizontal scrollbars are displayed only when needed..                                    |
| [Number](../JSLib/Number.md) | [HORIZONTAL_SCROLLBAR_NEVER](SCROLLBAR.md#HORIZONTAL_SCROLLBAR_NEVER)                   | Used to set the horizontal scroll bar policy so that horizontal scrollbars are never displayed..                                    |
| [Number](../JSLib/Number.md) | [SCROLLBARS_WHEN_NEEDED](SCROLLBAR.md#SCROLLBARS_WHEN_NEEDED)                   | Used to set the horizontal and vertical scroll bar policy so that both scrollbars are displayed only when needed..                                    |
| [Number](../JSLib/Number.md) | [VERTICAL_SCROLLBAR_ALWAYS](SCROLLBAR.md#VERTICAL_SCROLLBAR_ALWAYS)                   | Used to set the vertical scroll bar policy so that vertical scrollbars are always displayed..                                    |
| [Number](../JSLib/Number.md) | [VERTICAL_SCROLLBAR_AS_NEEDED](SCROLLBAR.md#VERTICAL_SCROLLBAR_AS_NEEDED)                   | Used to set the vertical scroll bar policy so that vertical scrollbars are displayed only when needed..                                    |
| [Number](../JSLib/Number.md) | [VERTICAL_SCROLLBAR_NEVER](SCROLLBAR.md#VERTICAL_SCROLLBAR_NEVER)                   | Used to set the vertical scroll bar policy so that vertical scrollbars are never displayed..                                    |

## Constants Details

### HORIZONTAL_SCROLLBAR_ALWAYS

Used to set the horizontal scroll bar policy so that horizontal scrollbars are always displayed.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var alwaysScrollbars = form.newField('my_table_text', JSField.TEXT_AREA, 230, 10, 100, 100);
alwaysScrollbars.scrollbars = SM_SCROLLBAR.HORIZONTAL_SCROLLBAR_ALWAYS | SM_SCROLLBAR.VERTICAL_SCROLLBAR_ALWAYS;
```
### HORIZONTAL_SCROLLBAR_AS_NEEDED

Used to set the horizontal scroll bar policy so that horizontal scrollbars are displayed only when needed.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var neededScrollbars = form.newField('my_table_text', JSField.TEXT_AREA, 120, 10, 100, 100);
neededScrollbars.scrollbars = SM_SCROLLBAR.HORIZONTAL_SCROLLBAR_AS_NEEDED | SM_SCROLLBAR.VERTICAL_SCROLLBAR_AS_NEEDED;
```
### HORIZONTAL_SCROLLBAR_NEVER

Used to set the horizontal scroll bar policy so that horizontal scrollbars are never displayed.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var noScrollbars = form.newField('my_table_text', JSField.TEXT_AREA, 10, 10, 100, 100);
noScrollbars.scrollbars = SM_SCROLLBAR.HORIZONTAL_SCROLLBAR_NEVER | SM_SCROLLBAR.VERTICAL_SCROLLBAR_NEVER;
```
### SCROLLBARS_WHEN_NEEDED

Used to set the horizontal and vertical scroll bar policy so that both scrollbars are displayed
only when needed.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var neededScrollbars = form.newField('my_table_text', JSField.TEXT_AREA, 120, 10, 100, 100);
// This is the default option, but if you really want you can set it explicitly.
neededScrollbars.scrollbars = SM_SCROLLBAR.SCROLLBARS_WHEN_NEEDED;
```
### VERTICAL_SCROLLBAR_ALWAYS

Used to set the vertical scroll bar policy so that vertical scrollbars are always displayed.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var alwaysScrollbars = form.newField('my_table_text', JSField.TEXT_AREA, 230, 10, 100, 100);
alwaysScrollbars.scrollbars = SM_SCROLLBAR.HORIZONTAL_SCROLLBAR_ALWAYS | SM_SCROLLBAR.VERTICAL_SCROLLBAR_ALWAYS;
```
### VERTICAL_SCROLLBAR_AS_NEEDED

Used to set the vertical scroll bar policy so that vertical scrollbars are displayed only when needed.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var neededScrollbars = form.newField('my_table_text', JSField.TEXT_AREA, 120, 10, 100, 100);
neededScrollbars.scrollbars = SM_SCROLLBAR.HORIZONTAL_SCROLLBAR_AS_NEEDED | SM_SCROLLBAR.VERTICAL_SCROLLBAR_AS_NEEDED;
```
### VERTICAL_SCROLLBAR_NEVER

Used to set the vertical scroll bar policy so that vertical scrollbars are never displayed.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var noScrollbars = form.newField('my_table_text', JSField.TEXT_AREA, 10, 10, 100, 100);
noScrollbars.scrollbars = SM_SCROLLBAR.HORIZONTAL_SCROLLBAR_NEVER | SM_SCROLLBAR.VERTICAL_SCROLLBAR_NEVER;
```

