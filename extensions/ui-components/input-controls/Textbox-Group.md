# TextBox Group

A textfield a font awesome icon and email validation.

## Table of contents

* [Textbox group properties](Textbox-Group.md#textbox-group-properties)
* [Textbox group events](Textbox-Group.md#textbox-group-events)

## Textbox group properties

The component has the following properties:

| Property        | Type         | Default      | Description                                                                |
| --------------- | ------------ | ------------ | -------------------------------------------------------------------------- |
| dataProviderID  | dataprovider | null         | Dataprovider to display in the textbox                                     |
| enabled         | enabled      | true         | When false textbox has disabled appearance and actions do not work         |
| format          | format       | type default | Format for the dataprovider                                                |
| faclass         | string       | null         | font awesome class of the icon to show                                     |
| inputType       | string       | text         | Input type, can be text or password.                                       |
| inputValidation | string       | null         | Input validation, can be none or email                                     |
| readOnly        | readOnly     | false        | Input can be editable or not                                               |
| placeholderText | tagstring    | null         | Placeholder text (will show in unfocused textfield when there is no value) |
| styleClass      | styleclass   | null         | Additional style class(es) of the component                                |
| tabSeq          | tabseq       | null         | Tab sequence number                                                        |
| visible         | visible      | true         | When false component is not visible                                        |

## Textbox group events

| Event                 | Params                                                               | Return  | Description                              |
| --------------------- | -------------------------------------------------------------------- | ------- | ---------------------------------------- |
| onActionMethodID      | event:JSEvent                                                        |         | Fired when you click the label           |
| onDataChangeMethodID  | oldValue:dataprovider type, newValue:dataprovider type event:JSEvent | boolean | Fired when textbox value changes         |
| onFocusGainedMethodID | event:JSEvent                                                        |         | Fired when textfield gets focus          |
| onFocusLostMethodID   | event:JSEvent                                                        |         | Fired when textfield looses focus        |
| onRightClickMethodID  | event:JSEvent                                                        |         | Fired when you right click the textfield |
