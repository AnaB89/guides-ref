# Example Usage
```javascript
var bgExpression =  "if(ctx.dataset.data[ctx.dataIndex])";
    bgExpression += "{var value = ctx.dataset.data[ctx.dataIndex].v;}";
    bgExpression += "else{alpha = 1;}; var alpha = (value + 3) / 10;";
    bgExpression += "return Color('blue').alpha(alpha).rgbString();";
		
	var data = {
		type: 'treemap',
		data: {			
			datasets: [{
				label: 'Basic treemap',
	                        tree: [6,6,5,4,3,2,2,1],
	                        fontColor: '#000',
	                        fontFamily: 'serif',
	                        fontSize: 12,
	                        fontStyle: 'normal',
				backgroundColor: {
					isFunction: true,
					params: ['ctx'],
					expression: bgExpression
				}
			}]
		}
	}

//Initialize the chart by using setData
elements.chart.setData(data);
```

## Options