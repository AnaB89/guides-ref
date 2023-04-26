# JSCalculation

## Property Summary

| Type                          | Name                                          | Summary                                                                        |
| ----------------------------- | --------------------------------------------- | ------------------------------------------------------------------------------ |
| [String](../js-lib/string.md) | [code](jscalculation.md#code)                 | The full source code of this method (including doc and function declaration).. |
| [Number](../js-lib/number.md) | [variableType](jscalculation.md#variableType) | Get or set the sql type of this variable..                                     |

## Methods Summary

| Type                            | Name                                           | Summary                                                   |
| ------------------------------- | ---------------------------------------------- | --------------------------------------------------------- |
| [String](../js-lib/string.md)   | [getName()](jscalculation.md#getname)          | This method returns the name of the stored calculation..  |
| [UUID](../application/uuid.md)  | [getUUID()](jscalculation.md#getuuid)          | Returns the UUID of the calculation..                     |
| [Boolean](../js-lib/boolean.md) | [hasFlag(flag)](jscalculation.md#hasflag-flag) | Check a flag of the calculation..                         |
| [Boolean](../js-lib/boolean.md) | [isStored()](jscalculation.md#isstored)        | Returns whether this calculation is a stored one or not.. |

## Properties Details

### code

The full source code of this method (including doc and function declaration).

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var calc = solutionModel.getDataSourceNode("db:/example_data/customers").getCalculation("myCalculation");
calc.code = "function myCalculation() { return 123; }";
```

### variableType

Get or set the sql type of this variable. Type should be one of JSVariable.DATETIME, JSVariable.TEXT, JSVariable.NUMBER , JSVariable.INTEGER or JSVariable.MEDIA.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var calc = solutionModel.getDataSourceNode("db:/example_data/customers").getCalculation("myCalculation");
calc.variableType = JSVariable.DATETIME;
```

## Methods Details

### getName()

This method returns the name of the stored calculation.

**Returns**\
[String](../js-lib/string.md) the name of the stored calculation

**Sample**

```javascript
var calc = solutionModel.newCalculation("function myCalculation() { return 123; }", JSVariable.INTEGER, "db:/example_data/customers");
application.output(calc.getName());
```

### getUUID()

Returns the UUID of the calculation.

**Returns**\
[UUID](../application/uuid.md)

**Sample**

```javascript
var calc = solutionModel.getDataSourceNode("db:/example_data/customers").newCalculation("function myCalculation() { return 123; }", JSVariable.INTEGER);
application.output(calc.getUUID().toString());
```

### hasFlag(flag)

Check a flag of the calculation. The flags are a bit pattern consisting of 1 or more of the following bits:

* JSColumn.UUID\_COLUMN

**Parameters**\
[Number](../js-lib/number.md) flag ;

**Returns**\
[Boolean](../js-lib/boolean.md) boolean whether flag is set.

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
[Boolean](../js-lib/boolean.md) true if the calculation is stored, false otherwise

**Sample**

```javascript
var calc = solutionModel.getDataSourceNode("db:/example_data/customers").newCalculation("function myCalculation() { return 123; }", JSVariable.INTEGER);
if (calc.isStored()) application.output("The calculation is stored");
else application.output("The calculation is not stored");
```
