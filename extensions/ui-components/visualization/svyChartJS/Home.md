Welcome to the svyChartJS wiki!

This wiki provides comprehensive documentation for using the **svyChartJS** web-component, which allows you to display a chart utlizing the Chart.JS library within Servoy's NGClient.

# Getting Started
First import the component using one of the release [binaries](https://github.com/Servoy/svyChartJS/releases) or via Servoy's Web Package Manager.

If you would like to see the component in an example install the included solution, [svyChartJSExample.servoy](https://github.com/Servoy/svyChartJS/releases).

# Example Usage
First add the component to a form by dragging it into the form using the Palette Wizard.  It should be under ChartJS (chart).

If using a custom dataset (non-foundset) you can setup a simple pie chart by doing the following:
```javascript
//Your data node object which requires a type and the data.
var data = {
	type: 'pie',
	data: {
		labels: ["Red",
		"Green",
		"Yellow"],
	datasets: [{
		data: [300, 50, 100],
		backgroundColor: [
                      "#F7464A",
		      "#46BFBD",
		      "#FDB45C"],
		hoverBackgroundColor: [
                      "#FF5A5E",
		      "#5AD3D1",
		      "#FFC870"]
		}]
	}
}

//Initialize the chart by using setData
elements.chart.setData(data);
```

To add options to a chart you can do the following :
```javascript
//The options object
var options = {
	responsive: false,
	scales: {
		xAxes: [{stacked: true}],
		yAxes: [{stacked: true}]
	}
}

//call the api to set the options
elements.chart.setOptions(options);
```
# Chart Customization
The ChartJS library has great potential for customization.  By passing in your own modified options or by using additional plugins.  We will try and support some of these options on a case by case basis.  Please post an issue for any feature requests which are relevant.

# Support for Outlabels plugin
https://piechart-outlabels.netlify.com/formatting

## Option callbacks
If you need to use callback functions as a part of your options object. You can use the following method to do so:
```javascript
//As Servoy sanitizes functions from server side we are not able to use callback functions like normal:
//Instead of passing in a normal function like below:
var label_callback = function (tooltip,data) {
return ' $'+data.datasets[0].data[tooltipItem.index]; }

//You will need to use a custom object for callbacks functionality to work:
//All functions require an isFunction(set to true), params(your parameters), and expression key/value pair
//Note that the expression can become invalid if params are undefined.  Make sure to use if conditionals to check.
label_callback = {
      isFunction: true,
      params: ['tooltipItem', 'data'],
      expression: "return ' $'+data.datasets[0].data[tooltipItem.index];"
}

var options = {
	tooltips: {
		callbacks: {label: label_callback 
		}
	}
}
//call the api to set the options
elements.chart.setOptions(options);
```
For additional options and documentation please refer to the official ChartJS [docs](https://www.chartjs.org/docs/2.9.4/). 

## Using with responsive forms
When using the component with responsive forms we need to add some additional CSS styling to the component.  In particular the **height** property must be greater than zero.


# API Documentation 

## Method Summary
### generateLegend
Returns a custom html stringed version of the legend. 

### drawChart
Force the chart to (re)Draw if for some reason it has not.

### refreshChart
Force the chart to update if it's options were changed.

### setData
Setup the chart's data. (This will automatically initialize and draw the chart)

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Object| data | options object which requires both a type and data key value { type : String, data : Object } | Required

### setPlugin
Register a plugin. (This method must be called prior to drawing the chart)

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Object| plugin | plugin object | Required

An example of a chart plugin object can be found [here](https://github.com/Servoy/svyChartJS/blob/master/svyChartUtils/chartPlugins.js).


### setOptions
Setup the chart's options. (This will automatically refresh the chart if it already exists)

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Object| option | options object | Required

### clearChart
Clears the chart.

### Events

| Event | Params | Return       | Description
| :--------- |:--------------| :------------:| :-------------------------------------------------------------------|
| onClick | | dataset_index (if using multiple datasets), index, label, value, event  | Fired when clicking on a point |
| onChartDrawn | | | Fired when the chart is rendered |

## Component Properties

Type | Name | Summary | Required
--- |--- | --- | ---
Object | foundset | Using the foundset's data for chart | Optional
String | LegendLabel | Show a default title of chart | Optional
Array<String> | backgroundColor | An array of colors to use for displaying the background of each series | Optional
String | borderColor | Color to use for displaying the chart's border | Optional
String | borderWidth | Border width of an data value | Optional
String | hoverBackgroundColor | Background color of hovered selection | Optional
String | hoverBorderColor | Border color of hovered selection | Optional
String | hoverBorderWidth | Border width of an data value of hovered selection | Optional
String | styleClass | Style class of the component's wrapper | Optional
