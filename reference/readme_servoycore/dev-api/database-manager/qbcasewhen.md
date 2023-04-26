# QBCaseWhen

## Methods Summary

| Type                | Name                                    | Summary                                                                                 |
| ------------------- | --------------------------------------- | --------------------------------------------------------------------------------------- |
| [QBCase](qbcase.md) | [then(value)](qbcasewhen.md#then-value) | Set the return value to use when the condition of the searched case expression is met.. |

## Methods Details

### then(value)

Set the return value to use when the condition of the searched case expression is met.

**Parameters**\
[Object](../js-lib/object.md) value The value.

**Returns**\
[QBCase](qbcase.md)

**Sample**

```javascript
var query = datasources.db.example_data.order_details.createSelect();

// case expressions can be added to the result of the query
	query.result.add(query.case.when(query.columns.quantity.ge(1000)).then('BIG').else('small'));

 // they can also be used in conditions
	query.where.add(query.case
		.when(query.columns.discount.gt(10)).then(50)
		.when(query.columns.quantity.le(20)).then(70)
		.else(100)
	.multiply(query.columns.unitprice).lt(10000));
```
