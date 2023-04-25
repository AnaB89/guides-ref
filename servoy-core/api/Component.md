#  Component


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Object](JSLib/Object.md) | [getClientProperty(key)](Component.md#getclientproperty-key)                   | Gets the specified client property for the element based on a key..                                    |
| [Object](JSLib/Object.md) | [getDesignProperties()](Component.md#getdesignproperties)                   | Get the design-time properties of an element..                                    |
| [Object](JSLib/Object.md) | [getDesignTimeProperty(key)](Component.md#getdesigntimeproperty-key)                   | Get a design-time property of an element..                                    |
| [String](JSLib/String.md) | [getElementType()](Component.md#getelementtype)                   | Returns the type of a specified element..                                    |
| [String](JSLib/String.md) | [getFormName()](Component.md#getformname)                   | Returns the name of the form..                                    |
| [String](JSLib/String.md) | [getName()](Component.md#getname)                   | Returns the name of an element..                                    |
|void | [putClientProperty(key, value)](Component.md#putclientproperty-key-value)                   | Sets the value for the specified element client property key..                                    |

## Methods Details

### getClientProperty(key)

Gets the specified client property for the element based on a key.

NOTE: Depending on the operating system, a user interface property name may be available.

**Parameters**\
[Object](JSLib/Object.md) key user interface key (depends on operating system)

**Returns**\
[Object](JSLib/Object.md) The value of the property for specified key.


**Sample**

```javascript
var property = %%elementName%%.getClientProperty('ToolTipText');
```
### getDesignProperties()

Get the design-time properties of an element.


**Returns**\
[Object](JSLib/Object.md) 


**Sample**

```javascript
var prop = forms.orders.elements.mylabel.getDesignProperties()
```
### getDesignTimeProperty(key)

Get a design-time property of an element.

**Parameters**\
[String](JSLib/String.md) key the name of the property

**Returns**\
[Object](JSLib/Object.md) 


**Sample**

```javascript
var prop = forms.orders.elements.mylabel.getDesignTimeProperty('myprop')
```
### getElementType()

Returns the type of a specified element.


**Returns**\
[String](JSLib/String.md) The display type of the element as String.


**Sample**

```javascript
var et = %%elementName%%.getElementType();
```
### getFormName()

Returns the name of the form. (may be empty string as well)


**Returns**\
[String](JSLib/String.md) The name of the form.


**Sample**

```javascript
var name = %%elementName%%.getFormName();
```
### getName()

Returns the name of an element. (may be null as well)


**Returns**\
[String](JSLib/String.md) The name of the element.


**Sample**

```javascript
var name = %%elementName%%.getName();
```
### putClientProperty(key, value)

Sets the value for the specified element client property key.

NOTE: Depending on the operating system, a user interface property name may be available.

**Parameters**\
[Object](JSLib/Object.md) key user interface key (depends on operating system)\
[Object](JSLib/Object.md) value a predefined value for the key

**Returns**\
void 


**Sample**

```javascript
%%elementName%%.putClientProperty('ToolTipText','some text');
```

