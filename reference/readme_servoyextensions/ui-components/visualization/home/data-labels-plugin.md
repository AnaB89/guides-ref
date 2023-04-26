# Example Usage
```javascript
	var DATA_COUNT = 10;
	var labels = [];

	for (var i = 0; i < DATA_COUNT; ++i) {
		labels.push('' + i);
	}

	var dt = [];
	var dt1 = [];
	var dt2 = [];
	for (i = 0; i < DATA_COUNT; ++i) {
		dt.push(Math.ceil((Math.random() * 100)));
		dt1.push(Math.ceil((Math.random() * 100)));
		dt2.push(Math.ceil((Math.random() * 100)));
	}

	var data = {
		type: 'line',
		data: {
			labels: labels,
			datasets: [{
				backgroundColor: 'teal',
				borderColor: 'teal',
				data: dt,
				datalabels: {
					align: 'start',
					anchor: 'start'
				}
			}, {
				backgroundColor: 'blue',
				borderColor: 'blue',
				data: dt1
			}, {
				backgroundColor: 'purple',
				borderColor: 'purple',
				data: dt2,
				datalabels: {
					align: 'end',
					anchor: 'end'
				}
			}]
		}
	}

	var options = {
		plugins: {
			datalabels: {
				backgroundColor: {
					isFunction: true,
					params: ['context'],
					expression: "return context.dataset.backgroundColor;"
				},
				borderRadius: 4,
				color: 'white',
				font: {
					weight: 'bold'
				},
				formatter: {
					isFunction: true,
					params: [''],
					expression: "return Math.round"
				},
				padding: 6
			}
		},

		// Core options
		legend: {
			display: false
		},
		title: {
			display: true,
			text: 'Data Labels'
		},
		aspectRatio: 5 / 3,
		layout: {
			padding: {
				top: 32,
				right: 16,
				bottom: 16,
				left: 8
			}
		},
		elements: {
			line: {
				fill: false
			}
		},
		tooltips: {
			  isFunction: true,
		      params: ['tooltipItem', 'data'],
		      expression: "return ''"
		},
		scales: {
			yAxes: [{
				stacked: true
			}]
		}
	}

	elements.chart.setData(data);
	elements.chart.setOptions(options);
```


*Note that this plugin will not work when used along side outlabels plugin (Use one or the other)

*Listeners not yet supported fully in current release.