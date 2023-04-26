# Progress Bar

The Progress Bar component shows a progress bar that can be used to indicate the progress of lengthy processes.

Example:

![Progress Bar](../../../../extensions/ui-components/visualization/progressbar/images/image\_01.png)

## Table of contents

* [Progress Bar properties](progress-bar.md#progress-bar-properties)
* [Progress Bar events](progress-bar.md#progress-bar-events)
* [Update Progress Bar](progress-bar.md#update-progress-bar)
* [Progress Bar API](progress-bar.md#progress-bar-api)

## Progress Bar properties

The component has the following properties:

| Property              | Type    | Default | Description                                                                                                                                                                                                                                                                                                                                                                                                                         |
| --------------------- | ------- | ------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| valueText             | String  | null    | When set, the given text is shown inside the progress bar                                                                                                                                                                                                                                                                                                                                                                           |
| max                   | Number  | 100     | The maximum value of the progress                                                                                                                                                                                                                                                                                                                                                                                                   |
| type                  | String  | true    | One of "info", "success", "warning", "danger" which controls the color of the bar similar to the bootstrap button colors                                                                                                                                                                                                                                                                                                            |
| animate               | Boolean | true    | When true, changes of the progress are animated                                                                                                                                                                                                                                                                                                                                                                                     |
| showValue             | Boolean | true    | When true, the value is shown as "value / max"; only used when no valueText is set                                                                                                                                                                                                                                                                                                                                                  |
| showValueAsPercentage | Boolean | true    | When true, the value is shown as as percentage of max                                                                                                                                                                                                                                                                                                                                                                               |
| value                 | Number  | null    | The current progress; when the progress should be updated while a lengthy process is running, you need to use the API method setProgress() to see the progress updating in the client                                                                                                                                                                                                                                               |
| styleClass            | String  | null    | Optional style class(es) to be set to the component. Add "progress-striped" to get a striped progress bar, "progress-striped active" to get "moving" stripes. Any other style class can be added. To specifically select the progress bar itself, use ".your-style-class > .progress-bar" as selector. To change the progress bar height, the height of the component itself and the line-height of the .progress-bar should be set |
| visible               | Boolean | true    | The visible property of the component, default true.                                                                                                                                                                                                                                                                                                                                                                                |

## Progress Bar API

| Method                                     | Params                         | Return | Description                                                   |
| ------------------------------------------ | ------------------------------ | ------ | ------------------------------------------------------------- |
| [setProgress](progress-bar.md#setprogress) | value:Number, valueText:String |        | Updates the progress, optionally setting the given value text |

### setProgress

Updates the progress, optionally setting the given value text

**Params**

| Type   | Name      | Description                                                 | Required |
| ------ | --------- | ----------------------------------------------------------- | -------- |
| Number | value     | The current progress                                        | Required |
| String | valueText | When given, this text will be shown inside the progress bar | Optional |

**Returns** void

## Update progress bar

To update the progress bar you should update the value of the progress bar.

`elements.myProgressBar.value = 60;`

Please note that runtime changes to element's properties are not pushed immediately to the UI. To reduce the number of the round-trip server to client, Servoy keep track of the runtime changes and push them to the client as soon the method thread is terminated or as soon an updateUI is forced. An updateUI can be explicitly invoked with application.updateUI().

The function below updates the progress bar only once the execution is terminated.

```
function onAction(event) {
 // UI is updated only when the the loop is over; there is 1 round-trip server to client
 for (var index = 0; index <= 100; index++) {
   elements.bs_progressbar.value = index;
   application.sleep(50);
 }
}
```

This function behave differently then the function above, updating the progress bar at each iteration.

```
function onAction(event) {
 // UI is updated at each iteration. There are 100 round-trip to server to client
 for (var index = 0; index <= 100; index++) {
   elements.bs_progressbar.value = index;
   application.updateUI();
   application.sleep(50);
 }
}
```

## Progress Bar events

The Progress Bar currently has no events.
