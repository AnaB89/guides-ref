# Rating

The rating component is a simple component to capture a value in a certain range by selecting a star or other icon from a number of icons shown.

Star example:

![Rating stars](<../../../../.gitbook/assets/image\_01 (3).png>)

Hearts example:

![Rating hearts](<../../../../.gitbook/assets/image\_02 (1).png>)

## Table of contents

* [Rating properties](rating.md#rating-properties)
* [Rating events](rating.md#rating-events)
* [Rating API](rating.md#rating-api)

## Rating properties

The component has the following properties:

| Property              | Type         | Default        | Description                                                                                                                                                          |
| --------------------- | ------------ | -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| dataProvider          | Dataprovider | null           | The dataprovider that provides the value                                                                                                                             |
| enabled               | Boolean      | true           | Whether the component is enabled or not                                                                                                                              |
| max                   | Number       | 5              | The maxmium value that can be selected (minimum is always 1)                                                                                                         |
| showPercentageOnHover | Boolean      | false          | Shows a little percentage indicator when hovering over the ratings                                                                                                   |
| stateOn               | String       | glyphicon-star | class name of the image shown when the value is less or equal to this item's value ( _tag); can be any glyphicon or font-awesome icon; defaults to 'glyphicon-star'_ |
| stateOff              | String       | glyphicon-star | class name of the image shown when the value is greater than this item's value ( _tag); can be any glyphicon or font-awesome icon; defaults to 'glyphicon-star'_     |
| visible               | Boolean      | true           | Whether the component is visible or not                                                                                                                              |

## Rating events

| Event   | Params                      | Return | Description                               |
| ------- | --------------------------- | ------ | ----------------------------------------- |
| onLeave | event:JSEvent, value:Number |        | Fired when the mouse leaves the component |
| onHover | event:JSEvent, value:Number |        | Fired when the mouse hovers over a rating |

## Rating API

The rating component currently has no API.
