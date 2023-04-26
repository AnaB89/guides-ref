# QBLogicalCondition

## Property Summary

| Type                              | Name                                                   | Summary                                                                       |
| --------------------------------- | ------------------------------------------------------ | ----------------------------------------------------------------------------- |
| [Array](../js-lib/array.md)       | [conditionnames](qblogicalcondition.md#conditionnames) | Get the names for the conditions in the logical condition..                   |
| [QBTableClause](qbtableclause.md) | [parent](qblogicalcondition.md#parent)                 | Get query builder parent table clause, this may be a query or a join clause.. |
| [QBSelect](qbselect.md)           | [root](qblogicalcondition.md#root)                     | Get query builder parent..                                                    |

## Methods Summary

| Type                                        | Name                                                             | Summary                                               |
| ------------------------------------------- | ---------------------------------------------------------------- | ----------------------------------------------------- |
| [QBLogicalCondition](qblogicalcondition.md) | [add(condition)](qblogicalcondition.md#add-condition)            | Add a condition to the AND or OR condition list..     |
| [QBLogicalCondition](qblogicalcondition.md) | [add(name, condition)](qblogicalcondition.md#add-name-condition) | Add a named condition to the logical condition..      |
| [QBLogicalCondition](qblogicalcondition.md) | [clear()](qblogicalcondition.md#clear)                           | Clear the conditions in the logical condition..       |
| [QBCondition](qbcondition.md)               | [getCondition(name)](qblogicalcondition.md#getcondition-name)    | Get a named condition in the logical condition..      |
| [QBLogicalCondition](qblogicalcondition.md) | [remove(name)](qblogicalcondition.md#remove-name)                | Remove a named condition from the logical condition.. |

## Properties Details

### conditionnames

Get the names for the conditions in the logical condition.

**Returns**\
[Array](../js-lib/array.md)

**Sample**

```javascript
var cond = query.getCondition('mycond')
for (var cname in cond.conditionnames)
{
	var subcond = cond.getCondition(cname)
}
```

### parent

Get query builder parent table clause, this may be a query or a join clause.

**Returns**\
[QBTableClause](qbtableclause.md)

**Sample**

```javascript
var query = datasources.db.example_data.person.createSelect();
	query.where.add(query.joins.person_to_parent.joins.person_to_parent.columns.name.eq('john'))
	foundset.loadRecords(query)
```

### root

Get query builder parent.

**Returns**\
[QBSelect](qbselect.md)

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

### add(condition)

Add a condition to the AND or OR condition list.

**Parameters**\
[QBCondition](qbcondition.md) condition the condition to add

**Returns**\
[QBLogicalCondition](qblogicalcondition.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.orderdate.isNull)
```

### add(name, condition)

Add a named condition to the logical condition.

**Parameters**\
[String](../js-lib/string.md) name the name of the condition\
[QBCondition](qbcondition.md) condition the condition to add

**Returns**\
[QBLogicalCondition](qblogicalcondition.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
// create a logical condition
var condition = query.and
// add named conditions
condition.add("undated", query.columns.orderdate.isNull)
condition.add("expensive", query.columns.orderamount.gt(10000))

query.where.add("mycond", condition)

// part of the condition can be removed again
condition.remove("undated")
```

### clear()

Clear the conditions in the logical condition.

**Returns**\
[QBLogicalCondition](qblogicalcondition.md)

**Sample**

```javascript
var cond = query.getCondition('mycond')
cond.clear()
```

### getCondition(name)

Get a named condition in the logical condition.

**Parameters**\
[String](../js-lib/string.md) name The condition name.

**Returns**\
[QBCondition](qbcondition.md)

**Sample**

```javascript
var cond = query.getCondition('mycond')
for (var cname in cond.conditionnames)
{
	var subcond = cond.getCondition(cname)
}
```

### remove(name)

Remove a named condition from the logical condition.

**Parameters**\
[String](../js-lib/string.md) name The condition name.

**Returns**\
[QBLogicalCondition](qblogicalcondition.md)

**Sample**

```javascript
var cond = query.getCondition('mycond')
cond.remove('mysubcond')
```
