Welcome to the svySignature wiki!

This wiki provides comprehensive documentation for using the **svySignature** web-component, which allows you to create a signature within Servoy's NGClient.

# Getting Started
First import the component using one of the release [binaries](https://github.com/Servoy/svySignature/releases) or via Servoy's Web Package Manager.

If you would like to see the component in an example install the included solution, [svySignatureExample.servoy](https://github.com/Servoy/svySignature/releases).

# Example Usage
First add the component to a form by dragging it into the form using the Palette Wizard.  It should be under svySignature (pad). 

```javascript

//when you want to save the signature, create a simple handler:
function onAction$save(event) {
var data = elements.pad.getDataUrl("image/png")
//data contains a base64 string of the signature.
}

```

# API Documentation 

## Method Summary

### clear
Clear the signature image pad.

### getDataUrl
Get signature image as base64 string.

### setDataUrl
Draw signature image with a base 64 string.

## Handlers
There two handlers which can detect when a user starts writing and when they are finished.
### onBegin
### onEnd

## Properties
* dotSize : (float or function) Radius of a single dot.
* minWidth : (float) Minimum width of a line. Defaults to 0.5.
* maxWidth : (float) Maximum width of a line. Defaults to 2.5.
* throttle : (integer) Draw the next point at most once per every x milliseconds. Set it to 0 to turn off throttling. Defaults to 16.
* minDistance : (integer) Add the next point only if the previous one is farther than x pixels. Defaults to 5.
* backgroundColor : (string) Color used to clear the background. Can be any color format accepted by context.fillStyle.Defaults to "rgba(0,0,0,0)" (transparent black). Use a non-transparent color e.g. "rgb(255,255,255)" (opaque white) if you'd like to save signatures as JPEG images.
* penColor: (string) Color used to draw the lines. Can be any color format accepted by context.fillStyle. Defaults to "black".
* velocityFilterWeight : (float) Weight used to modify new velocity based on the previous velocity. Defaults to 0.7.
