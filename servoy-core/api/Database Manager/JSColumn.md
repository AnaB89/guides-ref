#  JSColumn


## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [DATABASE_IDENTITY](JSColumn.md#DATABASE_IDENTITY)                   | Constant used when setting or getting the sequence type of columns..                                    |
| [Number](../JSLib/Number.md) | [DATABASE_SEQUENCE](JSColumn.md#DATABASE_SEQUENCE)                   | Constant used when setting or getting the sequence type of columns..                                    |
| [Number](../JSLib/Number.md) | [DATETIME](JSColumn.md#DATETIME)                   | Constant used when setting or getting the type of columns..                                    |
| [Number](../JSLib/Number.md) | [EXCLUDED_COLUMN](JSColumn.md#EXCLUDED_COLUMN)                   | Constant used when setting or getting the flags of columns..                                    |
| [Number](../JSLib/Number.md) | [INTEGER](JSColumn.md#INTEGER)                   | Constant used when setting or getting the type of columns..                                    |
| [Number](../JSLib/Number.md) | [MEDIA](JSColumn.md#MEDIA)                   | Constant used when setting or getting the type of columns..                                    |
| [Number](../JSLib/Number.md) | [NATIVE_COLUMN](JSColumn.md#NATIVE_COLUMN)                   | Constant used when setting or getting the flags of columns..                                    |
| [Number](../JSLib/Number.md) | [NONE](JSColumn.md#NONE)                   | Constant for column information indicating unset values..                                    |
| [Number](../JSLib/Number.md) | [NUMBER](JSColumn.md#NUMBER)                   | Constant used when setting or getting the type of columns..                                    |
| [Number](../JSLib/Number.md) | [PK_COLUMN](JSColumn.md#PK_COLUMN)                   | Constant used when setting or getting the row identifier type of columns..                                    |
| [Number](../JSLib/Number.md) | [ROWID_COLUMN](JSColumn.md#ROWID_COLUMN)                   | Constant used when setting or getting the row identifier type of columns..                                    |
| [Number](../JSLib/Number.md) | [SERVOY_SEQUENCE](JSColumn.md#SERVOY_SEQUENCE)                   | Constant used when setting or getting the sequence type of columns..                                    |
| [Number](../JSLib/Number.md) | [TENANT_COLUMN](JSColumn.md#TENANT_COLUMN)                   | Constant used when setting or getting the flags of columns..                                    |
| [Number](../JSLib/Number.md) | [TEXT](JSColumn.md#TEXT)                   | Constant used when setting or getting the type of columns..                                    |
| [Number](../JSLib/Number.md) | [UUID_COLUMN](JSColumn.md#UUID_COLUMN)                   | Constant used when setting or getting the flags of columns..                                    |
| [Number](../JSLib/Number.md) | [UUID_GENERATOR](JSColumn.md#UUID_GENERATOR)                   | Constant used when setting or getting the sequence type of columns..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../JSLib/Boolean.md) | [getAllowNull()](JSColumn.md#getallownull)                   | Get the allow-null flag of the column..                                    |
| [String](../JSLib/String.md) | [getDataProviderID()](JSColumn.md#getdataproviderid)                   | Get the data provider id for this column (which is the same as name if not explicitly defined otherwise)..                                    |
| [String](../JSLib/String.md) | [getDefaultFormat()](JSColumn.md#getdefaultformat)                   | Get the default format of the column..                                    |
| [String](../JSLib/String.md) | [getDescription()](JSColumn.md#getdescription)                   | Get the description property of the column..                                    |
| [String](../JSLib/String.md) | [getForeignType()](JSColumn.md#getforeigntype)                   | Get the foreign type of the column..                                    |
| [Number](../JSLib/Number.md) | [getLength()](JSColumn.md#getlength)                   | Get the length of the column as reported by the JDBC driver..                                    |
| [String](../JSLib/String.md) | [getName()](JSColumn.md#getname)                   | Get the name of the column as used by Servoy..                                    |
| [String](../JSLib/String.md) | [getQualifiedName()](JSColumn.md#getqualifiedname)                   | Get the qualified name (including table name) of the column as known by the database..                                    |
| [String](../JSLib/String.md) | [getQuotedSQLName()](JSColumn.md#getquotedsqlname)                   | Returns a quoted version of the column name, if necessary, as defined by the actual database used..                                    |
| [Number](../JSLib/Number.md) | [getRowIdentifierType()](JSColumn.md#getrowidentifiertype)                   | Get the row identifier type of the column..                                    |
| [String](../JSLib/String.md) | [getSQLName()](JSColumn.md#getsqlname)                   | Get the name of the column as known by the database..                                    |
| [Number](../JSLib/Number.md) | [getSQLType()](JSColumn.md#getsqltype)                   | Get the raw JDBC type of the column, which allows to check database specific types, like sting/byte column type variations..                                    |
| [Number](../JSLib/Number.md) | [getScale()](JSColumn.md#getscale)                   | Get the scale of the column as reported by the JDBC driver..                                    |
| [Number](../JSLib/Number.md) | [getSequenceType()](JSColumn.md#getsequencetype)                   | Get the sequence type of the column..                                    |
| [JSTable](./JSTable.md) | [getTable()](JSColumn.md#gettable)                   | Get the JSTable of this column..                                    |
| [String](../JSLib/String.md) | [getTitle()](JSColumn.md#gettitle)                   | Get the title property of the column..                                    |
| [Number](../JSLib/Number.md) | [getType()](JSColumn.md#gettype)                   | Get the JDBC type of the column..                                    |
| [String](../JSLib/String.md) | [getTypeAsString()](JSColumn.md#gettypeasstring)                   | Get the name JDBC type of the column..                                    |
| [Boolean](../JSLib/Boolean.md) | [hasFlag(flag)](JSColumn.md#hasflag-flag)                   | Check a flag of the column..                                    |

## Constants Details

### DATABASE_IDENTITY

Constant used when setting or getting the sequence type of columns.

**Returns**\
[Number](../JSLib/Number.md) 


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
### DATABASE_SEQUENCE

Constant used when setting or getting the sequence type of columns.

**Returns**\
[Number](../JSLib/Number.md) 


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
[Number](../JSLib/Number.md) 


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
### EXCLUDED_COLUMN

Constant used when setting or getting the flags of columns.
This flag identifies columns that are skipped in the sql.

**Returns**\
[Number](../JSLib/Number.md) 


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
[Number](../JSLib/Number.md) 


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
[Number](../JSLib/Number.md) 


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
### NATIVE_COLUMN

Constant used when setting or getting the flags of columns.
This flag identifies columns that are marked as a native type column (for example uniqueidentifier).

**Returns**\
[Number](../JSLib/Number.md) 


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
[Number](../JSLib/Number.md) 


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
[Number](../JSLib/Number.md) 


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
### PK_COLUMN

Constant used when setting or getting the row identifier type of columns.
This value identifies columns that are defined as primary key in the database.

**Returns**\
[Number](../JSLib/Number.md) 


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
### ROWID_COLUMN

Constant used when setting or getting the row identifier type of columns.
This value identifies columns that are defined as primary key by the developer (but not in the database).

**Returns**\
[Number](../JSLib/Number.md) 


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
### SERVOY_SEQUENCE

Constant used when setting or getting the sequence type of columns.

**Returns**\
[Number](../JSLib/Number.md) 


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
### TENANT_COLUMN

Constant used when setting or getting the flags of columns.
This flag identifies columns that are marked as a tenant column.

**Returns**\
[Number](../JSLib/Number.md) 


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
[Number](../JSLib/Number.md) 


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
### UUID_COLUMN

Constant used when setting or getting the flags of columns.
This flag identifies columns whose values are treated as UUID.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
if (column.hasFlag(JSColumn.UUID_COLUMN))
{
	// handle uuid column
}
```
### UUID_GENERATOR

Constant used when setting or getting the sequence type of columns.

**Returns**\
[Number](../JSLib/Number.md) 


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
[Boolean](../JSLib/Boolean.md) boolean allow-null flag.


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
[String](../JSLib/String.md) String dataprovider id.


**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
var dataProviderId = column.getDataProviderID()
```
### getDefaultFormat()

Get the default format of the column.


**Returns**\
[String](../JSLib/String.md) String column default format.


**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
var format = column.getDefaultFormat()
```
### getDescription()

Get the description property of the column.


**Returns**\
[String](../JSLib/String.md) String column description.


**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customername')
var desc = column.getDescription()
```
### getForeignType()

Get the foreign type of the column.
The foreign type can be defined design time as a foreign key reference to another table.


**Returns**\
[String](../JSLib/String.md) String foreign type.


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
[Number](../JSLib/Number.md) int column length.


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
[String](../JSLib/String.md) String column name


**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
var colName = column.getName()
```
### getQualifiedName()

Get the qualified name (including table name) of the column as known by the database.
The name is quoted, if necessary, as defined by the actual database used.


**Returns**\
[String](../JSLib/String.md) String qualified column name.


**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
var qualifiedSqlName = column.getQualifiedName()
```
### getQuotedSQLName()

Returns a quoted version of the column name, if necessary, as defined by the actual database used.


**Returns**\
[String](../JSLib/String.md) column name, quoted if needed.


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

Get the row identifier type of the column.
The sequence type is one of:
 - JSColumn.PK_COLUMN
 - JSColumn.ROWID_COLUMN
 - JSColumn.NONE


**Returns**\
[Number](../JSLib/Number.md) int row identifier type.


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
[String](../JSLib/String.md) String sql name


**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
var sqlName = column.getSQLName()
```
### getSQLType()

Get the raw JDBC type of the column, which allows to check database specific types, like sting/byte column type variations.


**Returns**\
[Number](../JSLib/Number.md) int sql type.


**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
var sqlType = column.getSQLType();
```
### getScale()

Get the scale of the column as reported by the JDBC driver.


**Returns**\
[Number](../JSLib/Number.md) int column scale.


**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customername')
var scale = column.getScale()
```
### getSequenceType()

Get the sequence type of the column.
The sequence type is one of:
 - JSColumn.NONE
 - JSColumn.SERVOY_SEQUENCE
 - JSColumn.DATABASE_SEQUENCE
 - JSColumn.DATABASE_IDENTITY
 - JSColumn.UUID_GENERATOR;


**Returns**\
[Number](../JSLib/Number.md) int sequence type.


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
[JSTable](./JSTable.md) table The JSTable of this column.


**Sample**

```javascript

```
### getTitle()

Get the title property of the column. If title is null will return column name.


**Returns**\
[String](../JSLib/String.md) String column title.


**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customername')
var title = column.getTitle()
```
### getType()

Get the JDBC type of the column.
The type reported by the JDBC driver will be mapped to one of:
 - JSColumn.DATETIME
 - JSColumn.TEXT
 - JSColumn.NUMBER
 - JSColumn.INTEGER
 - JSColumn.MEDIA


**Returns**\
[Number](../JSLib/Number.md) int sql type.


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

Get the name JDBC type of the column.
The same mapping as defined in JSColumn.getType() is applied.


**Returns**\
[String](../JSLib/String.md) String sql name.


**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
var typeName = column.getTypeAsString()
```
### hasFlag(flag)

Check a flag of the column.
The flags are a bit pattern consisting of 1 or more of the following bits:
 - JSColumn.UUID_COLUMN
 - JSColumn.EXCLUDED_COLUMN
 - JSColumn.TENANT_COLUMN
 - JSColumn.NATIVE_COLUMN

**Parameters**\
[Number](../JSLib/Number.md) flag  ;

**Returns**\
[Boolean](../JSLib/Boolean.md) boolean whether flag is set.


**Sample**

```javascript
var table = databaseManager.getTable('db:/example_data/orders')
var column = table.getColumn('customerid')
if (column.hasFlag(JSColumn.UUID_COLUMN))
{
	// handle uuid column
}
```

