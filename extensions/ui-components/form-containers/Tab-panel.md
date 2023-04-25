# TabPanel

The tab panel is used to show a number of sub forms in a form.

![Tab panel](https://github.com/Servoy/bootstrapcomponents/wiki/images/tabpanel.png)

## Table of contents

* [Tab panel properties](Tab-panel.md#tab-panel-properties)
* [Tab panel events](Tab-panel.md#tab-panel-events)
* [Tab panel API](Tab-panel.md#tab-panel-api)
  * [Tab type](Tab-panel.md#tab-type)

## Tab panel properties

The component has the following properties:

| Property            | Type       | Default | Description                                                                                         |
| ------------------- | ---------- | ------- | --------------------------------------------------------------------------------------------------- |
| closeIconStyleClass | styleclass |         | Class to style the optional tab close icon                                                          |
| containerStyleClass | styleclass |         | Class to style the outer container                                                                  |
| height              | String     |         | The minimum height of the component (used in responsive form). Can be 100% or a number (in pixels). |
| showTabCloseIcon    | Boolean    | false   | Whether the component should show an icon to close a tab                                            |
| styleClass          | String     |         | Style class of this component                                                                       |
| tabs                | tab\[]     |         | The tabs to be shown                                                                                |
| tabSeq              | Number     |         | Tab sequence index of the form                                                                      |
| visible             | Boolean    | true    | Whether the component is visible or not                                                             |

## Tab panel events

The component allows to attach handlers for the following events:

| Event        | Parameters                                               | Return | Description                                                                                                                                                                                                                 |
| ------------ | -------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| onChange     | previousIndex:Number, event:JSEvent                      |        | Fired after a different tab is selected                                                                                                                                                                                     |
| onTabClicked | event:JSEvent, clickedTabIndex:Number, dataTarget:String |        | Fired when the user clicks on a tab. When false is returned, the tab switch is prevented. The dataTarget parameter can be used in custom HTML rendered as the tab's text to determine where in the HTML the click occurred. |
| onTabClose   | event:JSEvent, clickedTabIndex:Number                    |        | Fired when the user clicks on the tab close icon. When false is returned, the tab close is prevented                                                                                                                        |

## Tab panel API

The component offers the following API methods:

| Method      | Parameters                                 | Return                       | Description                                              |
| ----------- | ------------------------------------------ | ---------------------------- | -------------------------------------------------------- |
| addTab      | form:form, tabText:String, \[index:Number] | [tab](Tab-panel.md#tab-type) | Adds the given form as a new tab                         |
| getTabAt    | index:Number                               | [tab](Tab-panel.md#tab-type) | Returns the tab at the given tab index (1 based)         |
| removeTabAt | index:Number                               |                              | Removes the tab at the given tab index (1 based)         |
| selectTabAt | index:Number                               |                              | Selects (shows) the tab at the given tab index (1 based) |

### Tab type

Tab is a custom type of the tab panel component holding properties of a single tab of the panel:

| Property       | Type       | Default | Description                                                                                     |
| -------------- | ---------- | ------- | ----------------------------------------------------------------------------------------------- |
| containedForm  | form       |         | The form shown in the tab                                                                       |
| disabled       | Boolean    | false   | Whether that tab is enabled or not                                                              |
| hideCloseIcon  | Boolean    | false   | Whether a close icon is shown or not (only applicable when `showTabCloseIcon` is set to `true`) |
| iconStyleClass | styleclass |         | Style class for the tab's icon                                                                  |
| imageMedia     | media      |         | Image to be drawn in tab header                                                                 |
| name           | String     |         | A name for this tab                                                                             |
| relationName   | relation   |         | Optional relation for the form to be shown                                                      |
| text           | String     |         | The tab's text (i18n and custom HTML supported)                                                 |
