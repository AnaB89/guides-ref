# JSColumn

## Constants Summary

| Type                          | Name                                                 | Summary                                                                    |
| ----------------------------- | ---------------------------------------------------- | -------------------------------------------------------------------------- |
| [Number](../js-lib/number.md) | [DATABASE\_IDENTITY](jscolumn.md#DATABASE\_IDENTITY) | Constant used when setting or getting the sequence type of columns..       |
| [Number](../js-lib/number.md) | [DATABASE\_SEQUENCE](jscolumn.md#DATABASE\_SEQUENCE) | Constant used when setting or getting the sequence type of columns..       |
| [Number](../js-lib/number.md) | [DATETIME](jscolumn.md#DATETIME)                     | Constant used when setting or getting the type of columns..                |
| [Number](../js-lib/number.md) | [EXCLUDED\_COLUMN](jscolumn.md#EXCLUDED\_COLUMN)     | Constant used when setting or getting the flags of columns..               |
| [Number](../js-lib/number.md) | [INTEGER](jscolumn.md#INTEGER)                       | Constant used when setting or getting the type of columns..                |
| [Number](../js-lib/number.md) | [MEDIA](jscolumn.md#MEDIA)                           | Constant used when setting or getting the type of columns..                |
| [Number](../js-lib/number.md) | [NATIVE\_COLUMN](jscolumn.md#NATIVE\_COLUMN)         | Constant used when setting or getting the flags of columns..               |
| [Number](../js-lib/number.md) | [NONE](jscolumn.md#NONE)                             | Constant for column information indicating unset values..                  |
| [Number](../js-lib/number.md) | [NUMBER](jscolumn.md#NUMBER)                         | Constant used when setting or getting the type of columns..                |
| [Number](../js-lib/number.md) | [PK\_COLUMN](jscolumn.md#PK\_COLUMN)                 | Constant used when setting or getting the row identifier type of columns.. |
| [Number](../js-lib/number.md) | [ROWID\_COLUMN](jscolumn.md#ROWID\_COLUMN)           | Constant used when setting or getting the row identifier type of columns.. |
| [Number](../js-lib/number.md) | [SERVOY\_SEQUENCE](jscolumn.md#SERVOY\_SEQUENCE)     | Constant used when setting or getting the sequence type of columns..       |
| [Number](../js-lib/number.md) | [TENANT\_COLUMN](jscolumn.md#TENANT\_COLUMN)         | Constant used when setting or getting the flags of columns..               |
| [Number](../js-lib/number.md) | [TEXT](jscolumn.md#TEXT)                             | Constant used when setting or getting the type of columns..                |
| [Number](../js-lib/number.md) | [UUID\_COLUMN](jscolumn.md#UUID\_COLUMN)             | Constant used when setting or getting the flags of columns..               |
| [Number](../js-lib/number.md) | [UUID\_GENERATOR](jscolumn.md#UUID\_GENERATOR)       | Constant used when setting or getting the sequence type of columns..       |

## Methods Summary

| Type                            | Name                                                       | Summary                                                                                                                      |
| ------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| [Boolean](../js-lib/boolean.md) | [getAllowNull()](jscolumn.md#getallownull)                 | Get the allow-null flag of the column..                                                                                      |
| [String](../js-lib/string.md)   | [getDataProviderID()](jscolumn.md#getdataproviderid)       | Get the data provider id for this column (which is the same as name if not explicitly defined otherwise)..                   |
| [String](../js-lib/string.md)   | [getDefaultFormat()](jscolumn.md#getdefaultformat)         | Get the default format of the column..                                                                                       |
| [String](../js-lib/string.md)   | [getDescription()](jscolumn.md#getdescription)             | Get the description property of the column..                                                                                 |
| [String](../js-lib/string.md)   | [getForeignType()](jscolumn.md#getforeigntype)             | Get the foreign type of the column..                                                                                         |
| [Number](../js-lib/number.md)   | [getLength()](jscolumn.md#getlength)                       | Get the length of the column as reported by the JDBC driver..                                                                |
| [String](../js-lib/string.md)   | [getName()](jscolumn.md#getname)                           | Get the name of the column as used by Servoy..                                                                               |
| [String](../js-lib/string.md)   | [getQualifiedName()](jscolumn.md#getqualifiedname)         | Get the qualified name (including table name) of the column as known by the database..                                       |
| [String](../js-lib/string.md)   | [getQuotedSQLName()](jscolumn.md#getquotedsqlname)         | Returns a quoted version of the column name, if necessary, as defined by the actual database used..                          |
| [Number](../js-lib/number.md)   | [getRowIdentifierType()](jscolumn.md#getrowidentifiertype) | Get the row identifier type of the column..                                                                                  |
| [String](../js-lib/string.md)   | [getSQLName()](jscolumn.md#getsqlname)                     | Get the name of the column as known by the database..                                                                        |
| [Number](../js-lib/number.md)   | [getSQLType()](jscolumn.md#getsqltype)                     | Get the raw JDBC type of the column, which allows to check database specific types, like sting/byte column type variations.. |
| [Number](../js-lib/number.md)   | [getScale()](jscolumn.md#getscale)                         | Get the scale of the column as reported by the JDBC driver..                                                                 |
| [Number](../js-lib/number.md)   | [getSequenceType()](jscolumn.md#getsequencetype)           | Get the sequence type of the column..                                                                                        |
| [JSTable](jstable.md)           | [getTable()](jscolumn.md#gettable)                         | Get the JSTable of this column..                                                                                             |
| [String](../js-lib/string.md)   | [getTitle()](jscolumn.md#gettitle)                         | Get the title property of the column..                                                                                       |
| [Number](../js-lib/number.md)   | [getType()](jscolumn.md#gettype)                           | Get the JDBC type of the column..                                                                                            |
| [String](../js-lib/string.md)   | [getTypeAsString()](jscolumn.md#gettypeasstring)           | Get the name JDBC type of the column..                                                                                       |
| [Boolean](../js-lib/boolean.md) | [hasFlag(flag)](jscolumn.md#hasflag-flag)                  | Check a flag of the column..                                                                                                 |

## Constants Details

### DATABASE\_IDENTITY

Constant used when setting or getting the sequence type of columns.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
switch (column.getSequenceType())
{
case JSColumn.NONE:
	// handle column with no sequence
break;

case JSColumn.UUID_GENERATOR:
	// handle uuid generated column
break;
}
```

### DATABASE\_SEQUENCE

Constant used when setting or getting the sequence type of columns.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
switch (column.getSequenceType())
{
case JSColumn.NONE:
	// handle column with no sequence
break;

case JSColumn.UUID_GENERATOR:
	// handle uuid generated column
break;
}
```

### DATETIME

Constant used when setting or getting the type of columns.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
switch (column.getType())
{
case JSColumn.TEXT:
	// handle text column
break;

case JSColumn.NUMBER:
case JSColumn.INTEGER:
	// handle numerical column
break;
}
```

### EXCLUDED\_COLUMN

Constant used when setting or getting the flags of columns. This flag identifies columns that are skipped in the sql.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
if (column.hasFlag(JSColumn.UUID_COLUMN))
{
	// handle uuid column
}
```

### INTEGER

Constant used when setting or getting the type of columns.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
switch (column.getType())
{
case JSColumn.TEXT:
	// handle text column
break;

case JSColumn.NUMBER:
case JSColumn.INTEGER:
	// handle numerical column
break;
}
```

### MEDIA

Constant used when setting or getting the type of columns.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
switch (column.getType())
{
case JSColumn.TEXT:
	// handle text column
break;

case JSColumn.NUMBER:
case JSColumn.INTEGER:
	// handle numerical column
break;
}
```

### NATIVE\_COLUMN

Constant used when setting or getting the flags of columns. This flag identifies columns that are marked as a native type column (for example uniqueidentifier).

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
if (column.hasFlag(JSColumn.UUID_COLUMN))
{
	// handle uuid column
}
```

### NONE

Constant for column information indicating unset values.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
switch (column.getSequenceType())
{
case JSColumn.NONE:
	// handle column with no sequence
break;

case JSColumn.UUID_GENERATOR:
	// handle uuid generated column
break;
}
```

### NUMBER

Constant used when setting or getting the type of columns.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
switch (column.getType())
{
case JSColumn.TEXT:
	// handle text column
break;

case JSColumn.NUMBER:
case JSColumn.INTEGER:
	// handle numerical column
break;
}
```

### PK\_COLUMN

Constant used when setting or getting the row identifier type of columns. This value identifies columns that are defined as primary key in the database.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
switch (column.getRowIdentifierType())
{
case JSColumn.NONE:
	// handle normal column
break;

case JSColumn.PK_COLUMN:
	// handle database pk column
break;

case JSColumn.ROWID_COLUMN:
	// handle developer defined pk column
break;
}
```

### ROWID\_COLUMN

Constant used when setting or getting the row identifier type of columns. This value identifies columns that are defined as primary key by the developer (but not in the database).

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
switch (column.getRowIdentifierType())
{
case JSColumn.NONE:
	// handle normal column
break;

case JSColumn.PK_COLUMN:
	// handle database pk column
break;

case JSColumn.ROWID_COLUMN:
	// handle developer defined pk column
break;
}
```

### SERVOY\_SEQUENCE

Constant used when setting or getting the sequence type of columns.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
switch (column.getSequenceType())
{
case JSColumn.NONE:
	// handle column with no sequence
break;

case JSColumn.UUID_GENERATOR:
	// handle uuid generated column
break;
}
```

### TENANT\_COLUMN

Constant used when setting or getting the flags of columns. This flag identifies columns that are marked as a tenant column.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
if (column.hasFlag(JSColumn.UUID_COLUMN))
{
	// handle uuid column
}
```

### TEXT

Constant used when setting or getting the type of columns.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
switch (column.getType())
{
case JSColumn.TEXT:
	// handle text column
break;

case JSColumn.NUMBER:
case JSColumn.INTEGER:
	// handle numerical column
break;
}
```

### UUID\_COLUMN

Constant used when setting or getting the flags of columns. This flag identifies columns whose values are treated as UUID.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
if (column.hasFlag(JSColumn.UUID_COLUMN))
{
	// handle uuid column
}
```

### UUID\_GENERATOR

Constant used when setting or getting the sequence type of columns.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
switch (column.getSequenceType())
{
case JSColumn.NONE:
	// handle column with no sequence
break;

case JSColumn.UUID_GENERATOR:
	// handle uuid generated column
break;
}
```

## Methods Details

### getAllowNull()

Get the allow-null flag of the column.

**Returns**\
[Boolean](../js-lib/boolean.md) boolean allow-null flag.

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
if (!column.getAllowNull())
{
	 // column cannot be null
}
```

### getDataProviderID()

Get the data provider id for this column (which is the same as name if not explicitly defined otherwise).

**Returns**\
[String](../js-lib/string.md) String dataprovider id.

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
var dataProviderId = column.getDataProviderID()
```

### getDefaultFormat()

Get the default format of the column.

**Returns**\
[String](../js-lib/string.md) String column default format.

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
var format = column.getDefaultFormat()
```

### getDescription()

Get the description property of the column.

**Returns**\
[String](../js-lib/string.md) String column description.

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customername')
var desc = column.getDescription()
```

### getForeignType()

Get the foreign type of the column. The foreign type can be defined design time as a foreign key reference to another table.

**Returns**\
[String](../js-lib/string.md) String foreign type.

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
var foreignType = column.getForeignType()
if (foreignType != null)
{
	var fkTable = databaseManager.getTable('example_data', foreignType)
}
```

### getLength()

Get the length of the column as reported by the JDBC driver.

**Returns**\
[Number](../js-lib/number.md) int column length.

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customername')
if (column.getLength() < 10)
{
	 // handle short column
}
```

### getName()

Get the name of the column as used by Servoy.

**Returns**\
[String](../js-lib/string.md) String column name

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
var colName = column.getName()
```

### getQualifiedName()

Get the qualified name (including table name) of the column as known by the database. The name is quoted, if necessary, as defined by the actual database used.

**Returns**\
[String](../js-lib/string.md) String qualified column name.

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
var qualifiedSqlName = column.getQualifiedName()
```

### getQuotedSQLName()

Returns a quoted version of the column name, if necessary, as defined by the actual database used.

**Returns**\
[String](../js-lib/string.md) column name, quoted if needed.

**Sample**

```javascript
//use with the raw SQL plugin:
//if the table name contains characters that are illegal in sql, the table name will be quoted
var jsTable = databaseManager.getTable('udm', 'campaigns')
var quotedTableName = jsTable.getQuotedSQLName()
var jsColumn = jsTable.getColumn('active')
var quotedColumnName = jsColumn.getQuotedSQLName()
plugins.rawSQL.executeSQL('udm',  quotedTableName,  'select * from ' + quotedTableName + ' where ' + quotedColumnName + ' = ?', [1])
```

### getRowIdentifierType()

Get the row identifier type of the column. The sequence type is one of:

* JSColumn.PK\_COLUMN
* JSColumn.ROWID\_COLUMN
* JSColumn.NONE

**Returns**\
[Number](../js-lib/number.md) int row identifier type.

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
switch (column.getRowIdentifierType())
{
case JSColumn.NONE:
	// handle normal column
break;

case JSColumn.PK_COLUMN:
	// handle database pk column
break;

case JSColumn.ROWID_COLUMN:
	// handle developer defined pk column
break;
}
```

### getSQLName()

Get the name of the column as known by the database.

**Returns**\
[String](../js-lib/string.md) String sql name

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
var sqlName = column.getSQLName()
```

### getSQLType()

Get the raw JDBC type of the column, which allows to check database specific types, like sting/byte column type variations.

**Returns**\
[Number](../js-lib/number.md) int sql type.

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
var sqlType = column.getSQLType();
```

### getScale()

Get the scale of the column as reported by the JDBC driver.

**Returns**\
[Number](../js-lib/number.md) int column scale.

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customername')
var scale = column.getScale()
```

### getSequenceType()

Get the sequence type of the column. The sequence type is one of:

* JSColumn.NONE
* JSColumn.SERVOY\_SEQUENCE
* JSColumn.DATABASE\_SEQUENCE
* JSColumn.DATABASE\_IDENTITY
* JSColumn.UUID\_GENERATOR;

**Returns**\
[Number](../js-lib/number.md) int sequence type.

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
switch (column.getSequenceType())
{
case JSColumn.NONE:
	// handle column with no sequence
break;

case JSColumn.UUID_GENERATOR:
	// handle uuid generated column
break;
}
```

### getTable()

Get the JSTable of this column.

**Returns**\
[JSTable](jstable.md) table The JSTable of this column.

**Sample**

```javascript
```

### getTitle()

Get the title property of the column. If title is null will return column name.

**Returns**\
[String](../js-lib/string.md) String column title.

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customername')
var title = column.getTitle()
```

### getType()

Get the JDBC type of the column. The type reported by the JDBC driver will be mapped to one of:

* JSColumn.DATETIME
* JSColumn.TEXT
* JSColumn.NUMBER
* JSColumn.INTEGER
* JSColumn.MEDIA

**Returns**\
[Number](../js-lib/number.md) int sql type.

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
switch (column.getType())
{
case JSColumn.TEXT:
	// handle text column
break;

case JSColumn.NUMBER:
case JSColumn.INTEGER:
	// handle numerical column
break;
}
```

### getTypeAsString()

Get the name JDBC type of the column. The same mapping as defined in JSColumn.getType() is applied.

**Returns**\
[String](../js-lib/string.md) String sql name.

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
var typeName = column.getTypeAsString()
```

### hasFlag(flag)

Check a flag of the column. The flags are a bit pattern consisting of 1 or more of the following bits:

* JSColumn.UUID\_COLUMN
* JSColumn.EXCLUDED\_COLUMN
* JSColumn.TENANT\_COLUMN
* JSColumn.NATIVE\_COLUMN

**Parameters**\
[Number](../js-lib/number.md) flag ;

**Returns**\
[Boolean](../js-lib/boolean.md) boolean whether flag is set.

**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
if (column.hasFlag(JSColumn.UUID_COLUMN))
{
	// handle uuid column
}
```
