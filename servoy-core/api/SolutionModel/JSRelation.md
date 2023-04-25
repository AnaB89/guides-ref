#  JSRelation


## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [FULL_JOIN](JSRelation.md#FULL_JOIN)                   | Constant for the joinType of a JSRelation..                                    |
| [Number](../JSLib/Number.md) | [INNER_JOIN](JSRelation.md#INNER_JOIN)                   | Constant for the joinType of a JSRelation..                                    |
| [Number](../JSLib/Number.md) | [LEFT_OUTER_JOIN](JSRelation.md#LEFT_OUTER_JOIN)                   | Constant for the joinType of a JSRelation..                                    |
| [Number](../JSLib/Number.md) | [RIGHT_OUTER_JOIN](JSRelation.md#RIGHT_OUTER_JOIN)                   | Constant for the joinType of a JSRelation..                                    |

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../JSLib/Boolean.md) | [allowCreationRelatedRecords](JSRelation.md#allowCreationRelatedRecords)                   | Flag that tells if related records can be created through this relation..                                    |
| [Boolean](../JSLib/Boolean.md) | [allowParentDeleteWhenHavingRelatedRecords](JSRelation.md#allowParentDeleteWhenHavingRelatedRecords)                   | Flag that tells if the parent record can be deleted while it has related records..                                    |
| [Boolean](../JSLib/Boolean.md) | [deleteRelatedRecords](JSRelation.md#deleteRelatedRecords)                   | Flag that tells if related records should be deleted or not when a parent record is deleted..                                    |
| [String](../JSLib/String.md) | [foreignDataSource](JSRelation.md#foreignDataSource)                   | Qualified name of the foreign data source..                                    |
| [String](../JSLib/String.md) | [initialSort](JSRelation.md#initialSort)                   | A String which specified a set of sort options for the initial sorting of data retrieved through this relation..                                    |
| [Number](../JSLib/Number.md) | [joinType](JSRelation.md#joinType)                   | The join type that is performed between the primary table and the foreign table..                                    |
| [String](../JSLib/String.md) | [name](JSRelation.md#name)                   | The name of the relation..                                    |
| [String](../JSLib/String.md) | [primaryDataSource](JSRelation.md#primaryDataSource)                   | Qualified name of the primary data source..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Array](../JSLib/Array.md) | [getRelationItems()](JSRelation.md#getrelationitems)                   | Returns an array of JSRelationItem objects representing the relation criteria defined for this relation..                                    |
| [UUID](../Application/UUID.md) | [getUUID()](JSRelation.md#getuuid)                   | Returns the UUID of the relation object.                                    |
| [JSRelationItem](./JSRelationItem.md) | [newRelationItem(dataprovider, operator, foreinColumnName)](JSRelation.md#newrelationitem-dataprovider-operator-foreincolumnname)                   | Creates a new relation item for this relation..                                    |
|void | [removeRelationItem(primaryDataProviderID, operator, foreignColumnName)](JSRelation.md#removerelationitem-primarydataproviderid-operator-foreigncolumnname)                   | Removes the desired relation item from the specified relation..                                    |

## Constants Details

### FULL_JOIN

Constant for the joinType of a JSRelation. It is also used in solutionModel.newRelation(...).

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.joinType = JSRelation.LEFT_OUTER_JOIN;
```
### INNER_JOIN

Constant for the joinType of a JSRelation. It is also used in solutionModel.newRelation(...).

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.joinType = JSRelation.LEFT_OUTER_JOIN;
```
### LEFT_OUTER_JOIN

Constant for the joinType of a JSRelation. It is also used in solutionModel.newRelation(...).

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.joinType = JSRelation.LEFT_OUTER_JOIN;
```
### RIGHT_OUTER_JOIN

Constant for the joinType of a JSRelation. It is also used in solutionModel.newRelation(...).

**Returns**\
[Number](../JSLib/Number.md) 


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
[Boolean](../JSLib/Boolean.md) 


**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.allowCreationRelatedRecords = true;
```
### allowParentDeleteWhenHavingRelatedRecords

Flag that tells if the parent record can be deleted while it has related records.

The default value of this flag is "true".

**Returns**\
[Boolean](../JSLib/Boolean.md) 


**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.allowParentDeleteWhenHavingRelatedRecords = false;
```
### deleteRelatedRecords

Flag that tells if related records should be deleted or not when a parent record is deleted.

The default value of this flag is "false".

**Returns**\
[Boolean](../JSLib/Boolean.md) 


**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.deleteRelatedRecords = true;
```
### foreignDataSource

Qualified name of the foreign data source. Contains both the name of the foreign
server and the name of the foreign table.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.primaryDataSource = 'db:/user_data/another_parent_table';
relation.foreignDataSource = 'db:/user_data/another_child_table';
```
### initialSort

A String which specified a set of sort options for the initial sorting of data
retrieved through this relation.

Has the form "column_name asc, another_column_name desc, ...".

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.initialSort = 'another_child_table_text asc';
```
### joinType

The join type that is performed between the primary table and the foreign table.
Can be "inner join" or "left outer join".

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.joinType = JSRelation.LEFT_OUTER_JOIN;
```
### name

The name of the relation.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
relation.name = 'anotherName';
var firstTab = tabs.newTab('firstTab', 'Child Form', childForm, relation);
firstTab.relationName = relation.name;
```
### primaryDataSource

Qualified name of the primary data source. Contains both the name of the primary server
and the name of the primary table.

**Returns**\
[String](../JSLib/String.md) 


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
[Array](../JSLib/Array.md) An array of JSRelationItem instances representing the relation criteria of this relation.


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
[UUID](../Application/UUID.md) 


**Sample**

```javascript
var relation = solutionModel.newRelation('parentToChild', 'db:/example_data/parent_table', 'db:/example_data/child_table', JSRelation.INNER_JOIN);
application.output(relation.getUUID().toString())
```
### newRelationItem(dataprovider, operator, foreinColumnName)

Creates a new relation item for this relation. The primary dataprovider, the foreign data provider 
and one relation operators (like '=' '!=' '>' '<') must be provided.

**Parameters**\
[String](../JSLib/String.md) dataprovider The name of the primary dataprovider.\
[String](../JSLib/String.md) operator The operator used to relate the primary and the foreign dataproviders.\
[String](../JSLib/String.md) foreinColumnName The name of the foreign dataprovider.

**Returns**\
[JSRelationItem](./JSRelationItem.md) A JSRelationItem instance representing the newly added relation item.


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
[String](../JSLib/String.md) primaryDataProviderID the primary data provider (column) name\
[String](../JSLib/String.md) operator the operator\
[String](../JSLib/String.md) foreignColumnName the foreign column name

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

