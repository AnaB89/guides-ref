#  JSInsetList

## **Supported Clients**

    MobileClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [headerDataProviderID](JSInsetList.md#headerDataProviderID)                   | The text of this data-provider will appear on top of the inset list; if not specified, 'headerText' will be used instead..                                    |
| [String](../JSLib/String.md) | [headerStyleClass](JSInsetList.md#headerStyleClass)                   | The styleClass of the list header..                                    |
| [String](../JSLib/String.md) | [headerText](JSInsetList.md#headerText)                   | This text will appear on top of the inset list if 'headerDataProviderID' is not set..                                    |
| [String](../JSLib/String.md) | [name](JSInsetList.md#name)                   | The name of this inset list..                                    |
| [String](../JSLib/String.md) | [relationName](JSInsetList.md#relationName)                   | Name of the relation to be used by the inset list..                                    |
| [Number](../JSLib/Number.md) | [x](JSInsetList.md#x)                   | The x coordinate of the component on the form..                                    |
| [Number](../JSLib/Number.md) | [y](JSInsetList.md#y)                   | The y coordinate of the component on the form..                                    |

## Properties Details

### headerDataProviderID

The text of this data-provider will appear on top of the inset list; if not specified, 'headerText' will be used instead.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
NGClient,MobileClient

**Sample**

```javascript
var insetList = jsform.getInsetList('il1');

var newInsetList = jsform.newInsetList(8,insetList.dataSource,insetList.relationName,insetList.headerText,insetList.textDataProviderID);
newInsetList.name = 'il2';
```
### headerStyleClass

The styleClass of the list header. Can have values from 'a' to 'e'.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
NGClient,MobileClient

**Sample**

```javascript
var newInsetList = jsform.newInsetList(8,insetList.dataSource,insetList.relationName,insetList.headerText,insetList.textDataProviderID);
newInsetList.headerStyleClass = 'e';
```
### headerText

This text will appear on top of the inset list if 'headerDataProviderID' is not set.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
NGClient,MobileClient

**Sample**

```javascript
var insetList = jsform.getInsetList('il1');

var newInsetList = jsform.newInsetList(8,insetList.dataSource,insetList.relationName,insetList.headerText,insetList.textDataProviderID);
newInsetList.name = 'il2';
```
### name

The name of this inset list.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
NGClient,MobileClient

**Sample**

```javascript
var insetList = jsform.getInsetList('il1');

var newInsetList = jsform.newInsetList(8,insetList.dataSource,insetList.relationName,insetList.headerText,insetList.textDataProviderID);
newInsetList.name = 'il2';
```
### relationName

Name of the relation to be used by the inset list.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
NGClient,MobileClient

**Sample**

```javascript
var insetList = jsform.getInsetList('il1');

var newInsetList = jsform.newInsetList(8,insetList.dataSource,insetList.relationName,insetList.headerText,insetList.textDataProviderID);
newInsetList.name = 'il2';
```
### x

The x coordinate of the component on the form.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
NGClient,MobileClient

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
[Number](../JSLib/Number.md) 

**Supported Clients**\
NGClient,MobileClient

**Sample**

```javascript
var newInsetList = jsform.newInsetList(8,insetList.dataSource,insetList.relationName,insetList.headerText,insetList.textDataProviderID);
newInsetList.x = 90;
newInsetList.y = 90;
application.output('location of newInsetList: ' + newInsetList.x + ', ' + newInsetList.y);
```

