# API Documentation 

## Method Summary
### activate
Activate card reader

### swipe
Prepare card reader to accept a swipe

### cancelTask
Cancel current task or swipe

### registerObservers
Register observers for reader events	

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Function | OnAttachment | device is attached | Optional
Function | OnDetachment | device is unattached | Optional
Function | OnConnect | device is connected. | Optional
Function | OnDisconnect | device is disconnected. | Optional
Function | OnPowering | device is powering on. | Optional
Function | OnCardSwipe | device is trying to receive swipe | Optional
Function | OnCardDataProcessing | device is trying to process data | Optional
Function | OnDidReceiveCardData | device swipe returned data | Optional
Function | OnCardSwipeFailed | device swipe failed | Optional
Function | OnCmdSending | note yet implemented | Optional
Function | OnDidReceiveCmdResponse | note yet implemented | Optional
Function | OnCMDFailed | note yet implemented | Optional
Function | OnSystemMessage | note yet implemented | Optional

# Example Usage
```javascript
var connected = false;

//on first show of form or scope, try to activate the device:
function onShow(firstShow, event) {
//disconnect if connected
if (connected) {plugins.svyphonegapUnimag.deactivate();}
//register listeners
plugins.svyphonegapUnimag.registerObservers(null, null, OnConnect, null, null, null, null, null, OnDidReceiveCardData, null, null, null, null, null)
//Activate device
plugins.svyphonegapUnimag.activate();

}

function OnConnect() {	
        connected = true;
	//start looking for a swipe
	plugins.svyphonegapUnimag.swipe();
}

function OnDidReceiveCardData(d1, d2) {
	var messages = 'Data retrieved: \n';

        //get base16 encoded string
	messages += d1 + '\n \n';
        //get ASCII string, with escape chars
	messages += d2;
        // print out data
	application.output(messages);
	
	//swipe the card again
	plugins.svyphonegapUnimag.swipe();
}
```
