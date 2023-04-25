#  JSCalculation

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [code](JSCalculation.md#code)                   | The full source code of this method (including doc and function declaration)..                                    |
| [Number](../JSLib/Number.md) | [variableType](JSCalculation.md#variableType)                   | Get or set the sql type of this variable..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [getName()](JSCalculation.md#getname)                   | This method returns the name of the stored calculation..                                    |
| [UUID](../Application/UUID.md) | [getUUID()](JSCalculation.md#getuuid)                   | Returns the UUID of the calculation..                                    |
| [Boolean](../JSLib/Boolean.md) | [hasFlag(flag)](JSCalculation.md#hasflag-flag)                   | Check a flag of the calculation..                                    |
| [Boolean](../JSLib/Boolean.md) | [isStored()](JSCalculation.md#isstored)                   | Returns whether this calculation is a stored one or not..                                    |

## Properties Details

### code

The full source code of this method (including doc and function declaration).

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var calc = solutionModel.getDataSourceNode("db:/example_data/customers").getCalculation("myCalculation");
calc.code = "function myCalculation() { return 123; }";
```
### variableType

Get or set the sql type of this variable.
Type should be one of JSVariable.DATETIME, JSVariable.TEXT, JSVariable.NUMBER , JSVariable.INTEGER or JSVariable.MEDIA.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var calc = solutionModel.getDataSourceNode("db:/example_data/customers").getCalculation("myCalculation");
calc.variableType = JSVariable.DATETIME;
```

## Methods Details

### getName()

This method returns the name of the stored calculation.


**Returns**\
[String](../JSLib/String.md) the name of the stored calculation

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var calc = solutionModel.newCalculation("function myCalculation() { return 123; }", JSVariable.INTEGER, "db:/example_data/customers");
application.output(calc.getName());
```
### getUUID()

Returns the UUID of the calculation.


**Returns**\
[UUID](../Application/UUID.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var calc = solutionModel.getDataSourceNode("db:/example_data/customers").newCalculation("function myCalculation() { return 123; }", JSVariable.INTEGER);
application.output(calc.getUUID().toString());
```
### hasFlag(flag)

Check a flag of the calculation.
The flags are a bit pattern consisting of 1 or more of the following bits:
 - JSColumn.UUID_COLUMN

**Parameters**\
[Number](../JSLib/Number.md) flag  ;

**Returns**\
[Boolean](../JSLib/Boolean.md) boolean whether flag is set.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var datasourceNode = solutionModel.getDataSourceNode('db:/example_data/orders')
var calculation = datasourceNode.getCalculation('mycalculation')
if (calculation.hasFlag(JSColumn.UUID_COLUMN))
{
	 // calculation was typed as UUID
}
```
### isStored()

Returns whether this calculation is a stored one or not.


**Returns**\
[Boolean](../JSLib/Boolean.md) true if the calculation is stored, false otherwise

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var calc = solutionModel.getDataSourceNode("db:/example_data/customers").newCalculation("function myCalculation() { return 123; }", JSVariable.INTEGER);
if (calc.isStored()) application.output("The calculation is stored");
else application.output("The calculation is not stored");
```

