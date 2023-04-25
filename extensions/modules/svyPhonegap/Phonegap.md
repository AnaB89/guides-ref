# API Documentation 

## Method Summary
### executeScript
Execute client side script

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
String | script | script to execute | required

### setOnResumeMethod
When resuming an application set a callback method.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Function | callback | on success callback | required

### setOnPauseMethod
When pausing an application set a callback method.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Function | callback | on success callback | required

### setOnBackMethod
When hitting the hardware back button set a callback method (Android only).

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Function | callback | on success callback | required

### exit
Exit the application ( not to be confused with Servoy's application.exit method which only exits server session)

### quitServoySolution
Quit/logout to the main solution (calling this instead of security.logout allows us to re-init plugins again)


# Example Usage
```javascript
//check if phonegap is supported
plugins.svyphonegapPhonegap.executeScript('', [], support);
//add check for back button press
plugins.svyphonegapPhonegap.setOnBackMethod(goBack);

function support() {
	application.output('supported');
	phonegapEnabled = true;
}

function goBack() {
var ans = plugins.dialogs.showQuestionDialog('INFO', 'Exit App?', 'Yes', 'No');
if (ans == 'Yes') {
//exit app
plugins.svyphonegapPhonegap.exit();}
}


//Play a beep sound/ringtone on the phone
function onAction$beep(event) {
	plugins.svyphonegapPhonegap.beep(1);
}

//Vibrate phone for 1000 ms
function onAction$vibrate(event) {
	plugins.svyphonegapPhonegap.vibrate(1000);	
}


```
