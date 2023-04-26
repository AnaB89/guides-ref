# Accordion Panel

## Table of contents

* [Accordion Pane properties](accordion-pane.md#accordion-pane-properties)
* [Accordion Pane events](accordion-pane.md#accordion-pane-events)
* [Accordion Pane API](accordion-pane.md#accordion-pane-api)

## Accordion Pane properties

The component has the following properties:

| Property            | Type    | Default | Description                               |
| ------------------- | ------- | ------- | ----------------------------------------- |
| containerStyleClass | String  |         | Style class of this component's container |
| tabs                | tab\[]  |         | Tabs of the accordion pane                |
| styleClass          | String  |         | Style class of this component             |
| height              | Number  | 500     | Height of this component                  |
| tabSeq              | Number  |         | Tab sequence index of the form            |
| visible             | Boolean | true    | Whether the component is visible or not   |

## Accordion Pane events

The component allows to attach handlers for the following events:

| Event    | Parameters                          | Return | Description                             |
| -------- | ----------------------------------- | ------ | --------------------------------------- |
| onChange | previousIndex:Number, event:JSEvent |        | Fired after a different tab is selected |

## Accordion Pane API

The component offers the following API methods:

| Method      | Parameters                                 | Return                            | Description                                              |
| ----------- | ------------------------------------------ | --------------------------------- | -------------------------------------------------------- |
| addTab      | form:form, tabText:String, \[index:Number] | [tab](accordion-pane.md#tab-type) | Adds the given form as a new tab                         |
| getTabAt    | index:Number                               | [tab](accordion-pane.md#tab-type) | Returns the tab at the given tab index (1 based)         |
| removeTabAt | index:Number                               |                                   | Removes the tab at the given tab index (1 based)         |
| selectTabAt | index:Number                               |                                   | Selects (shows) the tab at the given tab index (1 based) |

### Tab type

Tab is a custom type of the accordion pane component holding properties of a single tab of the panel:

| Property      | Type     | Default | Description                                     |
| ------------- | -------- | ------- | ----------------------------------------------- |
| containedForm | form     |         | The form shown in the tab                       |
| disabled      | Boolean  | false   | Whether that tab is enabled or not              |
| name          | String   |         | A name for this tab                             |
| relationName  | relation |         | Optional relation for the form to be shown      |
| text          | String   |         | The tab's text (i18n and custom HTML supported) |
