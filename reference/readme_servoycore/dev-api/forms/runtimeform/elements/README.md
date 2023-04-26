# elements

## Property Summary

| Type                                    | Name                     | Summary                                                  |
| --------------------------------------- | ------------------------ | -------------------------------------------------------- |
| [RuntimeComponent](runtimecomponent.md) | [\[index\]](./#\[index]) | Get an element of the form by its index..                |
| [RuntimeComponent](runtimecomponent.md) | [\[name\]](./#\[name])   | Get an element of the form by its name..                 |
| [Array](../../../js-lib/array.md)       | [allnames](./#allnames)  | Get the names of all elements of the form, as an array.. |
| [Number](../../../js-lib/number.md)     | [length](./#length)      | Get the number of elements of the form..                 |

## Properties Details

### \[index]

Get an element of the form by its index.

**Returns**\
[RuntimeComponent](runtimecomponent.md)

**Sample**

```javascript
for (var i=0; i<elements.length; i++)
{
	var elem = elements[i];
	application.output(elem.getName() + ": " + elem.getDataProviderID());
}
```

### \[name]

Get an element of the form by its name.

**Returns**\
[RuntimeComponent](runtimecomponent.md)

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
[Array](../../../js-lib/array.md)

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
[Number](../../../js-lib/number.md)

**Sample**

```javascript
for (var i=0; i<elements.length; i++)
{
	var elem = elements[i];
	application.output(elem.getName() + ": " + elem.getDataProviderID());
}
```
