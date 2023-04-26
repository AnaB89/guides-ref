# QBFunctions

## Property Summary

| Type                    | Name                            | Summary                                                                       |
| ----------------------- | ------------------------------- | ----------------------------------------------------------------------------- |
| [QBSelect](qbselect.md) | [parent](qbfunctions.md#parent) | Get query builder parent table clause, this may be a query or a join clause.. |
| [QBSelect](qbselect.md) | [root](qbfunctions.md#root)     | Get query builder parent..                                                    |

## Methods Summary

| Type                    | Name                                                                                                                                      | Summary                                        |
| ----------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| [QBColumn](qbcolumn.md) | [abs(value)](qbfunctions.md#abs-value)                                                                                                    | Create abs(column) expression.                 |
| [QBColumn](qbcolumn.md) | [bit\_length(value)](qbfunctions.md#bit\_length-value)                                                                                    | Create bit\_length(column) expression.         |
| [QBColumn](qbcolumn.md) | [cast(value, type)](qbfunctions.md#cast-value-type)                                                                                       | Cast using type name..                         |
| [QBColumn](qbcolumn.md) | [ceil(arg)](qbfunctions.md#ceil-arg)                                                                                                      | Create ceil(column) expression.                |
| [QBColumn](qbcolumn.md) | [coalesce(args)](qbfunctions.md#coalesce-args)                                                                                            | Create year(date) expression.                  |
| [QBColumn](qbcolumn.md) | [concat(arg1, arg2)](qbfunctions.md#concat-arg1-arg2)                                                                                     | Create concat(args, arg2) expression.          |
| [QBColumn](qbcolumn.md) | [custom(name, args)](qbfunctions.md#custom-name-args)                                                                                     | .                                              |
| [QBColumn](qbcolumn.md) | [day(arg)](qbfunctions.md#day-arg)                                                                                                        | Create day(date) expression.                   |
| [QBColumn](qbcolumn.md) | [divide(arg1, arg2)](qbfunctions.md#divide-arg1-arg2)                                                                                     | Create divide(args, arg2) expression.          |
| [QBColumn](qbcolumn.md) | [floor(arg)](qbfunctions.md#floor-arg)                                                                                                    | Create floor(column) expression.               |
| [QBColumn](qbcolumn.md) | [hour(arg)](qbfunctions.md#hour-arg)                                                                                                      | Create hour(date) expression.                  |
| [QBColumn](qbcolumn.md) | [len(value)](qbfunctions.md#len-value)                                                                                                    | Create length(column) expression.              |
| [QBColumn](qbcolumn.md) | [locate(string1, string2)](qbfunctions.md#locate-string1-string2)                                                                         | Create locate(str1, str2) expression.          |
| [QBColumn](qbcolumn.md) | [locate(string1, string2, start)](qbfunctions.md#locate-string1-string2-start)                                                            | Create locate(str1, str2, start) expression.   |
| [QBColumn](qbcolumn.md) | [lower(value)](qbfunctions.md#lower-value)                                                                                                | Create lower(column) expression.               |
| [QBColumn](qbcolumn.md) | [minus(arg1, arg2)](qbfunctions.md#minus-arg1-arg2)                                                                                       | Create minus(args, arg2) expression.           |
| [QBColumn](qbcolumn.md) | [minute(arg)](qbfunctions.md#minute-arg)                                                                                                  | Create minute(date) expression.                |
| [QBColumn](qbcolumn.md) | [mod(dividend, divisor)](qbfunctions.md#mod-dividend-divisor)                                                                             | Create mod(dividend, divisor) expression.      |
| [QBColumn](qbcolumn.md) | [month(arg)](qbfunctions.md#month-arg)                                                                                                    | Create month(date) expression.                 |
| [QBColumn](qbcolumn.md) | [multiply(arg1, arg2)](qbfunctions.md#multiply-arg1-arg2)                                                                                 | Create multiply(args, arg2) expression.        |
| [QBColumn](qbcolumn.md) | [nullif(arg1)](qbfunctions.md#nullif-arg1)                                                                                                | Create nullif(arg1, arg2) expression.          |
| [QBColumn](qbcolumn.md) | [plus(arg1, arg2)](qbfunctions.md#plus-arg1-arg2)                                                                                         | Create plus(args, arg2) expression.            |
| [QBColumn](qbcolumn.md) | [round(arg)](qbfunctions.md#round-arg)                                                                                                    | Create round(column) expression.               |
| [QBColumn](qbcolumn.md) | [round(arg, decimals)](qbfunctions.md#round-arg-decimals)                                                                                 | Create round(column) expression.               |
| [QBColumn](qbcolumn.md) | [second(arg)](qbfunctions.md#second-arg)                                                                                                  | Create second(date) expression.                |
| [QBColumn](qbcolumn.md) | [sqrt(value)](qbfunctions.md#sqrt-value)                                                                                                  | Create sqrt(column) expression.                |
| [QBColumn](qbcolumn.md) | [substring(arg, pos)](qbfunctions.md#substring-arg-pos)                                                                                   | Create substring(column, pos) expression.      |
| [QBColumn](qbcolumn.md) | [substring(arg, pos, len)](qbfunctions.md#substring-arg-pos-len)                                                                          | Create substring(column, pos, len) expression. |
| [QBColumn](qbcolumn.md) | [trim(value)](qbfunctions.md#trim-value)                                                                                                  | Create trim(column) expression.                |
| [QBColumn](qbcolumn.md) | [trim(leading\_trailing\_both, characters, fromKeyword, value)](qbfunctions.md#trim-leading\_trailing\_both-characters-fromkeyword-value) | Create trim(\[leading                          |
| [QBColumn](qbcolumn.md) | [upper(value)](qbfunctions.md#upper-value)                                                                                                | Create upper(column) expression.               |
| [QBColumn](qbcolumn.md) | [year(arg)](qbfunctions.md#year-arg)                                                                                                      | Create year(date) expression.                  |

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

### abs(value)

Create abs(column) expression

**Parameters**\
[Object](../js-lib/object.md) value ;

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynum.abs.eq(query.functions.abs(myval)))
foundset.loadRecords(query);
```

### bit\_length(value)

Create bit\_length(column) expression

**Parameters**\
[Object](../js-lib/object.md) value ;

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.bit_length.eq(query.functions.bit_length('Sample')))
foundset.loadRecords(query);
```

### cast(value, type)

Cast using type name.

**Parameters**\
[Object](../js-lib/object.md) value object to cast\
[String](../js-lib/string.md) type type see QUERY\_COLUMN\_TYPES

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```

### ceil(arg)

Create ceil(column) expression

**Parameters**\
[Object](../js-lib/object.md) arg number object

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.ceil.eq(query.functions.ceil(myvar))
foundset.loadRecords(query);
```

### coalesce(args)

Create year(date) expression

**Parameters**\
[Array](../js-lib/array.md) args arguments to coalesce

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mycol.coalesce('defval').eq(query.functions.coalesce(myvar, 'defval'))
foundset.loadRecords(query);
```

### concat(arg1, arg2)

Create concat(args, arg2) expression

**Parameters**\
[Object](../js-lib/object.md) arg1 ;\
[Object](../js-lib/object.md) arg2 ;

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.udm.contacts.createSelect();
	query.result.add(query.columns.name_first.concat(' ').concat(query.columns.name_last))
	var ds = databaseManager.getDataSetByQuery(query, -1)
```

### custom(name, args)

**Parameters**\
[String](../js-lib/string.md) name custom function name\
[Array](../js-lib/array.md) args function arguments

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
// select myadd(freight, 500) from orders
	var query = datasources.db.example_data.orders.createSelect();
	query.result.add(query.functions.custom('myadd', query.columns.freight, 500));
	var dataset = databaseManager.getDataSetByQuery(query, 100);
```

### day(arg)

Create day(date) expression

**Parameters**\
[Object](../js-lib/object.md) arg date object

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mydatecol.day.eq(query.functions.day(mydatevar))
foundset.loadRecords(query);
```

### divide(arg1, arg2)

Create divide(args, arg2) expression

**Parameters**\
[Object](../js-lib/object.md) arg1 ;\
[Object](../js-lib/object.md) arg2 ;

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.divide(2).eq(query.functions.divide(myvar, 2))
foundset.loadRecords(query);
```

### floor(arg)

Create floor(column) expression

**Parameters**\
[Object](../js-lib/object.md) arg number object

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.floor.eq(query.functions.floor(myvar))
foundset.loadRecords(query);
```

### hour(arg)

Create hour(date) expression

**Parameters**\
[Object](../js-lib/object.md) arg date object

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mydatecol.hour.eq(query.functions.hour(mydatevar))
foundset.loadRecords(query);
```

### len(value)

Create length(column) expression

**Parameters**\
[Object](../js-lib/object.md) value ;

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.len.eq(query.functions.len('Sample')))
foundset.loadRecords(query);
```

### locate(string1, string2)

Create locate(str1, str2) expression

**Parameters**\
[Object](../js-lib/object.md) string1 string to locate\
[Object](../js-lib/object.md) string2 string to search in

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.locate('amp').eq(query.functions.locate('amp', 'Sample')))
foundset.loadRecords(query);
```

### locate(string1, string2, start)

Create locate(str1, str2, start) expression

**Parameters**\
[Object](../js-lib/object.md) string1 string to locate\
[Object](../js-lib/object.md) string2 string to search in\
[Number](../js-lib/number.md) start start pos

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.locate('amp', 1).eq(query.functions.locate('amp', 'Sample', 1)))
foundset.loadRecords(query);
```

### lower(value)

Create lower(column) expression

**Parameters**\
[Object](../js-lib/object.md) value ;

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.lower.eq(query.functions.lower('Sample')))
foundset.loadRecords(query);
```

### minus(arg1, arg2)

Create minus(args, arg2) expression

**Parameters**\
[Object](../js-lib/object.md) arg1 ;\
[Object](../js-lib/object.md) arg2 ;

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.minus(2).eq(query.functions.minus(myvar, 2))
foundset.loadRecords(query);
```

### minute(arg)

Create minute(date) expression

**Parameters**\
[Object](../js-lib/object.md) arg date object

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mydatecol.minute.eq(query.functions.minute(mydatevar))
foundset.loadRecords(query);
```

### mod(dividend, divisor)

Create mod(dividend, divisor) expression

**Parameters**\
[Object](../js-lib/object.md) dividend ;\
[Object](../js-lib/object.md) divisor ;

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.mod(2).eq(query.functions.mod(myvar, 2))
foundset.loadRecords(query);
```

### month(arg)

Create month(date) expression

**Parameters**\
[Object](../js-lib/object.md) arg date object

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mydatecol.month.eq(query.functions.month(mydatevar))
foundset.loadRecords(query);
```

### multiply(arg1, arg2)

Create multiply(args, arg2) expression

**Parameters**\
[Object](../js-lib/object.md) arg1 ;\
[Object](../js-lib/object.md) arg2 ;

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.multiply(2).eq(query.functions.multiply(myvar, 2))
foundset.loadRecords(query);
```

### nullif(arg1)

Create nullif(arg1, arg2) expression

**Parameters**\
[Object](../js-lib/object.md) arg1 ;

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.nullif('none').eq(query.functions.nullif('Sample', 'none')))
foundset.loadRecords(query);
```

### plus(arg1, arg2)

Create plus(args, arg2) expression

**Parameters**\
[Object](../js-lib/object.md) arg1 ;\
[Object](../js-lib/object.md) arg2 ;

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.plus(2).eq(query.functions.plus(myvar, 2))
foundset.loadRecords(query);
```

### round(arg)

Create round(column) expression

**Parameters**\
[Object](../js-lib/object.md) arg number object

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.round.eq(query.functions.round(myvar))
foundset.loadRecords(query);
```

### round(arg, decimals)

Create round(column) expression

**Parameters**\
[Object](../js-lib/object.md) arg number object\
[Number](../js-lib/number.md) decimals The number of decimal places to round number to, default 0

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.round.eq(query.functions.round(myvar, 1))
foundset.loadRecords(query);
```

### second(arg)

Create second(date) expression

**Parameters**\
[Object](../js-lib/object.md) arg date object

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mydatecol.second.eq(query.functions.second(mydatevar))
foundset.loadRecords(query);
```

### sqrt(value)

Create sqrt(column) expression

**Parameters**\
[Object](../js-lib/object.md) value ;

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynum.sqrt.eq(query.functions.sqrt(myval)))
foundset.loadRecords(query);
```

### substring(arg, pos)

Create substring(column, pos) expression

**Parameters**\
[Object](../js-lib/object.md) arg column name\
[Number](../js-lib/number.md) pos position

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.substring(3).eq(query.functions.substring('Sample', 3)))
foundset.loadRecords(query);
```

### substring(arg, pos, len)

Create substring(column, pos, len) expression

**Parameters**\
[Object](../js-lib/object.md) arg column name\
[Number](../js-lib/number.md) pos position\
[Number](../js-lib/number.md) len length

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.substring(3, 2).eq(query.functions.substring('Sample', 3, 2)))
foundset.loadRecords(query);
```

### trim(value)

Create trim(column) expression

**Parameters**\
[Object](../js-lib/object.md) value ;

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.trim.eq(query.functions.trim('Sample')))
foundset.loadRecords(query);
```

### trim(leading\_trailing\_both, characters, fromKeyword, value)

Create trim(\[leading | trailing | both] \[characters] from column)

**Parameters**\
[String](../js-lib/string.md) leading\_trailing\_both 'leading', 'trailing' or 'both'\
[String](../js-lib/string.md) characters characters to remove\
[String](../js-lib/string.md) fromKeyword 'from'\
[Object](../js-lib/object.md) value value to trim

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
// show shipname but remove trailing space
query.result.add(query.functions.trim('trailing', ' ', 'from', query.columns.shipname));
foundset.loadRecords(query);
```

### upper(value)

Create upper(column) expression

**Parameters**\
[Object](../js-lib/object.md) value ;

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.upper.eq(query.functions.upper('Sample')))
foundset.loadRecords(query);
```

### year(arg)

Create year(date) expression

**Parameters**\
[Object](../js-lib/object.md) arg date object

**Returns**\
[QBColumn](qbcolumn.md)

**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mydatecol.year.eq(query.functions.year(mydatevar))
foundset.loadRecords(query);
```
