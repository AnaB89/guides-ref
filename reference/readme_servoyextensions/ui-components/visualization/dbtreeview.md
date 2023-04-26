# DBTreeview

Servoy extra components contains two tree components. The difference between the two is the model, the dbtreeview is based on foundset(s) while treeview is based on dataset.

DbTreeview shows multiple tree levels based on relation. From top foundset (datasource), one can show related nodes specified by a relation. Note that each relation is a database query , so for performance should not abuse the tree expand (from javascript). The tree works lazy and initializes data as requested.

Usual tree features are included, show a node checkbox, node image, tooltip, click callback, expand node... More information about model/api can be seen in Servoy Developer.

This component is a porting to NG of Servoy's DBTreeView bean, you can find more details about the migration here: https://wiki.servoy.com/display/DOCS/Upgrading+to+Servoy+8.x.x#UpgradingtoServoy8.x.x-DBTreeView

Here is a sample code of the tree initialization:

```
//set the relation to discover other nodes (when clicked open)
elements.dbtreeview.setNRelationName(controller.getDataSource(), 'book_nodes_to_book_nodes_parent_childs');
		
//set the name of dataprovider to use for text display on a node
elements.dbtreeview.setTextDataprovider(controller.getDataSource(), 'label_text');

//set the method to call and dataprovider value to pass when node clicked
elements.dbtreeview.setCallBackInfo(controller.getDataSource(), globals.node_selected,'node_id');

//search the root node(s)
controller.find();
parent_id = 0;
controller.search();

//set the root node(s) and set the name of dataprovider to use for text display on a node
elements.dbtreeview.addRoots(foundset);

var pathAr = new Array(1,2,3);
elements.dbtreeview.setSelectionPath(pathAr);
```

## Table of contents

* [DBTreeView properties](dbtreeview.md#dbtreeview-properties)
* [DBTreeView API](dbtreeview.md#dbtreeview-api)

## DBTreeView properties

The component has only one public property, component should be handled via API:

| Property         | Type    | Default | Description                                   |
| ---------------- | ------- | ------- | --------------------------------------------- |
| autoRefresh      | boolean | true    | When false component will not autorefresh     |
| enabled          | boolean | true    | When false component is not enabled           |
| responsiveHeight | int     | true    | Set component max height in responsive layout |
| visible          | visible | true    | When false component is not visible           |

## DBTreeView API

| Method                          | Params                                                         | Return    | Description                                                                                                                                                                                |
| ------------------------------- | -------------------------------------------------------------- | --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| addRoots                        | root:foundsetRef                                               |           | Add foundset to the list of foundsets used to create the tree's root nodes.                                                                                                                |
| removeAllRoots                  |                                                                |           | Remove all root foundsets.                                                                                                                                                                 |
| refresh                         |                                                                |           | Refresh the tree display.                                                                                                                                                                  |
| isNodeExpanded                  | pk:object\[]                                                   | boolean   | Returns if a node in tree is expanded. The path is given by an array of foundset primary keys, one pk for each level of the tree                                                           |
| setExpandNode                   | pk: object\[] , state: boolean                                 |           | Set expand state on node identified by array of primary keys.                                                                                                                              |
| setNodeLevelVisible             | level: int , visible: boolean                                  |           | Expand or collapse tree to certain level.                                                                                                                                                  |
| setTextDataprovider             | datasource: string , textdataprovider: string                  |           | Set dataprovider that will be displed for a foundset from the tree(each level in tree has foundset as a model).                                                                            |
| setNRelationName                | datasource: string , nrelationname: string                     |           | Set relation for displaying a datasource foundset.                                                                                                                                         |
| setHasCheckBoxDataprovider      | datasource: string , hascheckboxdataprovider: string           |           | Set dataprovider for deciding if checkbox will be displayed for a certain foundset (tree level).                                                                                           |
| setCallBackInfo                 | datasource: string , callbackfunction: function, param: string |           | Set callback method that will be called when expanding/collapsing a node in a foundset(tree level).                                                                                        |
| setCheckBoxValueDataprovider    | datasource: string , checkboxvaluedataprovider: string         |           | Set dataprovider for the checkbox value to show(checked/unchecked).                                                                                                                        |
| setMethodToCallOnCheckBoxChange | datasource: string , callbackfunction :function, param: string |           | Set callback method that will be called when checkbox is clicked/changed.                                                                                                                  |
| setToolTipTextDataprovider      | datasource: string , tooltiptextdataprovider: string           |           | Set dataprovider for the tooltip text displayed for a datasource foundset.                                                                                                                 |
| setImageURLDataprovider         | datasource: string , imageurldataprovider: string              |           | Set dataprovider for the image displayed in tree node for a datasource foundset.                                                                                                           |
| setChildSortDataprovider        | datasource: string , childsortdataprovider: string             |           | Set the dataprovider name to retrieve column name and sort order for the child nodes. The provided data must be a string of form : column\_name\_used\_for\_sort sort\_order(asc or desc). |
| setMethodToCallOnDoubleClick    | datasource: string , callbackfunction: function, param: string |           | Set callback info for a datasource foundset doubleclick event.                                                                                                                             |
| setSelectionPath                | pk:object\[]                                                   |           | Sets selected node in the tree. The path is given by an array of foundset primary keys, one pk for each level of the tree                                                                  |
| getSelectionPath                |                                                                | object\[] | Gets selected node in the tree. The path is given by an array of foundset primary keys, one pk for each level of the tree                                                                  |
| setInitialCheckBoxValues        | datasource: string, initialCheckboxValuesPks: string\[]        |           | Set intial checked checkboxes for a datasource foundset when no checkboxdataprovider is used                                                                                               |
| setHasCheckBoxValue             | datasource: string, hasCheckboxValuePks: string\[]             |           | Set the nodes that should have checkbox for a datasource when no hascheckboxdataprovider is used                                                                                           |
| updateCheckBoxValues            | datasource: string, pks: string\[], state:boolean              |           | Update checkbox state for nodes                                                                                                                                                            |
| getCheckBoxValues               | datasource: string                                             | string\[] | Returns array of pk of nodes that are checked for the datasource                                                                                                                           |
