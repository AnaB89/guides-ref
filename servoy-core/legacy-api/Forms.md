#  Forms

## **Supported Clients**

    SmartClient
    WebClient
    NGClient
    MobileClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [RuntimeForm](Forms/RuntimeForm.md) | [[name]](Forms.md#[name])                   | Get a form by name..                                    |
| [Number](JSLib/Number.md) | [length](Forms.md#length)                   | Get the number of forms loaded into memory..                                    |

## Properties Details

### [name]

Get a form by name.

**Returns**\
[RuntimeForm](Forms/RuntimeForm.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

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
[Number](JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
application.output("Number of forms loaded into memory: " + forms.length);
```

