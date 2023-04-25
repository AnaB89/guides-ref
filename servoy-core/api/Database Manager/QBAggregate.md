#  QBAggregate


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [QBColumn](./QBColumn.md) | [abs](QBAggregate.md#abs)                   | Create abs(column) expression.                                    |
| [QBSort](./QBSort.md) | [asc](QBAggregate.md#asc)                   | Create an ascending sort expression.                                    |
| [QBColumn](./QBColumn.md) | [avg](QBAggregate.md#avg)                   | Create an aggregate expression..                                    |
| [QBColumn](./QBColumn.md) | [bit_length](QBAggregate.md#bit_length)                   | Create bit_length(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [ceil](QBAggregate.md#ceil)                   | Create ceil(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [count](QBAggregate.md#count)                   | Create an aggregate expression..                                    |
| [QBColumn](./QBColumn.md) | [day](QBAggregate.md#day)                   | Extract day from date.                                    |
| [QBSort](./QBSort.md) | [desc](QBAggregate.md#desc)                   | Create an descending sort expression.                                    |
| [QBColumn](./QBColumn.md) | [distinct](QBAggregate.md#distinct)                   | Add a distinct qualifier to the aggregate.                                    |
| [QBColumn](./QBColumn.md) | [floor](QBAggregate.md#floor)                   | Create floor(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [hour](QBAggregate.md#hour)                   | Extract hour from date.                                    |
| [QBCondition](./QBCondition.md) | [isNull](QBAggregate.md#isNull)                   | Compare column with null..                                    |
| [QBColumn](./QBColumn.md) | [len](QBAggregate.md#len)                   | Create length(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [lower](QBAggregate.md#lower)                   | Create lower(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [max](QBAggregate.md#max)                   | Create an aggregate expression..                                    |
| [QBColumn](./QBColumn.md) | [min](QBAggregate.md#min)                   | Create an aggregate expression..                                    |
| [QBColumn](./QBColumn.md) | [minute](QBAggregate.md#minute)                   | Extract minute from date.                                    |
| [QBColumn](./QBColumn.md) | [month](QBAggregate.md#month)                   | Extract month from date.                                    |
| [QBColumn](./QBColumn.md) | [not](QBAggregate.md#not)                   | Create a negated condition..                                    |
| [QBTableClause](./QBTableClause.md) | [parent](QBAggregate.md#parent)                   | Get query builder parent table clause, this may be a query or a join clause..                                    |
| [QBSelect](./QBSelect.md) | [root](QBAggregate.md#root)                   | Get query builder parent..                                    |
| [QBColumn](./QBColumn.md) | [round](QBAggregate.md#round)                   | Create round(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [second](QBAggregate.md#second)                   | Extract second from date.                                    |
| [QBColumn](./QBColumn.md) | [sqrt](QBAggregate.md#sqrt)                   | Create sqrt(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [sum](QBAggregate.md#sum)                   | Create an aggregate expression..                                    |
| [QBColumn](./QBColumn.md) | [trim](QBAggregate.md#trim)                   | Create trim(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [upper](QBAggregate.md#upper)                   | Create upper(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [year](QBAggregate.md#year)                   | Extract year from date.                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [QBCondition](./QBCondition.md) | [between(value1, value2)](QBAggregate.md#between-value1-value2)                   | Compare column to a range of 2 values or other columns..                                    |
| [QBColumn](./QBColumn.md) | [cast(type)](QBAggregate.md#cast-type)                   | Create cast(column, type) expression.                                    |
| [QBColumn](./QBColumn.md) | [concat(arg)](QBAggregate.md#concat-arg)                   | Concatename with value.                                    |
| [QBColumn](./QBColumn.md) | [divide(arg)](QBAggregate.md#divide-arg)                   | Divide by value.                                    |
| [QBCondition](./QBCondition.md) | [eq(value)](QBAggregate.md#eq-value)                   | Compare column with a value or another column..                                    |
| [QBCondition](./QBCondition.md) | [ge(value)](QBAggregate.md#ge-value)                   | Compare column with a value or another column..                                    |
| [Number](../JSLib/Number.md) | [getFlags()](QBAggregate.md#getflags)                   | The flags are a bit pattern consisting of 1 or more of the following bits:  - JSColumn..                                    |
| [String](../JSLib/String.md) | [getTypeAsString()](QBAggregate.md#gettypeasstring)                   | Column type as a string.                                    |
| [QBCondition](./QBCondition.md) | [gt(value)](QBAggregate.md#gt-value)                   | Compare column with a value or another column..                                    |
| [QBCondition](./QBCondition.md) | [isin(query)](QBAggregate.md#isin-query)                   | Compare column with subquery result..                                    |
| [QBCondition](./QBCondition.md) | [isin(values)](QBAggregate.md#isin-values)                   | Compare column with values..                                    |
| [QBCondition](./QBCondition.md) | [isin(customQuery, args)](QBAggregate.md#isin-customquery-args)                   | Compare column with custom query result..                                    |
| [QBCondition](./QBCondition.md) | [le(value)](QBAggregate.md#le-value)                   | Compare column with a value or another column..                                    |
| [QBCondition](./QBCondition.md) | [like(pattern)](QBAggregate.md#like-pattern)                   | Compare column with a value or another column..                                    |
| [QBCondition](./QBCondition.md) | [like(pattern, escape)](QBAggregate.md#like-pattern-escape)                   | Compare column with a value or another column..                                    |
| [QBColumn](./QBColumn.md) | [locate(arg)](QBAggregate.md#locate-arg)                   | Create locate(arg) expression.                                    |
| [QBColumn](./QBColumn.md) | [locate(arg, start)](QBAggregate.md#locate-arg-start)                   | Create locate(arg, start) expression.                                    |
| [QBCondition](./QBCondition.md) | [lt(value)](QBAggregate.md#lt-value)                   | Compare column with a value or another column..                                    |
| [QBColumn](./QBColumn.md) | [minus(arg)](QBAggregate.md#minus-arg)                   | Subtract value.                                    |
| [QBColumn](./QBColumn.md) | [mod(arg)](QBAggregate.md#mod-arg)                   | Create mod(arg) expression.                                    |
| [QBColumn](./QBColumn.md) | [multiply(arg)](QBAggregate.md#multiply-arg)                   | Multiply with value.                                    |
| [QBColumn](./QBColumn.md) | [nullif(arg)](QBAggregate.md#nullif-arg)                   | Create nullif(arg) expression.                                    |
| [QBColumn](./QBColumn.md) | [plus(arg)](QBAggregate.md#plus-arg)                   | Add up value.                                    |
| [QBColumn](./QBColumn.md) | [substring(pos)](QBAggregate.md#substring-pos)                   | Create substring(pos) expression.                                    |
| [QBColumn](./QBColumn.md) | [substring(pos, len)](QBAggregate.md#substring-pos-len)                   | Create substring(pos, len) expression.                                    |

## Properties Details

### abs

Create abs(column) expression

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.custname.abs)
```
### asc

Create an ascending sort expression

**Returns**\
[QBSort](./QBSort.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.sort
.add(query.joins.orders_to_order_details.columns.quantity.asc)
.add(query.columns.companyid)
foundset.loadRecords(query)
```
### avg

Create an aggregate expression.

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
	query.groupBy.addPk() // have to group by on pk when using having-conditions in (foundset) pk queries
	.root.having.add(query.joins.orders_to_order_details.columns.quantity.avg.eq(1))
	foundset.loadRecords(query)
```
### bit_length

Create bit_length(column) expression

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.custname.bit_length)
```
### ceil

Create ceil(column) expression

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mycol.ceil)
```
### count

Create an aggregate expression.

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
	query.groupBy.addPk() // have to group by on pk when using having-conditions in (foundset) pk queries
	.root.having.add(query.joins.orders_to_order_details.columns.quantity.count.eq(0))
	foundset.loadRecords(query)
```
### day

Extract day from date

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mydatecol.day)
```
### desc

Create an descending sort expression

**Returns**\
[QBSort](./QBSort.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.sort
.add(query.joins.orders_to_order_details.columns.quantity.desc)
.add(query.columns.companyid)
foundset.loadRecords(query)
```
### distinct

Add a distinct qualifier to the aggregate

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
// count the number of countries that we ship orders to
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.columns.shipcountry.count.distinct);
```
### floor

Create floor(column) expression

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mycol.floor)
```
### hour

Extract hour from date

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mydatecol.hour)
```
### isNull

Compare column with null.

**Returns**\
[QBCondition](./QBCondition.md) 


**Sample**

```javascript
query.where.add(query.columns.flag.isNull)
```
### len

Create length(column) expression

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.custname.len)
```
### lower

Create lower(column) expression

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.custname.lower)
```
### max

Create an aggregate expression.

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
	query.groupBy.addPk() // have to group by on pk when using having-conditions in (foundset) pk queries
	.root.having.add(query.joins.orders_to_order_details.columns.quantity.count.max(10))
	foundset.loadRecords(query)
```
### min

Create an aggregate expression.

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
	query.groupBy.addPk() // have to group by on pk when using having-conditions in (foundset) pk queries
	.root.having.add(query.joins.orders_to_order_details.columns.quantity.count.min(10))
	foundset.loadRecords(query)
```
### minute

Extract minute from date

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mydatecol.minute)
```
### month

Extract month from date

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mydatecol.month)
```
### not

Create a negated condition.

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.where.add(query.columns.flag.not.eq(1))
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
### round

Create round(column) expression

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mycol.round)
```
### second

Extract second from date

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mydatecol.second)
```
### sqrt

Create sqrt(column) expression

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.custname.sqrt)
```
### sum

Create an aggregate expression.

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
	query.groupBy.addPk() // have to group by on pk when using having-conditions in (foundset) pk queries
	.root.having.add(query.joins.orders_to_order_details.columns.quantity.count.sum(10))
	foundset.loadRecords(query)
```
### trim

Create trim(column) expression

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.custname.trim)
```
### upper

Create upper(column) expression

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.custname.upper)
```
### year

Extract year from date

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mydatecol.year)
```

## Methods Details

### between(value1, value2)

Compare column to a range of 2 values or other columns.

**Parameters**\
[Object](../JSLib/Object.md) value1  ;\
[Object](../JSLib/Object.md) value2  ;

**Returns**\
[QBCondition](./QBCondition.md) 


**Sample**

```javascript
query.where.add(query.columns.flag.between(0, 5))
```
### cast(type)

Create cast(column, type) expression

**Parameters**\
[String](../JSLib/String.md) type string type, see QUERY_COLUMN_TYPES

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mycol.cast(QUERY_COLUMN_TYPES.TYPE_INTEGER))
```
### concat(arg)

Concatename with value

**Parameters**\
[Object](../JSLib/Object.md) arg valeu to concatenate with

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.firstname.concat(' ').concat(query.columns.lastname))
```
### divide(arg)

Divide by value

**Parameters**\
[Object](../JSLib/Object.md) arg nr to divide by

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mycol.divide(2))
```
### eq(value)

Compare column with a value or another column.
Operator: equals

**Parameters**\
[Object](../JSLib/Object.md) value  ;

**Returns**\
[QBCondition](./QBCondition.md) 


**Sample**

```javascript
query.where.add(query.columns.flag.eq(1))
```
### ge(value)

Compare column with a value or another column.
Operator: greaterThanOrEqual

**Parameters**\
[Object](../JSLib/Object.md) value  ;

**Returns**\
[QBCondition](./QBCondition.md) 


**Sample**

```javascript
query.where.add(query.columns.flag.ge(2))
```
### getFlags()

The flags are a bit pattern consisting of 1 or more of the following bits:
 - JSColumn.UUID_COLUMN
 - JSColumn.EXCLUDED_COLUMN
 - JSColumn.TENANT_COLUMN


**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```
### getTypeAsString()

Column type as a string


**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### gt(value)

Compare column with a value or another column.
Operator: greaterThan

**Parameters**\
[Object](../JSLib/Object.md) value  ;

**Returns**\
[QBCondition](./QBCondition.md) 


**Sample**

```javascript
query.where.add(query.columns.flag.gt(0))
```
### isin(query)

Compare column with subquery result.

**Parameters**\
[QBPart](./QBPart.md) query subquery

**Returns**\
[QBCondition](./QBCondition.md) 


**Sample**

```javascript
query.where.add(query.columns.flag.isin(query2))
```
### isin(values)

Compare column with values.

**Parameters**\
[Array](../JSLib/Array.md) values array of values

**Returns**\
[QBCondition](./QBCondition.md) 


**Sample**

```javascript
query.where.add(query.columns.flag.isin([1, 5, 99]))
```
### isin(customQuery, args)

Compare column with custom query result.

**Parameters**\
[String](../JSLib/String.md) customQuery custom query\
[Array](../JSLib/Array.md) args query arguments

**Returns**\
[QBCondition](./QBCondition.md) 


**Sample**

```javascript
query.where.add(query.columns.ccy.isin("select ccycode from currencies c where c.category = " + query.getTableAlias() + ".currency_category and c.flag = ?", ['T']))
```
### le(value)

Compare column with a value or another column.
Operator: lessThanOrEqual

**Parameters**\
[Object](../JSLib/Object.md) value  ;

**Returns**\
[QBCondition](./QBCondition.md) 


**Sample**

```javascript
query.where.add(query.columns.flag.le(2))
```
### like(pattern)

Compare column with a value or another column.
Operator: like

**Parameters**\
[Object](../JSLib/Object.md) pattern the string value of the pattern

**Returns**\
[QBCondition](./QBCondition.md) 


**Sample**

```javascript
query.where.add(query.columns.companyname.like('Serv%'))

// case-insensitive compares can be done using the upper (or lower) functions,
// this can be useful when using for example German letters like ß,
query.where.add(query.columns.companyname.upper.like(query.functions.upper('groß%')))
```
### like(pattern, escape)

Compare column with a value or another column.
Operator: like, with escape character

**Parameters**\
[Object](../JSLib/Object.md) pattern the string value of the pattern\
[Number](../JSLib/Number.md) escape the escape char

**Returns**\
[QBCondition](./QBCondition.md) 


**Sample**

```javascript
query.where.add(query.columns.companyname.like('X_%', '_'))
```
### locate(arg)

Create locate(arg) expression

**Parameters**\
[Object](../JSLib/Object.md) arg string to locate

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mycol.locate('sample'))
```
### locate(arg, start)

Create locate(arg, start) expression

**Parameters**\
[Object](../JSLib/Object.md) arg string to locate\
[Number](../JSLib/Number.md) start start pos

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mycol.locate('sample', 5))
```
### lt(value)

Compare column with a value or another column.
Operator: lessThan

**Parameters**\
[Object](../JSLib/Object.md) value  ;

**Returns**\
[QBCondition](./QBCondition.md) 


**Sample**

```javascript
query.where.add(query.columns.flag.lt(99))
```
### minus(arg)

Subtract value

**Parameters**\
[Object](../JSLib/Object.md) arg nr to subtract

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mycol.minus(2))
```
### mod(arg)

Create mod(arg) expression

**Parameters**\
[Object](../JSLib/Object.md) arg mod arg

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mycol.mod(2))
```
### multiply(arg)

Multiply with value

**Parameters**\
[Object](../JSLib/Object.md) arg nr to multiply with

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mycol.multiply(2))
```
### nullif(arg)

Create nullif(arg) expression

**Parameters**\
[Object](../JSLib/Object.md) arg object to compare

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mycol.nullif('none'))
```
### plus(arg)

Add up value

**Parameters**\
[Object](../JSLib/Object.md) arg nr to add

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mycol.plus(2))
```
### substring(pos)

Create substring(pos) expression

**Parameters**\
[Number](../JSLib/Number.md) pos  ;

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mycol.substring(3))
```
### substring(pos, len)

Create substring(pos, len) expression

**Parameters**\
[Number](../JSLib/Number.md) pos  ;\
[Number](../JSLib/Number.md) len  ;

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
query.result.add(query.columns.mycol.substring(3, 2))
```

