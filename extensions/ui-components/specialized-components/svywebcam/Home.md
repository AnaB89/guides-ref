Welcome to the svywebcam wiki!

This wiki provides comprehensive documentation for using the **svywebcam** web-component, which allows you to utilize the browser's webcam within Servoy's NGClient.  The component is a wrapper for the [jpeg_camera](https://github.com/amw/jpeg_camera) project.

# Getting Started
First import the component using one of the release [binaries](https://github.com/Servoy/svywebcam/releases) or via Servoy's Web Package Manager.

If you would like to see the component in an example - install the included sample solution, [webCamExample.servoy](https://github.com/Servoy/svywebcam/releases).

# Example Usage
First add the component to a form by dragging it into the form using the Palette Wizard.  It should be under svywebcam section.

Then setup an event handler for getBase64Data event.  This is a callback function that will return data once the snapshot is taken.

Finally capture an image using capture.  This will capture a shot and if successful data will be returned to the getBase64Data handler.

`elements.webcam.capture();`

# Known Issues
There is currently an issue with OSX and Safari Browsers preventing the component to initialize as expected.
If you are having an issue with this, please try adding the flash plugin and using that instead.

iOS requires that you have an HTTPS connection to use this component.

# API Documentation 

## Method Summary
### setOptions
Setup the component's options.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Object| option | options object | Required

Default Options:
```
var options = {
		mirror: false, //mirror image
		quality: 1, // 0-1 quality of image
		retry_success: false,
		scale: 1, //scale of image
		shutter: false, //use a shutter sound
		shutter_ogg_url: '', //audio location
		shutter_mp3_url: '', //audio location
		swf_url: '',
		timeout: 0 //how many seconds to wait before take a shot
	`}
```

### capture
Capture an image based on current options.  If successful this will execute the GetBase64Data handler and return data to the callback function you provide.