# Label

Simple label showing a text.

![Label](https://github.com/Servoy/bootstrapcomponents/wiki/images/label.png)

The label text can be static text, a locale translated value when using i18n or dynamic content when %% tags are use to display values from dataproviders, aggregations or standard tags (e.g. %%selectedIndex%% as used in the screenshot above).

## Table of contents

* [Label properties](label.md#label-properties)
* [Label events](label.md#label-events)
* [Label API](label.md#label-api)

## Label properties

The component has the following properties:

| Property             | Type         | Default | Description                                                                                                                                                                           |
| -------------------- | ------------ | ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| enabled              | Boolean      | true    | Whether the field is enabled ot not                                                                                                                                                   |
| imageStyleClass      | String       |         | An icon style class property (glyphicon, material design or Font Awesome). For Font Awesome icons it is required to install the Font Awesome service from the Servoy Package Manager. |
| labelFor             | String       |         | The field to which this label belongs (when the field is hidden, the label will also be hidden)                                                                                       |
| showAs               | String       | html    | Whether the label should show the text as is (`text`), as sanitized HTML (`html`) or as trusted, unsanitized HTML (`trusted_html`)                                                    |
| styleClass           | styleclass   |         | CSS style class for this component                                                                                                                                                    |
| styleClassExpression | dataprovider |         | A column or calculation that provides the CSS style class for this component                                                                                                          |
| tabSeq               | Number       |         | Tab sequence index of the form                                                                                                                                                        |
| tooltipText          | String       |         | Tooltip text shown when hovering over the component (i18n is supported)                                                                                                               |
| visible              | Boolean      |         | Whether the component is visible or not                                                                                                                                               |

## Label events

The component allows to attach handlers for the following events:

| Event         | Parameters                       | Return | Description                                   |
| ------------- | -------------------------------- | ------ | --------------------------------------------- |
| onAction      | event:JSEvent, dataTarget:string |        | Fired when the component is clicked on        |
| onDoubleClick | event:JSEvent, dataTarget:string |        | Fired when the component is double clicked on |
| onRightClick  | event:JSEvent, dataTarget:string |        | Fired when the omponent is right clicked on   |

The dataTarget parameter allows to identify inner html elements. Adding a data-target attribute on such element (shown in label html), will make the event receive the value of the attribute.

## Label API

The component currently has no API methods.
