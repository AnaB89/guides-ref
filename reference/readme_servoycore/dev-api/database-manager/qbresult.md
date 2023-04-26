# QBResult

## Property Summary

| Type                            | Name                             | Summary                                                                       |
| ------------------------------- | -------------------------------- | ----------------------------------------------------------------------------- |
| [Boolean](../js-lib/boolean.md) | [distinct](qbresult.md#distinct) | Get/set the distinct flag for the query..                                     |
| [QBSelect](qbselect.md)         | [parent](qbresult.md#parent)     | Get query builder parent table clause, this may be a query or a join clause.. |
| [QBSelect](qbselect.md)         | [root](qbresult.md#root)         | Get query builder parent..                                                    |

## Methods Summary

| Type                        | Name                                                                                      | Summary                                                                          |
| --------------------------- | ----------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| [QBResult](qbresult.md)     | [add(aggregate)](qbresult.md#add-aggregate)                                               | Add an aggregate to the query result..                                           |
| [QBResult](qbresult.md)     | [add(aggregate, alias)](qbresult.md#add-aggregate-alias)                                  | Add an aggregate with alias to the query result..                                |
| [QBResult](qbresult.md)     | [add(column)](qbresult.md#add-column)                                                     | Add a column to the query result..                                               |
| [QBResult](qbresult.md)     | [add(column, alias)](qbresult.md#add-column-alias)                                        | Add a column with alias to the query result..                                    |
| [QBResult](qbresult.md)     | [add(func)](qbresult.md#add-func)                                                         | Add a function result to the query result..                                      |
| [QBResult](qbresult.md)     | [add(func, alias)](qbresult.md#add-func-alias)                                            | Add a function with alias result to the query result..                           |
| [QBResult](qbresult.md)     | [add(qcase)](qbresult.md#add-qcase)                                                       | Add a case searched expression to the query result..                             |
| [QBResult](qbresult.md)     | [add(qcase, alias)](qbresult.md#add-qcase-alias)                                          | Add a case searched expression with alias to the query result..                  |
| [QBResult](qbresult.md)     | [addPk()](qbresult.md#addpk)                                                              | Add the tables' primary pk columns in alphabetical order to the query result..   |
| [QBResult](qbresult.md)     | [addSubSelect(query)](qbresult.md#addsubselect-query)                                     | Add a query to the query result..                                                |
| [QBResult](qbresult.md)     | [addSubSelect(query, alias)](qbresult.md#addsubselect-query-alias)                        | Add a query with alias to the query result..                                     |
| [QBResult](qbresult.md)     | [addSubSelect(customQuery, args)](qbresult.md#addsubselect-customquery-args)              | Add a custom subquery to the query result..                                      |
| [QBResult](qbresult.md)     | [addSubSelect(customQuery, args, alias)](qbresult.md#addsubselect-customquery-args-alias) | Add a custom subquery with alias to the query result..                           |
| [QBResult](qbresult.md)     | [addValue(value)](qbresult.md#addvalue-value)                                             | Add a value to the query result..                                                |
| [QBResult](qbresult.md)     | [addValue(value, alias)](qbresult.md#addvalue-value-alias)                                | Add a value with an alias to the query result..                                  |
| [QBResult](qbresult.md)     | [clear()](qbresult.md#clear)                                                              | Clear the columns in the query result..                                          |
| [Array](../js-lib/array.md) | [getColumns()](qbresult.md#getcolumns)                                                    | returns an array with all the columns that will be in the select of this query.. |

## Properties Details

### distinct

Get/set the distinct flag for the query.

**Returns**\
[Boolean](../js-lib/boolean.md)

**Sample**

```javascript
query.result.distinct = true
```

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

## Methods Details

### add(aggregate)

Add an aggregate to the query result.

**Parameters**\
[QBColumn](qbcolumn.md) aggregate the aggregate to add to result

**Returns**\
[QBResult](qbresult.md)

**Sample**

```javascript
query.result.add(query.columns.label_text.max)
```

### add(aggregate, alias)

Add an aggregate with alias to the query result.

**Parameters**\
[QBColumn](qbcolumn.md) aggregate the aggregate to add to result\
[String](../js-lib/string.md) alias aggregate alias

**Returns**\
[QBResult](qbresult.md)

**Sample**

```javascript
query.result.add(query.columns.item_count.max, 'maximum_items')
```

### add(column)

Add a column to the query result.

**Parameters**\
[QBColumn](qbcolumn.md) column column to add to result

**Returns**\
[QBResult](qbresult.md)

**Sample**

```javascript
query.result.add(query.columns.custname)
```

### add(column, alias)

Add a column with alias to the query result.

**Parameters**\
[QBColumn](qbcolumn.md) column column to add to result\
[String](../js-lib/string.md) alias column alias

**Returns**\
[QBResult](qbresult.md)

**Sample**

```javascript
query.result.add(query.columns.custname, 'customer_name')
```

### add(func)

Add a function result to the query result.

**Parameters**\
[QBColumn](qbcolumn.md) func the function to add to the result

**Returns**\
[QBResult](qbresult.md)

**Sample**

```javascript
query.result.add(query.columns.custname.upper())
```

### add(func, alias)

Add a function with alias result to the query result.

**Parameters**\
[QBColumn](qbcolumn.md) func the function to add to the result\
[String](../js-lib/string.md) alias function alias

**Returns**\
[QBResult](qbresult.md)

**Sample**

```javascript
query.result.add(query.columns.custname.upper(), 'customer_name')
```

### add(qcase)

Add a case searched expression to the query result.

**Parameters**\
[QBColumn](qbcolumn.md) qcase The searched case expression.

**Returns**\
[QBResult](qbresult.md)

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

### add(qcase, alias)

Add a case searched expression with alias to the query result.

**Parameters**\
[QBColumn](qbcolumn.md) qcase The searched case expression.\
[String](../js-lib/string.md) alias function alias

**Returns**\
[QBResult](qbresult.md)

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

### addPk()

Add the tables' primary pk columns in alphabetical order to the query result.

**Returns**\
[QBResult](qbresult.md)

**Sample**

```javascript
query.result.addPk()
```

### addSubSelect(query)

Add a query to the query result.

**Parameters**\
[QBSelect](qbselect.md) query query to add to result

**Returns**\
[QBResult](qbresult.md)

**Sample**

```javascript
// make sure the query returns exactly 1 value.
query.result.addSubSelect(subquery);
```

### addSubSelect(query, alias)

Add a query with alias to the query result.

**Parameters**\
[QBSelect](qbselect.md) query query to add to result\
[String](../js-lib/string.md) alias result alias

**Returns**\
[QBResult](qbresult.md)

**Sample**

```javascript
// make sure the query returns exactly 1 value.
query.result.addSubSelect(subquery, "mx");
```

### addSubSelect(customQuery, args)

Add a custom subquery to the query result.

**Parameters**\
[String](../js-lib/string.md) customQuery query to add to result\
[Array](../js-lib/array.md) args arguments to the query

**Returns**\
[QBResult](qbresult.md)

**Sample**

```javascript
// make sure the subquery returns exactly 1 value.
// select (select max from othertab where val = 'test') from tab
query.result.addSubSelect("select max(field) from othertab where val = ?", ["test"]);
```

### addSubSelect(customQuery, args, alias)

Add a custom subquery with alias to the query result.

**Parameters**\
[String](../js-lib/string.md) customQuery query to add to result\
[Array](../js-lib/array.md) args arguments to the query\
[String](../js-lib/string.md) alias result alias

**Returns**\
[QBResult](qbresult.md)

**Sample**

```javascript
// make sure the subquery returns exactly 1 value.
// select (select max from othertab where val = 'test') as mx from tab
query.result.addSubSelect("select max from othertab where val = ?", ["test"], "mx");
```

### addValue(value)

Add a value to the query result.

**Parameters**\
[Object](../js-lib/object.md) value value add to result

**Returns**\
[QBResult](qbresult.md)

**Sample**

```javascript
query.result.addValue(100)
```

### addValue(value, alias)

Add a value with an alias to the query result.

**Parameters**\
[Object](../js-lib/object.md) value value add to result\
[String](../js-lib/string.md) alias value alias

**Returns**\
[QBResult](qbresult.md)

**Sample**

```javascript
query.result.addValue(100, 'myvalue')
```

### clear()

Clear the columns in the query result.

**Returns**\
[QBResult](qbresult.md)

**Sample**

```javascript
query.result.clear()
```

### getColumns()

returns an array with all the columns that will be in the select of this query. can return empty array. Then the system will auto append the pk when this query is used.

**Returns**\
[Array](../js-lib/array.md) An array of QBColumn thats in the select of this query.

**Sample**

```javascript
var columns = query.result.getColumns();
```
