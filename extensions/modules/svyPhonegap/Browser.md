Required Phonegap plugins
--------------------
cordova-plugin-inappbrowser

cordova-plugin-device


# API Documentation 

## Method Summary
### OpenExternalLink
Open a link on device's default browser

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
String| url | html address of web page | Required

# Example Usage
```javascript
//will open 'https://servoy.com' on device browser.
plugins.svyphonegapBrowser.openExternalLink('https://servoy.com');
```
