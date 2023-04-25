#  RuntimeForm

## **Supported Clients**

    SmartClient
    WebClient
    NGClient
    MobileClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [RuntimeForm](./RuntimeForm.md) | [_super](RuntimeForm.md#_super)                   | Provides access to the methods of the parent of this form..                                    |
| [containers](RuntimeForm/containers.md) | [containers](RuntimeForm.md#containers)                   | Get an object with the containers of a responsive form..                                    |
| [controller](RuntimeForm/controller.md) | [controller](RuntimeForm.md#controller)                   | Get the controller of the form..                                    |
| [elements](RuntimeForm/elements.md) | [elements](RuntimeForm.md#elements)                   | Get an array with the elements in the form..                                    |
| [JSFoundSet](../Database%20Manager/JSFoundSet.md) | [foundset](RuntimeForm.md#foundset)                   | Get the foundset of the form..                                    |

## Properties Details

### _super

Provides access to the methods of the parent of this form.

**Returns**\
[RuntimeForm](./RuntimeForm.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
_super.some_method();
```
### containers

Get an object with the containers of a responsive form.

**Returns**\
[containers](RuntimeForm/containers.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
containers.mycontainer.addStyleClasses("red","blue");
```
### controller

Get the controller of the form.

**Returns**\
[controller](RuntimeForm/controller.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
controller.enabled = !controller.enabled;
```
### elements

Get an array with the elements in the form.

**Returns**\
[elements](RuntimeForm/elements.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var elems = elements;
application.output("This form has " + elems.length + " named elements.")
for (var i=0; i<elems.length; i++)
	application.output(elems[i].getName());
```
### foundset

Get the foundset of the form.

**Returns**\
[JSFoundSet](../Database%20Manager/JSFoundSet.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
application.output("selected index in form foundset: " + foundset.getSelectedIndex());
```

