# Type Ahead

A text field that offers values from a provided value list, filtering the list as the user starts typing.

![Type ahead](https://github.com/Servoy/bootstrapcomponents/wiki/images/typeahead.png)

## Table of contents

* [Type ahead properties](TypeAhead.md#type-ahead-properties)
* [Type ahead events](TypeAhead.md#type-ahead-events)
* [Type ahead API](TypeAhead.md#type-ahead-api)

## Type ahead properties

The component has the following properties:

| Property        | Type         | Default | Description                                                                  |
| --------------- | ------------ | ------- | ---------------------------------------------------------------------------- |
| dataProvider    | dataprovider |         | The column or variable to provide the data for this field                    |
| editable        | Boolean      | true    | Whether the field is editable or not                                         |
| enabled         | Boolean      | true    | Whether the field is enabled ot not                                          |
| format          | format       |         | A format to format the data shown                                            |
| placeholderText | String       |         | An optional placeholder text shown when no value is set yet (i18n supported) |
| selectOnEnter   | Boolean      | false   | Whether the whole content is selected when the field gets focus              |
| tabSeq          | Number       |         | Tab sequence index of the form                                               |
| tooltipText     | String       |         | Tooltip text shown when hovering over the calendar (i18n is supported)       |
| valuelist       | valuelist    |         | The value list which offers the values presented                             |
| visible         | Boolean      |         | Whether the component is visible or not                                      |

## Type ahead events

The component allows to attach handlers for the following events:

| Event         | Parameters                                  | Return  | Description                         |
| ------------- | ------------------------------------------- | ------- | ----------------------------------- |
| onAction      | event:JSEvent                               |         | Fired when the enter key is hit     |
| onDataChange  | oldValue:Date, newValue:Date, event:JSEvent | Boolean | Fired when the value is changed     |
| onFocusGained | event:JSEvent                               |         | Fired when the calendar gets focus  |
| onFocusLost   | event:JSEvent                               |         | Fired when the calendar loses focus |

## Type ahead API

The component offers the following API methods:

| Method       | Parameters                             | Return | Description                       |
| ------------ | -------------------------------------- | ------ | --------------------------------- |
| requestFocus | mustExecuteOnFocusGainedMethod:Boolean |        | Sets the focus to this component. |
