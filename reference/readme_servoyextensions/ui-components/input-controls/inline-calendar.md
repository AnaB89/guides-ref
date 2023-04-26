# Calendar Inline

Inline calendar shows the date picker of the [calendar component](https://github.com/Servoy/bootstrapcomponents/wiki/Calendar) directly in the form. The user cannot manually enter a date, just select from the picker.

![Calendar](https://github.com/Servoy/bootstrapcomponents/wiki/images/calendar\_inline.png)

## Table of contents

* [Inline calendar properties](inline-calendar.md#inline-calendar-properties)
* [Inline calendar events](inline-calendar.md#inline-calendar-events)
* [Inline calendar API](inline-calendar.md#inline-calendar-api)

## Inline calendar properties

The component has the following properties:

| Property     | Type         | Default | Description                                                                    |
| ------------ | ------------ | ------- | ------------------------------------------------------------------------------ |
| dataProvider | dataprovider |         | The dataprovider (a date column or variable)                                   |
| enabled      | Boolean      | true    | Whether the component is enabled or not; blocks onAction, onDataChange events. |
| styleClass   | String       |         | Style class of this calendar                                                   |
| toolTipText  | String       |         | Tooltip text shown when hovering over the calendar (i18n is supported)         |
| visible      | Boolean      | true    | Whether the calendar is visible or not                                         |

## Inline calendar events

The component allows to attach handlers for the following events:

| Event        | Parameters                                  | Return  | Description                     |
| ------------ | ------------------------------------------- | ------- | ------------------------------- |
| onDataChange | oldValue:Date, newValue:Date, event:JSEvent | Boolean | Fired when the value is changed |

## Inline calendar API

The component offers the following API methods:

| Method        | Parameters                                      | Return | Description                                                          |
| ------------- | ----------------------------------------------- | ------ | -------------------------------------------------------------------- |
| disableDates  | dateArray:Date\[], keepInvalid:Boolean          |        | Sets a list of dates that cannot be selected in the picker           |
| disableDays   | dayArray:Number\[], keepInvalid:Boolean         |        | Sets a list of days that cannot be selected in the picker            |
| setMinMaxDate | minDate:Date, maxDate:Date, keepInvalid:Boolean |        | Sets the minimum and maximum date that can be selected in the picker |
