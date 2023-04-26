# SQL\_ACTION\_TYPES

## Constants Summary

| Type                          | Name                                                   | Summary                                             |
| ----------------------------- | ------------------------------------------------------ | --------------------------------------------------- |
| [Number](../js-lib/number.md) | [DELETE\_ACTION](sql\_action\_types.md#DELETE\_ACTION) | Constant for the "delete" SQL action..              |
| [Number](../js-lib/number.md) | [INSERT\_ACTION](sql\_action\_types.md#INSERT\_ACTION) | Constant for the "insert" SQL action..              |
| [Number](../js-lib/number.md) | [NO\_ACTION](sql\_action\_types.md#NO\_ACTION)         | Constant expressing that no SQL action took place.. |
| [Number](../js-lib/number.md) | [SELECT\_ACTION](sql\_action\_types.md#SELECT\_ACTION) | Constant for the "select" SQL action..              |
| [Number](../js-lib/number.md) | [UPDATE\_ACTION](sql\_action\_types.md#UPDATE\_ACTION) | Constant for the "update" SQL action..              |

## Constants Details

### DELETE\_ACTION

Constant for the "delete" SQL action.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
if (action == SQL_ACTION_TYPES.INSERT_ACTION)
	application.output("it was an insert");
else if (action == SQL_ACTION_TYPES.DELETE_ACTION)
	application.output("it was a delete");
else if (action == SQL_ACTION_TYPES.UPDATE_ACTION)
	application.output("it was an update");
else if (action == SQL_ACTION_TYPES.SELECT_ACTION)
	application.output("it was a select");
else if (action == SQL_ACTION_TYPES.NO_ACTION)
	application.output("it was nothing");
else
	application.output("what was this?");
```

### INSERT\_ACTION

Constant for the "insert" SQL action.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
if (action == SQL_ACTION_TYPES.INSERT_ACTION)
	application.output("it was an insert");
else if (action == SQL_ACTION_TYPES.DELETE_ACTION)
	application.output("it was a delete");
else if (action == SQL_ACTION_TYPES.UPDATE_ACTION)
	application.output("it was an update");
else if (action == SQL_ACTION_TYPES.SELECT_ACTION)
	application.output("it was a select");
else if (action == SQL_ACTION_TYPES.NO_ACTION)
	application.output("it was nothing");
else
	application.output("what was this?");
```

### NO\_ACTION

Constant expressing that no SQL action took place.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
if (action == SQL_ACTION_TYPES.INSERT_ACTION)
	application.output("it was an insert");
else if (action == SQL_ACTION_TYPES.DELETE_ACTION)
	application.output("it was a delete");
else if (action == SQL_ACTION_TYPES.UPDATE_ACTION)
	application.output("it was an update");
else if (action == SQL_ACTION_TYPES.SELECT_ACTION)
	application.output("it was a select");
else if (action == SQL_ACTION_TYPES.NO_ACTION)
	application.output("it was nothing");
else
	application.output("what was this?");
```

### SELECT\_ACTION

Constant for the "select" SQL action.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
if (action == SQL_ACTION_TYPES.INSERT_ACTION)
	application.output("it was an insert");
else if (action == SQL_ACTION_TYPES.DELETE_ACTION)
	application.output("it was a delete");
else if (action == SQL_ACTION_TYPES.UPDATE_ACTION)
	application.output("it was an update");
else if (action == SQL_ACTION_TYPES.SELECT_ACTION)
	application.output("it was a select");
else if (action == SQL_ACTION_TYPES.NO_ACTION)
	application.output("it was nothing");
else
	application.output("what was this?");
```

### UPDATE\_ACTION

Constant for the "update" SQL action.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
if (action == SQL_ACTION_TYPES.INSERT_ACTION)
	application.output("it was an insert");
else if (action == SQL_ACTION_TYPES.DELETE_ACTION)
	application.output("it was a delete");
else if (action == SQL_ACTION_TYPES.UPDATE_ACTION)
	application.output("it was an update");
else if (action == SQL_ACTION_TYPES.SELECT_ACTION)
	application.output("it was a select");
else if (action == SQL_ACTION_TYPES.NO_ACTION)
	application.output("it was nothing");
else
	application.output("what was this?");
```
