Welcome to the svyGMaps wiki!

This wiki provides comprehensive documentation for using the **svyGMaps** web-component, which allows you to display a location using the Google Maps API within Servoy's NGClient.

Table of contents
* [Getting Started](#getting-started)
* [Example Usage](#example-usage)
* [Component Properties](#component-properties)
* [API](#api)
  * [createMarker](#createmarker)
  * [addMarker](#addmarker)
  * [addMarkers](#addmarkers)
  * [getMarker](#getmarker)
  * [getMarkerById](#getmarkerbyid)
  * [getMarkers](#getmarkers)
  * [removeAllMarkers](#removeallmarkers)
  * [refresh](#refresh)
  * [centerAtAddress](#centerataddress)
  * [centerAtLatLng](#centeratlatlng)
  * [getBounds](#getbounds)
  * [getCenter](#getcenter)
  * [fitBounds](#fitbounds)
  * [setOptions](#setoptions)
* [Handlers](#handlers)
  * [onMapEvent](#onmapevent)
  * [onMarkerEvent](#onmarkerevent)
  * [onMarkerGeocoded](#onmarkergeocoded)
  * [onRouteChanged](#onroutechanged)
* [Custom types](#custom-types)
  * [marker](#marker)
  * [routeSettings](#routesettings)
  * [routeResult](#routeresult)
  * [leg](#leg)
  * [latLng](#latlng)
  * [latLngBounds](#latlngbounds)

# Getting Started

First import the component using one of the release [binaries](https://github.com/Servoy/svyGMaps/releases) or via Servoy's Web Package Manager.

If you would like to see the component in an example install the included solution, [googleMapsExample.servoy](https://github.com/Servoy/svyGMaps/releases).

Most importantly the component **requires** a Google Map API key to function properly. You can get one [here](https://developers.google.com/maps/documentation/javascript/get-api-key) for free. Make sure to enable the GeoCoding API in addition to the Javascript Map API options.

# Example Usage

First add the component to a form and setup the apiKey.
Next you can add one or multiple markers to the component.
This can be done by adding markers in the property panel or from code.
You can add additional styling to the component using the styleClass property.  
For more information check out the example solution. 

## Component Properties

The component offers the following properties for configuration:

Type | Name | Summary | Required | default
--- |--- | --- | --- | ---
String | apiKey | Google Map API Key | **Required** | |
routeSettings | directionsSettings | Settings for the route calculation | | |
Boolean | fullscreenControl| hide fullscreen button | | false
String[] | mapEvents | any number of map events to be listened to via the onMapEvent handler | | 
String | mapType | type of mape to show, supported values ["ROADMAP", "SATELLITE","HYBRID","TERRAIN"] | | ROADMAP
Boolean | mapTypeControl | hide maptype control button | | false 
String[] | markerEvents | any number of marker events to be listened to via the onMarkerEvent handler | | 
markers[] | markers | Array of design time markers  | |
Boolean | streetViewControl | hide streetView control button | | false
Boolean | zoomControl | hide zoom control button | | false
dataprovider | zoomLevel | Setting the zoomlevel of the map based on a dataprovider type integer. When no dataprovider the default zoomlevel will be used. Zooming the map will also update the dataprovider | | 7
Boolean | useGoogleMapCluster | Use google maps in combination with clusterview | | false
Boolean | useGoogleMapDirections | Use google maps in combination with directions | | false
String | gestureHandling | Setup or Disable  gestureHandling for google maps, supported values ["auto", "greedy","cooperative","none"] | | auto
dataprovider | KmlLayerURL | Apply a KML file url to the map | |

## API

The component offers the following API methods:

### createMarker

Creates a new, empty marker

    var servoyMarker = elements.map.createMarker('svyMarker', 'Fred. Roeskestraat 97, 1076 EC Amsterdam', 'Servoy B.V.');
    servoyMarker.iconMedia = 'media:///servoy_marker.png';
    elements.map.addMarker(servoyMarker);

The method has the following parameters:

Name | Type | Summary | Optional
--- | --- | ------- | ---
markerId | Object | A unique identifier of this marker |  
addressOrLatLng | String/LatLng | Either an address string or a latLng object | 
title | String | Optional title for this marker | yes | 

### addMarker

Adds the given marker at the optional index.

    var servoyMarker = elements.map.createMarker('svyMarker', 'Fred. Roeskestraat 97, 1076 EC Amsterdam', 'Servoy B.V.');
    servoyMarker.iconMedia = 'media:///servoy_marker.png';
    elements.map.addMarker(servoyMarker);

The method has the following parameters:

Name | Type | Summary | Optional
--- | --- | ------- | ---
marker | marker | The marker to add |  
index | Number | The index to insert the marker at | yes

### addMarkers

Adds the given markers at the optional index.

    var markers = [];
    markers.push(elements.map.createMarker('marker-1', 'Fred. Roeskestraat 97, 1076 EC Amsterdam', 'Servoy'));
    markers.push(elements.map.createMarker('marker-2', '1600 Pennsylvania Avenue NW, Washington, DC 20500', 'White House'));
    elements.map.addMarkers(markers);

The method has the following parameters:

Name | Type | Summary | Optional
--- | --- | ------- | ---
marker[] | markers | The markers to add |  
index | Number | The index to insert the markers at | yes

### getMarker

Returns the marker at the given index

    var marker = elements.map.getMarker(index);

The method has the following parameters:

Name | Type | Summary | Optional
--- | --- | ------- | ---
index | Number | The index of the marker | 

### getMarkerById

Returns the marker with the given Id

    var marker = elements.map.getMarkerById(markerId);

The method has the following parameters:

Name | Type | Summary | Optional
--- | --- | ------- | ---
markerId | Object | The identifier of the marker | 

### getMarkers

Returns all markers

### removeMarker
Api to remove markers at given index.

    elements.map.removeMarker(5);

### removeAllMarkers
Api to remove all markers

    elements.map.removeAllMarkers();

### refresh
Api to force refresh google maps

    elements.map.refresh();

### centerAtAddress
Api to center the map at given address

    elements.map.centerAtAddress(shipaddress + ' ' + shipcity + ' ' + shipcountry);

### centerAtLatLng
Api to center the map at given lat long location

    elements.map.centerAtLatLng(33,-111);

### getBounds
Returns the lat/lng bounds of the current viewport as a `latLngBounds` object. If more than one copy of the world is visible, the bounds range in longitude from -180 to 180 degrees inclusive. If the map is not yet initialized (i.e. the mapType is still null), or center and zoom have not been set then the result is `null` or `undefined`.

### getCenter
Returns the position displayed at the center of the map as a `latLng` object.

### fitBounds
Sets the viewport to contain the given bounds (as `latLngBounds` object).

### setOptions
Sets Google Maps options. See here: https://developers.google.com/maps/documentation/javascript/reference/map#MapOptions the list of available options.

## Handlers

The component offers the following handler methods:

### onMapEvent

Callback method for any events assigned in the mapEvents property.

To listen for map events, use the mapEvents property to assign the events you want to listen for (e.g. "click"). The callback method will be fired whenever one of the events in the mapEvents list is detected and receives the event and an optional latLng object (Mouse events like "click" only).

The method receives the following parameters:

Name | Type | Summary | Optional
--- | --- | ------- | ---
event | JSEvent | The event | 
latLng | latLng | Optional latLng object when the event is fired by a mouse event | true

### onMarkerEvent

Callback method for any events assigned in the markerEvents property.

To listen for marker events, use the markerEvents property to assign the events you want to listen for (e.g. "click"). The callback method will be fired whenever one of the events in the markerEvents list is detected and receives the event, the marker index and an optional latLng object (Mouse events like "click" only).

The method receives the following parameters:

Name | Type | Summary | Optional
--- | --- | ------- | ---
event | JSEvent | The event | 
markerIndex | Number | The index of the marker | 
latLng | latLng | Optional latLng object when the event is fired by a mouse event | true

### onMarkerGeocoded

Callback method that fires whenever an address from a marker has successfully been geocoded.

The method receives the following parameters:

Name | Type | Summary | Optional
--- | --- | ------- | ---
marker | marker | The marker geocoded | 
latLng | latLng | The position found | 

### onRouteChanged
Function call when the route is changed.

## Custom types

The component uses a few custom types on API methods, handlers and properties:

### marker

When using in code you can define this type by using:

    /** @type {CustomType<googlemaps-svy-G-Maps.marker>} */
    var marker = {}

or by calling

`var marker = elements.map.createMarker(...)`

Type | Name | Summary | default
-- | --- | ---- | --
dataprovider | addressDataprovider | Dataprovider returning a string formated like: "Fred. Roeskestraat 97, Amsterdam, NL". |
String | addressString | String formated like: "Fred. Roeskestraat 97, Amsterdam, NL". This property will only work when no dataprovider is set. |
latLng | position | The position of this marker. This property will be filled also when an address needed to be geocoded | 
String | iconLabel | Label to display inside the marker or radius |
String | title |  Tooltip to show when hovering over a marker or radius |
String | iconUrl | Url for a marker label to display (samples: https://sites.google.com/site/gmapsdevelopment) |
Media | iconMedia | Media for a marker label to display |
tagstring | infoWindowString | Text or html to show in a popup when clicking on a marker or radius |
Boolean | drawRadius | Enable when you want to have a radius, will only work when iconUrl is empty | false
Integer | radiusMeters | Radius size to show, default in googlemaps is meters | 2000
Color | radiusColor | Radius color | "AA0000"
Boolean | draggable | If true, the marker can be dragged | false
String | animation | Any of the animation options (BOUNCE, DROP) | 
Boolean | clickable | If true, the marker receives mouse and touch events | true
Boolean | crossOnDrag | If false, disables cross that appears beneath the marker when dragging | true
Number | opacity | The marker's opacity between 0.0 and 1.0 | 
Boolean | visible | If true, the marker is visible | true
Integer | zIndex | All markers are displayed on the map in order of their zIndex, with higher values displaying in front | 
String | markerId | An ID that should be set to identify a marker provided to API or callback methods | 

### routeSettings

Settings for the route calculation, set on the `directionsSettings` property.

Type | Name | Summary | default
--- |--- | --- | ---
Boolean | optimize | Let google maps optimize the waypoints order | true
String | travelMode | specifies what mode of transport to use when calculating directions, options: ["driving", "walking","bicycling","transit"] | driving
Boolean | avoidFerries | when set to true indicates that the calculated route(s) should avoid ferries, if possible | false
Boolean | avoidHighways | when set to true indicates that the calculated route(s) should avoid major highways, if possible. | false
Boolean | avoidTolls | when set to true indicates that the calculated route(s) should avoid toll roads, if possible. | false

### routeResult

A route result object provided to the `onRouteChanged` handler holding all legs of the route and the total number of meters and the total number of seconds of the route calculated.

Type | Name | Summary
--- |--- | --- 
leg[] | legs | Array of the legs of the route
Number | total_distance | The total distance of the route in meters
Number | total_duration | The total number of seconds this route takes

### leg

A single leg of a route result

Type | Name | Summary
--- |--- | --- 
String | start_address | The start address of this leg
String | end_address | The end address of this leg
leg[] | legs | Array of the legs of the route
String | distance | The total distance of the route in the default unit
Number | distance_meters | The total distance of the route in meters
String | duration | Formatted duration of this leg
Number | duration _seconds | The total number of seconds of this leg

### latLng
A latLng is a point in geographical coordinates: latitude and longitude.

Type | Name | Summary | default
--- |--- | --- | ---
Number | lat | The latitude | 
Number | lng | The longitude | 

### latLngBounds
A latLngBounds instance represents a rectangle in geographical coordinates, including one that crosses the 180 degrees longitudinal meridian.

Type | Name | Summary | default
--- |--- | --- | ---
latLng | sw | The soutwest position | 
latLng | ne | The northeast position | 