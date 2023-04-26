# DEFAULTS

## Constants Summary

| Type                          | Name                                             | Summary                                                                                           |
| ----------------------------- | ------------------------------------------------ | ------------------------------------------------------------------------------------------------- |
| [JSMethod](jsmethod.md)       | [COMMAND\_DEFAULT](defaults.md#COMMAND\_DEFAULT) | Constants used for setting commands to "default"..                                                |
| [JSMethod](jsmethod.md)       | [COMMAND\_NONE](defaults.md#COMMAND\_NONE)       | Constant used for setting commands to "none"..                                                    |
| [Number](../js-lib/number.md) | [DEFAULT](defaults.md#DEFAULT)                   | Constant used in various places to set properties to their default value..                        |
| [Number](../js-lib/number.md) | [IGNORE](defaults.md#IGNORE)                     | Constant used to remove a component from the tab sequence or set form navigator to IGNORE value.. |
| [Number](../js-lib/number.md) | [NONE](defaults.md#NONE)                         | Constant used in various places to set properties to "none"..                                     |

## Constants Details

### COMMAND\_DEFAULT

Constants used for setting commands to "default".

**Returns**\
[JSMethod](jsmethod.md)

**Sample**

```javascript
var form = solutionModel.newForm('parentForm', 'db:/example_data/parent_table', null, false, 1200, 800);
form.onFindCmd = SM_DEFAULTS.COMMAND_DEFAULT; // This makes the find work like it does by default.
```

### COMMAND\_NONE

Constant used for setting commands to "none".

**Returns**\
[JSMethod](jsmethod.md)

**Sample**

```javascript
var form = solutionModel.newForm('parentForm', 'db:/example_data/parent_table', null, false, 1200, 800);
form.onFindCmd = SM_DEFAULTS.COMMAND_NONE; // This disables the find on the form.
```

### DEFAULT

Constant used in various places to set properties to their default value.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.newForm('parentForm', 'db:/example_data/parent_table', null, false, 1200, 800);
form.navigator = SM_DEFAULTS.DEFAULT; // Show the default navigator on the form.
```

### IGNORE

Constant used to remove a component from the tab sequence or set form navigator to IGNORE value.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
// Create three fields. Based on how they are placed, by default they will come one
// after another in the tab sequence.
var fieldOne = form.newField('parent_table_id', JSField.TEXT_FIELD, 10, 10, 100, 20);
var fieldTwo = form.newField('parent_table_text', JSField.TEXT_FIELD, 10, 40, 100, 20);
var fieldThree = form.newField('parent_table_id', JSField.TEXT_FIELD, 10, 70, 100, 20);
// Set the third field come before the first in the tab sequence, and remove the 
// second field from the tab sequence.
fieldOne.tabSeq = 2;
fieldTwo.tabSeq = SM_DEFAULTS.IGNORE;
fieldThree.tabSeq = 1;
```

### NONE

Constant used in various places to set properties to "none".

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var form = solutionModel.newForm('parentForm', 'db:/example_data/parent_table', null, false, 1200, 800);
form.navigator = SM_DEFAULTS.NONE; // Hide the navigator on the form.
```
