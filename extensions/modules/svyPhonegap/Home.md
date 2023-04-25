# svyPhonegap

Welcome to the svyPhonegap wiki! This wiki provides comprehensive documentation for using the svyPhonegap web-service, which is bridge to connect Servoy to Phonegap’s native plugins.

## Getting Started

Import the [**phonegap.servoy**](https://github.com/Servoy/svyPhonegap/releases) solution and add it as a module to your main solution. The svyPhonegap service should be automatically imported with solution. Within the onSolutionOpen event of your main solution initialize the phonegap scope as shown below:

```
function onSolutionOpen(arg, queryParams) {
//initialize phonegap module
scopes.phonegap.onSolutionOpen(arg,queryParams, onReadyCallback);

}	

function onReadyCallback(){
//device is ready, get information from a plugin
application.output(plugins.svyphonegapDevice.getDeviceInfo());
}

```

You can also add the phonegap module through source (GIT) then import as an existing project in your workspace.

## Working Example

To see a Servoy solution that utilizes this module check out [svyMobile](https://github.com/Servoy/svyMobile/).

## Building Native Binary (Android/IOS)

Use Servoy's [Mobile Build Generator](https://phonegaputils.servoy.com). This application can help you fill out the configurations required and generating a binary.

If you need to generate certificates for the relevant app store(s) read this [guide](https://docs.google.com/document/d/e/2PACX-1vTVw6Q4RYwnZE9F4f\_-kRxxhFX-yV0adL\_wdHwADJMNLGwBa9fUQaEF2LWuW3xD\_kW3sOowrQZEXbvY/pub?\&embedded=true).

## Documentation on specific services or plugins

For the web services to function, we need to have also installed the particular phonegap plugins mentioned.

[Browser](Browser.md) In-app browser related functions

[Camera](Camera.md) Camera and media functions

[Location](broken-reference) Geolocation functionality

[Push Notifications](Push-Notifications.md) Push Notification functionality
