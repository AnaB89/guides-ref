Welcome to the svyIdle wiki!
# Introduction
Simple web service to check if a user is idle or if browser window no longer active (NGclient only)

# Example Usage
```js

//setup callback functions for different events

/**
 * @properties={typeid:24,uuid:"E6949E1C-AA93-4145-9509-BF10CA66AC02"}
 */
function idle() {		
	application.output('im idle...');
}

/**
 * @properties={typeid:24,uuid:"09584FE2-2B10-420A-B685-A9A988A6261A"}
 */
function active() {	
	application.output('im active...');
}

/**
 * @properties={typeid:24,uuid:"06ACAC5D-4D1C-49BD-B786-3E9496DA3860"}
 */
function hide() {
	application.output('window hidden');
}

/**
 * @properties={typeid:24,uuid:"1A268EDF-BA18-4E67-A049-6E1305E08D72"}
 */
function show() {
	application.output('window shown');
}

//Then call the onIdle method and pass in callback methods to execute when idle or when windows become hidden/active.
plugins.svyIdle.onIdle(idle,active,hide,show,null,5000,true,false,false);
});
```

# API
## Method Summary
### onIdle
execute service

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Function| onIdle | triggers when user is idle | Optional
Function| onActive | triggers when user is active| Optional
Function| onHide | triggers when window is hidden | Optional
Function| onShow | triggers when window is shown | Optional
String| events| string of events that will reset idle time (default : 'mousemove keydown mousedown touchstart') | Optional
Number| idle | idle time in ms before activating trigger, default: 60000 | Optional
Boolean| keepTracking | set to false if we only want to track the first time (true by default) | Optional
Boolean| startAtIdle | if you want to start at idle, set to true | Optional
Boolean| recurIdleCall | use setInterval versus timeout, by default uses setTimeout | Optional