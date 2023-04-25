# Switch

The switch component can be used as an alternative for checkboxes and radios.

Switch example:

![switch](https://cloud.githubusercontent.com/assets/7150474/26816814/421ea9f0-4a59-11e7-9269-384d340c1ce5.PNG)

## Table of contents

* [Switch properties](Switch.md#switch-properties)
* [Switch events](Switch.md#switch-events)
* [Switch API](Switch.md#switch-api)

## Switch properties

The component has the following properties:

| Property      | Type         | Default | Description                                                                                                   |
| ------------- | ------------ | ------- | ------------------------------------------------------------------------------------------------------------- |
| animate       | Boolean      | true    | determines if the switch animates when toggled.                                                               |
| componentSize | String       | Normal  | determines size of switch, choose from (Mini,Small,Normal, and Large).                                        |
| dataProvider  | dataprovider | null    | The dataprovider for the switch.                                                                              |
| enabled       | Boolean      | true    | The enable state of the component, default true.                                                              |
| handleWidth   | Number       | 150     | sets the width of both handles.                                                                               |
| label         | String       | Switch  | sets the toggle label.                                                                                        |
| labelWidth    | Number       | 150     | sets the width of the middle label.                                                                           |
| offColor      | String       | Primary | sets the negative (unchecked) class, can be default (as default), primary, info, success, warning, or danger. |
| offText       | String       | Off     | sets the negative (unchecked) text                                                                            |
| onColor       | String       | Primary | sets the positive (checked) class, can be default (as default), primary, info, success, warning, or danger.   |
| onText        | String       | On      | sets the positive (checked) text                                                                              |
| styleClass    | String       | null    | Additional style class(es) of the component                                                                   |
| tabSeq        | Number       | null    | The element's tab sequence                                                                                    |
| visible       | Boolean      | true    | The visible property of the component, default true.                                                          |

## Switch events

| Event        | Params        | Return | Description                        |
| ------------ | ------------- | ------ | ---------------------------------- |
| onAction     | event:JSEvent |        | Fired when a switch is clicked     |
| onDataChange | event:JSEvent |        | Fired when dataprovider is updated |

## Switch API

Currently, the switch component has no API.
