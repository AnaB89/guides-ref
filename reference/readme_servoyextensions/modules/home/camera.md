Required Phonegap plugins
------------------
cordova-plugin-camera

# API Documentation 

## Method Summary
### getPicture
Take (using camera) or get an image file from the device's default gallery.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Function | successCallback | on success callback | Optional
Function | errorCallback | on error callback | Optional
Object | options | Options object | Optional

The options object's parameters can be aquired from the [cordova-plugin-camera](https://github.com/apache/cordova-plugin-camera) site.

# Example Usage
```javascript
var options = {
  quality: 50,
  destinationType: 0,
  sourceType: 1,
  correctOrientation: true
}

plugins.svyphonegapCamera.getPicture(getPicSuccess, getPicFail, options);

/**
 * Callback when picture received successfully
 * @properties={typeid:24,uuid:"8EEAFB0D-133F-4009-9C41-83B8A890D19B"}
 */
function getPicSuccess(res) {
	//display the image.
	elements.contact_photo.imageURL = '';
	elements.contact_photo.text = '<img src="data:image/png;base64,' + res + '"/>'
}

```
