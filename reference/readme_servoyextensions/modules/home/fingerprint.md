Required Phonegap plugins
------------------
cordova-plugin-fingerprint-aio

# API Documentation 

## Method Summary
### isAvailable
Check if fingerprint authentication is available.  If successful it will return a result object with information depending on device and OS.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Function | isAvailableSuccess | on success callback | Optional
Function | isAvailableError | on error callback | Optional

### show
Show authentication dialogue.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Object | config | {{clientId: String, clientSecret: String}} configuration for fingerprint, clientSecret only needed for Android | Required
Function | successCallback | on success callback | Optional
Function | errorCallback | on error callback | Optional


# Example Usage
```javascript

```
