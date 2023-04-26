# QBAggregate

## Property Summary

| Type                              | Name                                      | Summary                                                                       |
| --------------------------------- | ----------------------------------------- | ----------------------------------------------------------------------------- |
| [QBColumn](qbcolumn.md)           | [abs](qbaggregate.md#abs)                 | Create abs(column) expression.                                                |
| [QBSort](qbsort.md)               | [asc](qbaggregate.md#asc)                 | Create an ascending sort expression.                                          |
| [QBColumn](qbcolumn.md)           | [avg](qbaggregate.md#avg)                 | Create an aggregate expression..                                              |
| [QBColumn](qbcolumn.md)           | [bit\_length](qbaggregate.md#bit\_length) | Create bit\_length(column) expression.                                        |
| [QBColumn](qbcolumn.md)           | [ceil](qbaggregate.md#ceil)               | Create ceil(column) expression.                                               |
| [QBColumn](qbcolumn.md)           | [count](qbaggregate.md#count)             | Create an aggregate expression..                                              |
| [QBColumn](qbcolumn.md)           | [day](qbaggregate.md#day)                 | Extract day from date.                                                        |
| [QBSort](qbsort.md)               | [desc](qbaggregate.md#desc)               | Create an descending sort expression.                                         |
| [QBColumn](qbcolumn.md)           | [distinct](qbaggregate.md#distinct)       | Add a distinct qualifier to the aggregate.                                    |
| [QBColumn](qbcolumn.md)           | [floor](qbaggregate.md#floor)             | Create floor(column) expression.                                              |
| [QBColumn](qbcolumn.md)           | [hour](qbaggregate.md#hour)               | Extract hour from date.                                                       |
| [QBCondition](qbcondition.md)     | [isNull](qbaggregate.md#isNull)           | Compare column with null..                                                    |
| [QBColumn](qbcolumn.md)           | [len](qbaggregate.md#len)                 | Create length(column) expression.                                             |
| [QBColumn](qbcolumn.md)           | [lower](qbaggregate.md#lower)             | Create lower(column) expression.                                              |
| [QBColumn](qbcolumn.md)           | [max](qbaggregate.md#max)                 | Create an aggregate expression..                                              |
| [QBColumn](qbcolumn.md)           | [min](qbaggregate.md#min)                 | Create an aggregate expression..                                              |
| [QBColumn](qbcolumn.md)           | [minute](qbaggregate.md#minute)           | Extract minute from date.                                                     |
| [QBColumn](qbcolumn.md)           | [month](qbaggregate.md#month)             | Extract month from date.                                                      |
| [QBColumn](qbcolumn.md)           | [not](qbaggregate.md#not)                 | Create a negated condition..                                                  |
| [QBTableClause](qbtableclause.md) | [parent](qbaggregate.md#parent)           | Get query builder parent table clause, this may be a query or a join clause.. |
| [QBSelect](qbselect.md)           | [root](qbaggregate.md#root)               | Get query builder parent..                                                    |
| [QBColumn](qbcolumn.md)           | [round](qbaggregate.md#round)             | Create round(column) expression.                                              |
| [QBColumn](qbcolumn.md)           | [second](qbaggregate.md#second)           | Extract second from date.                                                     |
| [QBColumn](qbcolumn.md)           | [sqrt](qbaggregate.md#sqrt)               | Create sqrt(column) expression.                                               |
| [QBColumn](qbcolumn.md)           | [sum](qbaggregate.md#sum)                 | Create an aggregate expression..                                              |
| [QBColumn](qbcolumn.md)           | [trim](qbaggregate.md#trim)               | Create trim(column) expression.                                               |
| [QBColumn](qbcolumn.md)           | [upper](qbaggregate.md#upper)             | Create upper(column) expression.                                              |
| [QBColumn](qbcolumn.md)           | [year](qbaggregate.md#year)               | Extract year from date.                                                       |

## Methods Summary

| Type                          | Name                                                            | Summary                                                                                 |
| ----------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| [QBCondition](qbcondition.md) | [between(value1, value2)](qbaggregate.md#between-value1-value2) | Compare column to a range of 2 values or other columns..                                |
| [QBColumn](qbcolumn.md)       | [cast(type)](qbaggregate.md#cast-type)                          | Create cast(column, type) expression.                                                   |
| [QBColumn](qbcolumn.md)       | [concat(arg)](qbaggregate.md#concat-arg)                        | Concatename with value.                                                                 |
| [QBColumn](qbcolumn.md)       | [divide(arg)](qbaggregate.md#divide-arg)                        | Divide by value.                                                                        |
| [QBCondition](qbcondition.md) | [eq(value)](qbaggregate.md#eq-value)                            | Compare column with a value or another column..                                         |
| [QBCondition](qbcondition.md) | [ge(value)](qbaggregate.md#ge-value)                            | Compare column with a value or another column..                                         |
| [Number](../js-lib/number.md) | [getFlags()](qbaggregate.md#getflags)                           | The flags are a bit pattern consisting of 1 or more of the following bits: - JSColumn.. |
| [String](../js-lib/string.md) | [getTypeAsString()](qbaggregate.md#gettypeasstring)             | Column type as a string.                                                                |
| [QBCondition](qbcondition.md) | [gt(value)](qbaggregate.md#gt-value)                            | Compare column with a value or another column..                                         |
| [QBCondition](qbcondition.md) | [isin(query)](qbaggregate.md#isin-query)                        | Compare column with subquery result..                                                   |
| [QBCondition](qbcondition.md) | [isin(values)](qbaggregate.md#isin-values)                      | Compare column with values..                                                            |
| [QBCondition](qbcondition.md) | [isin(customQuery, args)](qbaggregate.md#isin-customquery-args) | Compare column with custom query result..                                               |
| [QBCondition](qbcondition.md) | [le(value)](qbaggregate.md#le-value)                            | Compare column with a value or another column..                                         |
| [QBCondition](qbcondition.md) | [like(pattern)](qbaggregate.md#like-pattern)                    | Compare column with a value or another column..                                         |
| [QBCondition](qbcondition.md) | [like(pattern, escape)](qbaggregate.md#like-pattern-escape)     | Compare column with a value or another column..                                         |
| [QBColumn](qbcolumn.md)       | [locate(arg)](qbaggregate.md#locate-arg)                        | Create locate(arg) expression.                                                          |
| [QBColumn](qbcolumn.md)       | [locate(arg, start)](qbaggregate.md#locate-arg-start)           | Create locate(arg, start) expression.                                                   |
| [QBCondition](qbcondition.md) | [lt(value)](qbaggregate.md#lt-value)                            | Compare column with a value or another column..                                         |
| [QBColumn](qbcolumn.md)       | [minus(arg)](qbaggregate.md#minus-arg)                          | Subtract value.                                                                         |
| [QBColumn](qbcolumn.md)       | [mod(arg)](qbaggregate.md#mod-arg)                              | Create mod(arg) expression.                                                             |
| [QBColumn](qbcolumn.md)       | [multiply(arg)](qbaggregate.md#multiply-arg)                    | Multiply with value.                                                                    |
| [QBColumn](qbcolumn.md)       | [nullif(arg)](qbaggregate.md#nullif-arg)                        | Create nullif(arg) expression.                                                          |
| [QBColumn](qbcolumn.md)       | [plus(arg)](qbaggregate.md#plus-arg)                            | Add up value.                                                                           |
| [QBColumn](qbcolumn.md)       | [substring(pos)](qbaggregate.md#substring-pos)                  | Create substring(pos) expression.                                                       |
| [QBColumn](qbcolumn.md)       | [substring(pos, len)](qbaggregate.md#substring-pos-len)         | Create substring(pos, len) expression.                                                  |

## Properties Details

### abs

Create abs(column) expression

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.custname.abs)
```

### asc

Create an ascending sort expression

**Returns**\
[QBSort](qbsort.md)

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
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
	query.groupBy.addPk() // have to group by on pk when using having-conditions in (foundset) pk queries
	.root.having.add(query.joins.orders_to_order_details.columns.quantity.avg.eq(1))
	foundset.loadRecords(query)
```

### bit\_length

Create bit\_length(column) expression

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.custname.bit_length)
```

### ceil

Create ceil(column) expression

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mycol.ceil)
```

### count

Create an aggregate expression.

**Returns**\
[QBColumn](qbcolumn.md)

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
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mydatecol.day)
```

### desc

Create an descending sort expression

**Returns**\
[QBSort](qbsort.md)

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
[QBColumn](qbcolumn.md)

**Sample**

```javascript
// count the number of countries that we ship orders to
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.columns.shipcountry.count.distinct);
```

### floor

Create floor(column) expression

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mycol.floor)
```

### hour

Extract hour from date

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mydatecol.hour)
```

### isNull

Compare column with null.

**Returns**\
[QBCondition](qbcondition.md)

**Sample**

```javascript
query.where.add(query.columns.flag.isNull)
```

### len

Create length(column) expression

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.custname.len)
```

### lower

Create lower(column) expression

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.custname.lower)
```

### max

Create an aggregate expression.

**Returns**\
[QBColumn](qbcolumn.md)

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
[QBColumn](qbcolumn.md)

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
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mydatecol.minute)
```

### month

Extract month from date

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mydatecol.month)
```

### not

Create a negated condition.

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.where.add(query.columns.flag.not.eq(1))
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

### round

Create round(column) expression

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mycol.round)
```

### second

Extract second from date

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mydatecol.second)
```

### sqrt

Create sqrt(column) expression

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.custname.sqrt)
```

### sum

Create an aggregate expression.

**Returns**\
[QBColumn](qbcolumn.md)

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
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.custname.trim)
```

### upper

Create upper(column) expression

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.custname.upper)
```

### year

Extract year from date

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mydatecol.year)
```

## Methods Details

### between(value1, value2)

Compare column to a range of 2 values or other columns.

**Parameters**\
[Object](../js-lib/object.md) value1 ;\
[Object](../js-lib/object.md) value2 ;

**Returns**\
[QBCondition](qbcondition.md)

**Sample**

```javascript
query.where.add(query.columns.flag.between(0, 5))
```

### cast(type)

Create cast(column, type) expression

**Parameters**\
[String](../js-lib/string.md) type string type, see QUERY\_COLUMN\_TYPES

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mycol.cast(QUERY_COLUMN_TYPES.TYPE_INTEGER))
```

### concat(arg)

Concatename with value

**Parameters**\
[Object](../js-lib/object.md) arg valeu to concatenate with

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.firstname.concat(' ').concat(query.columns.lastname))
```

### divide(arg)

Divide by value

**Parameters**\
[Object](../js-lib/object.md) arg nr to divide by

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mycol.divide(2))
```

### eq(value)

Compare column with a value or another column. Operator: equals

**Parameters**\
[Object](../js-lib/object.md) value ;

**Returns**\
[QBCondition](qbcondition.md)

**Sample**

```javascript
query.where.add(query.columns.flag.eq(1))
```

### ge(value)

Compare column with a value or another column. Operator: greaterThanOrEqual

**Parameters**\
[Object](../js-lib/object.md) value ;

**Returns**\
[QBCondition](qbcondition.md)

**Sample**

```javascript
query.where.add(query.columns.flag.ge(2))
```

### getFlags()

The flags are a bit pattern consisting of 1 or more of the following bits:

* JSColumn.UUID\_COLUMN
* JSColumn.EXCLUDED\_COLUMN
* JSColumn.TENANT\_COLUMN

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
```

### getTypeAsString()

Column type as a string

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
```

### gt(value)

Compare column with a value or another column. Operator: greaterThan

**Parameters**\
[Object](../js-lib/object.md) value ;

**Returns**\
[QBCondition](qbcondition.md)

**Sample**

```javascript
query.where.add(query.columns.flag.gt(0))
```

### isin(query)

Compare column with subquery result.

**Parameters**\
[QBPart](qbpart.md) query subquery

**Returns**\
[QBCondition](qbcondition.md)

**Sample**

```javascript
query.where.add(query.columns.flag.isin(query2))
```

### isin(values)

Compare column with values.

**Parameters**\
[Array](../js-lib/array.md) values array of values

**Returns**\
[QBCondition](qbcondition.md)

**Sample**

```javascript
query.where.add(query.columns.flag.isin([1, 5, 99]))
```

### isin(customQuery, args)

Compare column with custom query result.

**Parameters**\
[String](../js-lib/string.md) customQuery custom query\
[Array](../js-lib/array.md) args query arguments

**Returns**\
[QBCondition](qbcondition.md)

**Sample**

```javascript
query.where.add(query.columns.ccy.isin("select ccycode from currencies c where c.category = " + query.getTableAlias() + ".currency_category and c.flag = ?", ['T']))
```

### le(value)

Compare column with a value or another column. Operator: lessThanOrEqual

**Parameters**\
[Object](../js-lib/object.md) value ;

**Returns**\
[QBCondition](qbcondition.md)

**Sample**

```javascript
query.where.add(query.columns.flag.le(2))
```

### like(pattern)

Compare column with a value or another column. Operator: like

**Parameters**\
[Object](../js-lib/object.md) pattern the string value of the pattern

**Returns**\
[QBCondition](qbcondition.md)

**Sample**

```javascript
query.where.add(query.columns.companyname.like('Serv%'))

// case-insensitive compares can be done using the upper (or lower) functions,
// this can be useful when using for example German letters like ß,
query.where.add(query.columns.companyname.upper.like(query.functions.upper('groß%')))
```

### like(pattern, escape)

Compare column with a value or another column. Operator: like, with escape character

**Parameters**\
[Object](../js-lib/object.md) pattern the string value of the pattern\
[Number](../js-lib/number.md) escape the escape char

**Returns**\
[QBCondition](qbcondition.md)

**Sample**

```javascript
query.where.add(query.columns.companyname.like('X_%', '_'))
```

### locate(arg)

Create locate(arg) expression

**Parameters**\
[Object](../js-lib/object.md) arg string to locate

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mycol.locate('sample'))
```

### locate(arg, start)

Create locate(arg, start) expression

**Parameters**\
[Object](../js-lib/object.md) arg string to locate\
[Number](../js-lib/number.md) start start pos

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mycol.locate('sample', 5))
```

### lt(value)

Compare column with a value or another column. Operator: lessThan

**Parameters**\
[Object](../js-lib/object.md) value ;

**Returns**\
[QBCondition](qbcondition.md)

**Sample**

```javascript
query.where.add(query.columns.flag.lt(99))
```

### minus(arg)

Subtract value

**Parameters**\
[Object](../js-lib/object.md) arg nr to subtract

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mycol.minus(2))
```

### mod(arg)

Create mod(arg) expression

**Parameters**\
[Object](../js-lib/object.md) arg mod arg

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mycol.mod(2))
```

### multiply(arg)

Multiply with value

**Parameters**\
[Object](../js-lib/object.md) arg nr to multiply with

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mycol.multiply(2))
```

### nullif(arg)

Create nullif(arg) expression

**Parameters**\
[Object](../js-lib/object.md) arg object to compare

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mycol.nullif('none'))
```

### plus(arg)

Add up value

**Parameters**\
[Object](../js-lib/object.md) arg nr to add

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mycol.plus(2))
```

### substring(pos)

Create substring(pos) expression

**Parameters**\
[Number](../js-lib/number.md) pos ;

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mycol.substring(3))
```

### substring(pos, len)

Create substring(pos, len) expression

**Parameters**\
[Number](../js-lib/number.md) pos ;\
[Number](../js-lib/number.md) len ;

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
query.result.add(query.columns.mycol.substring(3, 2))
```
