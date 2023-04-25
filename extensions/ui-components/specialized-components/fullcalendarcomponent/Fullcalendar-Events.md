# Fullcalendar Events

## Event Object

An [Event](http://fullcalendar.io/docs/event\_data/Event\_Object/) is a javascript Object which store information about a calendar event. The calendar component renders calendar event as Event Objects.&#x20;

An Event Object must have a "**start"** date property and a "**title"**, it has other optionals properties which might modify it's behavior and it's style on the calendar component. Use the **"data"** property to add any other custom property to the event as "description", "location" and any other information that might be useful to the developer.

```
var event = {
	title: "lunch event",
	start: new Date(),
	allDay: false,
	editable: true,
	data : {
       description : "This is an event object", 
       location: "Amsterdam"
    }
}
```

## Event Source Object

An [EventSource](http://fullcalendar.io/docs/event\_data/Event\_Source\_Object/) is a javascript Object that provides Event data to the FullCalendar. It can be seen as a collection of Events. The Events associated to an EventSource inherit it's properties if are not specified in the event itself. For example an EventSource having set "yellow' as "backgroundColor\*\*" \*\*will color as yellow all the associated Events except of those having set their own "backgroundColor" property.

The Calendar component differentiates between different EventSource Types, depending on how Events are returned to the Fullcalendar.

* \*\*ArrayEventSourceType \*\*feeds the calendar with an Array of Event Objects.
* **FunctionEventSourceType** uses a Servoy function to feed the calendar with a collection of Event Objects. Any time the user navigates dates and/or calendar views the calendar will execute the events function to fetch Event Objects. The function must return an Array of EventType Objects. Set optional properties in the "data" property of the eventSource to use it as a filter parameters in the function feed.
* \*\*GoogleCalendarEventSourceType \*\*retrieves calendar event from a public Google Calendar feed. See the specific  [Google Calendar docs ](http://fullcalendar.io/docs/google\_calendar/)for further details.

```
// ArrayEventSourceType sample
/**
 * @type {svy-fullcalendar.EventSourceType}
 */
var arrayEventSource = {
	events: [{
    	title: "source event",
		start: new Date(),
		allDay: true
	}],
	color: 'yellow'
}

// FunctionEventSourceType sample
/**
 * @type {svy-fullcalendar.EventSourceType}
 */
var functionEventSource = {
	events: fetchFunction,
	data: {search: 'Amsterdam'},
	color: 'green',
	ignoreTimezone: false
};

/** 
 * @param {Date} start
 * @param {Date} end
 * @param {Object} [data] optional object to be used as filter parameters in fetching events
*/ 
function fetchFunction(start, end, data) {
 var foundset = databaseManager.getFoundSet("db:/yourserver/yourtable");
 // search data based on your search criteria
    if (foundset.find()) {
		if (data.search) foundset.location = data.search
        foundset.start_date = '>= ' + utils.dateFormat(scopes.svyDateUtils.toStartOfDay(new Date(start)), 'dd/MM/yyyy HH:mm:ss') + '|dd/MM/yyyy HH:mm:ss';
	    foundset.end_date = '<= ' + utils.dateFormat(scopes.svyDateUtils.toEndOfDay(new Date(end)), 'dd/MM/yyyy HH:mm:ss') + '|dd/MM/yyyy HH:mm:ss';
		foundset.search();
    }
	var events = []
    for (var i=1; i<=foundset.getSize(); i++ ) {
		var rec = foundset.getRecord(i)
		// Note: is up to the developer map a datasource to an event object
		events.push({
			start : rec.startDate,
			title :	rec.yourTitle,
			location: rec.location
		});
    }
	return events;
}
```

#### Populate the calendar

Populate the calendar with [Event Object](http://fullcalendar.io/docs/event\_data/Event\_Object/) and/or [EventSource Object](http://fullcalendar.io/docs/event\_data/Event\_Source\_Object/). Provide the events and eventSources to the **FullCalendar** constructor to populate the calendar as soon it's rendered.

Use the calendar API **renderEvent** and **addEventSource** to render new events at any time without forcing a re-create of the calendar, or the **removeEvents** and **removeEventSources** to remove them from the calendar component.&#x20;

```
// populate the calendar providing events and eventSources to the constructor
var options = {
		eventSources: [
			functionEventSource,
            arrayEventSource
		}]
	}
elements.fullcalendar.fullCalendar(options);
```

The API to remove event and eventSource requires the event id or eventSource id. If you haven't set any id to the event or eventSource object you won't be able to remove it.

```
// add an eventSource to a Fullcalendar Object
var eventSource = {
            id : 1,
			events: [{
				title: "green source event",
				start: new Date(),
			}],
			color: 'green'
	}
calendar.addEventSource(eventSource);

// remove the eventSource using the eventSource id
calendar.removeEventSource(1);
```

#### Update Event and EventSource

Call the FullCalendar method \*\*updateEvent \*\*to update an Event which is visible on the calendar. Provide the updated Event object to the API. To update successfully the event the developer must have used an unique id for the event object. The updateEvent API will return false if the id is not provide or if the event is not visible.

To update an eventSource the developer should remove the eventSource from the calendar using \*\*removeEventSource \*\*and add the updated eventSource using the method **addEventSource**.

_NOT SUPPORTED. To update an eventSource developer can modify the original EventSource Object and call the methods \*\*rerenderEvents \*\*to make a change visible in the calendar and the method **refetchEvents** in case events has been added or removed from the EventSource Object._

#### Display icon in the event object

Display a specific icon in the calendar event is a common use case. The FullCalendar component does not have an explicit property for event icons but such feature can be achieved using the \*\*className \*\*property of event or eventSource objects and CSS3 styling.

Use the CSS3 _before_ or _after_ pseudo-selector to place an icon before or after the event title (or event time). If you want to place the same icon on all the calendar events you can include the following CSS in your solution's CSS file.

```
/* display the icon before the title text */
.fc-event .fc-title:before {
	content: url('servoy16x16.png');  /* the icon is picked from the media folder of your Servoy solution */
}

/* display the icon before the event time */
.fc-event .fc-time:before {
	content: url('servoy16x16.png');  /* the icon is picked from the media folder of your Servoy solution */
}
```

If you want to display specific icon on specific events use the **className** property of the event object (or of the eventSource object if you want to display the same icon for all the events of the eventSource).

If your event has className equal to 'custom-icon' then your CSS should look like:

```
/* display the icon before the title text */
.fc-event.custom-icon .fc-title:before {
	content: url('servoy16x16.png');  /* the icon is picked from the media folder of your Servoy solution */
}

/* display the icon before the event time */
.fc-event.custom-icon .fc-time:before {
	content: url('servoy16x16.png');  /* the icon is picked from the media folder of your Servoy solution */
}
```

Font icons are often more effective then .png/.jpeg icons. You can easier control size color and other property of the icon from CSS. To use Font Icons include them in your solution's media folder and make sure are loaded togheter with your solution's styleSheet. You can simply use the same font icons content as in the example below:

```
/* display the glyphon calendar icon before the event time */
.fc-event .fc-time:before {
	font-family: 'Glyphicons Halflings';   /* use the glyphicons */
	content: "\e109";     /* the calendar icon to be displayed */
	padding: 0 3px;
}

/* display multiple icons at the same time for events having className icon-multiple*/
.fc-event.icon-multiple .fc-time:before {
	font-family: 'Glyphicons Halflings';   /* use the glyphicons */
	content: "\e109 \e023";     /* display calendar and time icon next to each other */
	padding: 0 3px;
}
```

## Event Property Summary

#### id

String|Number

Uniquely identifies the given event. Different instances of repeating events should all have the same id. Id is not a required property but is necessary to be able to update or remove the event on the calendar.

#### title

String

The text shown on the event element. **Required.**

#### start

Date

The date and time an event begins. **Required.**

#### end

Date

The date and time an event ends.

#### allDay

Boolean

Whether an event occurs at a specific time-of-day. This property affects whether an event's time is shown. Also, in the agenda views, determines if it is displayed in the "all-day" section.

If this value is not explicitly specified, [allDayDefault](http://fullcalendar.io/docs/event\_data/allDayDefault/) will be used if it is defined.

#### className

String|Array

A CSS class (or array of classes) that will be attached to this event's element.

#### data

Object

A custom object which can be used to add custom properties to the event object.

#### resourceIds

Array

Associate the event with the resource ids provided. Scheduler feature.

#### editable

Boolean

The event will not be editble if set to false.

#### startEditable

Boolean

#### durationEditable

Boolean

#### overlap

Boolean

#### rendering

String

Use value 'background' to render the event as a background event.

#### constraint

Object

#### color

Color

#### backgroundColor

Color

#### borderColor

Color

#### textcolor

Color

## Event Source Property Summary

#### id

String|Number

Uniquely identifies the given event source. Id is not a required property but is necessary to be able to remove the event source from the calendar without being force to redraw the calendar it self.

#### googleCalendarId

String

The Google Calendar ID to be used to fetch the google calendar events. Do not set the "events" property if you are using the eventSource to fetch Google Calendar events.

#### googleCalendaApiKey

String

The Google Calendar API Key which is required to allow the fetching of Google Calendar events.

#### className

Array

A CSS array of classes that will be attached to this event's element.

#### data

Object

A custom object which can be used to add custom properties to the event source object.

#### allDayDefault

Boolean

Determines the default value for each Event Object's `allDay` property when it is unspecified.

#### editable

Boolean

The event will not be editble if set to false.

#### startEditable

Boolean

#### durationEditable

Boolean

#### overlap

Boolean

#### rendering

String

Use value 'background' to render the event as a background event.

#### constraint

Object

#### color

Color

#### backgroundColor

Color

#### borderColor

Color

#### textColor
