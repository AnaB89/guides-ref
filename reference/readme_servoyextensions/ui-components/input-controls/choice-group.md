# Choice Group

![Choice group](https://github.com/Servoy/bootstrapcomponents/wiki/images/choicegroup.png)

A choice group offers values from a provided value list and returns the selected values as a carriage return-separated string to the dataprovider attached. When the value list offers display and return values, the return values are returned.

Note that if your value list does not have the "Allow empty value" check set, a user won't be able to remove the last selected value anymore.

The choice group component can be used in two modes: single select (either/or, aka radio button) or multi select. That mode can be controlled via the **inputType** property.

## Table of contents

* [Choice group properties](choice-group.md#choice-group-properties)
* [Choice group events](choice-group.md#choice-group-events)
* [Choice group API](choice-group.md#choice-group-api)

## Choice group properties

The component has the following properties:

| Property     | Type         | Default    | Description                                                                    |
| ------------ | ------------ | ---------- | ------------------------------------------------------------------------------ |
| dataProvider | dataprovider |            | The dataprovider (typically a string column or variable)                       |
| enabled      | Boolean      | true       | Whether the component is enabled or not; blocks onAction, onDataChange events. |
| inputType    | String       | "checkbox" | Whether the component should behave as a `radio` or `checkbox` group.          |
| styleClass   | String       |            | Style class of this component                                                  |
| tabSeq       | Number       |            | Tab sequence index of the form                                                 |
| text         | String       |            | The text shown as label next to the check                                      |
| toolTipText  | String       |            | Tooltip text shown when hovering over the calendar (i18n is supported)         |
| valuelist    | valuelist    |            | The value list which offers the values presented                               |
| visible      | Boolean      | true       | Whether the component is visible or not                                        |

## Choice group events

The component allows to attach handlers for the following events:

| Event         | Parameters                                  | Return  | Description                          |
| ------------- | ------------------------------------------- | ------- | ------------------------------------ |
| onAction      | event:JSEvent                               |         | Fired when clicked                   |
| onDataChange  | oldValue:Date, newValue:Date, event:JSEvent | Boolean | Fired when the value is changed      |
| onFocusGained | event:JSEvent                               |         | Fired when the component gets focus  |
| onFocusLost   | event:JSEvent                               |         | Fired when the component loses focus |

## Choice group API

The component offers the following API methods:

| Method       | Parameters                             | Return | Description                       |
| ------------ | -------------------------------------- | ------ | --------------------------------- |
| requestFocus | mustExecuteOnFocusGainedMethod:Boolean |        | Sets the focus to this component. |
