# JSRelation

## Constants Summary

| Type                          | Name                                                   | Summary                                     |
| ----------------------------- | ------------------------------------------------------ | ------------------------------------------- |
| [Number](../js-lib/number.md) | [FULL\_JOIN](jsrelation.md#FULL\_JOIN)                 | Constant for the joinType of a JSRelation.. |
| [Number](../js-lib/number.md) | [INNER\_JOIN](jsrelation.md#INNER\_JOIN)               | Constant for the joinType of a JSRelation.. |
| [Number](../js-lib/number.md) | [LEFT\_OUTER\_JOIN](jsrelation.md#LEFT\_OUTER\_JOIN)   | Constant for the joinType of a JSRelation.. |
| [Number](../js-lib/number.md) | [RIGHT\_OUTER\_JOIN](jsrelation.md#RIGHT\_OUTER\_JOIN) | Constant for the joinType of a JSRelation.. |

## Property Summary

| Type                            | Name                                                                                                 | Summary                                                                                                          |
| ------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| [Boolean](../js-lib/boolean.md) | [allowCreationRelatedRecords](jsrelation.md#allowCreationRelatedRecords)                             | Flag that tells if related records can be created through this relation..                                        |
| [Boolean](../js-lib/boolean.md) | [allowParentDeleteWhenHavingRelatedRecords](jsrelation.md#allowParentDeleteWhenHavingRelatedRecords) | Flag that tells if the parent record can be deleted while it has related records..                               |
| [Boolean](../js-lib/boolean.md) | [deleteRelatedRecords](jsrelation.md#deleteRelatedRecords)                                           | Flag that tells if related records should be deleted or not when a parent record is deleted..                    |
| [String](../js-lib/string.md)   | [foreignDataSource](jsrelation.md#foreignDataSource)                                                 | Qualified name of the foreign data source..                                                                      |
| [String](../js-lib/string.md)   | [initialSort](jsrelation.md#initialSort)                                                             | A String which specified a set of sort options for the initial sorting of data retrieved through this relation.. |
| [Number](../js-lib/number.md)   | [joinType](jsrelation.md#joinType)                                                                   | The join type that is performed between the primary table and the foreign table..                                |
| [String](../js-lib/string.md)   | [name](jsrelation.md#name)                                                                           | The name of the relation..                                                                                       |
| [String](../js-lib/string.md)   | [primaryDataSource](jsrelation.md#primaryDataSource)                                                 | Qualified name of the primary data source..                                                                      |

## Methods Summary

| Type                                | Name                                                                                                                                                        | Summary                                                                                                   |
| ----------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| [Array](../js-lib/array.md)         | [getRelationItems()](jsrelation.md#getrelationitems)                                                                                                        | Returns an array of JSRelationItem objects representing the relation criteria defined for this relation.. |
| [UUID](../application/uuid.md)      | [getUUID()](jsrelation.md#getuuid)                                                                                                                          | Returns the UUID of the relation object.                                                                  |
| [JSRelationItem](jsrelationitem.md) | [newRelationItem(dataprovider, operator, foreinColumnName)](jsrelation.md#newrelationitem-dataprovider-operator-foreincolumnname)                           | Creates a new relation item for this relation..                                                           |
| void                                | [removeRelationItem(primaryDataProviderID, operator, foreignColumnName)](jsrelation.md#removerelationitem-primarydataproviderid-operator-foreigncolumnname) | Removes the desired relation item from the specified relation..                                           |

## Constants Details

### FULL\_JOIN

Constant for the joinType of a JSRelation. It is also used in solutionModel.newRelation(...).

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.joinType = JSRelation.LEFT_OUTER_JOIN;
```

### INNER\_JOIN

Constant for the joinType of a JSRelation. It is also used in solutionModel.newRelation(...).

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.joinType = JSRelation.LEFT_OUTER_JOIN;
```

### LEFT\_OUTER\_JOIN

Constant for the joinType of a JSRelation. It is also used in solutionModel.newRelation(...).

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.joinType = JSRelation.LEFT_OUTER_JOIN;
```

### RIGHT\_OUTER\_JOIN

Constant for the joinType of a JSRelation. It is also used in solutionModel.newRelation(...).

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.joinType = JSRelation.LEFT_OUTER_JOIN;
```

## Properties Details

### allowCreationRelatedRecords

Flag that tells if related records can be created through this relation.

The default value of this flag is "false".

**Returns**\
[Boolean](../js-lib/boolean.md)

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.allowCreationRelatedRecords = true;
```

### allowParentDeleteWhenHavingRelatedRecords

Flag that tells if the parent record can be deleted while it has related records.

The default value of this flag is "true".

**Returns**\
[Boolean](../js-lib/boolean.md)

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.allowParentDeleteWhenHavingRelatedRecords = false;
```

### deleteRelatedRecords

Flag that tells if related records should be deleted or not when a parent record is deleted.

The default value of this flag is "false".

**Returns**\
[Boolean](../js-lib/boolean.md)

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.deleteRelatedRecords = true;
```

### foreignDataSource

Qualified name of the foreign data source. Contains both the name of the foreign server and the name of the foreign table.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.primaryDataSource = 'db:/user_data/another_parent_table';
relation.foreignDataSource = 'db:/user_data/another_child_table';
```

### initialSort

A String which specified a set of sort options for the initial sorting of data retrieved through this relation.

Has the form "column\_name asc, another\_column\_name desc, ...".

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.initialSort = 'another_child_table_text asc';
```

### joinType

The join type that is performed between the primary table and the foreign table. Can be "inner join" or "left outer join".

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.joinType = JSRelation.LEFT_OUTER_JOIN;
```

### name

The name of the relation.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.name = 'anotherName';
var firstTab = tabs.newTab('firstTab', 'Child Form', childForm, relation);
firstTab.relationName = relation.name;
```

### primaryDataSource

Qualified name of the primary data source. Contains both the name of the primary server and the name of the primary table.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.primaryDataSource = 'db:/user_data/another_parent_table';
relation.foreignDataSource = 'db:/user_data/another_child_table';
```

## Methods Details

### getRelationItems()

Returns an array of JSRelationItem objects representing the relation criteria defined for this relation.

**Returns**\
[Array](../js-lib/array.md) An array of JSRelationItem instances representing the relation criteria of this relation.

**Sample**

```javascript
var criteria = relation.getRelationItems();
for (var i=0; i<criteria.length; i++)
{
	var item = criteria[i];
	application.output('relation item no. ' + i);
	application.output('primary column: ' + item.primaryDataProviderID);
	application.output('operator: ' + item.operator);
	application.output('foreign column: ' + item.foreignColumnName);
}
```

### getUUID()

Returns the UUID of the relation object

**Returns**\
[UUID](../application/uuid.md)

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
application.output(relation.getUUID().toString())
```

### newRelationItem(dataprovider, operator, foreinColumnName)

Creates a new relation item for this relation. The primary dataprovider, the foreign data provider and one relation operators (like '=' '!=' '>' '<') must be provided.

**Parameters**\
[String](../js-lib/string.md) dataprovider The name of the primary dataprovider.\
[String](../js-lib/string.md) operator The operator used to relate the primary and the foreign dataproviders.\
[String](../js-lib/string.md) foreinColumnName The name of the foreign dataprovider.

**Returns**\
[JSRelationItem](jsrelationitem.md) A JSRelationItem instance representing the newly added relation item.

**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.newRelationItem('another_parent_table_id', '=', 'another_child_table_parent_id');
// for literals use a prefix
relation.newRelationItem(JSRelationItem.LITERAL_PREFIX + "'hello'",'=', 'mytextfield');
```

### removeRelationItem(primaryDataProviderID, operator, foreignColumnName)

Removes the desired relation item from the specified relation.

**Parameters**\
[String](../js-lib/string.md) primaryDataProviderID the primary data provider (column) name\
[String](../js-lib/string.md) operator the operator\
[String](../js-lib/string.md) foreignColumnName the foreign column name

**Returns**\
void

**Sample**

```javascript
var relation = solutionModel.newRelation('myRelation', 'db:/myServer/parentTable', 'db:/myServer/childTable', JSRelation.INNER_JOIN);
relation.newRelationItem('someColumn1', '=', 'someColumn2');
relation.newRelationItem('anotherColumn', '=', 'someOtherColumn');
relation.removeRelationItem('someColumn1', '=', 'someColumn2');
var criteria = relation.getRelationItems();
for (var i = 0; i < criteria.length; i++) {
	var item = criteria[i];
	application.output('primary column: ' + item.primaryDataProviderID);
	application.output('operator: ' + item.operator);
	application.output('foreign column: ' + item.foreignColumnName);
}
```
