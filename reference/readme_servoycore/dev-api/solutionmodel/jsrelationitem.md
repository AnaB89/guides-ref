# JSRelationItem

## **Return Types**

[JSRelationItem](jsrelationitem.md),

## Constants Summary

| Type                          | Name                                                 | Summary                                                      |
| ----------------------------- | ---------------------------------------------------- | ------------------------------------------------------------ |
| [String](../js-lib/string.md) | [LITERAL\_PREFIX](jsrelationitem.md#LITERAL\_PREFIX) | Constant for using literals in solution model in relations.. |

## Property Summary

| Type                          | Name                                                             | Summary                                                                                              |
| ----------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| [String](../js-lib/string.md) | [foreignColumnName](jsrelationitem.md#foreignColumnName)         | The name of the column from the destination table that this relation item is based on..              |
| [String](../js-lib/string.md) | [operator](jsrelationitem.md#operator)                           | The operator that defines the relationship between the primary dataprovider and the foreign column.. |
| [String](../js-lib/string.md) | [primaryDataProviderID](jsrelationitem.md#primaryDataProviderID) | The name of the column from the source table that this relation item is based on..                   |
| [Object](../js-lib/object.md) | [primaryLiteral](jsrelationitem.md#primaryLiteral)               | Get the literal..                                                                                    |

## Methods Summary

| Type                           | Name                                         | Summary                                 |
| ------------------------------ | -------------------------------------------- | --------------------------------------- |
| [String](../js-lib/string.md)  | [getComment()](jsrelationitem.md#getcomment) | Returns the comment of this component.. |
| [UUID](../application/uuid.md) | [getUUID()](jsrelationitem.md#getuuid)       | Returns the UUID of this component..    |

## Constants Details

### LITERAL\_PREFIX

Constant for using literals in solution model in relations. Strings must be passed as quoted value to make a distinction between string '5' and number 5.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
relation.newRelationItem(JSRelationItem.LITERAL_PREFIX + "'hello'",'=', 'mytextfield');
```

## Properties Details

### foreignColumnName

The name of the column from the destination table that this relation item is based on.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
var criteria = relation.newRelationItem('parent_table_id', '=', 'child_table_parent_id');
criteria.primaryDataProviderID = 'parent_table_text';
criteria.foreignColumnName = 'child_table_text';
criteria.operator = '<';
```

### operator

The operator that defines the relationship between the primary dataprovider and the foreign column.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
var criteria = relation.newRelationItem('parent_table_id', '=', 'child_table_parent_id');
criteria.primaryDataProviderID = 'parent_table_text';
criteria.foreignColumnName = 'child_table_text';
criteria.operator = '<';
```

### primaryDataProviderID

The name of the column from the source table that this relation item is based on.

**Returns**\
[String](../js-lib/string.md)

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
[Object](../js-lib/object.md)

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
[String](../js-lib/string.md)

**Sample**

```javascript
var comment = solutionModel.getForm("my_form").getButton("my_button").getComment();
application.output(comment);
```

### getUUID()

Returns the UUID of this component.

**Returns**\
[UUID](../application/uuid.md)

**Sample**

```javascript
var button_uuid = solutionModel.getForm("my_form").getButton("my_button").getUUID();
application.output(button_uuid.toString());
```
