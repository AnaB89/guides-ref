# Treeview

Servoy extra components contains two tree components. The difference between the two is the model, the dbtreeview is based on foundset(s) while treeview is based on dataset.

DbTreeview shows multiple tree levels based on relation. From top foundset (datasource), one can show related nodes specified by a relation. Note that each relation is a database query , so for performance should not abuse the tree expand (from javascript). The tree works lazy and initializes data as requested.

Usual tree features are included, show a node checkbox, node image, tooltip, click callback, expand node... More information about model/api can be seen in Servoy Developer.

## Table of contents

* [Tree properties](tree.md#tree-properties)
* [Tree example](tree.md#tree-example)
* [Tree events](tree.md#tree-events)
* [Tree API](tree.md#tree-api)

## Tree properties

The component has one property, API should be used for everything else:

| Property  | Type    | Default | Description                                                                                                                                                                                                                    |
| --------- | ------- | ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| jsDataSet | dataset | null    | Dataset that is the model of the tree. Each row in dataset represents a node in the tree. Dataset should have 4 columns: node id, parent node id (null in case of top nodes or another valid id), node text and icon media url |

Instead of 'icon' it is possible to use 'fa-icon', in this case the values in the column should be FontAwesome classes, ex: 'fa fa-users'

## Tree example

```
var treeviewDataSet = databaseManager.createEmptyDataSet( 0,  ['id', 'pid', 'treeColumn', 'icon']);
treeviewDataSet.addRow([1,		null,	'Main group',	'media:///group.png']);
treeviewDataSet.addRow([2,		null,	'Second group',	'media:///group.png']);
treeviewDataSet.addRow([3,		2,		'Subgroup',		'media:///group.png']);
treeviewDataSet.addRow([4,		3,		'Mark',			'media:///user.png']);
treeviewDataSet.addRow([5,		3,		'George',		'media:///user.png']);
elements.mytree.setDataSet(treeviewDataSet);
```

## Tree events

| Event           | Params        | Return | Description                               |
| --------------- | ------------- | ------ | ----------------------------------------- |
| onNodeClicked   | nodeID:object |        | Fired when node in the tree is clicked.   |
| onNodeExpanded  | nodeID:object |        | Fired when node in the tree is expanded.  |
| onNodeCollapsed | nodeID:object |        | Fired when node in the tree is collapsed. |
| onNodeSelected  | nodeID:object |        | Fired when node in the tree is selected.  |

## Tree API

| Method           | Params            | Return    | Description                                                                                |
| ---------------- | ----------------- | --------- | ------------------------------------------------------------------------------------------ |
| setDataSet       | jsDataSet:dataset |           | Set jsDataset property, see above for detailed explanation about dataset structure.        |
| refresh          |                   |           | Refresh the tree display.                                                                  |
| expandNode       | nodeID:object     |           | Expand a node in tree identified by its id.                                                |
| isNodeExpanded   | nodeID:object     | boolean   | Returns if a node in tree is expanded. The node is identified by its id (given in dataset) |
| collapseNode     | nodeID:object     |           | Collapse a node in tree identified by its id.                                              |
| setSelectionNode | nodeID:object     |           | Sets selected node in the tree.                                                            |
| getSelectionNode |                   | object    | Gets selected node (id) in the tree.                                                       |
| getChildNodes    | nodeID:object     | object\[] | Gets child nodes of a parent node. Returns and array of child nodes.                       |
| getParentNode    | nodeID:object     | object    | Gets parent node id or null if top node.                                                   |
| getNodeLevel     | nodeID:object     | int       | Gets the level where a node is situated in the tree.                                       |
| getRootNodes     |                   | object\[] | Gets the top level nodes from the tree.                                                    |
