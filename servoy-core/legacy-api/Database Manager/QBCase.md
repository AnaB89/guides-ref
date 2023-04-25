#  QBCase

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [QBTableClause](./QBTableClause.md) | [parent](QBCase.md#parent)                   | Get query builder parent table clause, this may be a query or a join clause..                                    |
| [QBSelect](./QBSelect.md) | [root](QBCase.md#root)                   | Get query builder parent..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [QBColumn](./QBColumn.md) | [else(value)](QBCase.md#else-value)                   | Set the return value to use when none of the when-clauses conditions are met..                                    |
| [QBCaseWhen](./QBCaseWhen.md) | [when(condition)](QBCase.md#when-condition)                   | Add a when-clause to the case searched expression..                                    |

## Properties Details

### parent

Get query builder parent table clause, this may be a query or a join clause.

**Returns**\
[QBTableClause](./QBTableClause.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var query = datasources.db.example_data.person.createSelect();
	query.where.add(query.joins.person_to_parent.joins.person_to_parent.columns.name.eq('john'))
	foundset.loadRecords(query)
```
### root

Get query builder parent.

**Returns**\
[QBSelect](./QBSelect.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var subquery = datasources.db.example_data.order_details.createSelect();

	var query = datasources.db.example_data.orders.createSelect();
	query.where.add(query
		.or
			.add(query.columns.order_id.not.isin([1, 2, 3]))

			.add(query.exists(
					subquery.where.add(subquery.columns.orderid.eq(query.columns.order_id)).root
			))
		)

	foundset.loadRecords(query)
```

## Methods Details

### else(value)

Set the return value to use when none of the when-clauses conditions are met.

**Parameters**\
[Object](../JSLib/Object.md) value The value.

**Returns**\
[QBColumn](./QBColumn.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

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
### when(condition)

Add a when-clause to the case searched expression.

**Parameters**\
[QBCondition](./QBCondition.md) condition The condition.

**Returns**\
[QBCaseWhen](./QBCaseWhen.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

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

