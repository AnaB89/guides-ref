#  SQL_ACTION_TYPES


## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [DELETE_ACTION](SQL_ACTION_TYPES.md#DELETE_ACTION)                   | Constant for the "delete" SQL action..                                    |
| [Number](../JSLib/Number.md) | [INSERT_ACTION](SQL_ACTION_TYPES.md#INSERT_ACTION)                   | Constant for the "insert" SQL action..                                    |
| [Number](../JSLib/Number.md) | [NO_ACTION](SQL_ACTION_TYPES.md#NO_ACTION)                   | Constant expressing that no SQL action took place..                                    |
| [Number](../JSLib/Number.md) | [SELECT_ACTION](SQL_ACTION_TYPES.md#SELECT_ACTION)                   | Constant for the "select" SQL action..                                    |
| [Number](../JSLib/Number.md) | [UPDATE_ACTION](SQL_ACTION_TYPES.md#UPDATE_ACTION)                   | Constant for the "update" SQL action..                                    |

## Constants Details

### DELETE_ACTION

Constant for the "delete" SQL action.

**Returns**\
[Number](../JSLib/Number.md) 


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
### INSERT_ACTION

Constant for the "insert" SQL action.

**Returns**\
[Number](../JSLib/Number.md) 


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
### NO_ACTION

Constant expressing that no SQL action took place.

**Returns**\
[Number](../JSLib/Number.md) 


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
### SELECT_ACTION

Constant for the "select" SQL action.

**Returns**\
[Number](../JSLib/Number.md) 


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
### UPDATE_ACTION

Constant for the "update" SQL action.

**Returns**\
[Number](../JSLib/Number.md) 


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

