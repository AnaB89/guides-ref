# Checkbox

![Checkbox](https://github.com/Servoy/bootstrapcomponents/wiki/images/checkbox.png)

## Table of contents

* [Checkbox properties](Checkbox.md#checkbox-properties)
* [Checkbox events](Checkbox.md#checkbox-events)
* [Checkbox API](Checkbox.md#checkbox-api)

## Checkbox properties

The component has the following properties:

| Property      | Type         | Default | Description                                                                    |
| ------------- | ------------ | ------- | ------------------------------------------------------------------------------ |
| dataProvider  | dataprovider |         | The dataprovider (typically an integer column or variable)                     |
| enabled       | Boolean      | true    | Whether the component is enabled or not; blocks onAction, onDataChange events. |
| selectedValue | String       |         | The value returned when the checkbox is checked (defaults to 1)                |
| styleClass    | String       |         | Style class of this component                                                  |
| tabSeq        | Number       |         | Tab sequence index of the form                                                 |
| text          | String       |         | The text shown as label next to the check                                      |
| toolTipText   | String       |         | Tooltip text shown when hovering over the calendar (i18n is supported)         |
| visible       | Boolean      | true    | Whether the component is visible or not                                        |

## Checkbox events

The component allows to attach handlers for the following events:

| Event         | Parameters                                  | Return  | Description                         |
| ------------- | ------------------------------------------- | ------- | ----------------------------------- |
| onAction      | event:JSEvent                               |         | Fired when the enter key is hit     |
| onDataChange  | oldValue:Date, newValue:Date, event:JSEvent | Boolean | Fired when the value is changed     |
| onFocusGained | event:JSEvent                               |         | Fired when the calendar gets focus  |
| onFocusLost   | event:JSEvent                               |         | Fired when the calendar loses focus |

## Checkbox API

The component offers the following API methods:

| Method       | Parameters | Return | Description                       |
| ------------ | ---------- | ------ | --------------------------------- |
| requestFocus |            |        | Sets the focus to this component. |
