# JSInsetList

## Property Summary

| Type                          | Name                                                        | Summary                                                                                                                    |
| ----------------------------- | ----------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| [String](../js-lib/string.md) | [headerDataProviderID](jsinsetlist.md#headerDataProviderID) | The text of this data-provider will appear on top of the inset list; if not specified, 'headerText' will be used instead.. |
| [String](../js-lib/string.md) | [headerStyleClass](jsinsetlist.md#headerStyleClass)         | The styleClass of the list header..                                                                                        |
| [String](../js-lib/string.md) | [headerText](jsinsetlist.md#headerText)                     | This text will appear on top of the inset list if 'headerDataProviderID' is not set..                                      |
| [String](../js-lib/string.md) | [name](jsinsetlist.md#name)                                 | The name of this inset list..                                                                                              |
| [String](../js-lib/string.md) | [relationName](jsinsetlist.md#relationName)                 | Name of the relation to be used by the inset list..                                                                        |
| [Number](../js-lib/number.md) | [x](jsinsetlist.md#x)                                       | The x coordinate of the component on the form..                                                                            |
| [Number](../js-lib/number.md) | [y](jsinsetlist.md#y)                                       | The y coordinate of the component on the form..                                                                            |

## Properties Details

### headerDataProviderID

The text of this data-provider will appear on top of the inset list; if not specified, 'headerText' will be used instead.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var insetList = jsform.getInsetList('il1');

var newInsetList = jsform.newInsetList(8,insetList.dataSource,insetList.relationName,insetList.headerText,insetList.textDataProviderID);
newInsetList.name = 'il2';
```

### headerStyleClass

The styleClass of the list header. Can have values from 'a' to 'e'.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var newInsetList = jsform.newInsetList(8,insetList.dataSource,insetList.relationName,insetList.headerText,insetList.textDataProviderID);
newInsetList.headerStyleClass = 'e';
```

### headerText

This text will appear on top of the inset list if 'headerDataProviderID' is not set.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var insetList = jsform.getInsetList('il1');

var newInsetList = jsform.newInsetList(8,insetList.dataSource,insetList.relationName,insetList.headerText,insetList.textDataProviderID);
newInsetList.name = 'il2';
```

### name

The name of this inset list.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var insetList = jsform.getInsetList('il1');

var newInsetList = jsform.newInsetList(8,insetList.dataSource,insetList.relationName,insetList.headerText,insetList.textDataProviderID);
newInsetList.name = 'il2';
```

### relationName

Name of the relation to be used by the inset list.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var insetList = jsform.getInsetList('il1');

var newInsetList = jsform.newInsetList(8,insetList.dataSource,insetList.relationName,insetList.headerText,insetList.textDataProviderID);
newInsetList.name = 'il2';
```

### x

The x coordinate of the component on the form.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var newInsetList = jsform.newInsetList(8,insetList.dataSource,insetList.relationName,insetList.headerText,insetList.textDataProviderID);
newInsetList.x = 90;
newInsetList.y = 90;
application.output('location of newInsetList: ' + newInsetList.x + ', ' + newInsetList.y);
```

### y

The y coordinate of the component on the form.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
var newInsetList = jsform.newInsetList(8,insetList.dataSource,insetList.relationName,insetList.headerText,insetList.textDataProviderID);
newInsetList.x = 90;
newInsetList.y = 90;
application.output('location of newInsetList: ' + newInsetList.x + ', ' + newInsetList.y);
```
