#  window

## **Return Types**
[Menu](./Menu.md),[RadioButton](./RadioButton.md),[CheckBox](./CheckBox.md),[FormPopup](./FormPopup.md),[MenuItem](./MenuItem.md),[Popup](./Popup.md),[ToolBar](./ToolBar.md),[MenuBar](./MenuBar.md),
## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [ToolBar](./ToolBar.md) | [addToolBar(window, name)](window.md#addtoolbar-window-name)                   | Creates and returns a toolbar for a specific window..                                    |
| [ToolBar](./ToolBar.md) | [addToolBar(window, name, row)](window.md#addtoolbar-window-name-row)                   | Creates and returns a toolbar for a specific window..                                    |
| [ToolBar](./ToolBar.md) | [addToolBar(window, name, displayname)](window.md#addtoolbar-window-name-displayname)                   | Creates and returns a toolbar for a specific window..                                    |
| [ToolBar](./ToolBar.md) | [addToolBar(window, name, displayname, row)](window.md#addtoolbar-window-name-displayname-row)                   | Creates and returns a toolbar for a specific window..                                    |
| [ToolBar](./ToolBar.md) | [addToolBar(name)](window.md#addtoolbar-name)                   | Add a toolbar..                                    |
| [ToolBar](./ToolBar.md) | [addToolBar(name, row)](window.md#addtoolbar-name-row)                   | Add a toolbar..                                    |
| [ToolBar](./ToolBar.md) | [addToolBar(name, displayname)](window.md#addtoolbar-name-displayname)                   | Add a toolbar..                                    |
| [ToolBar](./ToolBar.md) | [addToolBar(name, displayname, row)](window.md#addtoolbar-name-displayname-row)                   | Add a toolbar..                                    |
|void | [cancelFormPopup()](window.md#cancelformpopup)                   | Close the current form popup panel without assigning a value to the configured data provider..                                    |
|void | [closeFormPopup(retval)](window.md#closeformpopup-retval)                   | Close the current form popup panel and assign the value to the configured data provider..                                    |
| [FormPopup](./FormPopup.md) | [createFormPopup(form)](window.md#createformpopup-form)                   | Create a form popup that can be filled with data and shown..                                    |
| [Popup](./Popup.md) | [createPopupMenu()](window.md#createpopupmenu)                   | Creates a new popup menu that can be populated with items and displayed..                                    |
| [Boolean](../../JSLib/Boolean.md) | [createShortcut(shortcut, methodName)](window.md#createshortcut-shortcut-methodname)                   | Create a shortcut..                                    |
| [Boolean](../../JSLib/Boolean.md) | [createShortcut(shortcut, methodName, arguments)](window.md#createshortcut-shortcut-methodname-arguments)                   | Create a shortcut..                                    |
| [Boolean](../../JSLib/Boolean.md) | [createShortcut(shortcut, methodName, contextFilter)](window.md#createshortcut-shortcut-methodname-contextfilter)                   | Create a shortcut..                                    |
| [Boolean](../../JSLib/Boolean.md) | [createShortcut(shortcut, method, contextFilter, arguments)](window.md#createshortcut-shortcut-method-contextfilter-arguments)                   | Create a shortcut..                                    |
| [Boolean](../../JSLib/Boolean.md) | [createShortcut(shortcut, methodName, contextFilter, arguments, consumeEvent)](window.md#createshortcut-shortcut-methodname-contextfilter-arguments-consumeevent)                   | Create a shortcut..                                    |
| [Boolean](../../JSLib/Boolean.md) | [createShortcut(shortcut, method)](window.md#createshortcut-shortcut-method)                   | Create a shortcut..                                    |
| [Boolean](../../JSLib/Boolean.md) | [createShortcut(shortcut, method, arguments)](window.md#createshortcut-shortcut-method-arguments)                   | Create a shortcut..                                    |
| [Boolean](../../JSLib/Boolean.md) | [createShortcut(shortcut, method, contextFilter)](window.md#createshortcut-shortcut-method-contextfilter)                   | Create a shortcut..                                    |
| [Boolean](../../JSLib/Boolean.md) | [createShortcut(shortcut, method, contextFilter, arguments)](window.md#createshortcut-shortcut-method-contextfilter-arguments)                   | Create a shortcut..                                    |
| [Boolean](../../JSLib/Boolean.md) | [createShortcut(shortcut, method, contextFilter, arguments, consumeEvent)](window.md#createshortcut-shortcut-method-contextfilter-arguments-consumeevent)                   | Create a shortcut..                                    |
| [MenuBar](./MenuBar.md) | [getMenuBar()](window.md#getmenubar)                   | Get the menubar of the main window, or of a named window..                                    |
| [MenuBar](./MenuBar.md) | [getMenuBar(windowName)](window.md#getmenubar-windowname)                   | Get the menubar of the main window, or of a named window..                                    |
| [ToolBar](./ToolBar.md) | [getToolBar(window, name)](window.md#gettoolbar-window-name)                   | Get the toolbar of a specific window from the toolbar panel by name..                                    |
| [ToolBar](./ToolBar.md) | [getToolBar(name)](window.md#gettoolbar-name)                   | Get the toolbar from the toolbar panel by name..                                    |
| [Array](../../JSLib/Array.md) | [getToolbarNames()](window.md#gettoolbarnames)                   | Get all toolbar names from the toolbar panel..                                    |
| [Array](../../JSLib/Array.md) | [getToolbarNames(window)](window.md#gettoolbarnames-window)                   | Get all toolbar names from the toolbar panel of a specific window..                                    |
|void | [maximize()](window.md#maximize)                   | Maximize the current window or the window with the specified name (Smart client only)..                                    |
|void | [maximize(windowName)](window.md#maximize-windowname)                   | Maximize the current window or the window with the specified name (Smart client only)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [removeShortcut(shortcut)](window.md#removeshortcut-shortcut)                   | Remove a shortcut..                                    |
| [Boolean](../../JSLib/Boolean.md) | [removeShortcut(shortcut, contextFilter)](window.md#removeshortcut-shortcut-contextfilter)                   | Remove a shortcut..                                    |
|void | [removeToolBar(window, name)](window.md#removetoolbar-window-name)                   | Remove the toolbar from the toolbar panel of a specific window..                                    |
|void | [removeToolBar(name)](window.md#removetoolbar-name)                   | Remove the toolbar from the toolbar panel..                                    |
|void | [setFullScreen(full)](window.md#setfullscreen-full)                   | Bring the window into/out of fullsceen mode..                                    |
|void | [setStatusBarVisible(visible)](window.md#setstatusbarvisible-visible)                   | Show or hide the statusbar..                                    |
|void | [setToolBarAreaVisible(visible)](window.md#settoolbarareavisible-visible)                   | Show or hide the toolbar area..                                    |
|void | [showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID)](window.md#showformpopup-elementtoshowrelatedto-form-scope-dataproviderid)                   | Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope..                                    |
|void | [showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID, width, height)](window.md#showformpopup-elementtoshowrelatedto-form-scope-dataproviderid-width-height)                   | Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope..                                    |
|void | [showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID, width, height, x, y)](window.md#showformpopup-elementtoshowrelatedto-form-scope-dataproviderid-width-height-x-y)                   | Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope..                                    |
|void | [showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID, width, height, x, y, showBackdrop)](window.md#showformpopup-elementtoshowrelatedto-form-scope-dataproviderid-width-height-x-y-showbackdrop)                   | Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope..                                    |
|void | [showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID, width, height, x, y, showBackdrop, doNotCloseOnClickOutside)](window.md#showformpopup-elementtoshowrelatedto-form-scope-dataproviderid-width-height-x-y-showbackdrop-donotcloseonclickoutside)                   | Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope..                                    |
|void | [showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID, width, height, x, y, showBackdrop, doNotCloseOnClickOutside, onClose)](window.md#showformpopup-elementtoshowrelatedto-form-scope-dataproviderid-width-height-x-y-showbackdrop-donotcloseonclickoutside-onclose)                   | Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope..                                    |

## Methods Details

### addToolBar(window, name)

Creates and returns a toolbar for a specific window.

**Parameters**\
[JSWindow](../../Application/JSWindow.md) window  ;\
[String](../../JSLib/String.md) name the name by which this toolbar is identified in code. If display name is missing, name will be used as displayName as well.

**Returns**\
[ToolBar](./ToolBar.md) 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// Note: method addToolBar only works in the smart client.

// create a window
var win = application.createWindow("myWindow", JSWindow.WINDOW);

// add a toolbar with only a name
var toolbar0 = plugins.window.addToolBar(win,"toolbar_0");
toolbar0.addButton("click me 0", callback_function);

// add a toolbar with a name and the row you want it to show at
// row number starts at 0
var toolbar1 = plugins.window.addToolBar(win,"toolbar_1", 2);
toolbar1.addButton("click me 1", callback_function);

// add a toolbar with a name and display name
var toolbar2 = plugins.window.addToolBar(win,"toolbar_2", "toolbar_2_internal_name");
toolbar2.addButton("click me 2", callback_function);

// add a toolbar with a name, display name and the row you want the
// toolbar to show at. row number starts at 0
var toolbar3 = plugins.window.addToolBar(win,"toolbar_3", "toolbar_3_internal_name", 3);
toolbar3.addButton("click me 3", callback_function);

win.show(forms.Myform)
```
### addToolBar(window, name, row)

Creates and returns a toolbar for a specific window.

**Parameters**\
[JSWindow](../../Application/JSWindow.md) window  ;\
[String](../../JSLib/String.md) name the name by which this toolbar is identified in code. If display name is missing, name will be used as displayName as well.\
[Number](../../JSLib/Number.md) row the row inside the toolbar panel where this toolbar is to be added.

**Returns**\
[ToolBar](./ToolBar.md) 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// Note: method addToolBar only works in the smart client.

// create a window
var win = application.createWindow("myWindow", JSWindow.WINDOW);

// add a toolbar with only a name
var toolbar0 = plugins.window.addToolBar(win,"toolbar_0");
toolbar0.addButton("click me 0", callback_function);

// add a toolbar with a name and the row you want it to show at
// row number starts at 0
var toolbar1 = plugins.window.addToolBar(win,"toolbar_1", 2);
toolbar1.addButton("click me 1", callback_function);

// add a toolbar with a name and display name
var toolbar2 = plugins.window.addToolBar(win,"toolbar_2", "toolbar_2_internal_name");
toolbar2.addButton("click me 2", callback_function);

// add a toolbar with a name, display name and the row you want the
// toolbar to show at. row number starts at 0
var toolbar3 = plugins.window.addToolBar(win,"toolbar_3", "toolbar_3_internal_name", 3);
toolbar3.addButton("click me 3", callback_function);

win.show(forms.Myform)
```
### addToolBar(window, name, displayname)

Creates and returns a toolbar for a specific window.

**Parameters**\
[JSWindow](../../Application/JSWindow.md) window  ;\
[String](../../JSLib/String.md) name the name by which this toolbar is identified in code\
[String](../../JSLib/String.md) displayname the name by which this toolbar will be identified in the UI. (for example in the toolbar panel's context menu)

**Returns**\
[ToolBar](./ToolBar.md) 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// Note: method addToolBar only works in the smart client.

// create a window
var win = application.createWindow("myWindow", JSWindow.WINDOW);

// add a toolbar with only a name
var toolbar0 = plugins.window.addToolBar(win,"toolbar_0");
toolbar0.addButton("click me 0", callback_function);

// add a toolbar with a name and the row you want it to show at
// row number starts at 0
var toolbar1 = plugins.window.addToolBar(win,"toolbar_1", 2);
toolbar1.addButton("click me 1", callback_function);

// add a toolbar with a name and display name
var toolbar2 = plugins.window.addToolBar(win,"toolbar_2", "toolbar_2_internal_name");
toolbar2.addButton("click me 2", callback_function);

// add a toolbar with a name, display name and the row you want the
// toolbar to show at. row number starts at 0
var toolbar3 = plugins.window.addToolBar(win,"toolbar_3", "toolbar_3_internal_name", 3);
toolbar3.addButton("click me 3", callback_function);

win.show(forms.Myform)
```
### addToolBar(window, name, displayname, row)

Creates and returns a toolbar for a specific window.

**Parameters**\
[JSWindow](../../Application/JSWindow.md) window  ;\
[String](../../JSLib/String.md) name the name by which this toolbar is identified in code.\
[String](../../JSLib/String.md) displayname the name by which this toolbar will be identified in the UI. (for example in the toolbar panel's context menu)\
[Number](../../JSLib/Number.md) row the row inside the toolbar panel where this toolbar is to be added.

**Returns**\
[ToolBar](./ToolBar.md) 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// Note: method addToolBar only works in the smart client.

// create a window
var win = application.createWindow("myWindow", JSWindow.WINDOW);

// add a toolbar with only a name
var toolbar0 = plugins.window.addToolBar(win,"toolbar_0");
toolbar0.addButton("click me 0", callback_function);

// add a toolbar with a name and the row you want it to show at
// row number starts at 0
var toolbar1 = plugins.window.addToolBar(win,"toolbar_1", 2);
toolbar1.addButton("click me 1", callback_function);

// add a toolbar with a name and display name
var toolbar2 = plugins.window.addToolBar(win,"toolbar_2", "toolbar_2_internal_name");
toolbar2.addButton("click me 2", callback_function);

// add a toolbar with a name, display name and the row you want the
// toolbar to show at. row number starts at 0
var toolbar3 = plugins.window.addToolBar(win,"toolbar_3", "toolbar_3_internal_name", 3);
toolbar3.addButton("click me 3", callback_function);

win.show(forms.Myform)
```
### addToolBar(name)

Add a toolbar.

**Parameters**\
[String](../../JSLib/String.md) name the name by which this toolbar is identified in code. If display name is missing, name will be used as displayName as well.

**Returns**\
[ToolBar](./ToolBar.md) 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// Note: method addToolBar only works in the smart client.

// add a toolbar with only a name
var toolbar0 = plugins.window.addToolBar("toolbar_0");
toolbar0.addButton("click me 0", feedback_button);

// add a toolbar with a name and the row you want it to show at
// row number starts at 0
var toolbar1 = plugins.window.addToolBar("toolbar_1", 2);
toolbar1.addButton("click me 1", feedback_button);

// add a toolbar with a name and display name
var toolbar2 = plugins.window.addToolBar("toolbar_2", "toolbar_2_internal_name");
toolbar2.addButton("click me 2", feedback_button);

// add a toolbar with a name, display name and the row you want the
// toolbar to show at. row number starts at 0
var toolbar3 = plugins.window.addToolBar("toolbar_3", "toolbar_3_internal_name", 3);
toolbar3.addButton("click me 3", feedback_button);
```
### addToolBar(name, row)

Add a toolbar.

**Parameters**\
[String](../../JSLib/String.md) name the name by which this toolbar is identified in code. If display name is missing, name will be used as displayName as well.\
[Number](../../JSLib/Number.md) row the row inside the toolbar panel where this toolbar is to be added.

**Returns**\
[ToolBar](./ToolBar.md) 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// Note: method addToolBar only works in the smart client.

// add a toolbar with only a name
var toolbar0 = plugins.window.addToolBar("toolbar_0");
toolbar0.addButton("click me 0", feedback_button);

// add a toolbar with a name and the row you want it to show at
// row number starts at 0
var toolbar1 = plugins.window.addToolBar("toolbar_1", 2);
toolbar1.addButton("click me 1", feedback_button);

// add a toolbar with a name and display name
var toolbar2 = plugins.window.addToolBar("toolbar_2", "toolbar_2_internal_name");
toolbar2.addButton("click me 2", feedback_button);

// add a toolbar with a name, display name and the row you want the
// toolbar to show at. row number starts at 0
var toolbar3 = plugins.window.addToolBar("toolbar_3", "toolbar_3_internal_name", 3);
toolbar3.addButton("click me 3", feedback_button);
```
### addToolBar(name, displayname)

Add a toolbar.

**Parameters**\
[String](../../JSLib/String.md) name the name by which this toolbar is identified in code. If display name is missing, name will be used as displayName as well.\
[String](../../JSLib/String.md) displayname the name by which this toolbar will be identified in the UI. (for example in the toolbar panel's context menu)

**Returns**\
[ToolBar](./ToolBar.md) 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// Note: method addToolBar only works in the smart client.

// add a toolbar with only a name
var toolbar0 = plugins.window.addToolBar("toolbar_0");
toolbar0.addButton("click me 0", feedback_button);

// add a toolbar with a name and the row you want it to show at
// row number starts at 0
var toolbar1 = plugins.window.addToolBar("toolbar_1", 2);
toolbar1.addButton("click me 1", feedback_button);

// add a toolbar with a name and display name
var toolbar2 = plugins.window.addToolBar("toolbar_2", "toolbar_2_internal_name");
toolbar2.addButton("click me 2", feedback_button);

// add a toolbar with a name, display name and the row you want the
// toolbar to show at. row number starts at 0
var toolbar3 = plugins.window.addToolBar("toolbar_3", "toolbar_3_internal_name", 3);
toolbar3.addButton("click me 3", feedback_button);
```
### addToolBar(name, displayname, row)

Add a toolbar.

**Parameters**\
[String](../../JSLib/String.md) name the name by which this toolbar is identified in code. If display name is missing, name will be used as displayName as well.\
[String](../../JSLib/String.md) displayname the name by which this toolbar will be identified in the UI. (for example in the toolbar panel's context menu)\
[Number](../../JSLib/Number.md) row the row inside the toolbar panel where this toolbar is to be added.

**Returns**\
[ToolBar](./ToolBar.md) 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// Note: method addToolBar only works in the smart client.

// add a toolbar with only a name
var toolbar0 = plugins.window.addToolBar("toolbar_0");
toolbar0.addButton("click me 0", feedback_button);

// add a toolbar with a name and the row you want it to show at
// row number starts at 0
var toolbar1 = plugins.window.addToolBar("toolbar_1", 2);
toolbar1.addButton("click me 1", feedback_button);

// add a toolbar with a name and display name
var toolbar2 = plugins.window.addToolBar("toolbar_2", "toolbar_2_internal_name");
toolbar2.addButton("click me 2", feedback_button);

// add a toolbar with a name, display name and the row you want the
// toolbar to show at. row number starts at 0
var toolbar3 = plugins.window.addToolBar("toolbar_3", "toolbar_3_internal_name", 3);
toolbar3.addButton("click me 3", feedback_button);
```
### cancelFormPopup()

Close the current form popup panel without assigning a value to the configured data provider.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope.
plugins.window.showFormPopup(null,forms.orderPicker,foundset.getSelectedRecord(),"order_id");
// do call closeFormPopup(ordervalue) from the orderPicker form
```
### closeFormPopup(retval)

Close the current form popup panel and assign the value to the configured data provider.

**Parameters**\
[Object](../../JSLib/Object.md) retval return value for data provider

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope.
plugins.window.showFormPopup(null,forms.orderPicker,foundset.getSelectedRecord(),"order_id");
// do call closeFormPopup(ordervalue) from the orderPicker form
```
### createFormPopup(form)

Create a form popup that can be filled with data and shown.

**Parameters**\
[Object](../../JSLib/Object.md) form the form to show

**Returns**\
[FormPopup](./FormPopup.md) FormPopup

**Supported Clients**\
NGClient

**Sample**

```javascript
plugins.window.createFormPopup(forms.orderPicker).show();
```
### createPopupMenu()

Creates a new popup menu that can be populated with items and displayed.


**Returns**\
[Popup](./Popup.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// create a popup menu
var menu = plugins.window.createPopupMenu();
// add a menu item
menu.addMenuItem("an entry", feedback);

if (event.getSource()) {
	// display the popup over the component which is the source of the event
	menu.show(event.getSource());
	// display the popup over the components, at specified coordinates relative to the component
	//menu.show(event.getSource(), 10, 10);
	// display the popup at specified coordinates relative to the main window
	//menu.show(100, 100);
}
```
### createShortcut(shortcut, methodName)

Create a shortcut.

**Parameters**\
[String](../../JSLib/String.md) shortcut  ;\
[String](../../JSLib/String.md) methodName scopes.scopename.methodname or formname.methodname String to target the method to execute

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// this plugin uses the java keystroke parser
// see http://java.sun.com/j2se/1.5.0/docs/api/javax/swing/KeyStroke.html#getKeyStroke(java.lang.String)
// global handler
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut);
// global handler with a form context filter
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut, 'frm_contacts');
// form method called when shortcut is used
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut);
// form method called when shortcut is used and arguments are passed to the method
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut, new Array(argument1, argument2));
// Passing the method argument as a string prevents unnecessary form loading
//plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', new Array(argument1, argument2));
// Passing the method as a name and the contextFilter set so that this shortcut only trigger on the form 'frm_contacts'.
plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', 'frm_contacts', new Array(argument1, argument2));
// Num Lock and Substract shortcuts
plugins.window.createShortcut("NUMPAD8", handleMyShortcut);
plugins.window.createShortcut("SUBTRACT", handleMyShortcut);
// remove global shortcut and form-level shortcut
plugins.window.removeShortcut('menu 1');
plugins.window.removeShortcut('control RIGHT', 'frm_contacts');
// consuming they keystroke so that a default browser event will not happen
plugins.window.createShortcut('F4', scopes.globals.handleOrdersShortcut, 'frm_contacts', null, true);
// shortcut handlers are called with an JSEvent argument
///
// * Handle keyboard shortcut.
// 
// * @param {JSEvent} event the event that triggered the action
// */
//function handleShortcut(event)
//{
//  application.output(event.getType()) // returns 'menu 1'
//  application.output(event.getFormName()) // returns 'frm_contacts'
//  application.output(event.getElementName()) // returns 'contact_name_field' or null when no element is selected
//}
// NOTES:
// 1) shortcuts will not override existing operating system or browser shortcuts,
// choose your shortcuts carefully to make sure they work in all clients.
// 2) always use lower-case letters for modifiers (shift, control, etc.), otherwise createShortcut will fail.
```
### createShortcut(shortcut, methodName, arguments)

Create a shortcut.

**Parameters**\
[String](../../JSLib/String.md) shortcut  ;\
[String](../../JSLib/String.md) methodName scopes.scopename.methodname or formname.methodname String to target the method to execute\
[Array](../../JSLib/Array.md) arguments  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// this plugin uses the java keystroke parser
// see http://java.sun.com/j2se/1.5.0/docs/api/javax/swing/KeyStroke.html#getKeyStroke(java.lang.String)
// global handler
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut);
// global handler with a form context filter
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut, 'frm_contacts');
// form method called when shortcut is used
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut);
// form method called when shortcut is used and arguments are passed to the method
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut, new Array(argument1, argument2));
// Passing the method argument as a string prevents unnecessary form loading
//plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', new Array(argument1, argument2));
// Passing the method as a name and the contextFilter set so that this shortcut only trigger on the form 'frm_contacts'.
plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', 'frm_contacts', new Array(argument1, argument2));
// Num Lock and Substract shortcuts
plugins.window.createShortcut("NUMPAD8", handleMyShortcut);
plugins.window.createShortcut("SUBTRACT", handleMyShortcut);
// remove global shortcut and form-level shortcut
plugins.window.removeShortcut('menu 1');
plugins.window.removeShortcut('control RIGHT', 'frm_contacts');
// consuming they keystroke so that a default browser event will not happen
plugins.window.createShortcut('F4', scopes.globals.handleOrdersShortcut, 'frm_contacts', null, true);
// shortcut handlers are called with an JSEvent argument
///
// * Handle keyboard shortcut.
// 
// * @param {JSEvent} event the event that triggered the action
// */
//function handleShortcut(event)
//{
//  application.output(event.getType()) // returns 'menu 1'
//  application.output(event.getFormName()) // returns 'frm_contacts'
//  application.output(event.getElementName()) // returns 'contact_name_field' or null when no element is selected
//}
// NOTES:
// 1) shortcuts will not override existing operating system or browser shortcuts,
// choose your shortcuts carefully to make sure they work in all clients.
// 2) always use lower-case letters for modifiers (shift, control, etc.), otherwise createShortcut will fail.
```
### createShortcut(shortcut, methodName, contextFilter)

Create a shortcut.

**Parameters**\
[String](../../JSLib/String.md) shortcut  ;\
[String](../../JSLib/String.md) methodName scopes.scopename.methodname or formname.methodname String to target the method to execute\
[String](../../JSLib/String.md) contextFilter form or element name ( ng only - specified by formName.elementName); only triggers the shortcut when on this form/element

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// this plugin uses the java keystroke parser
// see http://java.sun.com/j2se/1.5.0/docs/api/javax/swing/KeyStroke.html#getKeyStroke(java.lang.String)
// global handler
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut);
// global handler with a form context filter
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut, 'frm_contacts');
// form method called when shortcut is used
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut);
// form method called when shortcut is used and arguments are passed to the method
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut, new Array(argument1, argument2));
// Passing the method argument as a string prevents unnecessary form loading
//plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', new Array(argument1, argument2));
// Passing the method as a name and the contextFilter set so that this shortcut only trigger on the form 'frm_contacts'.
plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', 'frm_contacts', new Array(argument1, argument2));
// Num Lock and Substract shortcuts
plugins.window.createShortcut("NUMPAD8", handleMyShortcut);
plugins.window.createShortcut("SUBTRACT", handleMyShortcut);
// remove global shortcut and form-level shortcut
plugins.window.removeShortcut('menu 1');
plugins.window.removeShortcut('control RIGHT', 'frm_contacts');
// consuming they keystroke so that a default browser event will not happen
plugins.window.createShortcut('F4', scopes.globals.handleOrdersShortcut, 'frm_contacts', null, true);
// shortcut handlers are called with an JSEvent argument
///
// * Handle keyboard shortcut.
// 
// * @param {JSEvent} event the event that triggered the action
// */
//function handleShortcut(event)
//{
//  application.output(event.getType()) // returns 'menu 1'
//  application.output(event.getFormName()) // returns 'frm_contacts'
//  application.output(event.getElementName()) // returns 'contact_name_field' or null when no element is selected
//}
// NOTES:
// 1) shortcuts will not override existing operating system or browser shortcuts,
// choose your shortcuts carefully to make sure they work in all clients.
// 2) always use lower-case letters for modifiers (shift, control, etc.), otherwise createShortcut will fail.
```
### createShortcut(shortcut, method, contextFilter, arguments)

Create a shortcut.

**Parameters**\
[String](../../JSLib/String.md) shortcut  ;\
[Object](../../JSLib/Object.md) method the method/function that needs to be called when the shortcut is hit\
[String](../../JSLib/String.md) contextFilter form or element name ( ng only - specified by formName.elementName); only triggers the shortcut when on this form/element\
[Array](../../JSLib/Array.md) arguments  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// this plugin uses the java keystroke parser
// see http://java.sun.com/j2se/1.5.0/docs/api/javax/swing/KeyStroke.html#getKeyStroke(java.lang.String)
// global handler
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut);
// global handler with a form context filter
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut, 'frm_contacts');
// form method called when shortcut is used
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut);
// form method called when shortcut is used and arguments are passed to the method
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut, new Array(argument1, argument2));
// Passing the method argument as a string prevents unnecessary form loading
//plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', new Array(argument1, argument2));
// Passing the method as a name and the contextFilter set so that this shortcut only trigger on the form 'frm_contacts'.
plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', 'frm_contacts', new Array(argument1, argument2));
// Num Lock and Substract shortcuts
plugins.window.createShortcut("NUMPAD8", handleMyShortcut);
plugins.window.createShortcut("SUBTRACT", handleMyShortcut);
// remove global shortcut and form-level shortcut
plugins.window.removeShortcut('menu 1');
plugins.window.removeShortcut('control RIGHT', 'frm_contacts');
// consuming they keystroke so that a default browser event will not happen
plugins.window.createShortcut('F4', scopes.globals.handleOrdersShortcut, 'frm_contacts', null, true);
// shortcut handlers are called with an JSEvent argument
///
// * Handle keyboard shortcut.
// 
// * @param {JSEvent} event the event that triggered the action
// */
//function handleShortcut(event)
//{
//  application.output(event.getType()) // returns 'menu 1'
//  application.output(event.getFormName()) // returns 'frm_contacts'
//  application.output(event.getElementName()) // returns 'contact_name_field' or null when no element is selected
//}
// NOTES:
// 1) shortcuts will not override existing operating system or browser shortcuts,
// choose your shortcuts carefully to make sure they work in all clients.
// 2) always use lower-case letters for modifiers (shift, control, etc.), otherwise createShortcut will fail.
```
### createShortcut(shortcut, methodName, contextFilter, arguments, consumeEvent)

Create a shortcut.

**Parameters**\
[String](../../JSLib/String.md) shortcut  ;\
[String](../../JSLib/String.md) methodName scopes.scopename.methodname or formname.methodname String to target the method to execute\
[String](../../JSLib/String.md) contextFilter form or element name ( ng only - specified by formName.elementName); only triggers the shortcut when on this form/element\
[Array](../../JSLib/Array.md) arguments  ;\
[Boolean](../../JSLib/Boolean.md) consumeEvent if true then the shotcut will consume the event and the default browser behavior will not be executed (default false)

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// this plugin uses the java keystroke parser
// see http://java.sun.com/j2se/1.5.0/docs/api/javax/swing/KeyStroke.html#getKeyStroke(java.lang.String)
// global handler
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut);
// global handler with a form context filter
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut, 'frm_contacts');
// form method called when shortcut is used
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut);
// form method called when shortcut is used and arguments are passed to the method
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut, new Array(argument1, argument2));
// Passing the method argument as a string prevents unnecessary form loading
//plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', new Array(argument1, argument2));
// Passing the method as a name and the contextFilter set so that this shortcut only trigger on the form 'frm_contacts'.
plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', 'frm_contacts', new Array(argument1, argument2));
// Num Lock and Substract shortcuts
plugins.window.createShortcut("NUMPAD8", handleMyShortcut);
plugins.window.createShortcut("SUBTRACT", handleMyShortcut);
// remove global shortcut and form-level shortcut
plugins.window.removeShortcut('menu 1');
plugins.window.removeShortcut('control RIGHT', 'frm_contacts');
// consuming they keystroke so that a default browser event will not happen
plugins.window.createShortcut('F4', scopes.globals.handleOrdersShortcut, 'frm_contacts', null, true);
// shortcut handlers are called with an JSEvent argument
///
// * Handle keyboard shortcut.
// 
// * @param {JSEvent} event the event that triggered the action
// */
//function handleShortcut(event)
//{
//  application.output(event.getType()) // returns 'menu 1'
//  application.output(event.getFormName()) // returns 'frm_contacts'
//  application.output(event.getElementName()) // returns 'contact_name_field' or null when no element is selected
//}
// NOTES:
// 1) shortcuts will not override existing operating system or browser shortcuts,
// choose your shortcuts carefully to make sure they work in all clients.
// 2) always use lower-case letters for modifiers (shift, control, etc.), otherwise createShortcut will fail.
```
### createShortcut(shortcut, method)

Create a shortcut.

**Parameters**\
[String](../../JSLib/String.md) shortcut  ;\
[Function](../../JSLib/Function.md) method the method/function that needs to be called when the shortcut is hit

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// this plugin uses the java keystroke parser
// see http://java.sun.com/j2se/1.5.0/docs/api/javax/swing/KeyStroke.html#getKeyStroke(java.lang.String)
// global handler
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut);
// global handler with a form context filter
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut, 'frm_contacts');
// form method called when shortcut is used
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut);
// form method called when shortcut is used and arguments are passed to the method
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut, new Array(argument1, argument2));
// Passing the method argument as a string prevents unnecessary form loading
//plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', new Array(argument1, argument2));
// Passing the method as a name and the contextFilter set so that this shortcut only trigger on the form 'frm_contacts'.
plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', 'frm_contacts', new Array(argument1, argument2));
// Num Lock and Substract shortcuts
plugins.window.createShortcut("NUMPAD8", handleMyShortcut);
plugins.window.createShortcut("SUBTRACT", handleMyShortcut);
// remove global shortcut and form-level shortcut
plugins.window.removeShortcut('menu 1');
plugins.window.removeShortcut('control RIGHT', 'frm_contacts');
// consuming they keystroke so that a default browser event will not happen
plugins.window.createShortcut('F4', scopes.globals.handleOrdersShortcut, 'frm_contacts', null, true);
// shortcut handlers are called with an JSEvent argument
///
// * Handle keyboard shortcut.
// 
// * @param {JSEvent} event the event that triggered the action
// */
//function handleShortcut(event)
//{
//  application.output(event.getType()) // returns 'menu 1'
//  application.output(event.getFormName()) // returns 'frm_contacts'
//  application.output(event.getElementName()) // returns 'contact_name_field' or null when no element is selected
//}
// NOTES:
// 1) shortcuts will not override existing operating system or browser shortcuts,
// choose your shortcuts carefully to make sure they work in all clients.
// 2) always use lower-case letters for modifiers (shift, control, etc.), otherwise createShortcut will fail.
```
### createShortcut(shortcut, method, arguments)

Create a shortcut.

**Parameters**\
[String](../../JSLib/String.md) shortcut  ;\
[Function](../../JSLib/Function.md) method the method/function that needs to be called when the shortcut is hit\
[Array](../../JSLib/Array.md) arguments  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// this plugin uses the java keystroke parser
// see http://java.sun.com/j2se/1.5.0/docs/api/javax/swing/KeyStroke.html#getKeyStroke(java.lang.String)
// global handler
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut);
// global handler with a form context filter
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut, 'frm_contacts');
// form method called when shortcut is used
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut);
// form method called when shortcut is used and arguments are passed to the method
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut, new Array(argument1, argument2));
// Passing the method argument as a string prevents unnecessary form loading
//plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', new Array(argument1, argument2));
// Passing the method as a name and the contextFilter set so that this shortcut only trigger on the form 'frm_contacts'.
plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', 'frm_contacts', new Array(argument1, argument2));
// Num Lock and Substract shortcuts
plugins.window.createShortcut("NUMPAD8", handleMyShortcut);
plugins.window.createShortcut("SUBTRACT", handleMyShortcut);
// remove global shortcut and form-level shortcut
plugins.window.removeShortcut('menu 1');
plugins.window.removeShortcut('control RIGHT', 'frm_contacts');
// consuming they keystroke so that a default browser event will not happen
plugins.window.createShortcut('F4', scopes.globals.handleOrdersShortcut, 'frm_contacts', null, true);
// shortcut handlers are called with an JSEvent argument
///
// * Handle keyboard shortcut.
// 
// * @param {JSEvent} event the event that triggered the action
// */
//function handleShortcut(event)
//{
//  application.output(event.getType()) // returns 'menu 1'
//  application.output(event.getFormName()) // returns 'frm_contacts'
//  application.output(event.getElementName()) // returns 'contact_name_field' or null when no element is selected
//}
// NOTES:
// 1) shortcuts will not override existing operating system or browser shortcuts,
// choose your shortcuts carefully to make sure they work in all clients.
// 2) always use lower-case letters for modifiers (shift, control, etc.), otherwise createShortcut will fail.
```
### createShortcut(shortcut, method, contextFilter)

Create a shortcut.

**Parameters**\
[String](../../JSLib/String.md) shortcut  ;\
[Function](../../JSLib/Function.md) method the method/function that needs to be called when the shortcut is hit\
[String](../../JSLib/String.md) contextFilter form or element name ( ng only - specified by formName.elementName); only triggers the shortcut when on this form/element

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// this plugin uses the java keystroke parser
// see http://java.sun.com/j2se/1.5.0/docs/api/javax/swing/KeyStroke.html#getKeyStroke(java.lang.String)
// global handler
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut);
// global handler with a form context filter
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut, 'frm_contacts');
// form method called when shortcut is used
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut);
// form method called when shortcut is used and arguments are passed to the method
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut, new Array(argument1, argument2));
// Passing the method argument as a string prevents unnecessary form loading
//plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', new Array(argument1, argument2));
// Passing the method as a name and the contextFilter set so that this shortcut only trigger on the form 'frm_contacts'.
plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', 'frm_contacts', new Array(argument1, argument2));
// Num Lock and Substract shortcuts
plugins.window.createShortcut("NUMPAD8", handleMyShortcut);
plugins.window.createShortcut("SUBTRACT", handleMyShortcut);
// remove global shortcut and form-level shortcut
plugins.window.removeShortcut('menu 1');
plugins.window.removeShortcut('control RIGHT', 'frm_contacts');
// consuming they keystroke so that a default browser event will not happen
plugins.window.createShortcut('F4', scopes.globals.handleOrdersShortcut, 'frm_contacts', null, true);
// shortcut handlers are called with an JSEvent argument
///
// * Handle keyboard shortcut.
// 
// * @param {JSEvent} event the event that triggered the action
// */
//function handleShortcut(event)
//{
//  application.output(event.getType()) // returns 'menu 1'
//  application.output(event.getFormName()) // returns 'frm_contacts'
//  application.output(event.getElementName()) // returns 'contact_name_field' or null when no element is selected
//}
// NOTES:
// 1) shortcuts will not override existing operating system or browser shortcuts,
// choose your shortcuts carefully to make sure they work in all clients.
// 2) always use lower-case letters for modifiers (shift, control, etc.), otherwise createShortcut will fail.
```
### createShortcut(shortcut, method, contextFilter, arguments)

Create a shortcut.

**Parameters**\
[String](../../JSLib/String.md) shortcut  ;\
[Function](../../JSLib/Function.md) method the method/function that needs to be called when the shortcut is hit\
[String](../../JSLib/String.md) contextFilter form or element name ( ng only - specified by formName.elementName); only triggers the shortcut when on this form/element\
[Array](../../JSLib/Array.md) arguments  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// this plugin uses the java keystroke parser
// see http://java.sun.com/j2se/1.5.0/docs/api/javax/swing/KeyStroke.html#getKeyStroke(java.lang.String)
// global handler
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut);
// global handler with a form context filter
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut, 'frm_contacts');
// form method called when shortcut is used
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut);
// form method called when shortcut is used and arguments are passed to the method
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut, new Array(argument1, argument2));
// Passing the method argument as a string prevents unnecessary form loading
//plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', new Array(argument1, argument2));
// Passing the method as a name and the contextFilter set so that this shortcut only trigger on the form 'frm_contacts'.
plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', 'frm_contacts', new Array(argument1, argument2));
// Num Lock and Substract shortcuts
plugins.window.createShortcut("NUMPAD8", handleMyShortcut);
plugins.window.createShortcut("SUBTRACT", handleMyShortcut);
// remove global shortcut and form-level shortcut
plugins.window.removeShortcut('menu 1');
plugins.window.removeShortcut('control RIGHT', 'frm_contacts');
// consuming they keystroke so that a default browser event will not happen
plugins.window.createShortcut('F4', scopes.globals.handleOrdersShortcut, 'frm_contacts', null, true);
// shortcut handlers are called with an JSEvent argument
///
// * Handle keyboard shortcut.
// 
// * @param {JSEvent} event the event that triggered the action
// */
//function handleShortcut(event)
//{
//  application.output(event.getType()) // returns 'menu 1'
//  application.output(event.getFormName()) // returns 'frm_contacts'
//  application.output(event.getElementName()) // returns 'contact_name_field' or null when no element is selected
//}
// NOTES:
// 1) shortcuts will not override existing operating system or browser shortcuts,
// choose your shortcuts carefully to make sure they work in all clients.
// 2) always use lower-case letters for modifiers (shift, control, etc.), otherwise createShortcut will fail.
```
### createShortcut(shortcut, method, contextFilter, arguments, consumeEvent)

Create a shortcut.

**Parameters**\
[String](../../JSLib/String.md) shortcut  ;\
[Function](../../JSLib/Function.md) method the method/function that needs to be called when the shortcut is hit\
[String](../../JSLib/String.md) contextFilter form or element name ( ng only - specified by formName.elementName); only triggers the shortcut when on this form/element\
[Array](../../JSLib/Array.md) arguments  ;\
[Boolean](../../JSLib/Boolean.md) consumeEvent if true then the shotcut will consume the event and the default browser behavior will not be executed (default false)

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// this plugin uses the java keystroke parser
// see http://java.sun.com/j2se/1.5.0/docs/api/javax/swing/KeyStroke.html#getKeyStroke(java.lang.String)
// global handler
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut);
// global handler with a form context filter
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut, 'frm_contacts');
// form method called when shortcut is used
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut);
// form method called when shortcut is used and arguments are passed to the method
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut, new Array(argument1, argument2));
// Passing the method argument as a string prevents unnecessary form loading
//plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', new Array(argument1, argument2));
// Passing the method as a name and the contextFilter set so that this shortcut only trigger on the form 'frm_contacts'.
plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', 'frm_contacts', new Array(argument1, argument2));
// Num Lock and Substract shortcuts
plugins.window.createShortcut("NUMPAD8", handleMyShortcut);
plugins.window.createShortcut("SUBTRACT", handleMyShortcut);
// remove global shortcut and form-level shortcut
plugins.window.removeShortcut('menu 1');
plugins.window.removeShortcut('control RIGHT', 'frm_contacts');
// consuming they keystroke so that a default browser event will not happen
plugins.window.createShortcut('F4', scopes.globals.handleOrdersShortcut, 'frm_contacts', null, true);
// shortcut handlers are called with an JSEvent argument
///
// * Handle keyboard shortcut.
// 
// * @param {JSEvent} event the event that triggered the action
// */
//function handleShortcut(event)
//{
//  application.output(event.getType()) // returns 'menu 1'
//  application.output(event.getFormName()) // returns 'frm_contacts'
//  application.output(event.getElementName()) // returns 'contact_name_field' or null when no element is selected
//}
// NOTES:
// 1) shortcuts will not override existing operating system or browser shortcuts,
// choose your shortcuts carefully to make sure they work in all clients.
// 2) always use lower-case letters for modifiers (shift, control, etc.), otherwise createShortcut will fail.
```
### getMenuBar()

Get the menubar of the main window, or of a named window.


**Returns**\
[MenuBar](./MenuBar.md) 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// create a new window
var win = application.createWindow("windowName", JSWindow.WINDOW);
// show a form in the new window
forms.my_form.controller.show(win);
// retrieve the menubar of the new window
var menubar = plugins.window.getMenuBar("windowName");
// add a new menu to the menubar, with an item in it
var menu = menubar.addMenu();
menu.text = "New Menu";
menu.addMenuItem("an entry", feedback);
// retrieve the menubar of the main window
var mainMenubar = plugins.window.getMenuBar();
// add a new menu to the menubar of the main window
var menuMain = mainMenubar.addMenu();
menuMain.text = "New Menu in Main Menubar";
menuMain.addMenuItem("another entry", feedback);
```
### getMenuBar(windowName)

Get the menubar of the main window, or of a named window.

**Parameters**\
[String](../../JSLib/String.md) windowName the name of the window

**Returns**\
[MenuBar](./MenuBar.md) 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// create a new window
var win = application.createWindow("windowName", JSWindow.WINDOW);
// show a form in the new window
forms.my_form.controller.show(win);
// retrieve the menubar of the new window
var menubar = plugins.window.getMenuBar("windowName");
// add a new menu to the menubar, with an item in it
var menu = menubar.addMenu();
menu.text = "New Menu";
menu.addMenuItem("an entry", feedback);
// retrieve the menubar of the main window
var mainMenubar = plugins.window.getMenuBar();
// add a new menu to the menubar of the main window
var menuMain = mainMenubar.addMenu();
menuMain.text = "New Menu in Main Menubar";
menuMain.addMenuItem("another entry", feedback);
```
### getToolBar(window, name)

Get the toolbar of a specific window from the toolbar panel by name.

**Parameters**\
[JSWindow](../../Application/JSWindow.md) window  ;\
[String](../../JSLib/String.md) name  ;

**Returns**\
[ToolBar](./ToolBar.md) 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// Note: method getToolBar only works in the smart client.

// create a window
	var win = application.createWindow("myWindow", JSWindow.WINDOW);
// the toolbar must first be created with a call to addToolbar
plugins.window.addToolBar(win,"toolbar_0");

// show the empty toolbar and wait 4 seconds
win.show(forms.MyForm)
application.updateUI(4000)

// get the toolbar at the panel by name
var toolbar = plugins.window.getToolBar(win,"toolbar_0");
// add a button to the toolbar
toolbar.addButton("button", callback_function);
```
### getToolBar(name)

Get the toolbar from the toolbar panel by name.

**Parameters**\
[String](../../JSLib/String.md) name  ;

**Returns**\
[ToolBar](./ToolBar.md) 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// Note: method getToolBar only works in the smart client.

// the toolbar must first be created with a call to addToolbar
plugins.window.addToolBar("toolbar_0");

// get the toolbar at the panel by name
var toolbar = plugins.window.getToolBar("toolbar_0");
// add a button to the toolbar
toolbar.addButton("button", feedback_button);
```
### getToolbarNames()

Get all toolbar names from the toolbar panel.


**Returns**\
[Array](../../JSLib/Array.md) 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// Note: method getToolbarNames only works in the smart client.

// create an array of toolbar names
var names = plugins.window.getToolbarNames();

// create an empty message variable
var message = "";

// loop through the array
for (var i = 0 ; i < names.length ; i++) {
	//add the name(s) to the message
	message += names[i] + "\n";
}

// show the message
plugins.dialogs.showInfoDialog("toolbar names", message);
```
### getToolbarNames(window)

Get all toolbar names from the toolbar panel of a specific window.

**Parameters**\
[JSWindow](../../Application/JSWindow.md) window  ;

**Returns**\
[Array](../../JSLib/Array.md) 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// Note: method getToolbarNames only works in the smart client.
// create a window
	var win = application.createWindow("myWindow", JSWindow.WINDOW);
// the toolbar must first be created with a call to addToolbar
	 plugins.window.addToolBar(win,"toolbar_0");
  plugins.window.addToolBar(win,"toolbar_1");
// create an array of toolbar names
var names = plugins.window.getToolbarNames(win);

// create an empty message variable
var message = "";

// loop through the array
for (var i = 0 ; i < names.length ; i++) {
	//add the name(s) to the message
	message += names[i] + "\n";
}

// show the message
plugins.dialogs.showInfoDialog("toolbar names", message);
```
### maximize()

Maximize the current window or the window with the specified name (Smart client only).


**Returns**\
void 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// maximize the main window:
plugins.window.maximize();

// create a new window
var win = application.createWindow("windowName", JSWindow.WINDOW);
// show a form in the new window
forms.my_form.controller.show(win);
// maximize the window
plugins.window.maximize("windowName");
```
### maximize(windowName)

Maximize the current window or the window with the specified name (Smart client only).

**Parameters**\
[String](../../JSLib/String.md) windowName  ;

**Returns**\
void 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// maximize the main window:
plugins.window.maximize();

// create a new window
var win = application.createWindow("windowName", JSWindow.WINDOW);
// show a form in the new window
forms.my_form.controller.show(win);
// maximize the window
plugins.window.maximize("windowName");
```
### removeShortcut(shortcut)

Remove a shortcut.

**Parameters**\
[String](../../JSLib/String.md) shortcut  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// this plugin uses the java keystroke parser
// see http://java.sun.com/j2se/1.5.0/docs/api/javax/swing/KeyStroke.html#getKeyStroke(java.lang.String)
// global handler
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut);
// global handler with a form context filter
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut, 'frm_contacts');
// form method called when shortcut is used
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut);
// form method called when shortcut is used and arguments are passed to the method
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut, new Array(argument1, argument2));
// Passing the method argument as a string prevents unnecessary form loading
//plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', new Array(argument1, argument2));
// Passing the method as a name and the contextFilter set so that this shortcut only trigger on the form 'frm_contacts'.
plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', 'frm_contacts', new Array(argument1, argument2));
// Num Lock and Substract shortcuts
plugins.window.createShortcut("NUMPAD8", handleMyShortcut);
plugins.window.createShortcut("SUBTRACT", handleMyShortcut);
// remove global shortcut and form-level shortcut
plugins.window.removeShortcut('menu 1');
plugins.window.removeShortcut('control RIGHT', 'frm_contacts');
// consuming they keystroke so that a default browser event will not happen
plugins.window.createShortcut('F4', scopes.globals.handleOrdersShortcut, 'frm_contacts', null, true);
// shortcut handlers are called with an JSEvent argument
///
// * Handle keyboard shortcut.
// 
// * @param {JSEvent} event the event that triggered the action
// */
//function handleShortcut(event)
//{
//  application.output(event.getType()) // returns 'menu 1'
//  application.output(event.getFormName()) // returns 'frm_contacts'
//  application.output(event.getElementName()) // returns 'contact_name_field' or null when no element is selected
//}
// NOTES:
// 1) shortcuts will not override existing operating system or browser shortcuts,
// choose your shortcuts carefully to make sure they work in all clients.
// 2) always use lower-case letters for modifiers (shift, control, etc.), otherwise createShortcut will fail.
```
### removeShortcut(shortcut, contextFilter)

Remove a shortcut.

**Parameters**\
[String](../../JSLib/String.md) shortcut  ;\
[String](../../JSLib/String.md) contextFilter form or element name ( ng only - specified by formName.elementName); only triggers the shortcut when on this form/element

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// this plugin uses the java keystroke parser
// see http://java.sun.com/j2se/1.5.0/docs/api/javax/swing/KeyStroke.html#getKeyStroke(java.lang.String)
// global handler
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut);
// global handler with a form context filter
plugins.window.createShortcut('control shift I', scopes.globals.handleOrdersShortcut, 'frm_contacts');
// form method called when shortcut is used
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut);
// form method called when shortcut is used and arguments are passed to the method
plugins.window.createShortcut('control RIGHT', forms.frm_contacts.handleMyShortcut, new Array(argument1, argument2));
// Passing the method argument as a string prevents unnecessary form loading
//plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', new Array(argument1, argument2));
// Passing the method as a name and the contextFilter set so that this shortcut only trigger on the form 'frm_contacts'.
plugins.window.createShortcut('control RIGHT', 'frm_contacts.handleMyShortcut', 'frm_contacts', new Array(argument1, argument2));
// Num Lock and Substract shortcuts
plugins.window.createShortcut("NUMPAD8", handleMyShortcut);
plugins.window.createShortcut("SUBTRACT", handleMyShortcut);
// remove global shortcut and form-level shortcut
plugins.window.removeShortcut('menu 1');
plugins.window.removeShortcut('control RIGHT', 'frm_contacts');
// consuming they keystroke so that a default browser event will not happen
plugins.window.createShortcut('F4', scopes.globals.handleOrdersShortcut, 'frm_contacts', null, true);
// shortcut handlers are called with an JSEvent argument
///
// * Handle keyboard shortcut.
// 
// * @param {JSEvent} event the event that triggered the action
// */
//function handleShortcut(event)
//{
//  application.output(event.getType()) // returns 'menu 1'
//  application.output(event.getFormName()) // returns 'frm_contacts'
//  application.output(event.getElementName()) // returns 'contact_name_field' or null when no element is selected
//}
// NOTES:
// 1) shortcuts will not override existing operating system or browser shortcuts,
// choose your shortcuts carefully to make sure they work in all clients.
// 2) always use lower-case letters for modifiers (shift, control, etc.), otherwise createShortcut will fail.
```
### removeToolBar(window, name)

Remove the toolbar from the toolbar panel of a specific window.

**Parameters**\
[JSWindow](../../Application/JSWindow.md) window  ;\
[String](../../JSLib/String.md) name  ;

**Returns**\
void 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// Note: method removeToolBar only works in the smart client.
// create a window
	var win = application.createWindow("myWindow", JSWindow.WINDOW);
// the toolbar must first be created with a call to addToolbar
var toolbar = plugins.window.addToolBar(win,"toolbar_0");

// add a button to the toolbar
toolbar.addButton("button", callcbackMethod);

// show the toolbar with the button and wait 4 seconds, then remove it
win.show(forms.MyForm)
application.updateUI(4000)

// removing a toolbar from the toolbar panel is done by name
// the plugin checks the existence of the toolbar
// when the toolbar does not exist it will not throw an error though.
plugins.window.removeToolBar(win,"toolbar_0");
```
### removeToolBar(name)

Remove the toolbar from the toolbar panel.

**Parameters**\
[String](../../JSLib/String.md) name  ;

**Returns**\
void 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// Note: method removeToolBar only works in the smart client.

// the toolbar must first be created with a call to addToolbar
var toolbar = plugins.window.addToolBar("toolbar_0");

// add a button to the toolbar
toolbar.addButton("button", feedback_button);

// removing a toolbar from the toolbar panel is done by name
// the plugin checks the existence of the toolbar
// when the toolbar does not exist it will not throw an error though.
plugins.window.removeToolBar("toolbar_0");
```
### setFullScreen(full)

Bring the window into/out of fullsceen mode.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) full  ;

**Returns**\
void 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// active fullscreen mode
plugins.window.setFullScreen(true);
```
### setStatusBarVisible(visible)

Show or hide the statusbar.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) visible  ;

**Returns**\
void 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// hide the statusbar
plugins.window.setStatusBarVisible(false);
```
### setToolBarAreaVisible(visible)

Show or hide the toolbar area.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) visible  ;

**Returns**\
void 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// hide the toolbar area
plugins.window.setToolBarAreaVisible(false);
```
### showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID)

Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope.

**Parameters**\
[Object](../../JSLib/Object.md) elementToShowRelatedTo element to show related to or null to center in screen\
[Object](../../JSLib/Object.md) form the form to show\
[Object](../../JSLib/Object.md) scope the scope to put retval into\
[String](../../JSLib/String.md) dataproviderID the dataprovider of scope to fill

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope.
plugins.window.showFormPopup(null,forms.orderPicker,foundset.getSelectedRecord(),"order_id");
// do call closeFormPopup(ordervalue) from the orderPicker form
```
### showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID, width, height)

Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope.

**Parameters**\
[Object](../../JSLib/Object.md) elementToShowRelatedTo element to show related to or null to center in screen\
[Object](../../JSLib/Object.md) form the form to show\
[Object](../../JSLib/Object.md) scope the scope to put retval into\
[String](../../JSLib/String.md) dataproviderID the dataprovider of scope to fill\
[Number](../../JSLib/Number.md) width popup width\
[Number](../../JSLib/Number.md) height popup height

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope.
plugins.window.showFormPopup(null,forms.orderPicker,foundset.getSelectedRecord(),"order_id");
// do call closeFormPopup(ordervalue) from the orderPicker form
```
### showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID, width, height, x, y)

Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope. Can show relative to a component or at specified coordinates.
Show on specified location is only supported in NGClient.

**Parameters**\
[Object](../../JSLib/Object.md) elementToShowRelatedTo element to show related to or null to center in screen\
[Object](../../JSLib/Object.md) form the form to show\
[Object](../../JSLib/Object.md) scope the scope to put retval into\
[String](../../JSLib/String.md) dataproviderID the dataprovider of scope to fill\
[Number](../../JSLib/Number.md) width popup width\
[Number](../../JSLib/Number.md) height popup height\
[Number](../../JSLib/Number.md) x popup x location\
[Number](../../JSLib/Number.md) y popup y location

**Returns**\
void 

**Supported Clients**\
NGClient

**Sample**

```javascript
// Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope.
plugins.window.showFormPopup(null,forms.orderPicker,foundset.getSelectedRecord(),"order_id");
// plugins.window.showFormPopup(null,forms.orderPicker,foundset.getSelectedRecord(),"order_id",-1,-1,100,100);
// do call closeFormPopup(ordervalue) from the orderPicker form
```
### showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID, width, height, x, y, showBackdrop)

Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope. Can show relative to a component or at specified coordinates.
Show on specified location and backdrop is only supported in NGClient.

**Parameters**\
[Object](../../JSLib/Object.md) elementToShowRelatedTo element to show related to or null to center in screen\
[Object](../../JSLib/Object.md) form the form to show\
[Object](../../JSLib/Object.md) scope the scope to put retval into\
[String](../../JSLib/String.md) dataproviderID the dataprovider of scope to fill\
[Number](../../JSLib/Number.md) width popup width\
[Number](../../JSLib/Number.md) height popup height\
[Number](../../JSLib/Number.md) x popup x location\
[Number](../../JSLib/Number.md) y popup y location\
[Boolean](../../JSLib/Boolean.md) showBackdrop whatever to show a dimmed backdrop under the popup

**Returns**\
void 

**Supported Clients**\
NGClient

**Sample**

```javascript
// Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope.
plugins.window.showFormPopup(null,forms.orderPicker,foundset.getSelectedRecord(),"order_id");
// plugins.window.showFormPopup(null,forms.orderPicker,foundset.getSelectedRecord(),"order_id",-1,-1,100,100,true);
// do call closeFormPopup(ordervalue) from the orderPicker form
```
### showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID, width, height, x, y, showBackdrop, doNotCloseOnClickOutside)

Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope. Can show relative to a component or at specified coordinates.
Show on specified location and backdrop is only supported in NGClient.
By setting the @param doNotCloseOnClickOutside as true, one can ensure that the popup will not be closed when clicking outside this popup.

**Parameters**\
[Object](../../JSLib/Object.md) elementToShowRelatedTo element to show related to or null to center in screen\
[Object](../../JSLib/Object.md) form the form to show\
[Object](../../JSLib/Object.md) scope the scope to put retval into\
[String](../../JSLib/String.md) dataproviderID the dataprovider of scope to fill\
[Number](../../JSLib/Number.md) width popup width\
[Number](../../JSLib/Number.md) height popup height\
[Number](../../JSLib/Number.md) x popup x location\
[Number](../../JSLib/Number.md) y popup y location\
[Boolean](../../JSLib/Boolean.md) showBackdrop whatever to show a dimmed backdrop under the popup\
[Boolean](../../JSLib/Boolean.md) doNotCloseOnClickOutside whether to close on not close the popup on clicking outside

**Returns**\
void 

**Supported Clients**\
NGClient

**Sample**

```javascript
// Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope.
plugins.window.showFormPopup(null,forms.orderPicker,foundset.getSelectedRecord(),"order_id");
// plugins.window.showFormPopup(null,forms.orderPicker,foundset.getSelectedRecord(),"order_id",-1,-1,100,100,true, true);
// do call closeFormPopup(ordervalue) from the orderPicker form
```
### showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID, width, height, x, y, showBackdrop, doNotCloseOnClickOutside, onClose)

Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope. Can show relative to a component or at specified coordinates.
Show on specified location and backdrop is only supported in NGClient.

**Parameters**\
[Object](../../JSLib/Object.md) elementToShowRelatedTo element to show related to or null to center in screen\
[Object](../../JSLib/Object.md) form the form to show\
[Object](../../JSLib/Object.md) scope the scope to put retval into\
[String](../../JSLib/String.md) dataproviderID the dataprovider of scope to fill\
[Number](../../JSLib/Number.md) width popup width\
[Number](../../JSLib/Number.md) height popup height\
[Number](../../JSLib/Number.md) x popup x location\
[Number](../../JSLib/Number.md) y popup y location\
[Boolean](../../JSLib/Boolean.md) showBackdrop whatever to show a dimmed backdrop under the popup\
[Boolean](../../JSLib/Boolean.md) doNotCloseOnClickOutside whether to close on not close the popup on clicking outside\
[Function](../../JSLib/Function.md) onClose a callback function that is being triggered once the formpopup window is being closed

**Returns**\
void 

**Supported Clients**\
NGClient

**Sample**

```javascript
// Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope.
plugins.window.showFormPopup(null,forms.orderPicker,foundset.getSelectedRecord(),"order_id");
// plugins.window.showFormPopup(null,forms.orderPicker,foundset.getSelectedRecord(),"order_id",-1,-1,100,100,true, false, onClose);
//
// function onClose(event) {application.output("Popup closed");}
```

