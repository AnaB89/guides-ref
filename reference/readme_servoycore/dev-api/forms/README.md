# Forms

## Property Summary

| Type                          | Name                   | Summary                                      |
| ----------------------------- | ---------------------- | -------------------------------------------- |
| [RuntimeForm](runtimeform/)   | [\[name\]](./#\[name]) | Get a form by name..                         |
| [Number](../js-lib/number.md) | [length](./#length)    | Get the number of forms loaded into memory.. |

## Properties Details

### \[name]

Get a form by name.

**Returns**\
[RuntimeForm](runtimeform/)

**Sample**

```javascript
var allForms = solutionModel.getForms();
application.output("There are " + allForms.length + " forms.");
for (var i=0; i<allForms.length; i++) 
{
	var f = forms[allForms[i].name];
	application.output("Form " + allForms[i].name + " has selected index " + f.controller.getSelectedIndex());
}
```

### length

Get the number of forms loaded into memory.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
application.output("Number of forms loaded into memory: " + forms.length);
```
