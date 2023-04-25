#  QBJoins


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [QBTableClause](./QBTableClause.md) | [parent](QBJoins.md#parent)                   | Get query builder parent table clause, this may be a query or a join clause..                                    |
| [QBSelect](./QBSelect.md) | [root](QBJoins.md#root)                   | Get query builder parent..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [QBJoin](./QBJoin.md) | [add(subqueryBuilder, joinType)](QBJoins.md#add-subquerybuilder-jointype)                   | Add a join clause from the parent query builder part to a derived table based on another query..                                    |
| [QBJoin](./QBJoin.md) | [add(subqueryBuilder, joinType, alias)](QBJoins.md#add-subquerybuilder-jointype-alias)                   | Add a join clause from the parent query builder part to a derived table based on another query..                                    |
| [QBJoin](./QBJoin.md) | [add(dataSource)](QBJoins.md#add-datasource)                   | Add a join with join type IQueryBuilderJoin#LEFT_OUTER_JOIN and no alias for the joining table..                                    |
| [QBJoin](./QBJoin.md) | [add(dataSource, joinType)](QBJoins.md#add-datasource-jointype)                   | Add a join with no alias for the joining table..                                    |
| [QBJoin](./QBJoin.md) | [add(dataSource, joinType, alias)](QBJoins.md#add-datasource-jointype-alias)                   | Add a join clause from the parent query builder part to the specified data source..                                    |
| [QBJoin](./QBJoin.md) | [add(dataSourceOrRelation, alias)](QBJoins.md#add-datasourceorrelation-alias)                   | Add a join based on relation or add a manual join..                                    |
| [Array](../JSLib/Array.md) | [getJoins()](QBJoins.md#getjoins)                   | .                                    |
| [QBJoins](./QBJoins.md) | [removeUnused(keepInnerjoins)](QBJoins.md#removeunused-keepinnerjoins)                   | Remove the joins that are not used anywhere in the query..                                    |

## Properties Details

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

### add(subqueryBuilder, joinType)

Add a join clause from the parent query builder part to a derived table based on another query.

**Parameters**\
[QBSelect](./QBSelect.md) subqueryBuilder  ;\
[Number](../JSLib/Number.md) joinType  ;

**Returns**\
[QBJoin](./QBJoin.md) 


**Sample**

```javascript

```
### add(subqueryBuilder, joinType, alias)

Add a join clause from the parent query builder part to a derived table based on another query.

**Parameters**\
[QBSelect](./QBSelect.md) subqueryBuilder  ;\
[Number](../JSLib/Number.md) joinType  ;\
[String](../JSLib/String.md) alias  ;

**Returns**\
[QBJoin](./QBJoin.md) 


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

Add a join with join type IQueryBuilderJoin#LEFT_OUTER_JOIN and no alias for the joining table.

**Parameters**\
[String](../JSLib/String.md) dataSource data source

**Returns**\
[QBJoin](./QBJoin.md) 


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
[String](../JSLib/String.md) dataSource data source\
[Number](../JSLib/Number.md) joinType join type, one of QBJoin.LEFT_OUTER_JOIN, QBJoin.INNER_JOIN, QBJoin.RIGHT_OUTER_JOIN, QBJoin.FULL_JOIN

**Returns**\
[QBJoin](./QBJoin.md) 


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
[String](../JSLib/String.md) dataSource data source\
[Number](../JSLib/Number.md) joinType join type, one of IQueryBuilderJoin#LEFT_OUTER_JOIN, IQueryBuilderJoin#INNER_JOIN, IQueryBuilderJoin#RIGHT_OUTER_JOIN, IQueryBuilderJoin#FULL_JOIN\
[String](../JSLib/String.md) alias the alias for joining table

**Returns**\
[QBJoin](./QBJoin.md) 


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

Add a join based on relation or add a manual join.
When dataSourceOrRelation is a relation name, a join will be added based on the relation.
When dataSourceOrRelation is a data source, an empty join will be added with join type IQueryBuilderJoin#LEFT_OUTER_JOIN.

**Parameters**\
[String](../JSLib/String.md) dataSourceOrRelation data source\
[String](../JSLib/String.md) alias the alias for joining table

**Returns**\
[QBJoin](./QBJoin.md) 


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
[Array](../JSLib/Array.md) 


**Sample**

```javascript

```
### removeUnused(keepInnerjoins)

Remove the joins that are not used anywhere in the query.

**Parameters**\
[Boolean](../JSLib/Boolean.md) keepInnerjoins when true inner joins are not removed, inner joins may impact the query result, even when not used

**Returns**\
[QBJoins](./QBJoins.md) 


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

