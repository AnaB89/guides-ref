#  JSRenderEvent

## **Supported Clients**

    SmartClient
    WebClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSRecord](../Database%20Manager/JSRecord.md) | [getRecord()](JSRenderEvent.md#getrecord)                   | Returns the record of the element that is being rendered..                                    |
| [Number](../JSLib/Number.md) | [getRecordIndex()](JSRenderEvent.md#getrecordindex)                   | Returns the record index of the element that is being rendered..                                    |
| [Renderable](./Renderable.md) | [getRenderable()](JSRenderEvent.md#getrenderable)                   | Returns the element that is being rendered..                                    |
| [Boolean](../JSLib/Boolean.md) | [hasFocus()](JSRenderEvent.md#hasfocus)                   | Returns whether or not the element that is being rendered has focus..                                    |
| [Boolean](../JSLib/Boolean.md) | [isRecordSelected()](JSRenderEvent.md#isrecordselected)                   | Returns whatever or not the record of the element that is being rendered is selected..                                    |

## Methods Details

### getRecord()

Returns the record of the element that is being rendered.
This is null for elements of type form when they are in table view mode.


**Returns**\
[JSRecord](../Database%20Manager/JSRecord.md) Record of the element that is being rendered

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// type the record returned from the call with JSDoc, fill in the right server/tablename
/** @type {JSRecord<db:/servername/tablename>} */
var record = event.getRecord();
```
### getRecordIndex()

Returns the record index of the element that is being rendered.


**Returns**\
[Number](../JSLib/Number.md) record index of the element that is being rendered

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
event.getRecordIndex()
```
### getRenderable()

Returns the element that is being rendered.


**Returns**\
[Renderable](./Renderable.md) Renderable the element that is being rendered

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
event.getRenderable();
```
### hasFocus()

Returns whether or not the element that is being rendered has focus.


**Returns**\
[Boolean](../JSLib/Boolean.md) true if the element that is being rendered has the focus, false otherwise

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
event.hasFocus();
```
### isRecordSelected()

Returns whatever or not the record of the element that is being rendered is selected.


**Returns**\
[Boolean](../JSLib/Boolean.md) true if the record of the element that is being rendered is selected

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
event.isRecordSelected()
```

