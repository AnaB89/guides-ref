#  Relation

## **Supported Clients**

    SmartClient
    WebClient
    NGClient
    MobileClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../JSLib/Boolean.md) | [allowCreationRelatedRecords](Relation.md#allowCreationRelatedRecords)                   | Flag that tells if related records can be created through this relation..                                    |
| [Boolean](../JSLib/Boolean.md) | [allowParentDeleteWhenHavingRelatedRecords](Relation.md#allowParentDeleteWhenHavingRelatedRecords)                   | Flag that tells if the parent record can be deleted while it has related records..                                    |
| [String](../JSLib/String.md) | [comment](Relation.md#comment)                   | .                                    |
| [Boolean](../JSLib/Boolean.md) | [deleteRelatedRecords](Relation.md#deleteRelatedRecords)                   | Flag that tells if related records should be deleted or not when a parent record is deleted..                                    |
| [String](../JSLib/String.md) | [deprecated](Relation.md#deprecated)                   | Gets the deprecate info for this element.                                    |
| [Number](../JSLib/Number.md) | [encapsulation](Relation.md#encapsulation)                   | The encapsulation mode of this Relation..                                    |
| [String](../JSLib/String.md) | [foreignDataSource](Relation.md#foreignDataSource)                   | Qualified name of the foreign data source..                                    |
| [String](../JSLib/String.md) | [initialSort](Relation.md#initialSort)                   | A String which specified a set of sort options for the initial sorting of data retrieved through this relation..                                    |
| [Number](../JSLib/Number.md) | [joinType](Relation.md#joinType)                   | The join type that is performed between the primary table and the foreign table..                                    |
| [String](../JSLib/String.md) | [name](Relation.md#name)                   | The name of the relation..                                    |
| [String](../JSLib/String.md) | [primaryDataSource](Relation.md#primaryDataSource)                   | Qualified name of the primary data source..                                    |

## Properties Details

### allowCreationRelatedRecords

Flag that tells if related records can be created through this relation.

The default value of this flag is "false".

**Returns**\
[Boolean](../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### allowParentDeleteWhenHavingRelatedRecords

Flag that tells if the parent record can be deleted while it has related records.

The default value of this flag is "true".

**Returns**\
[Boolean](../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### comment



**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### deleteRelatedRecords

Flag that tells if related records should be deleted or not when a parent record is deleted.

The default value of this flag is "false".

**Returns**\
[Boolean](../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### deprecated

Gets the deprecate info for this element

**Returns**\
[String](../JSLib/String.md) the deprecate info for this element or null if it is not deprecated

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### encapsulation

The encapsulation mode of this Relation. The following can be used/checked:

- Public (not a separate option - if none of the below options are selected)
- Hide in scripting; Module Scope - not available in scripting from any other context except the form itself. Available in designer for the same module.
- Module Scope - available in both scripting and designer but only in the same module.

**Returns**\
[Number](../JSLib/Number.md) the encapsulation mode/level of the persist.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### foreignDataSource

Qualified name of the foreign data source. Contains both the name of the foreign
server and the name of the foreign table.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### initialSort

A String which specified a set of sort options for the initial sorting of data
retrieved through this relation.

Has the form "column_name asc, another_column_name desc, ...".

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### joinType

The join type that is performed between the primary table and the foreign table.
Can be "inner join" or "left outer join".

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### name

The name of the relation.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### primaryDataSource

Qualified name of the primary data source. Contains both the name of the primary server
and the name of the primary table.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```

