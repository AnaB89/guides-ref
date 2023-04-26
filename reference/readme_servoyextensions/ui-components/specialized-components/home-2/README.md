# Fullcalendar Component

## Introduction

The component provides a full-sized, drag & drop event calendar. The component is based on the JQuery fullcalendar library, version 2.6.1. The calendar component is a 1-to-1 implementation of the fullcalendar library. For documentation you can referer to the fullcalendar v2 docs available at http://fullcalendar.io/docs/.

## Documentation

Read the documentation on the Fullcalendar and Fullcalendar Events.

* [Fullcalendar](fullcalendar.md).
* [Fullcalendar Events](fullcalendar-events.md)
* [Migrating calendar from Smart and Web Client to NG Client](migrating-calendar-from-smart-and-web-client-to-ng-client.md)

## Quick Start

To add the FullCalendar Component package in your Servoy solution or Servoy module open the Servoy Developer IDE and download the FullCalendar Component from the Web Package Manager (the Web Package Manager is accessible from the context menu of the Web Components node of your solution). The component will be available on the palette of the form designer to be easily dragged and drop into your form. The component has to be initialized programmatically using the fullcalendar constructor available from the element's API.

NOTE: make sure the calendar component in form has the element name set.

```javascript
/** @type {svy-fullcalendar.FullCalendarOptions} */
var options = {
        eventSources: [ {events: [{ title: "lunch event", start: new Date() }]}],
		selectable: true,
		editable: true,
		defaultView: 'agendaWeek',
		showCurrentTimeline: true
}
var calendar = elements.fullcalendarElementName.fullCalendar(options);
```

The options object contains the calendar properties; see the fullcalendar docs for available properties. All the properties are optional. Set the eventSources options to feed the calendar with Event Source Objects. Event Sources will populate the calendat with Event objects. Call the FullCalendar constructor for the same element to destroy and recreate the Calendar.

## Demo Solution

You can download the Fullcalendar Component demo solution [fullcalendarComponent.demo.servoy](https://github.com/Servoy/fullcalendarcomponent/releases) and import it into your workspace as a Servoy solution. The demo solution fetches events from a database called 'fullcalendar'; metadata for all database entities are included. Before importing the solution create a new database called 'fullcalendar', then allow the import of metadata during import procedure.

Note: the Fullcalendar component is not included in the demo solution export. Once the demo solution is successfully imported into your workspace, open the Web Package Manager to add the Fullcalendar Component.
