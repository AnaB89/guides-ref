#  QBSorts

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [QBSelect](./QBSelect.md) | [parent](QBSorts.md#parent)                   | Get query builder parent table clause, this may be a query or a join clause..                                    |
| [QBSelect](./QBSelect.md) | [root](QBSorts.md#root)                   | Get query builder parent..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [QBSorts](./QBSorts.md) | [add(columnSortAsc)](QBSorts.md#add-columnsortasc)                   | Ad an ascending sorting on a column to the query sort..                                    |
| [QBSorts](./QBSorts.md) | [add(functionSortAsc)](QBSorts.md#add-functionsortasc)                   | Ad an ascending sorting on a column to the query sort..                                    |
| [QBSorts](./QBSorts.md) | [add(sort)](QBSorts.md#add-sort)                   | Ad a sorting on a column to the query sort..                                    |
| [QBSorts](./QBSorts.md) | [addPk()](QBSorts.md#addpk)                   | Add the tables' primary pk columns in alphabetical order to the query sort..                                    |
| [QBSorts](./QBSorts.md) | [clear()](QBSorts.md#clear)                   | Clear the sorting clause for the query..                                    |

## Properties Details

### parent

Get query builder parent table clause, this may be a query or a join clause.

**Returns**\
[QBSelect](./QBSelect.md) 

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

### add(columnSortAsc)

Ad an ascending sorting on a column to the query sort.

**Parameters**\
[QBColumn](./QBColumn.md) columnSortAsc column to sort by

**Returns**\
[QBSorts](./QBSorts.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
query.sort.add(query.columns.orderid)
```
### add(functionSortAsc)

Ad an ascending sorting on a column to the query sort.

**Parameters**\
[QBColumn](./QBColumn.md) functionSortAsc function to add

**Returns**\
[QBSorts](./QBSorts.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
query.sort.add(query.columns.orderid)
```
### add(sort)

Ad a sorting on a column to the query sort.

**Parameters**\
[QBSort](./QBSort.md) sort the sort to add

**Returns**\
[QBSorts](./QBSorts.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
query.sort.add(query.columns.orderid.desc)
```
### addPk()

Add the tables' primary pk columns in alphabetical order to the query sort.


**Returns**\
[QBSorts](./QBSorts.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
query.sort.addPk()
```
### clear()

Clear the sorting clause for the query.


**Returns**\
[QBSorts](./QBSorts.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
query.sort.clear()
```

