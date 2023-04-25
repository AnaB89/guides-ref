# Badge

The badges component can be used to easily highlight new or unread items in labels or buttons.

Label example:

![Label](../../../.gitbook/assets/image\_01.png)

Button example:

![Button](../../../.gitbook/assets/image\_02.png)

## Table of contents

* [Badge properties](badges.md#badge-properties)
* [Badge events](badges.md#badge-events)
* [Badge API](badges.md#badge-api)

## Badge properties

The component has the following properties:

| Property    | Type    | Default | Description                                                                                                                                        |
| ----------- | ------- | ------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| enabled     | Boolean | true    | Whether the component is enabled or not                                                                                                            |
| displayType | String  | BUTTON  | Controls the display type of the component: either "BUTTON" or "LABEL"                                                                             |
| styleClass  | String  | null    | Additional style class(es) of the component. When the displayType is BUTTON, any of the bootstrap button classes (e.g. 'btn-primary') can be used. |
| text        | String  | Badge   | The text shown on the label or button                                                                                                              |
| badgeText   | String  | 0       | The badge text shown on the label or button                                                                                                        |
| visible     | Boolean | true    | The visible property of the component, default true.                                                                                               |

## Badge API

Currently, the badge API has no API.

## Badge events

| Event         | Params        | Return | Description                          |
| ------------- | ------------- | ------ | ------------------------------------ |
| onAction      | event:JSEvent |        | Fired when a badge is clicked        |
| onDoubleClick | event:JSEvent |        | Fired when a badge is double clicked |
| onRightClick  | event:JSEvent |        | Fired when a badge is right clicked  |
