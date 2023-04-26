# RuntimeWebComponent

## **Extends**

```
Component
```

## Methods Summary

| Type                                | Name                                                                                | Summary                                                             |
| ----------------------------------- | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------- |
| [Object](../../../js-lib/object.md) | [getClientProperty(key)](runtimewebcomponent.md#getclientproperty-key)              | Gets the specified client property for the element based on a key.. |
| [Object](../../../js-lib/object.md) | [getDesignProperties()](runtimewebcomponent.md#getdesignproperties)                 | Get the design-time properties of an element..                      |
| [Object](../../../js-lib/object.md) | [getDesignTimeProperty(key)](runtimewebcomponent.md#getdesigntimeproperty-key)      | Get a design-time property of an element..                          |
| [String](../../../js-lib/string.md) | [getElementType()](runtimewebcomponent.md#getelementtype)                           | Returns the type of a specified element..                           |
| [String](../../../js-lib/string.md) | [getFormName()](runtimewebcomponent.md#getformname)                                 | Returns the name of the form..                                      |
| [String](../../../js-lib/string.md) | [getName()](runtimewebcomponent.md#getname)                                         | Returns the name of an element..                                    |
| void                                | [putClientProperty(key, value)](runtimewebcomponent.md#putclientproperty-key-value) | Sets the value for the specified element client property key..      |

## Methods Details

### getClientProperty(key)

Gets the specified client property for the element based on a key.

NOTE: Depending on the operating system, a user interface property name may be available.

**Parameters**\
[Object](../../../js-lib/object.md) key user interface key (depends on operating system)

**Returns**\
[Object](../../../js-lib/object.md) The value of the property for specified key.

**Sample**

```javascript
var property = %%elementName%%.getClientProperty('ToolTipText');
```

### getDesignProperties()

Get the design-time properties of an element.

**Returns**\
[Object](../../../js-lib/object.md)

**Sample**

```javascript
var prop = forms.orders.elements.mylabel.getDesignProperties()
```

### getDesignTimeProperty(key)

Get a design-time property of an element.

**Parameters**\
[String](../../../js-lib/string.md) key the name of the property

**Returns**\
[Object](../../../js-lib/object.md)

**Sample**

```javascript
var prop = forms.orders.elements.mylabel.getDesignTimeProperty('myprop')
```

### getElementType()

Returns the type of a specified element.

**Returns**\
[String](../../../js-lib/string.md) The display type of the element as String.

**Sample**

```javascript
var et = %%elementName%%.getElementType();
```

### getFormName()

Returns the name of the form. (may be empty string as well)

**Returns**\
[String](../../../js-lib/string.md) The name of the form.

**Sample**

```javascript
var name = %%elementName%%.getFormName();
```

### getName()

Returns the name of an element. (may be null as well)

**Returns**\
[String](../../../js-lib/string.md) The name of the element.

**Sample**

```javascript
var name = %%elementName%%.getName();
```

### putClientProperty(key, value)

Sets the value for the specified element client property key.

NOTE: Depending on the operating system, a user interface property name may be available.

**Parameters**\
[Object](../../../js-lib/object.md) key user interface key (depends on operating system)\
[Object](../../../js-lib/object.md) value a predefined value for the key

**Returns**\
void

**Sample**

```javascript
%%elementName%%.putClientProperty('ToolTipText','some text');
```
