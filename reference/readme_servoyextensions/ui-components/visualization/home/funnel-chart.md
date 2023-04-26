# Funnel Chart

## Preview

![37270921-0021a42c-25d1-11e8-8823-926758ad0061](../../../../../extensions/ui-components/visualization/svyChartJS/images/66974809-00a84600-f062-11e9-855b-91523bde7c86.jpg) ![37270922-003b924c-25d1-11e8-9795-11a6dc35c68a](../../../../../extensions/ui-components/visualization/svyChartJS/images/66974871-2fbeb780-f062-11e9-9199-54c85e921555.jpg) ![37270924-00574fd2-25d1-11e8-933d-1a07ee16862d](../../../../../extensions/ui-components/visualization/svyChartJS/images/66974872-31887b00-f062-11e9-81c9-1652953576e6.jpg) ![37288346-514d2f0c-2607-11e8-8bcb-eacabd470d8f](../../../../../extensions/ui-components/visualization/svyChartJS/images/66974874-32211180-f062-11e9-8dcf-65ee713b542e.jpg) ![37288348-521abcb0-2607-11e8-87cb-b52fc5575f44](../../../../../extensions/ui-components/visualization/svyChartJS/images/66974877-33523e80-f062-11e9-8b04-5f16aa4418a2.jpg)

## Example Usage

```javascript
var data = {
	type: 'funnel',
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

### Options

**sort**

Reverse or not, you can set 'desc' to draw an upside-down funnel. Default is 'asc'.

**gap**

The gap between to trapezium in our funnel chart. The unit is px. Default is 2

**keep**

Draw element against left or right side. Default is 'auto'.

**topWidth**

The top-width of funnel chart, defualt is 0.

**bottomWidth**

The bottom-width of funnel chart, default use the width of canvas.
