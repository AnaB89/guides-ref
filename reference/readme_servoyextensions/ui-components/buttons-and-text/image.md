# Image

## Table of contents

* [Image properties](image.md#image-properties)
* [Image events](image.md#image-events)

## Image properties

The component has the following properties:

| Property     | Type       | Default | Description                                                             |
| ------------ | ---------- | ------- | ----------------------------------------------------------------------- |
| dataProvider | String     |         | The dataprovider of the component.                                      |
| enabled      | Boolean    | true    | Whether the component is enabled or not                                 |
| media        | Number     |         | The image media object that should be displayed inside the component.   |
| styleClass   | styleclass |         | CSS style class for this component                                      |
| tabSeq       | Number     |         | Tab sequence index of the form                                          |
| tooltipText  | String     |         | Tooltip text shown when hovering over the component (i18n is supported) |
| visible      | Boolean    | true    | Whether the component is visible or not                                 |

## Image events

The component allows to attach handlers for the following events:

| Event        | Parameters                        | Return  | Description                            |
| ------------ | --------------------------------- | ------- | -------------------------------------- |
| onAction     | event:JSEvent                     |         | Fired when the component is clicked on |
| onDataChange | oldValue, newValue, event:JSEvent | boolean | Fired when image media changes         |

onDataChange() handles changed data, returns false if the value should not be accepted. JSEvent.data will contain extra information about dataproviderid, its scope and the scope id (record datasource or form/global variable scope). Warning: Do not use dialogs, as a dialog will interfere with focus.
