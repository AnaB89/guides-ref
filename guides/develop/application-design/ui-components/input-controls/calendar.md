---
description: Guide for using the Calendar component
---

# Calendar

## Overview

The Calendar is an [Input Control](./) component. It presents as a formatted date field and it can show a popup date-picker when clicked. It can also accept keyboard input, like a regular Text Field.

Like all Input Control components, the Calendar is data-bound to a single Data Provider. It can be used to update database columns and variables that have a DateTime data type.

## Get Started

To get started using the Calendar component, drag it onto a form from the pallet.

{% hint style="info" %}
If the component does not appear in the pallet, it means you do not have the Bootstrap Components package installed. Click "Get more components" at the top of the pallet to open the Servoy Package Manager and install it.
{% endhint %}

### Data Binding

Setting up data-binding is the first step for an Input Control. In the form editor, select your Calendar component and edit the `dataProvider` property. The Data Provider chooser will be shown and you may select a DateTime column from the form's data source as well as any variable from the form or a top-level scope.

### Formatting

The Calendar, like any field, can be configured to format the Date value as String by applying a format. The `format` property can be directly set by entering the format string manually or by opening the Format Wizard.

For example

See the Date Formatting guide for more examples

### More Properties

The Calendar component has many properties, which can be configured at design-time and changed at runtime from the form's javascript file. A [complete list of properties](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/reference/readme\_servoyextensions/ui-components/input-controls/calendar#calendar-properties) is available in the reference documentation for this component.

### Events

The Calendar component has several UI events that you can capture and handle with custom logic.

Data Provider

Format

### See Also

[Reference Documentation](broken-reference)

[Calendar](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/reference/readme\_servoyextensions/ui-components/input-controls/calendar)

Working with Dates
