# Button

Just that!

![Button](https://github.com/Servoy/bootstrapcomponents/wiki/images/button.png)

## Table of contents

* [Button properties](button.md#button-properties)
* [Button events](button.md#button-events)
* [Button API](button.md#button-api)

## Properties Summary

The component has the following properties:

| Property        | Type    | Default           | Description                                                                                   |
| --------------- | ------- | ----------------- | --------------------------------------------------------------------------------------------- |
| enabled         | Boolean | true              | Whether the component is enabled or not; blocks onAction, onDoubleClick, onRightClick events. |
| imageStyleClass | String  |                   | Image style class for an optional image of the button (e.g. a FontAwesome or glyphicon class) |
| tabSeq          | Number  |                   | Tab sequence index of the form                                                                |
| styleClass      | String  | "btn btn-default" | Button style class, typically one of the bootstrap button classes (e.g. "btn btn-primary")    |
| text            | String  |                   | The text shown for the button (i18n is supported)                                             |
| toolTipText     | String  |                   | Tooltip text shown when hovering over the button (i18n is supported)                          |
| visible         | Boolean | true              | Whether the button is visible or not                                                          |

## Events Summary

The component allows to attach handlers for the following events:

| Event         | Params        | Return | Description                             |
| ------------- | ------------- | ------ | --------------------------------------- |
| onAction      | event:JSEvent |        | Fired when the button is clicked        |
| onDoubleClick | event:JSEvent |        | Fired when the button is double clicked |
| onRightClick  | event:JSEvent |        | Fired when the button is right clicked  |

## Methods Summary

The component offers the following API methods:

| Method       | Params | Return | Description                    |
| ------------ | ------ | ------ | ------------------------------ |
| requestFocus |        |        | Sets the focus to this button. |

## Properties Details

### text

### toolTipText

### imageStyleClass

## Events Details

### onClick

### onDoubleClick

### onRightClick

## Methods Details

### requestFocus

