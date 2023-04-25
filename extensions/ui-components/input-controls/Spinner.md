# Spinner

## Table of contents

* [Spinner properties](Spinner.md#spinner-properties)
* [Spinner events](Spinner.md#spinner-events)
* [Spinner API](Spinner.md#spinner-api)

## Spinner properties

The component has the following properties:

| Property         | Type         | Default | Description                                                                    |
| ---------------- | ------------ | ------- | ------------------------------------------------------------------------------ |
| dataProvider     | dataprovider |         | The dataprovider of the component                                              |
| displayTags      | Boolean      | true    | Whether texts should evaluate tags                                             |
| editable         | Boolean      | true    | Whether the component is editable                                              |
| enabled          | Boolean      | true    | Whether the component is enabled or not; blocks onAction, onDataChange events. |
| format           | format       |         | A format to format the data shown.                                             |
| placeholderText  | String       |         | Text shown when no value is yet selected (i18n is supported)                   |
| responsiveHeight | Number       |         | Component height                                                               |
| styleClass       | String       |         | Style class of this component                                                  |
| tabSeq           | Number       |         | Tab sequence index of the form                                                 |
| toolTipText      | String       |         | Tooltip text shown when hovering over the component (i18n is supported)        |
| valuelist        | valuelist    |         | The value list which offers the values presented                               |
| visible          | Boolean      | true    | Whether the component is visible or not                                        |

## Spinner events

The component allows to attach handlers for the following events:

| Event         | Parameters                                  | Return  | Description                          |
| ------------- | ------------------------------------------- | ------- | ------------------------------------ |
| onAction      | event:JSEvent                               |         | Fired when the enter key is hit      |
| onDataChange  | oldValue:Date, newValue:Date, event:JSEvent | Boolean | Fired when the value is changed      |
| onFocusGained | event:JSEvent                               |         | Fired when the component gets focus  |
| onFocusLost   | event:JSEvent                               |         | Fired when the component loses focus |
| onRightClick  | event:JSEvent                               |         | Fired for mouse right click          |

## Spinner API

The component offers the following API methods:

| Method       | Parameters                             | Return | Description                       |
| ------------ | -------------------------------------- | ------ | --------------------------------- |
| requestFocus | mustExecuteOnFocusGainedMethod:Boolean |        | Sets the focus to this component. |
