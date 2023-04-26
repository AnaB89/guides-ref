NOTE: this page is a reference for who is migrating from the Smart and Web client version of the fullcalendar to the NG version.

The Web and Smart version of the fullcalendar, which was based on the javaFX panel, should be replaced with the fullcalendar web component in the NG Client. The Calendar NG Component API forare mostly back-compatible with the Smart and Web client version.  

The initialization of the Calendar is slightly different in NG; read the documentation on how to use the Calendar NG Component.

In the Calendar NG Component most of the extra features that have been implemented for the Smart and Web client version of the calendar component have been deprecated; built-in feature of the fullcalendar library are used instead.

## Resources

Allow to use a calendar Resource View type which renders all the events related to the existing resources on the selected Date.  
The resourceView type has deprecated in favour of the fullcalendar Scheduler.  
See the Calendar Resources section for detailed documentation about the Scheduler.

## Annotations

Annotations Object are placed on the Agenda views slots. Use annotations to mark a specific timeslot and to change background color for the specified period.  

The annotations objects are deprecated in the NG version of the calendar component. Instead of annotations object the developer can use the calendar option businessHours or add to the calendar event objects as background events.   

The businessHours is used to emphasizes a specific time block in the agenda views. The businessHours is defined as a JSON object which may have any of the following properties

**start** The date/time the businessHours begins  
**end** The date/time an businessHours ends. Required  
**dow** The days of the week the businessHours is applied  

<pre>
var options = {
        eventSources: [events: [{ title: "lunch event", start: new Date(), id: 1 }]],
		businessHours: {
				start: new scopes.svyDateUtils.DateTime().toStartOfDay().addHours(9).date,
				end: new scopes.svyDateUtils.DateTime().toStartOfDay().addHours(17).date,
				dow: [1,2,3,4,5] // Apply businessHours Monday to Friday
		}
}
elements.calendarElementName.fullcalendar(options);
</pre>

Events that appear as background highlights can be achieved by setting an Event Object's rendering property to background.
Background events that are timed will only be rendered on the time slots in agenda view. Background events that are all-daywill only be rendered in month view or the all-day slots of agenda view.

The color of background events can be manipulated by targeting the fc-bgevent className, one of your own custom classNames provided by the Event Object's className property, or by explicitly specifying a color with each Event Object's orEvent Source's color or backgroundColor properties.

It is possible to define daily or weekly recurring events. Use Duration-ish times in the Event Object's start and endproperties, or use the dow property. See businessHours for more information.
For further details read the fullcalendar documentation on Background Events.

## Event rightClick
Triggered when the user right clicks an event.  
The eventRightClick is an event of the calendar component.

function( eventObject, event, view ) { }

**eventObject** is an Event Object that holds the event's information (date, title, etc).  
**event** the JSEvent that triggered the action.   
**view** holds the current View Object.  

## Calendar dayRightClick (deprecated)  

Triggered when the user right clicks on a Day.  

This event has been deprecated and is not supported in the NG version of the calendar component.

## Timeline

Show the current time as a red line in the calendar view.  
The calendar option showCurrentTimeline has been deprecated and replaced by the new calendar option nowIndicator.

Default: false

<pre>
var options = {
        eventSources: [events: [{ title: "lunch event", start: new Date()}]],
		nowIndicator: true
}
elements.calendarElementName.fullcalendar(options);
</pre>

Use CSS to style the .fc-now-indicator border-color and change the timeline color

<pre>
CSS to customize timeline
.fc-now-indicator {
	border-color: blue;
}
</pre>