# QBJoins

## Property Summary

| Type                              | Name                        | Summary                                                                       |
| --------------------------------- | --------------------------- | ----------------------------------------------------------------------------- |
| [QBTableClause](qbtableclause.md) | [parent](qbjoins.md#parent) | Get query builder parent table clause, this may be a query or a join clause.. |
| [QBSelect](qbselect.md)           | [root](qbjoins.md#root)     | Get query builder parent..                                                    |

## Methods Summary

| Type                        | Name                                                                                   | Summary                                                                                            |
| --------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| [QBJoin](qbjoin.md)         | [add(subqueryBuilder, joinType)](qbjoins.md#add-subquerybuilder-jointype)              | Add a join clause from the parent query builder part to a derived table based on another query..   |
| [QBJoin](qbjoin.md)         | [add(subqueryBuilder, joinType, alias)](qbjoins.md#add-subquerybuilder-jointype-alias) | Add a join clause from the parent query builder part to a derived table based on another query..   |
| [QBJoin](qbjoin.md)         | [add(dataSource)](qbjoins.md#add-datasource)                                           | Add a join with join type IQueryBuilderJoin#LEFT\_OUTER\_JOIN and no alias for the joining table.. |
| [QBJoin](qbjoin.md)         | [add(dataSource, joinType)](qbjoins.md#add-datasource-jointype)                        | Add a join with no alias for the joining table..                                                   |
| [QBJoin](qbjoin.md)         | [add(dataSource, joinType, alias)](qbjoins.md#add-datasource-jointype-alias)           | Add a join clause from the parent query builder part to the specified data source..                |
| [QBJoin](qbjoin.md)         | [add(dataSourceOrRelation, alias)](qbjoins.md#add-datasourceorrelation-alias)          | Add a join based on relation or add a manual join..                                                |
| [Array](../js-lib/array.md) | [getJoins()](qbjoins.md#getjoins)                                                      | .                                                                                                  |
| [QBJoins](qbjoins.md)       | [removeUnused(keepInnerjoins)](qbjoins.md#removeunused-keepinnerjoins)                 | Remove the joins that are not used anywhere in the query..                                         |

## Properties Details

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

### add(subqueryBuilder, joinType)

Add a join clause from the parent query builder part to a derived table based on another query.

**Parameters**\
[QBSelect](qbselect.md) subqueryBuilder ;\
[Number](../js-lib/number.md) joinType ;

**Returns**\
[QBJoin](qbjoin.md)

**Sample**

```javascript
```

### add(subqueryBuilder, joinType, alias)

Add a join clause from the parent query builder part to a derived table based on another query.

**Parameters**\
[QBSelect](qbselect.md) subqueryBuilder ;\
[Number](../js-lib/number.md) joinType ;\
[String](../js-lib/string.md) alias ;

**Returns**\
[QBJoin](qbjoin.md)

**Sample**

```javascript
var subquery = datasources.db.example_data.products.createSelect();
 subquery.where.add(subquery.columns.supplierid.eq(99));
 subquery.result.add(subquery.columns.categoryid, 'subcat')
 subquery.result.add(subquery.columns.productid, 'subprod')

 var query = datasources.db.example_data.order_details.createSelect();
 // add a join on a derived table using a subquery
 var join = query.joins.add(subquery, QBJoin.INNER_JOIN, 'subprods');
 join.on.add(query.columns.productid.eq(join.columns['subprod']));
 query.result.add(query.columns.quantity);
 query.result.add(join.columns['subcat']);
```

### add(dataSource)

Add a join with join type IQueryBuilderJoin#LEFT\_OUTER\_JOIN and no alias for the joining table.

**Parameters**\
[String](../js-lib/string.md) dataSource data source

**Returns**\
[QBJoin](qbjoin.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
 /** @type {QBJoin<db:/example_data/order_details>} */
	var join = query.joins.add('db:/example_data/order_details', QBJoin.INNER_JOIN, 'odetail')
	join.on.add(join.columns.orderid.eq(query.columns.orderid))
 // to add a join based on a relation, use the relation name
 var join2 = query.joins.add('orders_to_customers', 'cust')
	query.where.add(join2.columns.customerid.eq(999))
	foundset.loadRecords(query)
```

### add(dataSource, joinType)

Add a join with no alias for the joining table.

**Parameters**\
[String](../js-lib/string.md) dataSource data source\
[Number](../js-lib/number.md) joinType join type, one of QBJoin.LEFT\_OUTER\_JOIN, QBJoin.INNER\_JOIN, QBJoin.RIGHT\_OUTER\_JOIN, QBJoin.FULL\_JOIN

**Returns**\
[QBJoin](qbjoin.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
 /** @type {QBJoin<db:/example_data/order_details>} */
	var join = query.joins.add('db:/example_data/order_details', QBJoin.INNER_JOIN, 'odetail')
	join.on.add(join.columns.orderid.eq(query.columns.orderid))
 // to add a join based on a relation, use the relation name
 var join2 = query.joins.add('orders_to_customers', 'cust')
	query.where.add(join2.columns.customerid.eq(999))
	foundset.loadRecords(query)
```

### add(dataSource, joinType, alias)

Add a join clause from the parent query builder part to the specified data source.

**Parameters**\
[String](../js-lib/string.md) dataSource data source\
[Number](../js-lib/number.md) joinType join type, one of IQueryBuilderJoin#LEFT\_OUTER\_JOIN, IQueryBuilderJoin#INNER\_JOIN, IQueryBuilderJoin#RIGHT\_OUTER\_JOIN, IQueryBuilderJoin#FULL\_JOIN\
[String](../js-lib/string.md) alias the alias for joining table

**Returns**\
[QBJoin](qbjoin.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
 /** @type {QBJoin<db:/example_data/order_details>} */
	var join = query.joins.add('db:/example_data/order_details', QBJoin.INNER_JOIN, 'odetail')
	join.on.add(join.columns.orderid.eq(query.columns.orderid))
 // to add a join based on a relation, use the relation name
 var join2 = query.joins.add('orders_to_customers', 'cust')
	query.where.add(join2.columns.customerid.eq(999))
	foundset.loadRecords(query)
```

### add(dataSourceOrRelation, alias)

Add a join based on relation or add a manual join. When dataSourceOrRelation is a relation name, a join will be added based on the relation. When dataSourceOrRelation is a data source, an empty join will be added with join type IQueryBuilderJoin#LEFT\_OUTER\_JOIN.

**Parameters**\
[String](../js-lib/string.md) dataSourceOrRelation data source\
[String](../js-lib/string.md) alias the alias for joining table

**Returns**\
[QBJoin](qbjoin.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
 /** @type {QBJoin<db:/example_data/order_details>} */
	var join = query.joins.add('db:/example_data/order_details', QBJoin.INNER_JOIN, 'odetail')
	join.on.add(join.columns.orderid.eq(query.columns.orderid))
 // to add a join based on a relation, use the relation name
 var join2 = query.joins.add('orders_to_customers', 'cust')
	query.where.add(join2.columns.customerid.eq(999))
	foundset.loadRecords(query)
```

### getJoins()

**Returns**\
[Array](../js-lib/array.md)

**Sample**

```javascript
```

### removeUnused(keepInnerjoins)

Remove the joins that are not used anywhere in the query.

**Parameters**\
[Boolean](../js-lib/boolean.md) keepInnerjoins when true inner joins are not removed, inner joins may impact the query result, even when not used

**Returns**\
[QBJoins](qbjoins.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect()
 // a joins is added from the relation
 query.sort.add(query.joins.orders_to_detail.columns.price.sum.asc)
 // clearing the sort does not remove the joins
 query.sort.clear()
 // remove the unused joins
 query.joins.removeUnused(false)
```
