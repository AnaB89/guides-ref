#  ColumnInfo


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [autoEnterSubType](ColumnInfo.md#autoEnterSubType)                   | The subtype of autoenter configured for the column..                                    |
| [Number](../JSLib/Number.md) | [autoEnterType](ColumnInfo.md#autoEnterType)                   | The type of autoenter configured for the column..                                    |
| [String](../JSLib/String.md) | [converterName](ColumnInfo.md#converterName)                   | The name of the converter used for this column..                                    |
| [String](../JSLib/String.md) | [converterProperties](ColumnInfo.md#converterProperties)                   | The properties of the converter used for this column..                                    |
| [String](../JSLib/String.md) | [databaseDefaultValue](ColumnInfo.md#databaseDefaultValue)                   | The database default value that is used when autoenter is set to database default..                                    |
| [String](../JSLib/String.md) | [databaseSequenceName](ColumnInfo.md#databaseSequenceName)                   | The database sequence name that is used when autoenter is set to sequence and autoenter subtype is set to database sequence..                                    |
| [String](../JSLib/String.md) | [defaultFormat](ColumnInfo.md#defaultFormat)                   | The default format of the column..                                    |
| [String](../JSLib/String.md) | [defaultValue](ColumnInfo.md#defaultValue)                   | The value that is used when autoenter is set to custom value..                                    |
| [String](../JSLib/String.md) | [description](ColumnInfo.md#description)                   | The description of the column..                                    |
| [String](../JSLib/String.md) | [foreignType](ColumnInfo.md#foreignType)                   | The foreign type of the column..                                    |
| [String](../JSLib/String.md) | [lookupValue](ColumnInfo.md#lookupValue)                   | The lookup value that is used when autotype is set to lookup..                                    |
| [String](../JSLib/String.md) | [titleText](ColumnInfo.md#titleText)                   | The title of the column..                                    |
| [String](../JSLib/String.md) | [validatorName](ColumnInfo.md#validatorName)                   | The name of the validator used for the column..                                    |
| [String](../JSLib/String.md) | [validatorProperties](ColumnInfo.md#validatorProperties)                   | The properties of the validator used for the column..                                    |

## Properties Details

### autoEnterSubType

The subtype of autoenter configured for the column. The available options depend
on the type of autoenter.

If autoenter is set to system value, then the subtype can be one of: none, creation datetime,
creation username, modification datetime, modification username, database managed,
creation user uid, modification user uid, creation server datetime or modification server datetime.

If autoenter is set to sequence, then the subtype can be one of: none, Servoy sequence,
database sequence, database identity or universally unique identifier.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```
### autoEnterType

The type of autoenter configured for the column. Can be one of: none,
system value, sequence, custom value or lookup value.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```
### converterName

The name of the converter used for this column.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### converterProperties

The properties of the converter used for this column.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### databaseDefaultValue

The database default value that is used when autoenter is set to database default.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### databaseSequenceName

The database sequence name that is used when autoenter is set to sequence and autoenter subtype
is set to database sequence.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### defaultFormat

The default format of the column.
Currently only strings or numbers are supported.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### defaultValue

The value that is used when autoenter is set to custom value.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### description

The description of the column.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### foreignType

The foreign type of the column. It is used for foreign key columns, to hold the foreign table they point to.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### lookupValue

The lookup value that is used when autotype is set to lookup.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### titleText

The title of the column.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### validatorName

The name of the validator used for the column.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### validatorProperties

The properties of the validator used for the column.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```

