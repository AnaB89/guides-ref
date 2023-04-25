# TextBox

Shows a dataprovider in an editable text box.

![Text box](https://github.com/Servoy/bootstrapcomponents/wiki/images/textbox.png)

## Table of contents

* [Text box properties](TextBox.md#text-box-properties)
* [Text box events](TextBox.md#text-box-events)
* [Text box API](TextBox.md#text-box-api)
* [Using HTML5 input types](TextBox.md#using-html5-input-types)
* [Using autocomplete values](TextBox.md#using-autocomplete-values)

## Text box properties

The component has the following properties:

| Property        | Type         | Default | Description                                                                                                                                                        |
| --------------- | ------------ | ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| autocomplete    | String       | "off"   | Autocomplete attribute to allow the browser to provide assistance in filling out the field (see [Using autocomplete values](TextBox.md#using-autocomplete-values)) |
| dataProvider    | dataprovider |         | The column or variable to provide the data for this field                                                                                                          |
| editable        | Boolean      | true    | Whether the field is editable or not                                                                                                                               |
| enabled         | Boolean      | true    | Whether the field is enabled ot not                                                                                                                                |
| format          | format       |         | A format to format the data shown                                                                                                                                  |
| inputType       | String       | text    | Attribute to control how the browser renders the component (see [Using HTML5 input types](TextBox.md#using-html5-input-types))                                     |
| placeholderText | String       |         | An optional placeholder text shown when no value is set yet (i18n supported)                                                                                       |
| selectOnEnter   | Boolean      | false   | Whether the whole content is selected when the field gets focus                                                                                                    |
| styleClass      | styleclass   |         | CSS style class for this component                                                                                                                                 |
| tabSeq          | Number       |         | Tab sequence index of the form                                                                                                                                     |
| tooltipText     | String       |         | Tooltip text shown when hovering over the component (i18n is supported)                                                                                            |
| visible         | Boolean      |         | Whether the component is visible or not                                                                                                                            |

## Text box events

The component allows to attach handlers for the following events:

| Event         | Parameters                                  | Return  | Description                           |
| ------------- | ------------------------------------------- | ------- | ------------------------------------- |
| onAction      | event:JSEvent                               |         | Fired when the enter key is hit       |
| onDataChange  | oldValue:Date, newValue:Date, event:JSEvent | Boolean | Fired when the value is changed       |
| onFocusGained | event:JSEvent                               |         | Fired when the component gets focus   |
| onFocusLost   | event:JSEvent                               |         | Fired when the component loses focus  |
| onRightClick  | event:JSEvent                               |         | Fired when the component right clicks |

## Text box API

The component offers the following API methods:

| Method       | Parameters | Return | Description                                                                                                   |
| ------------ | ---------- | ------ | ------------------------------------------------------------------------------------------------------------- |
| setInputType | String     |        | Dynamically set the input type at runtime (see [Using HTML5 input types](TextBox.md#using-html5-input-types)) |

## Using HTML5 input types

In HTML5, an `<input>` can have a `type` attribute that controls how the browser renders the component. A type `number` for example will show a little spinner in many browsers and on a mobile device, the keyboard would typically switch to a number layout. The default type is `text`.

In order to make use of this feature, you can use one of the following new HTML5 input types for example:

* email
* tel
* date
* time
* datetime-local
* month
* week
* number
* color

**NOTE**: On IOS, it is not possible to change the width of a native date/time component. The only way you can force that, is to disable the WebKit appearance on it, by adding " -webkit-appearance: none;" to its CSS class

## Using autocomplete values

The `autocomplete` attribute lets web developers specify what if any permission the browser has to provide automated assistance in filling out form field values, as well as guidance to the browser as to the type of information expected in the field. The source of the suggested values is generally up to the browser; typically values come from past values entered by the user, but they may also come from pre-configured values. For instance, a browser might let the user save their name, address, phone number, and email addresses for autocomplete purposes.

There are many possible values that you can provide to hint the browser on expected input, e.g. `name`, `email`, `country` etc.

By default the autocomplete attribute is set to off (that means it should never appear).
