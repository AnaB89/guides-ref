Required Phonegap plugins
------------------
cordova-plugin-geolocation

# API Documentation 

## Method Summary
### getCurrentPosition
Returns the device's current position to the successCallback callback with a Position object as the parameter. If there is an error, the errorCallback function is passed a PositionError object. 

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Function | successCallback | on success callback | Optional
Function | errorCallback | on error callback | Optional
Object | options | Options {maximumAge: Number, timeout: Number, enableHighAccuracy: Boolean} | Optional

### watchPosition
Add a watcher to keep track of the GPS position.  As the device moves the watcher will send this information back to the successCallback callback with a Position object as the parameter. If there is an error, the errorCallback function is passed a PositionError object. 

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Function | onWatchSetCallback| on success callback (gets a watcherID)  | Optional
Function | successCallback | on success callback | Optional
Function | errorCallback | on error callback | Optional
Object | options | Options {maximumAge: Number, timeout: Number, enableHighAccuracy: Boolean} | Optional

### clearWatch
Remove an existing watcher which will disable tracking of location.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Number | watchId| watchID to remove | Optional

# Example Usage
```javascript
//watch when location changes.
var options = { enableHighAccuracy: true }
plugins.svyphonegapLocation.watchPosition(null, getLocationSuccess, getLocationFail, options);

/**
 * Callback when location is acquired
 * @properties={typeid:24,uuid:"14E1CB25-B697-47B0-A9A6-F52B0050EF39"}
 */
function getLocationSuccess(pos) {	
	//send location to google map component named 'map')
	elements.map.latitude = pos.coords.latitude;
	elements.map.longitude = pos.coords.longitude;	
        //clear watch once location found
	plugins.svyphonegapLocation.clearWatch();
}

```
