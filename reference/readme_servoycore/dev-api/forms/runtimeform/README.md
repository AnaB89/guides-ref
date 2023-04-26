# RuntimeForm

## Property Summary

| Type                                               | Name                        | Summary                                                     |
| -------------------------------------------------- | --------------------------- | ----------------------------------------------------------- |
| [RuntimeForm](./)                                  | [\_super](./#\_super)       | Provides access to the methods of the parent of this form.. |
| [containers](containers/)                          | [containers](./#containers) | Get an object with the containers of a responsive form..    |
| [controller](controller.md)                        | [controller](./#controller) | Get the controller of the form..                            |
| [elements](elements/)                              | [elements](./#elements)     | Get an array with the elements in the form..                |
| [JSFoundSet](../../database-manager/jsfoundset.md) | [foundset](./#foundset)     | Get the foundset of the form..                              |

## Properties Details

### \_super

Provides access to the methods of the parent of this form.

**Returns**\
[RuntimeForm](./)

**Sample**

```javascript
_super.some_method();
```

### containers

Get an object with the containers of a responsive form.

**Returns**\
[containers](containers/)

**Sample**

```javascript
containers.mycontainer.addStyleClasses("red","blue");
```

### controller

Get the controller of the form.

**Returns**\
[controller](controller.md)

**Sample**

```javascript
controller.enabled = !controller.enabled;
```

### elements

Get an array with the elements in the form.

**Returns**\
[elements](elements/)

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
[JSFoundSet](../../database-manager/jsfoundset.md)

**Sample**

```javascript
application.output("selected index in form foundset: " + foundset.getSelectedIndex());
```
