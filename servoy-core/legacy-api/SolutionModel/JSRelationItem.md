#  JSRelationItem

## **Return Types**
[JSRelationItem](./JSRelationItem.md),
## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [String](../JSLib/String.md) | [LITERAL_PREFIX](JSRelationItem.md#LITERAL_PREFIX)                   | Constant for using literals in solution model in relations..                                    |

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [foreignColumnName](JSRelationItem.md#foreignColumnName)                   | The name of the column from the destination table that this relation item is based on..                                    |
| [String](../JSLib/String.md) | [operator](JSRelationItem.md#operator)                   | The operator that defines the relationship between the primary dataprovider and the foreign column..                                    |
| [String](../JSLib/String.md) | [primaryDataProviderID](JSRelationItem.md#primaryDataProviderID)                   | The name of the column from the source table that this relation item is based on..                                    |
| [Object](../JSLib/Object.md) | [primaryLiteral](JSRelationItem.md#primaryLiteral)                   | Get the literal..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [getComment()](JSRelationItem.md#getcomment)                   | Returns the comment of this component..                                    |
| [UUID](../Application/UUID.md) | [getUUID()](JSRelationItem.md#getuuid)                   | Returns the UUID of this component..                                    |

## Constants Details

### LITERAL_PREFIX

Constant for using literals in solution model in relations.
Strings must be passed as quoted value to make a distinction between string '5' and number 5.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
relation.newRelationItem(JSRelationItem.LITERAL_PREFIX + "'hello'",'=', 'mytextfield');
```

## Properties Details

### foreignColumnName

The name of the column from the destination table
that this relation item is based on.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
var criteria = relation.newRelationItem('parent_table_id', '=', 'child_table_parent_id');
criteria.primaryDataProviderID = 'parent_table_text';
criteria.foreignColumnName = 'child_table_text';
criteria.operator = '<';
```
### operator

The operator that defines the relationship between the primary dataprovider
and the foreign column.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
var criteria = relation.newRelationItem('parent_table_id', '=', 'child_table_parent_id');
criteria.primaryDataProviderID = 'parent_table_text';
criteria.foreignColumnName = 'child_table_text';
criteria.operator = '<';
```
### primaryDataProviderID

The name of the column from the source table
that this relation item is based on.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
var criteria = relation.newRelationItem('parent_table_id', '=', 'child_table_parent_id');
criteria.primaryDataProviderID = 'parent_table_text';
criteria.foreignColumnName = 'child_table_text';
criteria.operator = '<';
```
### primaryLiteral

Get the literal.

**Returns**\
[Object](../JSLib/Object.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
var criteria = relation.newRelationItem(JSRelationItem.LITERAL_PREFIX + "'hello'",'=', 'myTextField');
criteria.primaryLiteral = 'literal_text';
//criteria.primaryLiteral = number;
var primaryLiteral = criteria.primaryLiteral;
```

## Methods Details

### getComment()

Returns the comment of this component.


**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var comment = solutionModel.getForm("my_form").getButton("my_button").getComment();
application.output(comment);
```
### getUUID()

Returns the UUID of this component.


**Returns**\
[UUID](../Application/UUID.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var button_uuid = solutionModel.getForm("my_form").getButton("my_button").getUUID();
application.output(button_uuid.toString());
```

