# svyCapture

Welcome to the svyCapture wiki!

## Introduction

svyCapture is a simple service to capture screenshots and audio from browser to a callback method executing on the server.

Table of contents

* [svycapture-screen API](Home.md#svycapture-screen-api)
* [svycapture-audio API](Home.md#svycapture-audio-api)

## svycapture-screen API

| Method                                                   | Params                              | Return | Description                                 |
| -------------------------------------------------------- | ----------------------------------- | :----: | ------------------------------------------- |
| [capture](Home.md#capture)                               | className:string, callback:Function |        | Executes screen-capture using canvas        |
| [captureViaDisplayMedia](Home.md#captureviadisplaymedia) | callback:Function                   |        | Executes screen-capture using display media |

### capture

Executes screen-capture using canvas to html approach.

**Params**

| Type     | Name      | Description                                           | Required |
| -------- | --------- | ----------------------------------------------------- | -------- |
| string   | className | The callback key.                                     | Optional |
| Function | callback  | The function will be called and given screenshot data | Required |

**Returns** void

### captureViaDisplayMedia

Executes screen-capture using display media API.

**Params**

| Type     | Name     | Description                                           | Required |
| -------- | -------- | ----------------------------------------------------- | -------- |
| Function | callback | The function will be called and given screenshot data | Required |

**Returns** void

#### example

```javascript
function onAction(event) {
	plugins.svycaptureScreen.capture(null, getImage);
}

function getImage(img) {
        //do something with b64 image data.
        var img_data = '<img src="'+img+'"/>';
}

```

## svycapture-audio API

| Method                           | Params                               | Return | Description             |
| -------------------------------- | ------------------------------------ | ------ | ----------------------- |
| [capture](Home.md#capture-audio) | callback:Function, callback:Function |        | Executes audio recorder |
| [stop](Home.md#stop)             | callback:Function,callback:Function  |        | Stops audio recording   |

### capture

Executes audio recorder.

**Params**

| Type     | Name            | Description                                                                    | Required |
| -------- | --------------- | ------------------------------------------------------------------------------ | -------- |
| Function | successCallback | The function will be called when finished with audio recording and return data | Required |
| Function | errorCallback   | The function will be called if something fails                                 | Optional |

**Returns** void

### stop

Stops audio recording. **Params**

| Type     | Name            | Description                                                     | Required |
| -------- | --------------- | --------------------------------------------------------------- | -------- |
| Function | successCallback | The function will be called if successful in stopping recording | Optional |
| Function | errorCallback   | The function will be called if something fails                  | Optional |

**Returns** void

#### example

```javascript
function onAction$captureAudio(event) {
	plugins.svycaptureAudio.capture(audioCB, null);
}

function audioCB(data) {
        //print out b64 data with audio recording
	application.output(data);
}

function onAction$StopAudio(event) {
	plugins.svycaptureAudio.stop(null, null);
}

```
