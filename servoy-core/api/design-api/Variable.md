#  Variable


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [comment](Variable.md#comment)                   | Property for setting and getting the jsdoc text (comment) of the script variable..                                    |
| [String](../JSLib/String.md) | [defaultValue](Variable.md#defaultValue)                   | The default value of the variable..                                    |
| [String](../JSLib/String.md) | [name](Variable.md#name)                   | The name of the variable..                                    |
| [String](../JSLib/String.md) | [scopeName](Variable.md#scopeName)                   | The name of the scope..                                    |
| [Number](../JSLib/Number.md) | [variableType](Variable.md#variableType)                   | The type of the variable..                                    |

## Properties Details

### comment

Property for setting and getting the jsdoc text (comment) of the script variable.

**Returns**\
[String](../JSLib/String.md) the value of the jsdoc text (comment) of the script variable


**Sample**

```javascript

```
### defaultValue

The default value of the variable.

It is interpreted as a JS expression.

For form variables ,setting this property requires the form instances to be destroyed (history.remove("formName")).
If you want to use a default value for a newly created variable  create the variable using the 3 parameter version newVariable(name,type,defaultValue).

For INTEGER variables it can be an integer constant, like 10 for example.
For NUMBER variables it can be a real constant, like 22.41. For DATETIME
variables it can be "now", or a JS expression like "new Date()". For TEXT
variables it can be any string surrounded with quotes, like "'some text'".

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### name

The name of the variable.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### scopeName

The name of the scope.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### variableType

The type of the variable. Can be one of: TEXT, INTEGER, NUMBER, DATETIME or MEDIA.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```

