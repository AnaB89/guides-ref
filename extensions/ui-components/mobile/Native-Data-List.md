# Native Data List

## Table of contents

* [Native Data List properties](Native-Data-List.md#native-data-list-properties)
* [Native Data List events](Native-Data-List.md#native-data-list-events)
* [Native Data List API](Native-Data-List.md#native-data-list-api)

## Native Data List properties

The component has the following properties:

| Property        | Type         | Default | Description                                                                    |
| --------------- | ------------ | ------- | ------------------------------------------------------------------------------ |
| dataProvider    | dataprovider |         | The dataprovider of the component                                              |
| enabled         | Boolean      | true    | Whether the component is enabled or not; blocks onAction, onDataChange events. |
| styleClass      | String       |         | Style class of this component                                                  |
| tabSeq          | Number       |         | Tab sequence index of the form                                                 |
| toolTipText     | String       |         | Tooltip text shown when hovering over the component (i18n is supported)        |
| valuelist       | valuelist    |         | The value list which offers the values presented                               |
| placeholderText | String       |         | Text shown when no value is yet selected (i18n is supported)                   |
| visible         | Boolean      | true    | Whether the component is visible or not                                        |

## Native Data List events

The component allows to attach handlers for the following events:

| Event         | Parameters                                  | Return  | Description                          |
| ------------- | ------------------------------------------- | ------- | ------------------------------------ |
| onAction      | event:JSEvent                               |         | Fired when the enter key is hit      |
| onDataChange  | oldValue:Date, newValue:Date, event:JSEvent | Boolean | Fired when the value is changed      |
| onFocusGained | event:JSEvent                               |         | Fired when the component gets focus  |
| onFocusLost   | event:JSEvent                               |         | Fired when the component loses focus |

## Native Data List API

The component offers the following API methods:

| Method       | Parameters                             | Return | Description                       |
| ------------ | -------------------------------------- | ------ | --------------------------------- |
| requestFocus | mustExecuteOnFocusGainedMethod:Boolean |        | Sets the focus to this component. |
