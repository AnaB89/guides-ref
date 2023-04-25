#  window

## **Return Types**
[Menu](./Menu.md),[RadioButton](./RadioButton.md),[CheckBox](./CheckBox.md),[FormPopup](./FormPopup.md),[MenuItem](./MenuItem.md),[Popup](./Popup.md),[ToolBar](./ToolBar.md),[MenuBar](./MenuBar.md),

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
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
| [Boolean](../../JSLib/Boolean.md) | [removeShortcut(shortcut)](window.md#removeshortcut-shortcut)                   | Remove a shortcut..                                    |
| [Boolean](../../JSLib/Boolean.md) | [removeShortcut(shortcut, contextFilter)](window.md#removeshortcut-shortcut-contextfilter)                   | Remove a shortcut..                                    |
|void | [showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID)](window.md#showformpopup-elementtoshowrelatedto-form-scope-dataproviderid)                   | Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope..                                    |
|void | [showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID, width, height)](window.md#showformpopup-elementtoshowrelatedto-form-scope-dataproviderid-width-height)                   | Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope..                                    |
|void | [showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID, width, height, x, y)](window.md#showformpopup-elementtoshowrelatedto-form-scope-dataproviderid-width-height-x-y)                   | Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope..                                    |
|void | [showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID, width, height, x, y, showBackdrop)](window.md#showformpopup-elementtoshowrelatedto-form-scope-dataproviderid-width-height-x-y-showbackdrop)                   | Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope..                                    |
|void | [showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID, width, height, x, y, showBackdrop, doNotCloseOnClickOutside)](window.md#showformpopup-elementtoshowrelatedto-form-scope-dataproviderid-width-height-x-y-showbackdrop-donotcloseonclickoutside)                   | Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope..                                    |
|void | [showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID, width, height, x, y, showBackdrop, doNotCloseOnClickOutside, onClose)](window.md#showformpopup-elementtoshowrelatedto-form-scope-dataproviderid-width-height-x-y-showbackdrop-donotcloseonclickoutside-onclose)                   | Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope..                                    |

## Methods Details

### cancelFormPopup()

Close the current form popup panel without assigning a value to the configured data provider.


**Returns**\
void 


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


**Sample**

```javascript
plugins.window.createFormPopup(forms.orderPicker).show();
```
### createPopupMenu()

Creates a new popup menu that can be populated with items and displayed.


**Returns**\
[Popup](./Popup.md) 


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
### removeShortcut(shortcut)

Remove a shortcut.

**Parameters**\
[String](../../JSLib/String.md) shortcut  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


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
### showFormPopup(elementToShowRelatedTo, form, scope, dataproviderID)

Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope.

**Parameters**\
[Object](../../JSLib/Object.md) elementToShowRelatedTo element to show related to or null to center in screen\
[Object](../../JSLib/Object.md) form the form to show\
[Object](../../JSLib/Object.md) scope the scope to put retval into\
[String](../../JSLib/String.md) dataproviderID the dataprovider of scope to fill

**Returns**\
void 


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


**Sample**

```javascript
// Show a form as popup panel, where the closeFormPopup can pass return a value to a dataprovider in the specified scope.
plugins.window.showFormPopup(null,forms.orderPicker,foundset.getSelectedRecord(),"order_id");
// plugins.window.showFormPopup(null,forms.orderPicker,foundset.getSelectedRecord(),"order_id",-1,-1,100,100,true, false, onClose);
//
// function onClose(event) {application.output("Popup closed");}
```

