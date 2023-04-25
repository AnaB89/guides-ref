# Group Buttons

Group a series of buttons together on a single line

![Button group](https://github.com/Servoy/bootstrapextracomponents/wiki/buttongroup/images/image\_01.png)

## Table of contents

* [Style](Button-group.md#style)
* [Button group properties](Button-group.md#button-group-properties)
* [Button group events](Button-group.md#button-group-events)

## Style

The Buttons Radio can be styled as a Bootstrap Button. Style the buttons adding the Bootstrap style classes on the styleClass property, or customize the style of the component from your solution's styleSheet.

The Buttons are styled by default with the css class 'btn-default'.

The component provide it's own CSS selector, .bts-extra-btn-radio, for easy restyle of the component. Combine these selector with the class selectors of the Bootstrap Button for fine grade customization.

## Button group properties

The component has the following properties:

| Property     | Type         | Default       | Description                                                            |
| ------------ | ------------ | ------------- | ---------------------------------------------------------------------- |
| dataProvider | dataprovider |               | The dataprovider (typically a string column or variable)               |
| enabled      | Boolean      | true          | Whether the component is enabled or not; blocks onDataChange event.    |
| inputType    | String       | "radio"       | Whether the component should behave as a `radio` or `checkbox` group.  |
| styleClass   | String       | "btn-default" | Style class of this component                                          |
| tabSeq       | Number       |               | Tab sequence index of the form                                         |
| text         | String       |               | The text shown as label next to the check                              |
| toolTipText  | String       |               | Tooltip text shown when hovering over the calendar (i18n is supported) |
| valuelist    | valuelist    |               | The value list which offers the values presented                       |
| visible      | Boolean      | true          | Whether the component is visible or not                                |

## Button group events

The component allows to attach handlers for the following events:

| Event        | Parameters                                  | Return  | Description                     |
| ------------ | ------------------------------------------- | ------- | ------------------------------- |
| onDataChange | oldValue:Date, newValue:Date, event:JSEvent | Boolean | Fired when the value is changed |
