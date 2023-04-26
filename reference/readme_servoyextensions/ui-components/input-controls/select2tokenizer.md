# select2tokenizer

Since V1.1.0

Select2Tokenizer is a component which allow the user to select multiple values as 'tokens' from a search field. The component is implemented on top of the [Select2](https://select2.github.io/examples.html#tokenizer) library.

![Select2Tokenizer](http://content.screencast.com/users/paronne/folders/Jing/media/55628f72-7e0f-4f16-95d2-199473a16247/2016-11-21\_1059.png).

## Table of contents

* [Styling Select2Tokenizer](select2tokenizer.md#styling-select2tokenizer)
* [Select2Tokenizer Properties](select2tokenizer.md#select2tokenizer-properties)
* [Select2Tokenizer Events](select2tokenizer.md#select2tokenizer-events)
* [Select2Tokenizer API](select2tokenizer.md#select2tokenizer-api)

## Styling Select2Tokenizer

The component has it's own CSS selector to be used for the restyle of the component. Note that fine-grained styling of the component is depending on the internal selectors of the select2 libary

| element selector                     | summary                                   |
| ------------------------------------ | ----------------------------------------- |
| .svy-select2-autotokenizer           | style the select2tokenizer                |
| .svy-select2-autotokenizer-container | style the select2tokenizer tags container |
| .svy-select2-autotokenizer-dropdown  | style the select2tokenizer dropdown       |

#### Sizing

To adjust the Select2Tokenizer size, apart from stylying the component with your own CSS, you can use one the control size classes; the Select2Tokenizer offers 4 control size classes. Please note that each size class requires a certain height of the component for nice stylying and to avoid vertical scrollbars. To use the size classes just add one of them into the component's styleClass property. Default size class is select2-sm.

| size class | min-height | font-size |
| ---------- | :--------: | --------- |
| select2-xs |    20px    | 12px      |
| select2-sm |    32px    | 14px      |
| select2-md |    36px    | 16px      |
| select2-lg |    44px    | 18px      |

## Select2Tokenizer Properties

| Property  | Type                   | Default          | Description                                                                                                                                                                                                      |
| --------- | ---------------------- | ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Boolean   | allowNewEntries        | false            | Allow the user to enter new entries not available in valuelist                                                                                                                                                   |
| Boolean   | closeOnSelect          | true             | Allow the user to select multiple options before closing the dropdown when set to false.                                                                                                                         |
| Boolean   | selectOnClose          | false            | Select the highlighted option when closing the dropdown.                                                                                                                                                         |
| Boolean   | openOnUnselect         | true             | Open the dropdown menu when the user removes a tag.                                                                                                                                                              |
| Boolean   | clearSerchTextOnSelect | false            | This option is relevant only in combination with 'closeOnSelect' is false. When set to true the search text is cleared each time the user select an option from the dropdown, mantaining the dropdown open.      |
| Boolean   | containSearchText      | false            | When set to true will search for any value containing the search term. By default will suggest all the items starting with the search term text.                                                                 |
| String    | dataProvider           |                  | The dataprovider of the component. Show the dataprovider value as selected tokens. Multiple choices in dataProvider are separated by a new line character '\n'.                                                  |
| Boolean   | enabled                | true             | The enable state of the component, default true.                                                                                                                                                                 |
| String    | noMatchesFoundText     | No matches found | The message shown when no matches are found.                                                                                                                                                                     |
| String    | placeholderText        | Select...        | The placeholder text shown when there is no selected value.                                                                                                                                                      |
| Number    | tabSeq                 |                  | The element's tab sequence                                                                                                                                                                                       |
| String    | toolTipText            |                  | The text displayed when hovering over the component with a mouse cursor.                                                                                                                                         |
| String    | styleClass             |                  | the element style Classes.                                                                                                                                                                                       |
| Valuelist | valuelist              |                  | The valuelist that is used by this field to populate the list of items in the dropdown. The displayValue "-" is a special item which is replaced with a divider between the previous and the next items in menu. |
| Boolean   | visible                | true             | The visible property of the component, default true.                                                                                                                                                             |

## Select2Tokenizer Events

| Event                                                  | Params                                          | Return  | Description                                                                     |
| ------------------------------------------------------ | ----------------------------------------------- | ------- | ------------------------------------------------------------------------------- |
| onDataChange                                           | oldValue:String, newValue:String, event:JSEvent | Boolean | Method that is executed when the data in the component is successfully changed. |
| Multiple entries are separated by a new line char '\n' |                                                 |         |                                                                                 |
| onFocusGained                                          | event:JSEvent                                   |         | The method that is executed when the component gains focus.                     |
| onFocusLost                                            | event:JSEvent                                   |         | The method that is executed when the component looses focus.                    |

## Select2Tokenizer API

| Event        | Params                                 | Return | Description                                                                                                                 |
| ------------ | -------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------------------------- |
| requestFocus | mustExecuteOnFocusGainedMethod:Boolean |        | Request focus for the select2tokenizer. The user should press ENTER to open the dropdown list once the field has the focus. |
