The Calendar Component is a Servoy NG Component. Use the form editor to place the **fullcalendar** NG Component into your form and use the calendar element's API to initialize the calendar. The component has to be initialized programmatically using the fullcalendar constructor available from the element's API.

NOTE: make sure the calendar component in form has the element name set.

<div class="code panel pdl" style="border-width: 1px;">

<div class="codeContent panelContent pdl">

<pre class="syntaxhighlighter-pre" data-syntaxhighlighter-params="brush: jscript; gutter: false; theme: Eclipse" data-theme="Eclipse">var options = {
        eventSources: [ events: [{ title: "lunch event", start: new Date() }]],
		selectable: true,
		editable: true,
		defaultView: 'agendaWeek',
		showCurrentTimeline: true
}
var calendar = elements.fullcalendarElementName.fullCalendar(options);</pre>

</div>

</div>

# Calendar Options

The `options` object contains the calendar properties; see the [fullcalendar docs](http://fullcalendar.io/docs/) for available properties. All the properties are optional.  
Set the eventSources options to feed the calendar with [Event Source](http://fullcalendar.io/docs/event_data/Event_Source_Object/) Objects. Event Sources will populate the calendat with [Event](http://fullcalendar.io/docs/event_data/Event_Object/) objects.  
Call the FullCalendar constructor for the same element to destroy and recreate the Calendar.
Read more about Event and Event Sources at [Fullcalendar Events](https://wiki.servoy.com/display/WEB/Fullcalendar+Events).

# Update Calendar Options

The options `height` , `contentHeight`, `aspectRatio` can be updated at runtime using the calendar's API **options**.

To update any other of the calendar options call again the fullcalendar constructor to force the calendar to be destroyed and be recreated again with the new options.

Note: when calling the constructor the calendar view will be resetted to the default view ( for example if the user has navigated from _Today_ to a different date as 1st December 2016, if the calendar constructor is called the calendar will re-render itself to _Today_'s date ). To preserve the calendar navigation set to **true **the additional argument _renderOnCurrentView _of the calendar constructor_._

<div class="code panel pdl" style="border-width: 1px;">

<div class="codeContent panelContent pdl">

<pre class="syntaxhighlighter-pre" data-syntaxhighlighter-params="brush: jscript; gutter: false; theme: Eclipse" data-theme="Eclipse">// update the calendar aspect ratio
var calendar = elements.fullcalendarElementName.options(aspectRatio, 2);

// update the the calendar to scroll at 13.00.00
// for such update the calendar has to be destroyed and re-rendered again
// set renderOnCurrentView to true on the constructor to maintain the navigation date and view
var options = elements.fullcalendarElementName.getFullCalendarOptions();
options.scrollTime = "13:00:00";
elements.fullcalendarElementName.fullCalendar(options, true);</pre>

</div>

</div>

The calendar component offers several events handlers. You can register to the calendar events you would like to interact with from the properties view of the form editor.

# Fullcalendar Event Details

#### onSelect

<div class="sIndent">The method that is executed when user select any area of the calendar.</div>

**Parameters**

{Date} start - start date of the selected area  
{Date} end - end date of the selected area  
{JSEvent} event - the event that triggered the action  
{Object} view - the calendar view object  
{Object} resource - the selected resource (scheduler feature only)

#### onDayClick

<div class="sIndent">The method that is executed when the user clicks on any space of the calendar.</div>

**Parameters**

{Date} date - the clicked date  
{JSEvent} event - the event that triggered the action  
{Object} view - the calendar view object  
{Object} resource - the selected resource (scheduler feature only)

#### onEventClick

<div class="sIndent">The method that is executed when the user clicks any event object rendered in the calendar.</div>

**Parameters**

{Object} eventObject - the calendar event the user has clicked on  
{JSEvent} event - the event that triggered the action  
{Object} view - the calendar view object

#### onEventRightClick

The method that is executed when the user right clicks any event object rendered in the calendar.

**Parameters**

{Object} eventObject - the calendar event the user has clicked on  
{JSEvent} event - the event that triggered the action

#### onEventDrop

The method that is executed when an event is dropped on the calendar.
**Parameters**

{EventType} eventObject - the calendar event being dropped  
{Number} delta - the difference in time from the previous start time of the event  
{JSEvent} event - the event that triggered the action  
{Object} view - the calendar view object

#### onEventResize

<div class="sIndent">The method that is executed when an event is resized on the calendar.</div>

**Parameters**

{EventType} eventObject - the calendar event being resized  
{Number} delta - the difference in time from the previous end time of the event  
{JSEvent} event - the event that triggered the action  
{Object} view - the calendar view object

# Fullcalendar Property Summary

#### styleClass

The name of the style class that should be applied to this component.

#### tooltipExpression

The text expression to be shown as a tooltip when hovering on the calendar events. Use double curly brackets to evaluate {{propertyName}} the event's properties

**Example**

<pre>
This is the event title:{{title}}. The event starts at: {{start}}. Description: {{data.description}} 
</pre>
