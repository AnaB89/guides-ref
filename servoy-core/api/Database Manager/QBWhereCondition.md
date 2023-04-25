#  QBWhereCondition


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Array](../JSLib/Array.md) | [conditionnames](QBWhereCondition.md#conditionnames)                   | Get the names for the conditions in the logical condition..                                    |
| [QBTableClause](./QBTableClause.md) | [parent](QBWhereCondition.md#parent)                   | Get query builder parent table clause, this may be a query or a join clause..                                    |
| [QBSelect](./QBSelect.md) | [root](QBWhereCondition.md#root)                   | Get query builder parent..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [QBLogicalCondition](./QBLogicalCondition.md) | [add(condition)](QBWhereCondition.md#add-condition)                   | Add a condition to the AND or OR condition list..                                    |
| [QBLogicalCondition](./QBLogicalCondition.md) | [add(name, condition)](QBWhereCondition.md#add-name-condition)                   | Add a named condition to the AND or OR condition list..                                    |
| [QBLogicalCondition](./QBLogicalCondition.md) | [clear()](QBWhereCondition.md#clear)                   | Clear the conditions in the query where-clause..                                    |
| [QBCondition](./QBCondition.md) | [getCondition(name)](QBWhereCondition.md#getcondition-name)                   | Get a named condition in the logical condition..                                    |
| [QBLogicalCondition](./QBLogicalCondition.md) | [remove(name)](QBWhereCondition.md#remove-name)                   | Remove a named condition from the AND or OR condition list..                                    |

## Properties Details

### conditionnames

Get the names for the conditions in the logical condition.

**Returns**\
[Array](../JSLib/Array.md) 


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
[QBTableClause](./QBTableClause.md) 


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
[QBCondition](./QBCondition.md) condition the condition to add

**Returns**\
[QBLogicalCondition](./QBLogicalCondition.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.orderdate.isNull)
```
### add(name, condition)

Add a named condition to the AND or OR condition list.

**Parameters**\
[String](../JSLib/String.md) name the name of the condition\
[QBCondition](./QBCondition.md) condition the condition to add

**Returns**\
[QBLogicalCondition](./QBLogicalCondition.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add("mycond", query.columns.orderdate.isNull)
```
### clear()

Clear the conditions in the query where-clause.


**Returns**\
[QBLogicalCondition](./QBLogicalCondition.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.clear()
```
### getCondition(name)

Get a named condition in the logical condition.

**Parameters**\
[String](../JSLib/String.md) name The condition name.

**Returns**\
[QBCondition](./QBCondition.md) 


**Sample**

```javascript
var cond = query.getCondition('mycond')
for (var cname in cond.conditionnames)
{
	var subcond = cond.getCondition(cname)
}
```
### remove(name)

Remove a named condition from the AND or OR condition list.

**Parameters**\
[String](../JSLib/String.md) name The condition name.

**Returns**\
[QBLogicalCondition](./QBLogicalCondition.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.remove("mycond")
```

