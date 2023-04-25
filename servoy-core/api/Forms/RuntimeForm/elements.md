#  elements


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [RuntimeComponent](elements/RuntimeComponent.md) | [[index]](elements.md#[index])                   | Get an element of the form by its index..                                    |
| [RuntimeComponent](elements/RuntimeComponent.md) | [[name]](elements.md#[name])                   | Get an element of the form by its name..                                    |
| [Array](../../JSLib/Array.md) | [allnames](elements.md#allnames)                   | Get the names of all elements of the form, as an array..                                    |
| [Number](../../JSLib/Number.md) | [length](elements.md#length)                   | Get the number of elements of the form..                                    |

## Properties Details

### [index]

Get an element of the form by its index.

**Returns**\
[RuntimeComponent](elements/RuntimeComponent.md) 


**Sample**

```javascript
for (var i=0; i<elements.length; i++)
{
	var elem = elements[i];
	application.output(elem.getName() + ": " + elem.getDataProviderID());
}
```
### [name]

Get an element of the form by its name.

**Returns**\
[RuntimeComponent](elements/RuntimeComponent.md) 


**Sample**

```javascript
for (var i=0; i<elements.allnames.length; i++)
{
	var name = elements.allnames[i];
	var elem = elements[name];
	application.output(name + ": " + elem.getDataProviderID());	
}
```
### allnames

Get the names of all elements of the form, as an array.

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
for (var i=0; i<elements.allnames.length; i++)
{
	var name = elements.allnames[i];
	var elem = elements[name];
	application.output(name + ": " + elem.getDataProviderID());	
}
```
### length

Get the number of elements of the form.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
for (var i=0; i<elements.length; i++)
{
	var elem = elements[i];
	application.output(elem.getName() + ": " + elem.getDataProviderID());
}
```

