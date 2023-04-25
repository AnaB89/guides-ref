#  dialogs


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../../JSLib/String.md) | [showErrorDialog(dialogTitle, dialogMessage, buttonsText)](dialogs.md#showerrordialog-dialogtitle-dialogmessage-buttonstext)                   | Shows a message dialog with the specified title, message and a customizable set of buttons..                                    |
| [String](../../JSLib/String.md) | [showInfoDialog(dialogTitle, dialogMessage, buttonsText)](dialogs.md#showinfodialog-dialogtitle-dialogmessage-buttonstext)                   | Shows a message dialog with the specified title, message and a customizable set of buttons..                                    |
| [String](../../JSLib/String.md) | [showInputDialog()](dialogs.md#showinputdialog)                   | Shows an input dialog where the user can enter data..                                    |
| [String](../../JSLib/String.md) | [showInputDialog(dialog_title)](dialogs.md#showinputdialog-dialog_title)                   | Shows an input dialog where the user can enter data..                                    |
| [String](../../JSLib/String.md) | [showInputDialog(dialog_title, msg)](dialogs.md#showinputdialog-dialog_title-msg)                   | Shows an input dialog where the user can enter data..                                    |
| [String](../../JSLib/String.md) | [showInputDialog(dialog_title, msg, initialValue)](dialogs.md#showinputdialog-dialog_title-msg-initialvalue)                   | Shows an input dialog where the user can enter data..                                    |
| [String](../../JSLib/String.md) | [showQuestionDialog(dialogTitle, dialogMessage, buttonsText)](dialogs.md#showquestiondialog-dialogtitle-dialogmessage-buttonstext)                   | Shows a message dialog with the specified title, message and a customizable set of buttons..                                    |
| [String](../../JSLib/String.md) | [showSelectDialog(dialog_title, msg, optionArray)](dialogs.md#showselectdialog-dialog_title-msg-optionarray)                   | Shows a selection dialog, where the user can select an entry from a list of options..                                    |
| [String](../../JSLib/String.md) | [showSelectDialog(dialog_title, msg, options)](dialogs.md#showselectdialog-dialog_title-msg-options)                   | Shows a selection dialog, where the user can select an entry from a list of options..                                    |
| [String](../../JSLib/String.md) | [showWarningDialog(dialogTitle, dialogMessage, buttonsText)](dialogs.md#showwarningdialog-dialogtitle-dialogmessage-buttonstext)                   | Shows a message dialog with the specified title, message and a customizable set of buttons..                                    |

## Methods Details

### showErrorDialog(dialogTitle, dialogMessage, buttonsText)

Shows a message dialog with the specified title, message and a customizable set of buttons.
Returns pressed button text, in case window is closed without pressing any button return value depends on client type.

**Parameters**\
[String](../../JSLib/String.md) dialogTitle Dialog title.\
[String](../../JSLib/String.md) dialogMessage Dialog message.\
[Array](../../JSLib/Array.md) buttonsText variable arguments of button texts.

**Returns**\
[String](../../JSLib/String.md) pressed button text


**Sample**

```javascript
//show dialog
var thePressedButton = plugins.dialogs.showErrorDialog('Title', 'Value not allowed','OK', 'Cancel');
```
### showInfoDialog(dialogTitle, dialogMessage, buttonsText)

Shows a message dialog with the specified title, message and a customizable set of buttons.
Returns pressed button text, in case window is closed without pressing any button return value depends on client type.

**Parameters**\
[String](../../JSLib/String.md) dialogTitle Dialog title.\
[String](../../JSLib/String.md) dialogMessage Dialog message.\
[Array](../../JSLib/Array.md) buttonsText variable arguments of button texts.

**Returns**\
[String](../../JSLib/String.md) pressed button text


**Sample**

```javascript
//show dialog
var thePressedButton = plugins.dialogs.showInfoDialog('Title', 'Value not allowed','OK');
```
### showInputDialog()

Shows an input dialog where the user can enter data. Returns the entered data, or nothing when canceled.


**Returns**\
[String](../../JSLib/String.md) input text or null


**Sample**

```javascript
//show input dialog ,returns nothing when canceled
var typedInput = plugins.dialogs.showInputDialog('Specify','Your name');
```
### showInputDialog(dialog_title)

Shows an input dialog where the user can enter data. Returns the entered data, or nothing when canceled.

**Parameters**\
[String](../../JSLib/String.md) dialog_title  ;

**Returns**\
[String](../../JSLib/String.md) input text or null


**Sample**

```javascript
//show input dialog ,returns nothing when canceled
var typedInput = plugins.dialogs.showInputDialog('Specify','Your name');
```
### showInputDialog(dialog_title, msg)

Shows an input dialog where the user can enter data. Returns the entered data, or nothing when canceled.

**Parameters**\
[String](../../JSLib/String.md) dialog_title  ;\
[String](../../JSLib/String.md) msg  ;

**Returns**\
[String](../../JSLib/String.md) input text or null


**Sample**

```javascript
//show input dialog ,returns nothing when canceled
var typedInput = plugins.dialogs.showInputDialog('Specify','Your name');
```
### showInputDialog(dialog_title, msg, initialValue)

Shows an input dialog where the user can enter data. Returns the entered data, or nothing when canceled.

**Parameters**\
[String](../../JSLib/String.md) dialog_title  ;\
[String](../../JSLib/String.md) msg  ;\
[String](../../JSLib/String.md) initialValue  ;

**Returns**\
[String](../../JSLib/String.md) input text or null


**Sample**

```javascript
//show input dialog ,returns nothing when canceled
var typedInput = plugins.dialogs.showInputDialog('Specify','Your name');
```
### showQuestionDialog(dialogTitle, dialogMessage, buttonsText)

Shows a message dialog with the specified title, message and a customizable set of buttons.
Returns pressed button text, in case window is closed without pressing any button return value depends on client type.

**Parameters**\
[String](../../JSLib/String.md) dialogTitle Dialog title.\
[String](../../JSLib/String.md) dialogMessage Dialog message.\
[Array](../../JSLib/Array.md) buttonsText variable arguments of button texts.

**Returns**\
[String](../../JSLib/String.md) pressed button text


**Sample**

```javascript
//show dialog
var thePressedButton = plugins.dialogs.showQuestionDialog('Title', 'Value not allowed','OK', 'Cancel');
```
### showSelectDialog(dialog_title, msg, optionArray)

Shows a selection dialog, where the user can select an entry from a list of options. Returns the selected entry, or nothing when canceled.

**Parameters**\
[String](../../JSLib/String.md) dialog_title  ;\
[String](../../JSLib/String.md) msg  ;\
[Array](../../JSLib/Array.md) optionArray  ;

**Returns**\
[String](../../JSLib/String.md) selected value or null


**Sample**

```javascript
//show select,returns nothing when canceled
var selectedValue = plugins.dialogs.showSelectDialog('Select','please select a name','jan','johan','sebastiaan');
//also possible to pass array with options
//var selectedValue = plugins.dialogs.showSelectDialog('Select','please select a name', new Array('jan','johan','sebastiaan'));
```
### showSelectDialog(dialog_title, msg, options)

Shows a selection dialog, where the user can select an entry from a list of options. Returns the selected entry, or nothing when canceled.

**Parameters**\
[String](../../JSLib/String.md) dialog_title  ;\
[String](../../JSLib/String.md) msg  ;\
[Array](../../JSLib/Array.md) options  ;

**Returns**\
[String](../../JSLib/String.md) selected value or null


**Sample**

```javascript
//show select,returns nothing when canceled
var selectedValue = plugins.dialogs.showSelectDialog('Select','please select a name','jan','johan','sebastiaan');
//also possible to pass array with options
//var selectedValue = plugins.dialogs.showSelectDialog('Select','please select a name', new Array('jan','johan','sebastiaan'));
```
### showWarningDialog(dialogTitle, dialogMessage, buttonsText)

Shows a message dialog with the specified title, message and a customizable set of buttons.
Returns pressed button text, in case window is closed without pressing any button return value depends on client type.

**Parameters**\
[String](../../JSLib/String.md) dialogTitle Dialog title.\
[String](../../JSLib/String.md) dialogMessage Dialog message.\
[Array](../../JSLib/Array.md) buttonsText variable arguments of button texts.

**Returns**\
[String](../../JSLib/String.md) pressed button text


**Sample**

```javascript
//show dialog
var thePressedButton = plugins.dialogs.showWarningDialog('Title', 'Value not allowed','OK', 'Cancel');
```

