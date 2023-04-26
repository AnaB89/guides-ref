# Html Area

Table of contents

* [Html Area properties](html-area.md#html-area-properties)
* [Html Area events](html-area.md#html-area-events)
* [Html Area API](html-area.md#html-area-api)

## Html Area properties

The component has the following properties:

| Property         | Type         | Default | Description                                                                    |
| ---------------- | ------------ | ------- | ------------------------------------------------------------------------------ |
| dataProvider     | dataprovider |         | The dataprovider of the component                                              |
| displayTags      | Boolean      | true    | Whether texts should evaluate tags                                             |
| editable         | Boolean      | true    | Whether the component is editable                                              |
| enabled          | Boolean      | true    | Whether the component is enabled or not; blocks onAction, onDataChange events. |
| placeholderText  | String       |         | Text shown when no value is yet selected (i18n is supported)                   |
| responsiveHeight | Number       |         | Component height                                                               |
| scrollbars       | Scrollbars   |         | Component height                                                               |
| styleClass       | String       |         | Style class of this component                                                  |
| tabSeq           | Number       |         | Tab sequence index of the form                                                 |
| toolTipText      | String       |         | Tooltip text shown when hovering over the component (i18n is supported)        |
| text             | String       |         | Display text                                                                   |
| visible          | Boolean      | true    | Whether the component is visible or not                                        |

## Html Area events

The component allows to attach handlers for the following events:

| Event         | Parameters                                  | Return  | Description                          |
| ------------- | ------------------------------------------- | ------- | ------------------------------------ |
| onAction      | event:JSEvent                               |         | Fired when the enter key is hit      |
| onDataChange  | oldValue:Date, newValue:Date, event:JSEvent | Boolean | Fired when the value is changed      |
| onFocusGained | event:JSEvent                               |         | Fired when the component gets focus  |
| onFocusLost   | event:JSEvent                               |         | Fired when the component loses focus |
| onRightClick  | event:JSEvent                               |         | Fired for mouse right click          |

## Html Area API

The component offers the following API methods:

| Method              | Parameters                              | Return | Description                                                                                                               |
| ------------------- | --------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------------------- |
| getAsPlainText      |                                         | Strin  | Gets the plain text for the formatted Html Area                                                                           |
| getScrollX          |                                         | Number | Returns the x scroll location of specified element                                                                        |
| getScrollY          |                                         | Number | Returns the y scroll location of specified element                                                                        |
| getSelectedText     |                                         | String | Returns the currently selected text in the specified Html Area                                                            |
| replaceSelectedText | s:String                                |        | Replaces the selected text; if no text has been selected, the replaced value will be inserted at the last cursor position |
| requestFocus        | mustExecuteOnFocusGainedMethod: Boolean |        | Set the focus to this Html Area                                                                                           |
| selectAll           |                                         |        | Selects all the contents of the Html Area                                                                                 |
| setScroll           | x:Number, y:Number                      |        | Sets the scroll location of an element                                                                                    |
