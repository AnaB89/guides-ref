# QBSort

## Property Summary

| Type                    | Name                       | Summary                                                                       |
| ----------------------- | -------------------------- | ----------------------------------------------------------------------------- |
| [QBSelect](qbselect.md) | [parent](qbsort.md#parent) | Get query builder parent table clause, this may be a query or a join clause.. |
| [QBSelect](qbselect.md) | [root](qbsort.md#root)     | Get query builder parent..                                                    |

## Properties Details

### parent

Get query builder parent table clause, this may be a query or a join clause.

**Returns**\
[QBSelect](qbselect.md)

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
