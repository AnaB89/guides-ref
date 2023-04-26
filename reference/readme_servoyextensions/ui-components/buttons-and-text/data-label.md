# Data Label

A label that can show dynamic text and possibly an image.

![Data Label](https://github.com/Servoy/bootstrapcomponents/wiki/images/dataLabel.png)

## Table of contents

* [Data Label properties](data-label.md#data-label-properties)
* [Data Label events](data-label.md#data-label-events)
* [Data Label API](data-label.md#data-label-api)

## Data Label properties

The component has the following properties:

| Property             | Type         | Default | Description                                                                                                                                                                               |
| -------------------- | ------------ | ------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| dataProvider         | dataprovider |         | The column or variable to provide the data for this label.                                                                                                                                |
| enabled              | Boolean      | true    | Whether the field is enabled or not                                                                                                                                                       |
| format               | format       |         | A format to format the data shown.                                                                                                                                                        |
| imageStyleClass      | String       |         | An icon style class property (glyphicon, material design or Font Awesome). For Font Awesome icons it is required to install the **Font Awesome service** from the Servoy Package Manager. |
| labelFor             | String       |         | The field to which this label belongs (when the field is hidden, the label will also be hidden)                                                                                           |
| showAs               | String       | html    | Whether the label should show the text as is (`text`), as sanitized HTML (`html`) or as trusted, unsanitized HTML (`trusted_html`)                                                        |
| styleClass           | styleclass   |         | CSS style class for this component                                                                                                                                                        |
| styleClassExpression | dataprovider |         | A column or calculation that provides the CSS style class for this component                                                                                                              |
| tabSeq               | Number       |         | Tab sequence index of the form                                                                                                                                                            |
| tooltipText          | String       |         | Tooltip text shown when hovering over the component (i18n is supported)                                                                                                                   |
| valuelist            | valuelist    |         | The value list which offers the value presented                                                                                                                                           |
| visible              | Boolean      |         | Whether the component is visible or not                                                                                                                                                   |

## Data Label events

The component allows to attach handlers for the following events:

| Event         | Parameters                       | Return | Description                                   |
| ------------- | -------------------------------- | ------ | --------------------------------------------- |
| onAction      | event:JSEvent, dataTarget:string |        | Fired when the component is clicked on        |
| onDoubleClick | event:JSEvent, dataTarget:string |        | Fired when the component is double clicked on |
| onRightClick  | event:JSEvent, dataTarget:string |        | Fired when the component is right clicked on  |

The dataTarget parameter allows to identify inner html elements. Adding a data-target attribute on such element (shown in label html), will make the event receive the value of the attribute.

## Data Label API

The component currently has no API methods.
