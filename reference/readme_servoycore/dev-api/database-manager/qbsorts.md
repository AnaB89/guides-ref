# QBSorts

## Property Summary

| Type                    | Name                        | Summary                                                                       |
| ----------------------- | --------------------------- | ----------------------------------------------------------------------------- |
| [QBSelect](qbselect.md) | [parent](qbsorts.md#parent) | Get query builder parent table clause, this may be a query or a join clause.. |
| [QBSelect](qbselect.md) | [root](qbsorts.md#root)     | Get query builder parent..                                                    |

## Methods Summary

| Type                  | Name                                                   | Summary                                                                      |
| --------------------- | ------------------------------------------------------ | ---------------------------------------------------------------------------- |
| [QBSorts](qbsorts.md) | [add(columnSortAsc)](qbsorts.md#add-columnsortasc)     | Ad an ascending sorting on a column to the query sort..                      |
| [QBSorts](qbsorts.md) | [add(functionSortAsc)](qbsorts.md#add-functionsortasc) | Ad an ascending sorting on a column to the query sort..                      |
| [QBSorts](qbsorts.md) | [add(sort)](qbsorts.md#add-sort)                       | Ad a sorting on a column to the query sort..                                 |
| [QBSorts](qbsorts.md) | [addPk()](qbsorts.md#addpk)                            | Add the tables' primary pk columns in alphabetical order to the query sort.. |
| [QBSorts](qbsorts.md) | [clear()](qbsorts.md#clear)                            | Clear the sorting clause for the query..                                     |

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

## Methods Details

### add(columnSortAsc)

Ad an ascending sorting on a column to the query sort.

**Parameters**\
[QBColumn](qbcolumn.md) columnSortAsc column to sort by

**Returns**\
[QBSorts](qbsorts.md)

**Sample**

```javascript
query.sort.add(query.columns.orderid)
```

### add(functionSortAsc)

Ad an ascending sorting on a column to the query sort.

**Parameters**\
[QBColumn](qbcolumn.md) functionSortAsc function to add

**Returns**\
[QBSorts](qbsorts.md)

**Sample**

```javascript
query.sort.add(query.columns.orderid)
```

### add(sort)

Ad a sorting on a column to the query sort.

**Parameters**\
[QBSort](qbsort.md) sort the sort to add

**Returns**\
[QBSorts](qbsorts.md)

**Sample**

```javascript
query.sort.add(query.columns.orderid.desc)
```

### addPk()

Add the tables' primary pk columns in alphabetical order to the query sort.

**Returns**\
[QBSorts](qbsorts.md)

**Sample**

```javascript
query.sort.addPk()
```

### clear()

Clear the sorting clause for the query.

**Returns**\
[QBSorts](qbsorts.md)

**Sample**

```javascript
query.sort.clear()
```
