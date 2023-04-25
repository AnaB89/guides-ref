Required Phonegap plugins
------------------
cordova-plugin-fcm

Requirements for Firebase
------------------
An Server key is required from Google Firebase Cloud Messaging Service.  You can get one [here](https://firebase.google.com/).  Follow instructions to attain a google-services.json file as you will need it for the build.

We may also need to update the config.xml depending on the SDK to include that resource file.  You can add the following line for the Android platform:
`<resource-file src="google-services.json" target="google-services.json"/>`

For iOS you can add a plist file with the proper values:
`<resource-file src="GoogleService-Info.plist"/>`

For iOS, you will also need to generate an Apple Push Notification certificate (APN) within the Certificates, Identifiers, and Profiles page.  Within FCM console, make sure to upload those certificates.

# API Documentation 

## Method Summary
### onTokenRefresh
Get a callback every time a token is generated, including the initial generation.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Function | successCallback | on success callback | Optional
Function | errorCallback | on error callback | Optional

### getToken
Generate a token

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Function | successCallback | on success callback | Optional
Function | errorCallback | on error callback | Optional

### subscribeToTopic
Subscribe to a topic and get notifications
All devices are subscribed automatically to 'all' and 'ios' or 'android' topic respectively.
Topic String must match the following regular expression: "[a-zA-Z0-9-_.~%]{1,900}".

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Function | successCallback | on success callback | Optional
Function | errorCallback | on error callback | Optional
String | Topic | Topic to subscribe | Required

### unubscribeFromTopic
unSubscribe from a topic and no longer receive notifications.
All devices are subscribed automatically to 'all' and 'ios' or 'android' topic respectively.
Topic String must match the following regular expression: "[a-zA-Z0-9-_.~%]{1,900}".

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Function | successCallback | on success callback | Optional
Function | errorCallback | on error callback | Optional
String | Topic | Topic to unsubscribe from | Required

### onNotification
Define the behavior receiving a notification.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Function | onNotificationCallback | when notification is received | Optional
Function | successCallback | on success callback | Optional
Function | errorCallback | on error callback | Optional

### sendNotification
Send a notification to devices that are subscribed to a particular topic.
An Server key is required from Google Firebase Cloud Messaging Service.  You can get one [here](https://firebase.google.com/).

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
String | authKey | FCM server key | Required
String | title | Notification Title | Required
String | body | Notification Body | Required
String | topic | send to subscribed notification topic | Optional
Function | successCallback | on success callback | Optional
Function | errorCallback | on error callback | Optional



# Example Usage
```javascript

//initialize and generate a notification token.
plugins.svyphonegapPush.getToken(null, null);

//subscribe to notifications where topic = svyMobile.
plugins.svyphonegapPush.subscribeToTopic(null, null, 'svyMobile')

//when receiving a notification display a message if UI is visible.
plugins.svyphonegapPush.onNotification(showMessage, null, null)

//Use a callback function to designate behavior when notification is received.
function showMessage(data) {
//if application is in background
	if (data.wasTapped) {
		plugins.dialogs.showInfoDialog('INFO', 'Notification received while UI closed.')
	} else {
//if application is active
		plugins.dialogs.showInfoDialog('INFO', 'Notification received while UI visible.')
	}
}

//Sending a message
plugins.svyphonegapPush.sendNotification('fcmAuthKey', 'INFO', 'This is a push notification message for you', 'svyMobile',null,null )

```
