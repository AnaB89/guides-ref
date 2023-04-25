#  QBFunctions


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [QBSelect](./QBSelect.md) | [parent](QBFunctions.md#parent)                   | Get query builder parent table clause, this may be a query or a join clause..                                    |
| [QBSelect](./QBSelect.md) | [root](QBFunctions.md#root)                   | Get query builder parent..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [QBColumn](./QBColumn.md) | [abs(value)](QBFunctions.md#abs-value)                   | Create abs(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [bit_length(value)](QBFunctions.md#bit_length-value)                   | Create bit_length(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [cast(value, type)](QBFunctions.md#cast-value-type)                   | Cast using type name..                                    |
| [QBColumn](./QBColumn.md) | [ceil(arg)](QBFunctions.md#ceil-arg)                   | Create ceil(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [coalesce(args)](QBFunctions.md#coalesce-args)                   | Create year(date) expression.                                    |
| [QBColumn](./QBColumn.md) | [concat(arg1, arg2)](QBFunctions.md#concat-arg1-arg2)                   | Create concat(args, arg2) expression.                                    |
| [QBColumn](./QBColumn.md) | [custom(name, args)](QBFunctions.md#custom-name-args)                   | .                                    |
| [QBColumn](./QBColumn.md) | [day(arg)](QBFunctions.md#day-arg)                   | Create day(date) expression.                                    |
| [QBColumn](./QBColumn.md) | [divide(arg1, arg2)](QBFunctions.md#divide-arg1-arg2)                   | Create divide(args, arg2) expression.                                    |
| [QBColumn](./QBColumn.md) | [floor(arg)](QBFunctions.md#floor-arg)                   | Create floor(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [hour(arg)](QBFunctions.md#hour-arg)                   | Create hour(date) expression.                                    |
| [QBColumn](./QBColumn.md) | [len(value)](QBFunctions.md#len-value)                   | Create length(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [locate(string1, string2)](QBFunctions.md#locate-string1-string2)                   | Create locate(str1, str2) expression.                                    |
| [QBColumn](./QBColumn.md) | [locate(string1, string2, start)](QBFunctions.md#locate-string1-string2-start)                   | Create locate(str1, str2, start) expression.                                    |
| [QBColumn](./QBColumn.md) | [lower(value)](QBFunctions.md#lower-value)                   | Create lower(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [minus(arg1, arg2)](QBFunctions.md#minus-arg1-arg2)                   | Create minus(args, arg2) expression.                                    |
| [QBColumn](./QBColumn.md) | [minute(arg)](QBFunctions.md#minute-arg)                   | Create minute(date) expression.                                    |
| [QBColumn](./QBColumn.md) | [mod(dividend, divisor)](QBFunctions.md#mod-dividend-divisor)                   | Create mod(dividend, divisor) expression.                                    |
| [QBColumn](./QBColumn.md) | [month(arg)](QBFunctions.md#month-arg)                   | Create month(date) expression.                                    |
| [QBColumn](./QBColumn.md) | [multiply(arg1, arg2)](QBFunctions.md#multiply-arg1-arg2)                   | Create multiply(args, arg2) expression.                                    |
| [QBColumn](./QBColumn.md) | [nullif(arg1)](QBFunctions.md#nullif-arg1)                   | Create nullif(arg1, arg2) expression.                                    |
| [QBColumn](./QBColumn.md) | [plus(arg1, arg2)](QBFunctions.md#plus-arg1-arg2)                   | Create plus(args, arg2) expression.                                    |
| [QBColumn](./QBColumn.md) | [round(arg)](QBFunctions.md#round-arg)                   | Create round(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [round(arg, decimals)](QBFunctions.md#round-arg-decimals)                   | Create round(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [second(arg)](QBFunctions.md#second-arg)                   | Create second(date) expression.                                    |
| [QBColumn](./QBColumn.md) | [sqrt(value)](QBFunctions.md#sqrt-value)                   | Create sqrt(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [substring(arg, pos)](QBFunctions.md#substring-arg-pos)                   | Create substring(column, pos) expression.                                    |
| [QBColumn](./QBColumn.md) | [substring(arg, pos, len)](QBFunctions.md#substring-arg-pos-len)                   | Create substring(column, pos, len) expression.                                    |
| [QBColumn](./QBColumn.md) | [trim(value)](QBFunctions.md#trim-value)                   | Create trim(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [trim(leading_trailing_both, characters, fromKeyword, value)](QBFunctions.md#trim-leading_trailing_both-characters-fromkeyword-value)                   | Create trim([leading | trailing | both] [characters] from column).                                    |
| [QBColumn](./QBColumn.md) | [upper(value)](QBFunctions.md#upper-value)                   | Create upper(column) expression.                                    |
| [QBColumn](./QBColumn.md) | [year(arg)](QBFunctions.md#year-arg)                   | Create year(date) expression.                                    |

## Properties Details

### parent

Get query builder parent table clause, this may be a query or a join clause.

**Returns**\
[QBSelect](./QBSelect.md) 


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

### abs(value)

Create abs(column) expression

**Parameters**\
[Object](../JSLib/Object.md) value  ;

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynum.abs.eq(query.functions.abs(myval)))
foundset.loadRecords(query);
```
### bit_length(value)

Create bit_length(column) expression

**Parameters**\
[Object](../JSLib/Object.md) value  ;

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.bit_length.eq(query.functions.bit_length('Sample')))
foundset.loadRecords(query);
```
### cast(value, type)

Cast using type name.

**Parameters**\
[Object](../JSLib/Object.md) value object to cast\
[String](../JSLib/String.md) type type see QUERY_COLUMN_TYPES

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.functions.cast("22",QUERY_COLUMN_TYPES.TYPE_INTEGER)).add(query.columns.amt_discount.cast(QUERY_COLUMN_TYPES.TYPE_STRING));
application.output(databaseManager.getDataSetByQuery(query,1).getAsHTML())
```
### ceil(arg)

Create ceil(column) expression

**Parameters**\
[Object](../JSLib/Object.md) arg number object

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.ceil.eq(query.functions.ceil(myvar))
foundset.loadRecords(query);
```
### coalesce(args)

Create year(date) expression

**Parameters**\
[Array](../JSLib/Array.md) args arguments to coalesce

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mycol.coalesce('defval').eq(query.functions.coalesce(myvar, 'defval'))
foundset.loadRecords(query);
```
### concat(arg1, arg2)

Create concat(args, arg2) expression

**Parameters**\
[Object](../JSLib/Object.md) arg1  ;\
[Object](../JSLib/Object.md) arg2  ;

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.udm.contacts.createSelect();
	query.result.add(query.columns.name_first.concat(' ').concat(query.columns.name_last))
	var ds = databaseManager.getDataSetByQuery(query, -1)
```
### custom(name, args)



**Parameters**\
[String](../JSLib/String.md) name custom function name\
[Array](../JSLib/Array.md) args function arguments

**Returns**\
[QBColumn](./QBColumn.md) 


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
[Object](../JSLib/Object.md) arg date object

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mydatecol.day.eq(query.functions.day(mydatevar))
foundset.loadRecords(query);
```
### divide(arg1, arg2)

Create divide(args, arg2) expression

**Parameters**\
[Object](../JSLib/Object.md) arg1  ;\
[Object](../JSLib/Object.md) arg2  ;

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.divide(2).eq(query.functions.divide(myvar, 2))
foundset.loadRecords(query);
```
### floor(arg)

Create floor(column) expression

**Parameters**\
[Object](../JSLib/Object.md) arg number object

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.floor.eq(query.functions.floor(myvar))
foundset.loadRecords(query);
```
### hour(arg)

Create hour(date) expression

**Parameters**\
[Object](../JSLib/Object.md) arg date object

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mydatecol.hour.eq(query.functions.hour(mydatevar))
foundset.loadRecords(query);
```
### len(value)

Create length(column) expression

**Parameters**\
[Object](../JSLib/Object.md) value  ;

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.len.eq(query.functions.len('Sample')))
foundset.loadRecords(query);
```
### locate(string1, string2)

Create locate(str1, str2) expression

**Parameters**\
[Object](../JSLib/Object.md) string1 string to locate\
[Object](../JSLib/Object.md) string2 string to search in

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.locate('amp').eq(query.functions.locate('amp', 'Sample')))
foundset.loadRecords(query);
```
### locate(string1, string2, start)

Create locate(str1, str2, start) expression

**Parameters**\
[Object](../JSLib/Object.md) string1 string to locate\
[Object](../JSLib/Object.md) string2 string to search in\
[Number](../JSLib/Number.md) start start pos

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.locate('amp', 1).eq(query.functions.locate('amp', 'Sample', 1)))
foundset.loadRecords(query);
```
### lower(value)

Create lower(column) expression

**Parameters**\
[Object](../JSLib/Object.md) value  ;

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.lower.eq(query.functions.lower('Sample')))
foundset.loadRecords(query);
```
### minus(arg1, arg2)

Create minus(args, arg2) expression

**Parameters**\
[Object](../JSLib/Object.md) arg1  ;\
[Object](../JSLib/Object.md) arg2  ;

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.minus(2).eq(query.functions.minus(myvar, 2))
foundset.loadRecords(query);
```
### minute(arg)

Create minute(date) expression

**Parameters**\
[Object](../JSLib/Object.md) arg date object

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mydatecol.minute.eq(query.functions.minute(mydatevar))
foundset.loadRecords(query);
```
### mod(dividend, divisor)

Create mod(dividend, divisor) expression

**Parameters**\
[Object](../JSLib/Object.md) dividend  ;\
[Object](../JSLib/Object.md) divisor  ;

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.mod(2).eq(query.functions.mod(myvar, 2))
foundset.loadRecords(query);
```
### month(arg)

Create month(date) expression

**Parameters**\
[Object](../JSLib/Object.md) arg date object

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mydatecol.month.eq(query.functions.month(mydatevar))
foundset.loadRecords(query);
```
### multiply(arg1, arg2)

Create multiply(args, arg2) expression

**Parameters**\
[Object](../JSLib/Object.md) arg1  ;\
[Object](../JSLib/Object.md) arg2  ;

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.multiply(2).eq(query.functions.multiply(myvar, 2))
foundset.loadRecords(query);
```
### nullif(arg1)

Create nullif(arg1, arg2) expression

**Parameters**\
[Object](../JSLib/Object.md) arg1  ;

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.nullif('none').eq(query.functions.nullif('Sample', 'none')))
foundset.loadRecords(query);
```
### plus(arg1, arg2)

Create plus(args, arg2) expression

**Parameters**\
[Object](../JSLib/Object.md) arg1  ;\
[Object](../JSLib/Object.md) arg2  ;

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.plus(2).eq(query.functions.plus(myvar, 2))
foundset.loadRecords(query);
```
### round(arg)

Create round(column) expression

**Parameters**\
[Object](../JSLib/Object.md) arg number object

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.round.eq(query.functions.round(myvar))
foundset.loadRecords(query);
```
### round(arg, decimals)

Create round(column) expression

**Parameters**\
[Object](../JSLib/Object.md) arg number object\
[Number](../JSLib/Number.md) decimals The number of decimal places to round number to, default 0

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynumcol.round.eq(query.functions.round(myvar, 1))
foundset.loadRecords(query);
```
### second(arg)

Create second(date) expression

**Parameters**\
[Object](../JSLib/Object.md) arg date object

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mydatecol.second.eq(query.functions.second(mydatevar))
foundset.loadRecords(query);
```
### sqrt(value)

Create sqrt(column) expression

**Parameters**\
[Object](../JSLib/Object.md) value  ;

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mynum.sqrt.eq(query.functions.sqrt(myval)))
foundset.loadRecords(query);
```
### substring(arg, pos)

Create substring(column, pos) expression

**Parameters**\
[Object](../JSLib/Object.md) arg column name\
[Number](../JSLib/Number.md) pos position

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.substring(3).eq(query.functions.substring('Sample', 3)))
foundset.loadRecords(query);
```
### substring(arg, pos, len)

Create substring(column, pos, len) expression

**Parameters**\
[Object](../JSLib/Object.md) arg column name\
[Number](../JSLib/Number.md) pos position\
[Number](../JSLib/Number.md) len length

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.substring(3, 2).eq(query.functions.substring('Sample', 3, 2)))
foundset.loadRecords(query);
```
### trim(value)

Create trim(column) expression

**Parameters**\
[Object](../JSLib/Object.md) value  ;

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.trim.eq(query.functions.trim('Sample')))
foundset.loadRecords(query);
```
### trim(leading_trailing_both, characters, fromKeyword, value)

Create trim([leading | trailing | both] [characters] from column)

**Parameters**\
[String](../JSLib/String.md) leading_trailing_both 'leading', 'trailing' or 'both'\
[String](../JSLib/String.md) characters characters to remove\
[String](../JSLib/String.md) fromKeyword 'from'\
[Object](../JSLib/Object.md) value value to trim

**Returns**\
[QBColumn](./QBColumn.md) 


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
[Object](../JSLib/Object.md) value  ;

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.shipname.upper.eq(query.functions.upper('Sample')))
foundset.loadRecords(query);
```
### year(arg)

Create year(date) expression

**Parameters**\
[Object](../JSLib/Object.md) arg date object

**Returns**\
[QBColumn](./QBColumn.md) 


**Sample**

```javascript
var query = datasources.db.example_data.orders.createSelect();
query.where.add(query.columns.mydatecol.year.eq(query.functions.year(mydatevar))
foundset.loadRecords(query);
```

