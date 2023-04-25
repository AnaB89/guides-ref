#  FormPopup

## **Supported Clients**

    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Object](../../JSLib/Object.md) | [component()](FormPopup.md#component)                   | Get the component form popup will be shown relative to..                                    |
|void | [component(component)](FormPopup.md#component-component)                   | Set component form popup will be shown relative to..                                    |
| [String](../../JSLib/String.md) | [dataprovider()](FormPopup.md#dataprovider)                   | Get the popup form dataprovider (which was set using setter)..                                    |
|void | [dataprovider(dataprovider)](FormPopup.md#dataprovider-dataprovider)                   | Set form popup dataprovider that will be set..                                    |
| [Number](../../JSLib/Number.md) | [height()](FormPopup.md#height)                   | Get the popup form height (which was set using setter)..                                    |
|void | [height(height)](FormPopup.md#height-height)                   | Set form popup height..                                    |
| [Object](../../JSLib/Object.md) | [scope()](FormPopup.md#scope)                   | Get the popup form scope (which was set using setter)..                                    |
|void | [scope(scope)](FormPopup.md#scope-scope)                   | Set form popup scope that will be modified..                                    |
|void | [show()](FormPopup.md#show)                   | Show form popup using parameters that were set.                                    |
| [Boolean](../../JSLib/Boolean.md) | [showBackdrop()](FormPopup.md#showbackdrop)                   | Get the popup form show backdrop (which was set using setter)..                                    |
|void | [showBackdrop(showBackdrop)](FormPopup.md#showbackdrop-showbackdrop)                   | Set whether backdrop will be shown..                                    |
| [Number](../../JSLib/Number.md) | [width()](FormPopup.md#width)                   | Get the popup form width (which was set using setter)..                                    |
|void | [width(width)](FormPopup.md#width-width)                   | Set form popup width..                                    |
| [Number](../../JSLib/Number.md) | [x()](FormPopup.md#x)                   | Get the popup form x location (which was set using setter)..                                    |
|void | [x(x)](FormPopup.md#x-x)                   | Set form popup x location..                                    |
| [Number](../../JSLib/Number.md) | [y()](FormPopup.md#y)                   | Get the popup form y location (which was set using setter)..                                    |
|void | [y(y)](FormPopup.md#y-y)                   | Set form popup y location..                                    |

## Methods Details

### component()

Get the component form popup will be shown relative to.


**Returns**\
[Object](../../JSLib/Object.md) IComponent

**Supported Clients**\
NGClient

**Sample**

```javascript
popupform.component();
```
### component(component)

Set component form popup will be shown relative to. If null, will use coordinates or show at screen center.

**Parameters**\
[Object](../../JSLib/Object.md) component the form to show

**Returns**\
void 

**Supported Clients**\
NGClient

**Sample**

```javascript
plugins.window.createFormPopup(forms.orderPicker).component(elements.myelement).show();
```
### dataprovider()

Get the popup form dataprovider (which was set using setter).


**Returns**\
[String](../../JSLib/String.md) String

**Supported Clients**\
NGClient

**Sample**

```javascript
popupform.dataprovider();
```
### dataprovider(dataprovider)

Set form popup dataprovider that will be set. If this is set, also scope needs to be specified.

**Parameters**\
[String](../../JSLib/String.md) dataprovider form popup dataprovider

**Returns**\
void 

**Supported Clients**\
NGClient

**Sample**

```javascript
plugins.window.createFormPopup(forms.orderPicker).dataprovider('myid').scope(foundset.getSelectedRecord()).show();
```
### height()

Get the popup form height (which was set using setter).


**Returns**\
[Number](../../JSLib/Number.md) int

**Supported Clients**\
NGClient

**Sample**

```javascript
popupform.height();
```
### height(height)

Set form popup height. If not set, form design height will be used.

**Parameters**\
[Number](../../JSLib/Number.md) height form popup height

**Returns**\
void 

**Supported Clients**\
NGClient

**Sample**

```javascript
plugins.window.createFormPopup(forms.orderPicker).height(100).show();
```
### scope()

Get the popup form scope (which was set using setter).


**Returns**\
[Object](../../JSLib/Object.md) Object

**Supported Clients**\
NGClient

**Sample**

```javascript
popupform.scope();
```
### scope(scope)

Set form popup scope that will be modified. If this is set, also dataprovider needs to be specified.

**Parameters**\
[Object](../../JSLib/Object.md) scope form popup scope to modify

**Returns**\
void 

**Supported Clients**\
NGClient

**Sample**

```javascript
plugins.window.createFormPopup(forms.orderPicker).dataprovider('myid').scope(foundset.getSelectedRecord()).show();
```
### show()

Show form popup using parameters that were set


**Returns**\
void 

**Supported Clients**\
NGClient

**Sample**

```javascript
plugins.window.createFormPopup(forms.orderPicker).x(100).y(100).width(100).height(100).showBackdrop(true).show();
```
### showBackdrop()

Get the popup form show backdrop (which was set using setter).


**Returns**\
[Boolean](../../JSLib/Boolean.md) boolean

**Supported Clients**\
NGClient

**Sample**

```javascript
popupform.showBackdrop();
```
### showBackdrop(showBackdrop)

Set whether backdrop will be shown. Default value is false.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) showBackdrop form popup showBackdrop

**Returns**\
void 

**Supported Clients**\
NGClient

**Sample**

```javascript
plugins.window.createFormPopup(forms.orderPicker).showBackdrop(true).show();
```
### width()

Get the popup form width (which was set using setter).


**Returns**\
[Number](../../JSLib/Number.md) int

**Supported Clients**\
NGClient

**Sample**

```javascript
popupform.width();
```
### width(width)

Set form popup width. If not set, form design width will be used.

**Parameters**\
[Number](../../JSLib/Number.md) width form popup width

**Returns**\
void 

**Supported Clients**\
NGClient

**Sample**

```javascript
plugins.window.createFormPopup(forms.orderPicker).width(100).show();
```
### x()

Get the popup form x location (which was set using setter).


**Returns**\
[Number](../../JSLib/Number.md) int

**Supported Clients**\
NGClient

**Sample**

```javascript
popupform.x();
```
### x(x)

Set form popup x location. The priority sequence for location is: related element, set location, center of screen.

**Parameters**\
[Number](../../JSLib/Number.md) x form popup x location

**Returns**\
void 

**Supported Clients**\
NGClient

**Sample**

```javascript
plugins.window.createFormPopup(forms.orderPicker).x(100).show();
```
### y()

Get the popup form y location (which was set using setter).


**Returns**\
[Number](../../JSLib/Number.md) int

**Supported Clients**\
NGClient

**Sample**

```javascript
popupform.y();
```
### y(y)

Set form popup y location. The priority sequence for location is: related element, set location, center of screen.

**Parameters**\
[Number](../../JSLib/Number.md) y form popup y location

**Returns**\
void 

**Supported Clients**\
NGClient

**Sample**

```javascript
plugins.window.createFormPopup(forms.orderPicker).y(100).show();
```

