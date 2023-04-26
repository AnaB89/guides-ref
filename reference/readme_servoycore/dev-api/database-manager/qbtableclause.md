# QBTableClause

## Property Summary

| Type                                                                     | Name                                | Summary                                                                                         |
| ------------------------------------------------------------------------ | ----------------------------------- | ----------------------------------------------------------------------------------------------- |
| [QBColumns](../../../../servoy-core/api/Database%20Manager/QBColumns.md) | [columns](qbtableclause.md#columns) | Get all the columns of the datasource that can be used for this query (select or where clause). |
| [QBJoins](qbjoins.md)                                                    | [joins](qbtableclause.md#joins)     | Get the joins clause of this table based clause..                                               |
| [QBTableClause](qbtableclause.md)                                        | [parent](qbtableclause.md#parent)   | Get query builder parent table clause, this may be a query or a join clause..                   |
| [QBSelect](qbselect.md)                                                  | [root](qbtableclause.md#root)       | Get query builder parent..                                                                      |

## Methods Summary

| Type                          | Name                                                                                  | Summary                                        |
| ----------------------------- | ------------------------------------------------------------------------------------- | ---------------------------------------------- |
| [QBColumn](qbcolumn.md)       | [getColumn(name)](qbtableclause.md#getcolumn-name)                                    | Get a column from the table..                  |
| [QBColumn](qbcolumn.md)       | [getColumn(columnTableAlias, name)](qbtableclause.md#getcolumn-columntablealias-name) | Get a column from the table with given alias.. |
| [String](../js-lib/string.md) | [getDataSource()](qbtableclause.md#getdatasource)                                     | Returns the datasource for this..              |
| [String](../js-lib/string.md) | [getTableAlias()](qbtableclause.md#gettablealias)                                     | Returns the table alias for this..             |

## Properties Details

### columns

Get all the columns of the datasource that can be used for this query (select or where clause)

**Returns**\
[QBColumns](../../../../servoy-core/api/Database%20Manager/QBColumns.md)

**Sample**

```javascript
var query = foundset.getQuery();
query.result.add(query.columns.name, "name");
query.where.add(query.columns.orderdate.isNull)
```

### joins

Get the joins clause of this table based clause. Joins added to this clause will be based on this table clauses table.

**Returns**\
[QBJoins](qbjoins.md)

**Sample**

```javascript
foundset.getQuery().joins
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

### getColumn(name)

Get a column from the table.

**Parameters**\
[String](../js-lib/string.md) name the name of column to get

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
foundset.getQuery().getColumn('orderid')
```

### getColumn(columnTableAlias, name)

Get a column from the table with given alias. The alias may be of the main table or any level deep joined table.

**Parameters**\
[String](../js-lib/string.md) columnTableAlias the alias for the table\
[String](../js-lib/string.md) name the name of column to get

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
foundset.getQuery().getColumn('orderid', 'opk')
```

### getDataSource()

Returns the datasource for this.

**Returns**\
[String](../js-lib/string.md) the dataSource

**Sample**

```javascript
```

### getTableAlias()

Returns the table alias for this.

**Returns**\
[String](../js-lib/string.md) the tableAlias

**Sample**

```javascript
```
