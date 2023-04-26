# Block UI

## Block UI

Welcome to the svyBlockUI wiki!

### Introduction

svyBlockUI is a simple service to block the UI either with a message and/or a spinner. The service can be used to let the user know that a certain operation may take a while for example.

The UI is blocked by an overlay that prevents the user from clicking anywhere in the background while the UI is blocked. The services provides 11 different spinners and the possibility to update the message during a process

Here is a screenshot of a blocked UI with message and the "Tree bounce" spinner.

![Screenshot](../../../extensions/browser-plugins/svyBlockUI/images/image\_01.png)

### svyBlockUI in NGClient2

## svyBlockUI in NGClient2

In NGClient2 , we use a different library for [svyBlockUI implementation](https://github.com/kuuurt13/ng-block-ui). The styling of the new component is different than NGClient1, the UI customizations are currently not available currently in NGClient2 as those should be done via CSS. The classes to use are: block-ui-wrapper (all overlay), loader (child class for spinner implementation) and message (child class for message).

Table of contents

* [svyBlockUI properties](home.md#svyblockui-properties)
* [svyBlockUI API](home.md#svyblockui-api)

### svyBlockUI properties

The service has the following properties:

| Property          | Type   | Default | Description                                                                                                                                                                                           |
| ----------------- | ------ | ------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| spinnerBgColor    | String | null    | Color for most of the available spinners (it does not work for "Circle", "Cube grid", "Fading circle" and "Folding cube")                                                                             |
| overlayColor      | String | #ffffff | The color of the overlay (default is white)                                                                                                                                                           |
| overlayOpacity    | Number | 0.5     | The opacity of the overlay (default is 50%)                                                                                                                                                           |
| messageStyleClass | String | null    | Style class of the message container; if set, properties from that style class are applied.                                                                                                           |
| spinner           | String | null    | The name of the spinner to show; one of "Rotating plane", "Double bounce", "Wave", "Wandering cubes", "Pulse", "Chasing dots", "Three bounce", "Circle", "Cube grid", "Fading circle", "Folding cube" |

### svyBlockUI API

| Method                           | Params                      | Return | Description                                         |
| -------------------------------- | --------------------------- | ------ | --------------------------------------------------- |
| [show](home.md#show)             | message:String,delay:Number |        | Blocks the UI, optionally showing the given message |
| [stop](home.md#stop)             |                             |        | Stops (hides) all UI blockers                       |
| [setMessage](home.md#setmessage) | message:String              |        | Updates the message shown                           |

#### show

Blocks the UI, optionally showing the given message.

**Params**

| Type   | Name    | Description                                                                                                                       | Required |
| ------ | ------- | --------------------------------------------------------------------------------------------------------------------------------- | -------- |
| String | message | The message to show; when null, no message will be shown.                                                                         | Optional |
| Number | delay   | The wait time before showing the message. Ideal for when an operation may complete quickly, in which case blocking might not show | Optional |

**Returns** void

#### stop

Stops (hides) all UI blockers.

**Params** none

**Returns** void

#### setMessage

Updates the message shown

**Params**

| Type   | Name    | Description         | Required |
| ------ | ------- | ------------------- | -------- |
| String | message | The message to show | Required |

**Returns** void
