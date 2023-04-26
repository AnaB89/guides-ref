# JSWindow

## Constants Summary

| Type                          | Name                                       | Summary                                                                                                                                |
| ----------------------------- | ------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------- |
| [Number](../js-lib/number.md) | [DEFAULT](jswindow.md#DEFAULT)             | Value used for x, y, width, height of initial bounds when you want the window to auto-determine bounds when shown for the first time.. |
| [Number](../js-lib/number.md) | [DIALOG](jswindow.md#DIALOG)               | Window type constant that identifies a non-modal dialog type..                                                                         |
| [Number](../js-lib/number.md) | [FULL\_SCREEN](jswindow.md#FULL\_SCREEN)   | Value that can be used for bounds in order to specify that a dialog/window should completely fill the screen..                         |
| [Number](../js-lib/number.md) | [MODAL\_DIALOG](jswindow.md#MODAL\_DIALOG) | c Window type constant that identifies a modal dialog type..                                                                           |
| [Number](../js-lib/number.md) | [WINDOW](jswindow.md#WINDOW)               | Window type constant that identifies a window type..                                                                                   |

## Property Summary

| Type                                             | Name                                   | Summary                                                                                     |
| ------------------------------------------------ | -------------------------------------- | ------------------------------------------------------------------------------------------- |
| [controller](../forms/runtimeform/controller.md) | [controller](jswindow.md#controller)   | Get the current controller from the window/dialog..                                         |
| [Number](../js-lib/number.md)                    | [opacity](jswindow.md#opacity)         | Gets/Sets the opacity property..                                                            |
| [Boolean](../js-lib/boolean.md)                  | [resizable](jswindow.md#resizable)     | Gets/Sets whether or not this window can be resized by the user (default true)..            |
| [Boolean](../js-lib/boolean.md)                  | [storeBounds](jswindow.md#storeBounds) | Tells whether or not the bounds of this window should be stored/persisted (default false).. |
| [String](../js-lib/string.md)                    | [title](jswindow.md#title)             | Gets/Sets the title text..                                                                  |
| [Boolean](../js-lib/boolean.md)                  | [transparent](jswindow.md#transparent) | Gets/Sets the transparency property..                                                       |
| [Boolean](../js-lib/boolean.md)                  | [undecorated](jswindow.md#undecorated) | Gets/Sets the undecorated property..                                                        |

## Methods Summary

| Type                            | Name                                                                                   | Summary                                                                                                                     |
| ------------------------------- | -------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| void                            | [destroy()](jswindow.md#destroy)                                                       | Frees the resources allocated by this window..                                                                              |
| [Number](../js-lib/number.md)   | [getHeight()](jswindow.md#getheight)                                                   | Returns the height..                                                                                                        |
| [String](../js-lib/string.md)   | [getName()](jswindow.md#getname)                                                       | Returns the window name..                                                                                                   |
| [JSWindow](jswindow.md)         | [getParent()](jswindow.md#getparent)                                                   | Returns the parent JSWindow, if available..                                                                                 |
| [Number](../js-lib/number.md)   | [getType()](jswindow.md#gettype)                                                       | Returns the window type..                                                                                                   |
| [Number](../js-lib/number.md)   | [getWidth()](jswindow.md#getwidth)                                                     | Returns the width..                                                                                                         |
| [Number](../js-lib/number.md)   | [getX()](jswindow.md#getx)                                                             | Returns the x coordinate..                                                                                                  |
| [Number](../js-lib/number.md)   | [getY()](jswindow.md#gety)                                                             | Returns the y coordinate..                                                                                                  |
| [Boolean](../js-lib/boolean.md) | [hide()](jswindow.md#hide)                                                             | Hides the window..                                                                                                          |
| [Boolean](../js-lib/boolean.md) | [isVisible()](jswindow.md#isvisible)                                                   | Returns true if the window is visible, false otherwise..                                                                    |
| void                            | [resetBounds()](jswindow.md#resetbounds)                                               | Deletes the window's currently stored bounds..                                                                              |
| void                            | [setCSSClass(cssClassName)](jswindow.md#setcssclass-cssclassname)                      | Sets the dialog CSS class, can not be used to alter it when already showing, this should be set before the dialog is used.. |
| void                            | [setInitialBounds(x, y, width, height)](jswindow.md#setinitialbounds-x-y-width-height) | Sets the initial window bounds..                                                                                            |
| void                            | [setLocation(x, y)](jswindow.md#setlocation-x-y)                                       | Set the window location..                                                                                                   |
| void                            | [setSize(width, height)](jswindow.md#setsize-width-height)                             | Set the window size..                                                                                                       |
| void                            | [show(form)](jswindow.md#show-form)                                                    | Shows the given form(form name, form object or JSForm) in this window..                                                     |
| void                            | [showTextToolbar(showTextToolbar)](jswindow.md#showtexttoolbar-showtexttoolbar)        | Sets whether or not this window should have a text tool bar..                                                               |
| void                            | [toBack()](jswindow.md#toback)                                                         | Shows this window behind other windows, if possible..                                                                       |
| void                            | [toFront()](jswindow.md#tofront)                                                       | Bring this window in front of other windows, if possible..                                                                  |

## Constants Details

### DEFAULT

Value used for x, y, width, height of initial bounds when you want the window to auto-determine bounds when shown for the first time.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
// show a dialog that self-determines bounds the first time it it open, then remembers last bounds for future show operations
var win = application.createWindow("myName", JSWindow.DIALOG);
win.setInitialBounds(JSWindow.DEFAULT, JSWindow.DEFAULT, JSWindow.DEFAULT, JSWindow.DEFAULT); // will be shown initially centred and with preferred size
forms.myForm.show(win);
```

### DIALOG

Window type constant that identifies a non-modal dialog type. Non-modal dialogs will allow the user to interact with parent windows, but are less independent then windows with WINDOW type. Dialogs will stay on top of parent windows and are less accessible through the OS window manager. In web-client dialogs will not open in a separate browser window.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
// create a non-modal dialog on top of current active form's window and show a form inside it
var myWindow = application.createWindow("myName", JSWindow.DIALOG);
myWindow.show(forms.myForm);
```

### FULL\_SCREEN

Value that can be used for bounds in order to specify that a dialog/window should completely fill the screen.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
// create and show a window, with specified title, full screen
var win = application.createWindow("windowName", JSWindow.WINDOW);
win.setInitialBounds(JSWindow.FULL_SCREEN, JSWindow.FULL_SCREEN, JSWindow.FULL_SCREEN, JSWindow.FULL_SCREEN);
win.setTitle("This is a window");
controller.show(win);
```

### MODAL\_DIALOG

c Window type constant that identifies a modal dialog type. Modal dialogs will not allow the user to interact with the parent window(s) until closed. Dialogs will stay on top of parent windows and are less accessible through the OS window manager. In web-client dialogs will not open in a separate browser window. NOTE: no code is executed in Smart Client after a modal dialog is shown (the show operation blocks) until this dialog closes.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
// create a modal dialog on top of current active form's window and show a form inside it
var myWindow = application.createWindow("myName", JSWindow.MODAL_DIALOG);
myWindow.show(forms.myForm);
```

### WINDOW

Window type constant that identifies a window type. WINDOW type is the most independent type of window. It will be more accessible through the OS window manager, it can appear both in front of and under other windows and it doesn't block user interaction for other windows. In web-client windows will open in a separate browser window.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
// create a window and show a form inside it
var myWindow = application.createWindow("myName", JSWindow.WINDOW);
myWindow.show(forms.myForm);
```

## Properties Details

### controller

Get the current controller from the window/dialog.

**Returns**\
[controller](../forms/runtimeform/controller.md)

**Sample**

```javascript
var formName = application.getWindow('test').controller.getName();
```

### opacity

Gets/Sets the opacity property. By default will have value 1 (completely opaque), and can be assigned to values between 0 and 1. If set then window will also be undecorated. This should be set before the dialog/window is shown, otherwise it has no effect.

**Returns**\
[Number](../js-lib/number.md) the opacity of this window

**Sample**

```javascript
var someWindow = application.createWindow("someWindowName", JSWindow.WINDOW, null);
someWindow.setInitialBounds(200, 200, 450, 350);
controller.show(someWindow);

var name = "Name: " + someWindow.getName() + "\n"
var parent = "Parent: " + (someWindow.getParent() == null ? "none" : someWindow.getParent()) + "\n"
var type = "TypeNumber: " + someWindow.getType() + "\n"
var height = "Height: " + someWindow.getHeight() + "\n"
var width = "Width: " + someWindow.getWidth() + "\n"
var undecorated = "Undecorated: " + someWindow.isUndecorated() + "\n"
var opacity = "Opacity: " + someWindow.opacity + "\n"
var transparent = "Transparent: " + someWindow.transparent + "\n"
var locationX = "Location-X-coordinate: " + someWindow.getX() + "\n"
var locationY = "Location-Y-coordinate: " + someWindow.getY() + "\n"
var info = name + parent + type + height + width + locationX + locationY + undecorated + "\n"
var closeMsg = "Press 'Ok' to close this dialog."

var infoDialog = plugins.dialogs.showInfoDialog("Window Info", info + closeMsg, "Ok");
if (infoDialog == "Ok") someWindow.close()
```

### resizable

Gets/Sets whether or not this window can be resized by the user (default true).

**Returns**\
[Boolean](../js-lib/boolean.md)

**Sample**

```javascript
var someWindow = application.getWindow("someWindowName");
if (someWindow.isVisible() == false) {
	controller.show(someWindow);
	someWindow.resizable = false;
}
```

### storeBounds

Tells whether or not the bounds of this window should be stored/persisted (default false). If true, the window's bounds will be stored when the window is closed. Stored bounds will be used when the window is shown again instead of initialBounds. For non resizable windows, only location is stored/persisted.

**Returns**\
[Boolean](../js-lib/boolean.md)

**Sample**

```javascript
var win1 = application.createWindow("Window 1", JSWindow.DIALOG, null);
win1.setInitialBounds(200, 200, 450, 350);
win1.resizable = false;
win1.storeBounds = true;
win1.title = "Window 1";
controller.show(win1);
```

### title

Gets/Sets the title text.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var win1 = application.createWindow("Window 1", JSWindow.WINDOW, null);
win1.setInitialBounds(200, 200, 450, 350);
win1.title = "Window 1";
controller.show(win1);
```

### transparent

Gets/Sets the transparency property. NOTE: For smart clients, the window must be undecorated or the servoy.smartclient.allowLAFWindowDecoration property set to true

**Returns**\
[Boolean](../js-lib/boolean.md) transparency state of the window

**Sample**

```javascript
var someWindow = application.createWindow("someWindowName", JSWindow.WINDOW, null);
someWindow.setInitialBounds(200, 200, 450, 350);
controller.show(someWindow);

var name = "Name: " + someWindow.getName() + "\n"
var parent = "Parent: " + (someWindow.getParent() == null ? "none" : someWindow.getParent()) + "\n"
var type = "TypeNumber: " + someWindow.getType() + "\n"
var height = "Height: " + someWindow.getHeight() + "\n"
var width = "Width: " + someWindow.getWidth() + "\n"
var undecorated = "Undecorated: " + someWindow.isUndecorated() + "\n"
var opacity = "Opacity: " + someWindow.opacity + "\n"
var transparent = "Transparent: " + someWindow.transparent + "\n"
var locationX = "Location-X-coordinate: " + someWindow.getX() + "\n"
var locationY = "Location-Y-coordinate: " + someWindow.getY() + "\n"
var info = name + parent + type + height + width + locationX + locationY + undecorated + "\n"
var closeMsg = "Press 'Ok' to close this dialog."

var infoDialog = plugins.dialogs.showInfoDialog("Window Info", info + closeMsg, "Ok");
if (infoDialog == "Ok") someWindow.close()
```

### undecorated

Gets/Sets the undecorated property. If set then this window will not have any decoration and can't be moved/resized or closed. This should be set before dialog/window is shown, otherwise has no effect.

**Returns**\
[Boolean](../js-lib/boolean.md) if this window will be undecorated

**Sample**

```javascript
var someWindow = application.createWindow("someWindowName", JSWindow.WINDOW, null);
someWindow.setInitialBounds(200, 200, 450, 350);
controller.show(someWindow);

var name = "Name: " + someWindow.getName() + "\n"
var parent = "Parent: " + (someWindow.getParent() == null ? "none" : someWindow.getParent()) + "\n"
var type = "TypeNumber: " + someWindow.getType() + "\n"
var height = "Height: " + someWindow.getHeight() + "\n"
var width = "Width: " + someWindow.getWidth() + "\n"
var undecorated = "Undecorated: " + someWindow.isUndecorated() + "\n"
var opacity = "Opacity: " + someWindow.opacity + "\n"
var transparent = "Transparent: " + someWindow.transparent + "\n"
var locationX = "Location-X-coordinate: " + someWindow.getX() + "\n"
var locationY = "Location-Y-coordinate: " + someWindow.getY() + "\n"
var info = name + parent + type + height + width + locationX + locationY + undecorated + "\n"
var closeMsg = "Press 'Ok' to close this dialog."

var infoDialog = plugins.dialogs.showInfoDialog("Window Info", info + closeMsg, "Ok");
if (infoDialog == "Ok") someWindow.close()
```

## Methods Details

### destroy()

Frees the resources allocated by this window. If window is visible, it will close it first. The window will no longer be available with application.getWindow('windowName') and will no longer be usable.

The main application window cannot be destroyed.

**Returns**\
void

**Sample**

```javascript
var getWindow = application.getWindow("someWindowName");
getWindow.destroy();
getWindow = application.getWindow("someWindowName");
if (getWindow == null) {
	application.output("Window has been destroyed");
} else {
	application.output("Window could not be destroyed");
}
```

### getHeight()

Returns the height.

**Returns**\
[Number](../js-lib/number.md) the height.

**Sample**

```javascript
var someWindow = application.createWindow("someWindowName", JSWindow.WINDOW, null);
someWindow.setInitialBounds(200, 200, 450, 350);
controller.show(someWindow);

var name = "Name: " + someWindow.getName() + "\n"
var parent = "Parent: " + (someWindow.getParent() == null ? "none" : someWindow.getParent()) + "\n"
var type = "TypeNumber: " + someWindow.getType() + "\n"
var height = "Height: " + someWindow.getHeight() + "\n"
var width = "Width: " + someWindow.getWidth() + "\n"
var undecorated = "Undecorated: " + someWindow.isUndecorated() + "\n"
var opacity = "Opacity: " + someWindow.opacity + "\n"
var transparent = "Transparent: " + someWindow.transparent + "\n"
var locationX = "Location-X-coordinate: " + someWindow.getX() + "\n"
var locationY = "Location-Y-coordinate: " + someWindow.getY() + "\n"
var info = name + parent + type + height + width + locationX + locationY + undecorated + "\n"
var closeMsg = "Press 'Ok' to close this dialog."

var infoDialog = plugins.dialogs.showInfoDialog("Window Info", info + closeMsg, "Ok");
if (infoDialog == "Ok") someWindow.close()
```

### getName()

Returns the window name. It will be null in case of main application frame.

**Returns**\
[String](../js-lib/string.md) the window name.

**Sample**

```javascript
var someWindow = application.createWindow("someWindowName", JSWindow.WINDOW, null);
someWindow.setInitialBounds(200, 200, 450, 350);
controller.show(someWindow);

var name = "Name: " + someWindow.getName() + "\n"
var parent = "Parent: " + (someWindow.getParent() == null ? "none" : someWindow.getParent()) + "\n"
var type = "TypeNumber: " + someWindow.getType() + "\n"
var height = "Height: " + someWindow.getHeight() + "\n"
var width = "Width: " + someWindow.getWidth() + "\n"
var undecorated = "Undecorated: " + someWindow.isUndecorated() + "\n"
var opacity = "Opacity: " + someWindow.opacity + "\n"
var transparent = "Transparent: " + someWindow.transparent + "\n"
var locationX = "Location-X-coordinate: " + someWindow.getX() + "\n"
var locationY = "Location-Y-coordinate: " + someWindow.getY() + "\n"
var info = name + parent + type + height + width + locationX + locationY + undecorated + "\n"
var closeMsg = "Press 'Ok' to close this dialog."

var infoDialog = plugins.dialogs.showInfoDialog("Window Info", info + closeMsg, "Ok");
if (infoDialog == "Ok") someWindow.close()
```

### getParent()

Returns the parent JSWindow, if available.

**Returns**\
[JSWindow](jswindow.md) the parent JSWindow, if available. If there is no parent JSWindow, it will return null.

**Sample**

```javascript
var someWindow = application.createWindow("someWindowName", JSWindow.WINDOW, null);
someWindow.setInitialBounds(200, 200, 450, 350);
controller.show(someWindow);

var name = "Name: " + someWindow.getName() + "\n"
var parent = "Parent: " + (someWindow.getParent() == null ? "none" : someWindow.getParent()) + "\n"
var type = "TypeNumber: " + someWindow.getType() + "\n"
var height = "Height: " + someWindow.getHeight() + "\n"
var width = "Width: " + someWindow.getWidth() + "\n"
var undecorated = "Undecorated: " + someWindow.isUndecorated() + "\n"
var opacity = "Opacity: " + someWindow.opacity + "\n"
var transparent = "Transparent: " + someWindow.transparent + "\n"
var locationX = "Location-X-coordinate: " + someWindow.getX() + "\n"
var locationY = "Location-Y-coordinate: " + someWindow.getY() + "\n"
var info = name + parent + type + height + width + locationX + locationY + undecorated + "\n"
var closeMsg = "Press 'Ok' to close this dialog."

var infoDialog = plugins.dialogs.showInfoDialog("Window Info", info + closeMsg, "Ok");
if (infoDialog == "Ok") someWindow.close()
```

### getType()

Returns the window type.

**Returns**\
[Number](../js-lib/number.md) the window type. Can be one of JSWindow.DIALOG, JSWindow.MODAL\_DIALOG, JSWindow.WINDOW.

**Sample**

```javascript
var someWindow = application.createWindow("someWindowName", JSWindow.WINDOW, null);
someWindow.setInitialBounds(200, 200, 450, 350);
controller.show(someWindow);

var name = "Name: " + someWindow.getName() + "\n"
var parent = "Parent: " + (someWindow.getParent() == null ? "none" : someWindow.getParent()) + "\n"
var type = "TypeNumber: " + someWindow.getType() + "\n"
var height = "Height: " + someWindow.getHeight() + "\n"
var width = "Width: " + someWindow.getWidth() + "\n"
var undecorated = "Undecorated: " + someWindow.isUndecorated() + "\n"
var opacity = "Opacity: " + someWindow.opacity + "\n"
var transparent = "Transparent: " + someWindow.transparent + "\n"
var locationX = "Location-X-coordinate: " + someWindow.getX() + "\n"
var locationY = "Location-Y-coordinate: " + someWindow.getY() + "\n"
var info = name + parent + type + height + width + locationX + locationY + undecorated + "\n"
var closeMsg = "Press 'Ok' to close this dialog."

var infoDialog = plugins.dialogs.showInfoDialog("Window Info", info + closeMsg, "Ok");
if (infoDialog == "Ok") someWindow.close()
```

### getWidth()

Returns the width.

**Returns**\
[Number](../js-lib/number.md) the width.

**Sample**

```javascript
var someWindow = application.createWindow("someWindowName", JSWindow.WINDOW, null);
someWindow.setInitialBounds(200, 200, 450, 350);
controller.show(someWindow);

var name = "Name: " + someWindow.getName() + "\n"
var parent = "Parent: " + (someWindow.getParent() == null ? "none" : someWindow.getParent()) + "\n"
var type = "TypeNumber: " + someWindow.getType() + "\n"
var height = "Height: " + someWindow.getHeight() + "\n"
var width = "Width: " + someWindow.getWidth() + "\n"
var undecorated = "Undecorated: " + someWindow.isUndecorated() + "\n"
var opacity = "Opacity: " + someWindow.opacity + "\n"
var transparent = "Transparent: " + someWindow.transparent + "\n"
var locationX = "Location-X-coordinate: " + someWindow.getX() + "\n"
var locationY = "Location-Y-coordinate: " + someWindow.getY() + "\n"
var info = name + parent + type + height + width + locationX + locationY + undecorated + "\n"
var closeMsg = "Press 'Ok' to close this dialog."

var infoDialog = plugins.dialogs.showInfoDialog("Window Info", info + closeMsg, "Ok");
if (infoDialog == "Ok") someWindow.close()
```

### getX()

Returns the x coordinate.

**Returns**\
[Number](../js-lib/number.md) the x coordinate.

**Sample**

```javascript
var someWindow = application.createWindow("someWindowName", JSWindow.WINDOW, null);
someWindow.setInitialBounds(200, 200, 450, 350);
controller.show(someWindow);

var name = "Name: " + someWindow.getName() + "\n"
var parent = "Parent: " + (someWindow.getParent() == null ? "none" : someWindow.getParent()) + "\n"
var type = "TypeNumber: " + someWindow.getType() + "\n"
var height = "Height: " + someWindow.getHeight() + "\n"
var width = "Width: " + someWindow.getWidth() + "\n"
var undecorated = "Undecorated: " + someWindow.isUndecorated() + "\n"
var opacity = "Opacity: " + someWindow.opacity + "\n"
var transparent = "Transparent: " + someWindow.transparent + "\n"
var locationX = "Location-X-coordinate: " + someWindow.getX() + "\n"
var locationY = "Location-Y-coordinate: " + someWindow.getY() + "\n"
var info = name + parent + type + height + width + locationX + locationY + undecorated + "\n"
var closeMsg = "Press 'Ok' to close this dialog."

var infoDialog = plugins.dialogs.showInfoDialog("Window Info", info + closeMsg, "Ok");
if (infoDialog == "Ok") someWindow.close()
```

### getY()

Returns the y coordinate.

**Returns**\
[Number](../js-lib/number.md) the y coordinate.

**Sample**

```javascript
var someWindow = application.createWindow("someWindowName", JSWindow.WINDOW, null);
someWindow.setInitialBounds(200, 200, 450, 350);
controller.show(someWindow);

var name = "Name: " + someWindow.getName() + "\n"
var parent = "Parent: " + (someWindow.getParent() == null ? "none" : someWindow.getParent()) + "\n"
var type = "TypeNumber: " + someWindow.getType() + "\n"
var height = "Height: " + someWindow.getHeight() + "\n"
var width = "Width: " + someWindow.getWidth() + "\n"
var undecorated = "Undecorated: " + someWindow.isUndecorated() + "\n"
var opacity = "Opacity: " + someWindow.opacity + "\n"
var transparent = "Transparent: " + someWindow.transparent + "\n"
var locationX = "Location-X-coordinate: " + someWindow.getX() + "\n"
var locationY = "Location-Y-coordinate: " + someWindow.getY() + "\n"
var info = name + parent + type + height + width + locationX + locationY + undecorated + "\n"
var closeMsg = "Press 'Ok' to close this dialog."

var infoDialog = plugins.dialogs.showInfoDialog("Window Info", info + closeMsg, "Ok");
if (infoDialog == "Ok") someWindow.close()
```

### hide()

Hides the window. It can be shown again using window.show(), controller.show() or controller.showRecords(). The main application window cannot be hidden.

**Returns**\
[Boolean](../js-lib/boolean.md) Boolean true if the window was successfully closed and false otherwise.

**Sample**

```javascript
//creates and shows a window for 3 seconds before closing it
var win = application.createWindow("someWindowName", JSWindow.WINDOW, null);
win.setInitialBounds(200, 200, 450, 350);
controller.show(win);
application.sleep(3000);
win.hide();
```

### isVisible()

Returns true if the window is visible, false otherwise.

**Returns**\
[Boolean](../js-lib/boolean.md) true if the window is visible, false otherwise.

**Sample**

```javascript
var someWindow = application.getWindow("someWindowName");
if (someWindow.isVisible() == false) {
	controller.show(someWindow);
	someWindow.resizable = false;
}
```

### resetBounds()

Deletes the window's currently stored bounds. It will only affect the next show of the window.

**Returns**\
void

**Sample**

```javascript
var win1 = application.createWindow("Window 1", JSWindow.DIALOG, null);
win1.title = "Window 1";
win1.setInitialBounds(200, 200, 400, 600);
win1.storeBounds = true;
if (newSolutionVersion) win1.resetBounds();
win1.show(forms.myform);
```

### setCSSClass(cssClassName)

Sets the dialog CSS class, can not be used to alter it when already showing, this should be set before the dialog is used. See sample code for examples of CSS classes for display customizations

**Parameters**\
[String](../js-lib/string.md) cssClassName CSS class name

**Returns**\
void

**Sample**

```javascript
// Here are some examples of a classes for customizing the display of the window

//	.myDlgCSS {
//		border-radius: initial; // show edged dialog corners
//		-webkit-box-shadow: 0 5px 15px rgba(0,0,0,.0); // hide dialog box shadow
//		box-shadow: 0 5px 15px rgba(0,0,0,.0); // hide dialog box shadow
//	}
//
//	// dialog header styling
//	.myDlgCSS .window-header {
//		background: green;
//	}
//
//	// style/hide dialog close button
//	.myDlgCSS .window-header .svy-dialog-close {
//		display: none;
//	}
//
//	// dialog body styling
//	.myDlgCSS .window-body {
//		background: yellow;
//	}
//
//	// dialog footer styling/hiding
//	.myDlgCSS .window-footer {
//		background: blue;
//		display: none !important;
//	}

var win = application.createWindow("myName", JSWindow.DIALOG);
win.setCSSClass('myDlgCSS');
```

### setInitialBounds(x, y, width, height)

Sets the initial window bounds. The initial bounds are only used the first time this window is shown (what first show means depends on storeBounds property).

**Parameters**\
[Number](../js-lib/number.md) x the initial x coordinate of the window. Can be JSWindow.DEFAULT, JSWindow.FULL\_SCREEN.\
[Number](../js-lib/number.md) y the initial y coordinate of the window. Can be JSWindow.DEFAULT, JSWindow.FULL\_SCREEN.\
[Number](../js-lib/number.md) width the initial width of the window. Can be JSWindow.DEFAULT, JSWindow.FULL\_SCREEN.\
[Number](../js-lib/number.md) height the initial height of the window. Can be JSWindow.DEFAULT, JSWindow.FULL\_SCREEN.

**Returns**\
void

**Sample**

```javascript
var win = application.createWindow("myName", JSWindow.DIALOG);
win.setInitialBounds(20, 10, 300, 200);
forms.myForm.show(win);
```

### setLocation(x, y)

Set the window location. If the coordinates are not valid they might be corrected. (for example out of screen locations)

**Parameters**\
[Number](../js-lib/number.md) x x coordinate.\
[Number](../js-lib/number.md) y y coordinate.

**Returns**\
void

**Sample**

```javascript
var window = application.createWindow('test',JSWindow.DIALOG);
window.setLocation(0,0);
window.setSize(400,600);
window.show(forms.child1);
```

### setSize(width, height)

Set the window size.

**Parameters**\
[Number](../js-lib/number.md) width the width.\
[Number](../js-lib/number.md) height the height.

**Returns**\
void

**Sample**

```javascript
var window = application.createWindow('test',JSWindow.DIALOG);
window.setLocation(0,0);
window.setSize(400,600);
window.show(forms.child1);
```

### show(form)

Shows the given form(form name, form object or JSForm) in this window.

**Parameters**\
[Object](../js-lib/object.md) form the form that will be shown inside this window. It can be a form name or a form object (actual form or JSForm).

**Returns**\
void

**Sample**

```javascript
win.show(forms.myForm);
// win.show("myForm");
```

### showTextToolbar(showTextToolbar)

Sets whether or not this window should have a text tool bar. Has no effect on web client or smart client main application frame.

**Parameters**\
[Boolean](../js-lib/boolean.md) showTextToolbar true if you want a text tool bar to be added to this window, false otherwise.

**Returns**\
void

**Sample**

```javascript
var win1 = application.createWindow("Window 1", JSWindow.WINDOW, null);
win1.setInitialBounds(200, 200, 450, 350);
win1.setTitle("Window 1");
win1.showTextToolbar(false);
controller.show(win1);

var win2 = application.createWindow("Window 2", JSWindow.WINDOW, null);
win2.setInitialBounds(500, 500, 450, 350);
win2.setTitle("Window 2");
win2.showTextToolbar(false);
controller.show(win2);

var win3 = application.createWindow("Window 3", JSWindow.WINDOW, null);
win3.setInitialBounds(650, 700, 450, 350);
win3.setTitle("Window 3");
win3.showTextToolbar(true);
controller.show(win3);

application.sleep(2000);
win3.toBack();
application.sleep(2000);
win1.toFront();
```

### toBack()

Shows this window behind other windows, if possible.

**Returns**\
void

**Sample**

```javascript
var win1 = application.createWindow("Window 1", JSWindow.WINDOW, null);
win1.setInitialBounds(200, 200, 450, 350);
win1.setTitle("Window 1");
win1.showTextToolbar(false);
controller.show(win1);

var win2 = application.createWindow("Window 2", JSWindow.WINDOW, null);
win2.setInitialBounds(500, 500, 450, 350);
win2.setTitle("Window 2");
win2.showTextToolbar(false);
controller.show(win2);

var win3 = application.createWindow("Window 3", JSWindow.WINDOW, null);
win3.setInitialBounds(650, 700, 450, 350);
win3.setTitle("Window 3");
win3.showTextToolbar(true);
controller.show(win3);

application.sleep(2000);
win3.toBack();
application.sleep(2000);
win1.toFront();
```

### toFront()

Bring this window in front of other windows, if possible.

**Returns**\
void

**Sample**

```javascript
var win1 = application.createWindow("Window 1", JSWindow.WINDOW, null);
win1.setInitialBounds(200, 200, 450, 350);
win1.setTitle("Window 1");
win1.showTextToolbar(false);
controller.show(win1);

var win2 = application.createWindow("Window 2", JSWindow.WINDOW, null);
win2.setInitialBounds(500, 500, 450, 350);
win2.setTitle("Window 2");
win2.showTextToolbar(false);
controller.show(win2);

var win3 = application.createWindow("Window 3", JSWindow.WINDOW, null);
win3.setInitialBounds(650, 700, 450, 350);
win3.setTitle("Window 3");
win3.showTextToolbar(true);
controller.show(win3);

application.sleep(2000);
win3.toBack();
application.sleep(2000);
win1.toFront();
```
