#  History


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](JSLib/Boolean.md) | [buttonsEnabled](History.md#buttonsEnabled)                   | Set/Get the history buttons enabled..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [back()](History.md#back)                   | Navigates back in the history stack; shows the previous form (if present)..                                    |
|void | [clear()](History.md#clear)                   | Clear the entire history stack..                                    |
|void | [forward()](History.md#forward)                   | Navigates forward in the history stack; shows the next form (if present)..                                    |
| [Number](JSLib/Number.md) | [getCurrentIndex()](History.md#getcurrentindex)                   | Get the current absolute index in the history stack..                                    |
| [String](JSLib/String.md) | [getFormName(i)](History.md#getformname-i)                   | Get the form name based on the specified absolute index in the history stack location..                                    |
|void | [go(i)](History.md#go-i)                   | Navigates to the relative index based on current position in the history..                                    |
| [Boolean](JSLib/Boolean.md) | [removeForm(formName)](History.md#removeform-formname)                   | Removes the named form item from the history stack (and from memory) if not currently shown..                                    |
| [Boolean](JSLib/Boolean.md) | [removeIndex(index)](History.md#removeindex-index)                   | Removes an absolute index based history stack form item..                                    |
| [Number](JSLib/Number.md) | [size()](History.md#size)                   | Returns the total size of the history stack..                                    |

## Properties Details

### buttonsEnabled

Set/Get the history buttons enabled.

**Returns**\
[Boolean](JSLib/Boolean.md) 


**Sample**

```javascript
history.buttonsEnabled = true;
var status = history.buttonsEnabled;
```

## Methods Details

### back()

Navigates back in the history stack; shows the previous form (if present).


**Returns**\
void 


**Sample**

```javascript
history.back();
```
### clear()

Clear the entire history stack.


**Returns**\
void 


**Sample**

```javascript
history.clear();
```
### forward()

Navigates forward in the history stack; shows the next form (if present).


**Returns**\
void 


**Sample**

```javascript
history.forward();
```
### getCurrentIndex()

Get the current absolute index in the history stack.


**Returns**\
[Number](JSLib/Number.md) the current absolute index


**Sample**

```javascript
var abs_index = history.getCurrentIndex();
```
### getFormName(i)

Get the form name based on the specified absolute index in the history stack location.

**Parameters**\
[Number](JSLib/Number.md) i the absolute index

**Returns**\
[String](JSLib/String.md) the formName


**Sample**

```javascript
var name = history.getFormName(history.getCurrentIndex());
```
### go(i)

Navigates to the relative index based on current position in the history.

**Parameters**\
[Number](JSLib/Number.md) i the relative index

**Returns**\
void 


**Sample**

```javascript
history.go(-3);
```
### removeForm(formName)

Removes the named form item from the history stack (and from memory) if not currently shown.
Will return false when the form can't be removed, this can happen in certain situations:
1> The form is visible,
2> The form is executing a function (is actively used),
3> There are references to this form by a global variable/array,
4> If the form has a separate foundset with edited records that can't be saved (for example autosave is false)

**Parameters**\
[String](JSLib/String.md) formName the name of the form to remove.

**Returns**\
[Boolean](JSLib/Boolean.md) true if successful


**Sample**

```javascript
var done = history.removeForm('mypreviousform');
```
### removeIndex(index)

Removes an absolute index based history stack form item.

**Parameters**\
[Number](JSLib/Number.md) index the index of the form to remove.

**Returns**\
[Boolean](JSLib/Boolean.md) true if successful


**Sample**

```javascript
var done = history.removeIndex(history.getCurrentIndex()+1);
```
### size()

Returns the total size of the history stack.


**Returns**\
[Number](JSLib/Number.md) the size


**Sample**

```javascript
var size = history.size();
```

