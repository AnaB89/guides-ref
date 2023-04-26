# JSVariable

## Constants Summary

| Type                          | Name                               | Summary                                                                 |
| ----------------------------- | ---------------------------------- | ----------------------------------------------------------------------- |
| [Number](../js-lib/number.md) | [DATETIME](jsvariable.md#DATETIME) | Constant to be used when the type of a variable needs to be specified.. |
| [Number](../js-lib/number.md) | [INTEGER](jsvariable.md#INTEGER)   | Constant to be used when the type of a variable needs to be specified.. |
| [Number](../js-lib/number.md) | [MEDIA](jsvariable.md#MEDIA)       | Constant to be used when the type of a variable needs to be specified.. |
| [Number](../js-lib/number.md) | [NUMBER](jsvariable.md#NUMBER)     | Constant to be used when the type of a variable needs to be specified.. |
| [Number](../js-lib/number.md) | [TEXT](jsvariable.md#TEXT)         | Constant to be used when the type of a variable needs to be specified.. |

## Property Summary

| Type                          | Name                                       | Summary                             |
| ----------------------------- | ------------------------------------------ | ----------------------------------- |
| [String](../js-lib/string.md) | [defaultValue](jsvariable.md#defaultValue) | The default value of the variable.. |
| [String](../js-lib/string.md) | [name](jsvariable.md#name)                 | The name of the variable..          |
| [Number](../js-lib/number.md) | [variableType](jsvariable.md#variableType) | The type of the variable..          |

## Methods Summary

| Type                           | Name                                         | Summary                           |
| ------------------------------ | -------------------------------------------- | --------------------------------- |
| [String](../js-lib/string.md)  | [getScopeName()](jsvariable.md#getscopename) | Get scope name.                   |
| [UUID](../application/uuid.md) | [getUUID()](jsvariable.md#getuuid)           | Returns the UUID of the variable. |

## Constants Details

### DATETIME

Constant to be used when the type of a variable needs to be specified.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var dateVar = solutionModel.newGlobalVariable('globals', 'gDate', JSVariable.DATETIME);
dateVar.defaultValue = 'now';
application.output(scopes.globals.gDate); // Prints the current date and time.
```

### INTEGER

Constant to be used when the type of a variable needs to be specified.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var intVar = solutionModel.newGlobalVariable('globals', 'gInt', JSVariable.INTEGER);
intVar.defaultValue = 997;
application.output(scopes.globals.gInt); // Prints 997
```

### MEDIA

Constant to be used when the type of a variable needs to be specified.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var mediaVar = solutionModel.newGlobalVariable('globals', 'gMedia', JSVariable.MEDIA);
mediaVar.defaultValue = 'new Array(1, 2, 3, 4)';
application.output(scopes.globals.gMedia); // Prints out the array with four elements.
```

### NUMBER

Constant to be used when the type of a variable needs to be specified.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var numberVar = solutionModel.newGlobalVariable('globals', 'gNumber', JSVariable.NUMBER);
numberVar.defaultValue = 192.334;
application.output(scopes.globals.gNumber); // Prints 192.334
```

### TEXT

Constant to be used when the type of a variable needs to be specified.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var txtVar = solutionModel.newGlobalVariable('globals', 'gText', JSVariable.TEXT);
txtVar.defaultValue = '"some text"'; // Use two pairs of quotes if you want to assign a String as default value.
application.output(scopes.globals.gText); // Prints 'some text' (without quotes).
```

## Properties Details

### defaultValue

The default value of the variable.

It is interpreted as a JS expression.

For form variables ,setting this property requires the form instances to be destroyed (history.remove("formName")). If you want to use a default value for a newly created variable create the variable using the 3 parameter version newVariable(name,type,defaultValue).

For INTEGER variables it can be an integer constant, like 10 for example. For NUMBER variables it can be a real constant, like 22.41. For DATETIME variables it can be "now", or a JS expression like "new Date()". For TEXT variables it can be any string surrounded with quotes, like "'some text'".

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var intVar = solutionModel.newGlobalVariable('globals', 'gInt', JSVariable.INTEGER);
intVar.defaultValue = 997;
application.output(scopes.globals.gInt); // Prints 997
var numberVar = solutionModel.newGlobalVariable('globals', 'gNumber', JSVariable.NUMBER);
numberVar.defaultValue = 192.334;
application.output(scopes.globals.gNumber); // Prints 192.334
var dateVar = solutionModel.newGlobalVariable('globals', 'gDate', JSVariable.DATETIME);
dateVar.defaultValue = 'now';
application.output(scopes.globals.gDate); // Prints the current date and time.
var txtVar = solutionModel.newGlobalVariable('globals', 'gText', JSVariable.TEXT);
txtVar.defaultValue = '"some text"'; // Use two pairs of quotes if you want to assign a String as default value.
application.output(scopes.globals.gText); // Prints 'some text' (without quotes).
var mediaVar = solutionModel.newGlobalVariable('globals', 'gMedia', JSVariable.MEDIA);
mediaVar.defaultValue = 'new Array(1, 2, 3, 4)';
application.output(scopes.globals.gMedia); // Prints out the array with four elements.
```

### name

The name of the variable.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var gVar = solutionModel.newGlobalVariable('globals', 'gtext', JSVariable.TEXT);
gVar.name = 'anotherName';
gVar.defaultValue = '"default text"';
// The next two lines will print the same output.
application.output(scopes.globals[gVar.name]);
application.output(scopes.globals.anotherName);
```

### variableType

The type of the variable. Can be one of: TEXT, INTEGER, NUMBER, DATETIME or MEDIA.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var g = solutionModel.newGlobalVariable('globals', 'gtext',JSVariable.TEXT);
scopes.globals.gtext = 'some text';
g.variableType = JSVariable.DATETIME;
scopes.globals.gtext = 'another text'; // This will raise an error now, because the variable is not longer of type text.
```

## Methods Details

### getScopeName()

Get scope name

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var globalVariables = solutionModel.getGlobalVariables();
for (var i in globalVariables)
	application.output(globalVariables[i].name + ' is defined in scope ' + globalVariables[i].getScopeName());
```

### getUUID()

Returns the UUID of the variable

**Returns**\
[UUID](../application/uuid.md)

**Sample**

```javascript
var dateVar = solutionModel.newGlobalVariable('globals', 'gDate', JSVariable.DATETIME);
application.output(dateVar.getUUID().toString());
```
