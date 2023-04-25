#  QBLogicalCondition

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Array](../JSLib/Array.md) | [conditionnames](QBLogicalCondition.md#conditionnames)                   | Get the names for the conditions in the logical condition..                                    |
| [QBTableClause](./QBTableClause.md) | [parent](QBLogicalCondition.md#parent)                   | Get query builder parent table clause, this may be a query or a join clause..                                    |
| [QBSelect](./QBSelect.md) | [root](QBLogicalCondition.md#root)                   | Get query builder parent..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [QBLogicalCondition](./QBLogicalCondition.md) | [add(condition)](QBLogicalCondition.md#add-condition)                   | Add a condition to the AND or OR condition list..                                    |
| [QBLogicalCondition](./QBLogicalCondition.md) | [add(name, condition)](QBLogicalCondition.md#add-name-condition)                   | Add a named condition to the logical condition..                                    |
| [QBLogicalCondition](./QBLogicalCondition.md) | [clear()](QBLogicalCondition.md#clear)                   | Clear the conditions in the logical condition..                                    |
| [QBCondition](./QBCondition.md) | [getCondition(name)](QBLogicalCondition.md#getcondition-name)                   | Get a named condition in the logical condition..                                    |
| [QBLogicalCondition](./QBLogicalCondition.md) | [remove(name)](QBLogicalCondition.md#remove-name)                   | Remove a named condition from the logical condition..                                    |

## Properties Details

### conditionnames

Get the names for the conditions in the logical condition.

**Returns**\
[Array](../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

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

### add(condition)

Add a condition to the AND or OR condition list.

**Parameters**\
[QBCondition](./QBCondition.md) condition the condition to add

**Returns**\
[QBLogicalCondition](./QBLogicalCondition.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.orderdate.isNull)
```
### add(name, condition)

Add a named condition to the logical condition.

**Parameters**\
[String](../JSLib/String.md) name the name of the condition\
[QBCondition](./QBCondition.md) condition the condition to add

**Returns**\
[QBLogicalCondition](./QBLogicalCondition.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

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
[QBLogicalCondition](./QBLogicalCondition.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var cond = query.getCondition('mycond')
cond.clear()
```
### getCondition(name)

Get a named condition in the logical condition.

**Parameters**\
[String](../JSLib/String.md) name The condition name.

**Returns**\
[QBCondition](./QBCondition.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

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
[String](../JSLib/String.md) name The condition name.

**Returns**\
[QBLogicalCondition](./QBLogicalCondition.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var cond = query.getCondition('mycond')
cond.remove('mysubcond')
```

