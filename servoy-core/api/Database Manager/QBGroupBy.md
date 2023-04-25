#  QBGroupBy


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [QBSelect](./QBSelect.md) | [parent](QBGroupBy.md#parent)                   | Get query builder parent table clause, this may be a query or a join clause..                                    |
| [QBSelect](./QBSelect.md) | [root](QBGroupBy.md#root)                   | Get query builder parent..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [QBGroupBy](./QBGroupBy.md) | [add(column)](QBGroupBy.md#add-column)                   | Add column name to group-by clause..                                    |
| [QBGroupBy](./QBGroupBy.md) | [add(function)](QBGroupBy.md#add-function)                   | Add column name to group-by clause..                                    |
| [QBGroupBy](./QBGroupBy.md) | [addPk()](QBGroupBy.md#addpk)                   | Add the tables' primary pk columns in alphabetical order to the group by clause..                                    |
| [QBGroupBy](./QBGroupBy.md) | [clear()](QBGroupBy.md#clear)                   | Clear the to group-by clause..                                    |

## Properties Details

### parent

Get query builder parent table clause, this may be a query or a join clause.

**Returns**\
[QBSelect](./QBSelect.md) 


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

### add(column)

Add column name to group-by clause.

Same as query.groupBy().add(join.getColumn("value"))

**Parameters**\
[QBColumn](./QBColumn.md) column the column to add to the query condition

**Returns**\
[QBGroupBy](./QBGroupBy.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.groupBy.add(query.columns.orderid) // have to group by on pk when using having-conditions in (foundset) pk queries
.root.having.add(query.joins.orders_to_order_details.columns.quantity.count.eq(0))
foundset.loadRecords(query)
```
### add(function)

Add column name to group-by clause.

Same as query.groupBy().add(join.getColumn("value"))

**Parameters**\
[QBColumn](./QBColumn.md) function the function to add to the query

**Returns**\
[QBGroupBy](./QBGroupBy.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.groupBy.add(query.columns.orderid) // have to group by on pk when using having-conditions in (foundset) pk queries
.root.having.add(query.joins.orders_to_order_details.columns.quantity.count.eq(0))
foundset.loadRecords(query)
```
### addPk()

Add the tables' primary pk columns in alphabetical order to the group by clause.


**Returns**\
[QBGroupBy](./QBGroupBy.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.groupBy.addPk() // have to group by on pk when using having-conditions in (foundset) pk queries
.root.having.add(query.joins.orders_to_order_details.columns.quantity.count.eq(0))
foundset.loadRecords(query)
```
### clear()

Clear the to group-by clause.


**Returns**\
[QBGroupBy](./QBGroupBy.md) 


**Sample**

```javascript
var q = foundset.getQuery()
q.where.add(q.columns.x.eq(100))
query.groupBy.clear.root.clearHaving()
foundset.loadRecords(q);
```

