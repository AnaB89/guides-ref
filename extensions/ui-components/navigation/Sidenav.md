# sidenav

Since V1.1.0

Eager to get started ? Check out this [**video intro**](https://youtu.be/u4LVCbUdiOU)

Sidenav is a 4-levels depth navigation component. Is a side menu with selectable and collapsible nested menu items. The user can select or expand one menu item per time; a selected menu item is automatically expanded. The developer can control the sidenav component programmatically by editing the element's runtime properties and using the element's API. The sidenav can slide in/out to the left side or to the right side. The component can be used as a tablesspanel container, having a containedForm on the side of the menu which animates together with the menu. The component is fully stylable with CSS3.

![Sidenav Component](http://content.screencast.com/users/paronne/folders/Jing/media/e81454f1-3356-42ea-b76a-3d18f295ca42/sidenav.png)

## Table of contents

* [Getting Started](Sidenav.md#getting-started)
* [Menu Item](Sidenav.md#menu-item)
* [Styling Sidenav](Sidenav.md#styling-sidenav)
* [Sidenav Properties](Sidenav.md#sidenav-properties)
* [Sidenav Events](Sidenav.md#sidenav-events)
* [Sidenav API](Sidenav.md#sidenav-api)

## Getting Started

Use the api **setRootMenuItems** to populate the sidenav with [Menu Items](Sidenav.md#menu-item). You can nest Menu Items up to 4 levels depth.

```
var menu = [{
    id: 1,
    text: "Sample Item #1",
    styleClass : "sn-large",
    iconStyleClass:  "glyphicon glyphicon-search",
    data: { description: "This is sample information that can be added to a menuItem" },
    menuItems: [{
  	  id: 5,
  	  text: "Sub Item #1"
  	}, {
  	  id: 6,
  	  text: "Sub Item #2"}]
  }, {
    id: 2,
    text: "Sample Item #2"
  },{
    isDivider: true
  },{
    id: 3,
    text: "Sample Item #3",
    enabled: false
}];

  elements.sideNavigation.setRootMenuItems(menu);
```

The method setRootMenuItems requires an Array of Menu Item object.

## Menu Item

The menu item is a JSON object representing an item in the sidenav. A menu item may nest other menu items. A menu item may be also used as divider, which is nothing else then a line separating the menu item above and below, in this case all other properties of the menu item are ignored.

| Property       | Type           | Required | Description                                                                                                                                                                                                                                   |
| -------------- | -------------- | -------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| String, Number | id             | yes      | uniquely identifies the menuItem in the menu object.                                                                                                                                                                                          |
| String         | text           | no       | The menu text, optional, default is empty.                                                                                                                                                                                                    |
| String         | styleClass     | no       | add style classes to the menuItem, optional,. Separate multiple value with a SPACE char. example 'nav-large nav-primary'.                                                                                                                     |
| String         | iconStyleClass | no       | use style classes to display icons as Font Icons, optional. example 'glyphicon glyphicon-search'.                                                                                                                                             |
| Boolean        | enabled        | no       | menuItem cannot be selected or expanded if disabled, optional. Default true.                                                                                                                                                                  |
| Object         | data           | no       | data object can be used to add custom properties to the menuItem, optional. For example you may set the formName to be shown when the menuItem is selected { formName: "aFormName", description: "This menu item will open the given form" }. |
| Array          | menuItems      | no       | an array of nested menuItems, optional.                                                                                                                                                                                                       |
| Boolean        | isDivider      | no       | if true render a divider into the menu instead of a menuItem, optional. All other properties are ignored. Default false.                                                                                                                      |

This is a menu item with 2 sub menu items

```
var menuItem = {
    id: 1,
    text: "Sample Item #1",
    styleClass : "sn-large",
    iconStyleClass:  "glyphicon glyphicon-search",
    data: { description: "This is sample information that can be added to a menuItem" },
    menuItems: [{
  	  id: 5,
  	  text: "Sub Item #1"
  	}, {
  	  id: 6,
  	  text: "Sub Item #2"}]
  };
```

This menu item is instead rendered as a divider

```
 var menuDivider = {
    isDivider: true
  };
```

### Update a Menu Item

To update a menu item you should get the menu item object using the component's API [getMenuItem](Sidenav.md#getmenuitem), any change to the returned object will be reflected on the sidenav component.

Example

```
var menuItem = elements.sidenav.getMenuItem(1);
menuItem.text = "Update the text of the menuItem";
menuItem.styleClass = "nav-large nav-bold";
menuItem.data = { "lastUpdate" : new Date(); }
```

Updating an old reference of the menuItem which has not been retrieved via API it won't be possible.

Don't do this:

```
var menuItem = { id:1, text: "init text"};
elements.sidenav.addMenuItem(menuItem);
menuItem.text = "Update text of menu item 1 like this is not reflected on UI"
```

Instead do

```
var menuItem = { id:1, text: "init text"};
elements.sidenav.addMenuItem(menuItem);
// get the menuItem via API
menuItem = elements.sidenav.getMenuItem(1); 
menuItem.text = "Update text of menu item 1 like this is correct"
```

## Styling Sidenav

There are several CSS class selectors you can use for fine-grained styling of the sidenav component.

| element selector           | summary                                                                   |
| -------------------------- | ------------------------------------------------------------------------- |
| .svy-extra-sidenav         | the root element, style is applied to the sidenav and to the tablesspanel |
| .svy-sidenav               | style the whole sidenav component                                         |
| .svy-sidenav-tablesspanel  | style the tablesspanel container                                          |
| .svy-sidenav-menu          | style the menu and all it's content                                       |
| .svy-sidenav-dropdown      | style the dropdown list in each menu level                                |
| .svy-sidenav-item          | style the menu item in dropdown list                                      |
| .svy-sidenav-collapse-icon | stlye the collapse/expand icon                                            |
| .svy-sidenav-divider       | style the divider                                                         |
| .svy-navitem-selected      | style the selected menu item                                              |
| .svy-sidenav-collapsed     | style the menu item expanded                                              |
| .svy-sidenav-disabled      | style the menu item disabled                                              |
| .svy-slide-out             | stlye the nav menu when is closed                                         |

To style a specif element on a specific level combine the element element selector above with the level selector below

| level selector | summary                          |
| -------------- | -------------------------------- |
| .sn-level-1    | the elements in root level       |
| .sn-level-2    | the elements in the second level |
| .sn-level-3    | the elements in the third level  |
| .sn-level-4    | the elements in the fourth level |

Examples

```
/* Style all the menu items */
.svy-sidenav-item {
    font-size: 12px;
    color : #444;
    padding: 8px 15px;
}

/*Style the menu item in the first level only */
.svy-sidenav-item.sn-level-1 {
    font-size: 18px;
    color: #000;
}

/* Show a border the the selected item in the first level only */
.svy-navitem-selected.sn-level-1 {
    border-left: 3px solid;
}
```

## Sidenav Properties

| Property | Type                   | Default           | Description                                                                                                                                                                                                                                                                                                                                                                                                               |
| -------- | ---------------------- | ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Boolean  | animate                | true              | The menu animates when opened/closed and when items are expanded/collapsed.                                                                                                                                                                                                                                                                                                                                               |
| Boolean  | enabled                | true              | The menu is disabled, menu items cannot be selected or expanded. If disabled the items cannot be selected/collapsed neither programmatically via API.                                                                                                                                                                                                                                                                     |
| Form     | containedForm          |                   | The contained form property behaves as a tablesspanel container. The form is shown at the side of the menu and uses the same animation when the menu is opened or closed.                                                                                                                                                                                                                                                 |
| String   | iconCollapseStyleClass | fa fa-cart-down   | Font Icon used as icon for the menu item when is expanded.                                                                                                                                                                                                                                                                                                                                                                |
| String   | iconExpandStyleClass   | fa fa-caret-right | Font Icon used as icon for the menu item when is collapsed.                                                                                                                                                                                                                                                                                                                                                               |
| String   | iconOpenStyleClass     | fa fa-bars        | Font Icon used as icon for the toggle button to close the side menu.                                                                                                                                                                                                                                                                                                                                                      |
| String   | iconCloseStyleClass    | fa fa-bars        | Font Icon used as icon for the toggle button to open the side menu.                                                                                                                                                                                                                                                                                                                                                       |
| Boolean  | open                   | true              | If true the menu is open, when changed to false the menu slides away. Open cannot be set to false if the slidePosition is STATIC.                                                                                                                                                                                                                                                                                         |
| String   | scrollbarPosition      | LEFT              | defines the position of the srollbar for the sidenav. Possible values are LEFT and RIGHT.                                                                                                                                                                                                                                                                                                                                 |
| Number   | sidenavWidth           | 300               | the width, in pixel, of the sidenav menu; the containedForm will use the remaing width. The menu will use all the available width if sidenavWidth is set to 0. This option is ignored in a non-responsive form when the menu doesn't have a containedForm.                                                                                                                                                                |
| Number   | responsiveHeight       | 0                 | the height, in pixel, of the sidenav menu in a responsive form; The menu will use all the necessary height if the height is set to 0. This option is ignored in non-responsive forms.                                                                                                                                                                                                                                     |
| String   | slidePosition          | LEFT              | defines to which side the menu slides out when closed. Possible values are LEFT, RIGHT and STATIC. A STATIC menu cannot slide away, is always open.                                                                                                                                                                                                                                                                       |
| String   | slideAnimation         | SLIDE-MENU        | type SLIDE-MENU the menu slides away and is not visible when 'open' is false; for the type COLLAPSE-MENU the menu is collapsed and only the icons are visible when the 'open' is false; the menu is auto-expanded when hovered. COLLAPSE-MENU-NOHOVER has the same behavior of COLLAPSE-MENU but it doesn't automatically expand when hovered; note sub-level menu items won't be accessible when collapsed in this case. |
| String   | togglePosition         | FIXED-TOGGLE      | defines the position of the toggle button. possible values are FIXED-TOGGLE, SIDE-TOGGLE and HIDE-TOGGLE.                                                                                                                                                                                                                                                                                                                 |
| String   | styleClass             |                   | menu style Classes.                                                                                                                                                                                                                                                                                                                                                                                                       |
| Boolean  | visible                | true              | if the menu is visible or not.                                                                                                                                                                                                                                                                                                                                                                                            |

## Sidenav Events

| Event               | Params                                  | Return  | Description                                                                                                           |
| ------------------- | --------------------------------------- | ------- | --------------------------------------------------------------------------------------------------------------------- |
| onMenuItemCollapsed | menuItemId:String-Number, event:JSEvent |         | Event executed when the user collapses a Menu Item.                                                                   |
| onMenuItemExpanded  | menuItemId:String-Number, event:JSEvent |         | Event executed when a Menu Item is expanded.                                                                          |
| onMenuItemSelected  | menuItemId:String-Number, event:JSEvent | Boolean | Event executed when a Menu Item is selected. The selection will be prevented if the onMenuItemSelected returns false. |
| onOpenToggled       | event:JSEvent                           |         | Event executed when the user clicks on the open button to open or close the menu.                                     |

## Sidenav API

| Method                                                | Params                                                                                                             | Return                                                                          | Description                                                                                                  |
| ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| [addMenuItem](Sidenav.md#addmenuitem)                 | menuItem:[MenuItem](Sidenav.md#menu-item), menuItemId:String-Number, index:Number                                  | Boolean                                                                         | Add a menu item. The menu is added as sub Menu Item if a menuItemId is provided, otherwise is added in root. |
| [clearMenuItems](Sidenav.md#clearmenuitems)           | \[depth:Number]                                                                                                    |                                                                                 | Remove all the menu items. If depth is specified removes all the menu items at depth.                        |
| [getMenuItem](Sidenav.md#getmenuitem)                 | menuItemId:String-Number                                                                                           | [MenuItem](Sidenav.md#menu-item)                                                | Returns the menu item object.                                                                                |
| [getParentMenuItem](Sidenav.md#getparentmenuitem)     | menuItemId:String-Number                                                                                           | [MenuItem](Sidenav.md#menu-item)                                                | Returns the parent of the menu item object with id menuItemId.                                               |
| [getRootMenuItems](Sidenav.md#getrootmenuitems)       |                                                                                                                    | Array<[MenuItem](Sidenav.md#menu-item)>                                         | Returns the root menu items.                                                                                 |
| [getSelectedMenuItem](Sidenav.md#getselectedmenuitem) | \[level:Number]                                                                                                    | [MenuItem](Sidenav.md#menu-item)                                                | Returns the selected menu item.                                                                              |
| [getSubMenuItems](Sidenav.md#getsubmenuitems)         | menuItemId:String-Number                                                                                           | <p>menuItems:</p><p>Array&#x3C;<a href="Sidenav.md#menu-item">MenuItem</a>></p> | Get the menuItems of the menu item with id 'menuItemId'.                                                     |
| [isMenuItemEnabled](Sidenav.md#ismenuitemenabled)     | menuItemId:String-Number                                                                                           | Boolean                                                                         | Returns true if the menuItem and all it's ancestors are enabled.                                             |
| [isMenuItemExpanded](Sidenav.md#ismenuitemexpaned)    | menuItemId:String                                                                                                  | Number                                                                          | Boolean                                                                                                      |
| [setMenuItemEnabled](Sidenav.md#setmenuitemenabled)   | menuItemId:String-Number, enabled:Boolean                                                                          | Boolean                                                                         | Enable or disable the menu item.                                                                             |
| [setMenuItemExpanded](Sidenav.md#setmenuitemexpanded) | menuItemId:String-Number, expanded:Boolean, \[mustExecuteOnMenuItemExpand:Boolean]                                 | Boolean                                                                         | Force the menuItem to be expanded or collapsed.                                                              |
| [setRootMenuItems](Sidenav.md#setrootmenuitems)       | Array<[MenuItem](Sidenav.md#menu-item)>                                                                            |                                                                                 |                                                                                                              |
| [setSelectedMenuItem](Sidenav.md#setselectedmenuitem) | menuItemId:String, \[mustExecuteOnMenuItemSelect:Boolean], \[mustExecuteOnMenuItemExpand:Boolean], \[level:Number] | Boolean                                                                         | Select the menu item with the given id.                                                                      |
| [setSubMenuItems](Sidenav.md#setsubmenuitems)         | menuItemId:String-Number, menuItems:Array<[MenuItem](Sidenav.md#menu-item)>                                        | Boolean                                                                         | Set the menuItems as sub menu items of the menu item with id menuItemId.                                     |
| [removeMenuItem](removemenuitem/)                     | menuItemId:String-Number                                                                                           | Boolean                                                                         | Remove the menu item and all it's subMenuItems from the tree.                                                |
| [removeSubMenuItems](removesubmenuitems/)             | menuItemId:String-Number                                                                                           | Boolean                                                                         | Remove all the sub menu items of the menu item with id 'menuItemId'.                                         |

### addMenuItem

**Params**

| Type                             | Name       | Description                                                                                                           | Required                                     |
| -------------------------------- | ---------- | --------------------------------------------------------------------------------------------------------------------- | -------------------------------------------- |
| [MenuItem](Sidenav.md#menu-item) | menuItem   | the menu item object to be added.                                                                                     | Required                                     |
| String-Number                    | menuItemId | add the item as subMenuItem of the menuItemId.                                                                        | Optional, Default add the menu item as root. |
| Number                           | index      | 0-based. The index at which to insert the item. Optional. Index value should not be greater then number of sibelings. | Optional, Default is at the end.             |

**Returns** Boolean

Add a menu item. The menu is added as sub Menu Item if a menuItemId is provided, otherwise is added in root. If index is provided the menu is added at the specified index position, otherwise is added as last element. Return false if menuItemId cannot be found.

Example

```
 var menuItem = {
  id: 100,
  text: "Sample Item #1",
  styleClass : "nav-large nav-primary",
  iconStyleClass:  "glyphicon glyphicon-search",
  data: { description: "This is sample information that can be added to a menuItem" },
  menuItems: [{
  	id: 101,
  	text: "Sub Item #1"
  	}, {
  	id: 102,
  	text: "Sub Item #2"}]
  };
  elements.sideNavigation.addMenuItem(menuItem, 1, 0);
```

### clearMenuItems

**Params**

| Type   | Name  | Description                                            | Required            |
| ------ | ----- | ------------------------------------------------------ | ------------------- |
| Number | depth | 1-based. The depth to be cleared of all it's menuItems | Optional, Default 1 |

**Returns** void

Remove all the menu items. If depth is specified removes all the menu items at depth. If depth is equal to 1 all roots will be removed. Default depth is 1.

Example

```
 // clear the whole menu removing all nodes. 
 elements.sidenav.clearMenuItems();
  
 // clear menu at depth 2 removes the sub menu items of each root menu.
 elements.sidenav.clearMenuItems(2);
```

### getMenuItem

**Params**

| Type          | Name       | Description       | Required |
| ------------- | ---------- | ----------------- | -------- |
| String-Number | menuItemId | the menu item id. | Required |

**Returns** [MenuItem](Sidenav.md#menu-item)

Returns the menu item object.

### getParentMenuItem

**Params**

| Type          | Name       | Description       | Required |
| ------------- | ---------- | ----------------- | -------- |
| String-Number | menuItemId | the menu item id. | Required |

**Returns** [MenuItem](Sidenav.md#menu-item)

Returns the parent menu item object of the menu item with id menuItemId. Nothing is returned if the menu item is in the root menu.

### getRootMenuItems

**Params** _none_

**Returns** Array<[MenuItem](Sidenav.md#menu-item)>

Returns the root menu items.

### getSelectedMenuItem

**Params**

| Type   | Name  | Description                                                      | Required |
| ------ | ----- | ---------------------------------------------------------------- | -------- |
| Number | level | if level is provided search for the selected menu item at level. | Required |

**Returns** [MenuItem](Sidenav.md#menu-item)

Returns the selected menu item.

### getSubMenuItems

**Params**

| Type          | Name       | Description              | Required |
| ------------- | ---------- | ------------------------ | -------- |
| String-Number | menuItemId | the id of the menu item. | Required |

**Returns** Array<[MenuItem](Sidenav.md#menu-item)>

Get the menuItems of the menu item with id 'menuItemId'.

### isMenuItemEnabled

**Params**

| Type          | Name       | Description              | Required |
| ------------- | ---------- | ------------------------ | -------- |
| String-Number | menuItemId | the id of the menu item. | Required |

**Returns** Boolean

Returns true if the menuItem and all it's ancestors are enabled. Return false if menuItemId cannot be found or is disabled.

NOTE: The method returns false if any ancestor of the menuItem is not enabled; if the property enabled of the menuItem is set to true, but has a parent with the enabled property set to false, then isMenuItemEnabled returns false.

### isMenuItemExpanded

**Params**

| Type          | Name       | Description              | Required |
| ------------- | ---------- | ------------------------ | -------- |
| String-Number | menuItemId | the id of the menu item. | Required |

**Returns** Boolean

Returns true if the menuItem is expanded.

### setMenuItemEnabled

**Params**

| Type          | Name       | Description                                       | Required |
| ------------- | ---------- | ------------------------------------------------- | -------- |
| String-Number | menuItemId | the id of the menu item.                          | Required |
| Boolean       | enabled    | true to enable the menu item, false to disable it | Required |

**Returns** Boolean

Enable or disable the menu item. Return false if menuItemId cannot be found.

### setMenuItemExpanded

**Params**

| Type          | Name                        | Description                                                  | Required                 |
| ------------- | --------------------------- | ------------------------------------------------------------ | ------------------------ |
| String-Number | menuItemId                  | the id of the menu item.                                     | Required                 |
| Boolean       | expanded                    | force the menuItem to expand if true, is collapsed otherwise | Required                 |
| Boolean       | mustExecuteOnMenuItemExpand | force the onMenuItemExpand to be executed.                   | Optional, Default false. |

**Returns** Boolean

Return false if menuItemId cannot be found or is disabled.

### setRootMenuItems

**Params**

| Type                                    | Name      | Description                                                                                                                                                                                                                                                                                              | Required |
| --------------------------------------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- |
| Array<[MenuItem](Sidenav.md#menu-item)> | menuItems | is an array of MenuItem objects. Each MenuItem object should set the required properties 'id', which uniquely identifies the menuItem object in menu, and 'text' property. The MenuItem may contain the optional properties 'styleClass', 'iconStyleClass', 'data', 'enabled', 'menuItems', 'isDivider'. | Required |

**Returns** _void_

Init the menu setting the root menuItems.

Example

```
var menu = [{
  id: 1,
  text: "Sample Item #1",
  styleClass : "sn-large",
  iconStyleClass:  "glyphicon glyphicon-search",
  data: { description: "This is sample information that can be added to a menuItem" },
  menuItems: [{
  	id: 5,
  	text: "Sub Item #1"
  	}, {
  	id: 6,
  	text: "Sub Item #2"
  }]
  }, {
  id: 2,
  text: "Sample Item #2"
  },{
  isDivider: true
  },{
  id: 3,
  text: "Sample Item #3",
  enabled: false
  }];
  elements.sideNavigation.setRootMenuItems(menu);
```

### setSelectedMenuItem

**Params**

| Type          | Name                        | Description                                                                                | Required                               |
| ------------- | --------------------------- | ------------------------------------------------------------------------------------------ | -------------------------------------- |
| String-Number | menuItemId                  | the id of the menu item.                                                                   | Required                               |
| Boolean       | mustExecuteOnMenuItemSelect | force the onMenuItemSelect to be executed.                                                 | <p>Optional,</p><p>Default false.</p>  |
| Boolean       | mustExecuteOnMenuItemExpand | force the onMenuItemExpand to be executed.                                                 | <p>Optional, </p><p>Default false.</p> |
| Number        | level                       | reduce the search to the selected menuItem at level, if any menuItem is selected at level. | Optional                               |

**Returns** Boolean

Select the menu item with the given id. If level is provided search is optimized since it will search only within the descendant of the selected menuItem at level. For example if a root menuItem is selected and level is equal 2 search only in the subMenuItems of the selected root. Return false if menuItemId cannot be found or is disabled.

### setSubMenuItems

**Params**

| Type                                    | Name       | Description                                                                                                                                                                                                                                                                                              | Required |
| --------------------------------------- | ---------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- |
| String-Number                           | menuItemId | the id of the menu item.                                                                                                                                                                                                                                                                                 | Required |
| Array<[MenuItem](Sidenav.md#menu-item)> | menuItems  | is an array of MenuItem objects. Each MenuItem object should set the required properties 'id', which uniquely identifies the menuItem object in menu, and 'text' property. The MenuItem may contain the optional properties 'styleClass', 'iconStyleClass', 'data', 'enabled', 'menuItems', 'isDivider'. | Required |

**Returns** Boolean

Set the menuItems as sub menu items of the menu item with id 'menuItemId' Return false if menuItemId cannot be found.

Example

```
var menuItems = [{
  id: 10,
  text: "Sample Item #1",
  styleClass : "sn-large",
  iconStyleClass:  "glyphicon glyphicon-search",
  data: { description: "This is sample information that can be added to a menuItem" },
  menuItems: [{
  	id: 12,
  	text: "Sub Item #1"
  	}
  }]
  }, {
  id: 11,
  text: "Sample Item #2"
  },{
  isDivider: true
  }];
  elements.sideNavigation.setSubMenuItems(menuItems);
```

### removeMenuItem

**Params**

| Type          | Name       | Description              | Required |
| ------------- | ---------- | ------------------------ | -------- |
| String-Number | menuItemId | The id of the menu item. | Required |

**Returns** Boolean

Remove the menu item and all it's subMenuItems from the tree. Return false if menuItemId cannot be found.

### removeSubMenuItems

**Params**

| Type          | Name       | Description              | Required |
| ------------- | ---------- | ------------------------ | -------- |
| String-Number | menuItemId | The id of the menu item. | Required |

**Returns** Boolean

Remove all the sub menu items of the menu item with id 'menuItemId'. Return false if menuItemId cannot be found.
