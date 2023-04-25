#  ToolBar

## **Supported Clients**

    SmartClient
    WebClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [addButton(text, method)](ToolBar.md#addbutton-text-method)                   | Add a Button to the toolbar..                                    |
|void | [addButton(text, method, arguments)](ToolBar.md#addbutton-text-method-arguments)                   | Add a Button to the toolbar..                                    |
|void | [addButton(text, method, arguments, icon)](ToolBar.md#addbutton-text-method-arguments-icon)                   | Add a Button to the toolbar..                                    |
|void | [addButton(text, method, arguments, icon, tooltip)](ToolBar.md#addbutton-text-method-arguments-icon-tooltip)                   | Add a Button to the toolbar..                                    |
|void | [addButton(text, method, arguments, icon, tooltip, enabled)](ToolBar.md#addbutton-text-method-arguments-icon-tooltip-enabled)                   | Add a Button to the toolbar..                                    |
|void | [addButton(text, method, arguments, icon, tooltip, enabled, visible)](ToolBar.md#addbutton-text-method-arguments-icon-tooltip-enabled-visible)                   | Add a Button to the toolbar..                                    |
|void | [addCheckBox(text, method)](ToolBar.md#addcheckbox-text-method)                   | Add a CheckBox to the toolbar..                                    |
|void | [addCheckBox(text, method, selected)](ToolBar.md#addcheckbox-text-method-selected)                   | Add a CheckBox to the toolbar..                                    |
|void | [addCheckBox(text, method, selected, tooltip)](ToolBar.md#addcheckbox-text-method-selected-tooltip)                   | Add a CheckBox to the toolbar..                                    |
|void | [addCheckBox(text, method, selected, tooltip, enabled)](ToolBar.md#addcheckbox-text-method-selected-tooltip-enabled)                   | Add a CheckBox to the toolbar..                                    |
|void | [addCheckBox(text, method, selected, tooltip, enabled, visible)](ToolBar.md#addcheckbox-text-method-selected-tooltip-enabled-visible)                   | Add a CheckBox to the toolbar..                                    |
|void | [addComboBox(method, index, values)](ToolBar.md#addcombobox-method-index-values)                   | Add a ComboBox to the toolbar..                                    |
|void | [addComboBox(method, index, values, tooltip)](ToolBar.md#addcombobox-method-index-values-tooltip)                   | Add a ComboBox to the toolbar..                                    |
|void | [addComboBox(method, index, values, tooltip, enabled)](ToolBar.md#addcombobox-method-index-values-tooltip-enabled)                   | Add a ComboBox to the toolbar..                                    |
|void | [addComboBox(method, index, values, tooltip, enabled, visible)](ToolBar.md#addcombobox-method-index-values-tooltip-enabled-visible)                   | Add a ComboBox to the toolbar..                                    |
|void | [addField(method, text)](ToolBar.md#addfield-method-text)                   | Add a Field to the toolbar..                                    |
|void | [addField(method, text, length)](ToolBar.md#addfield-method-text-length)                   | Add a Field to the toolbar..                                    |
|void | [addField(method, text, length, tooltip)](ToolBar.md#addfield-method-text-length-tooltip)                   | Add a Field to the toolbar..                                    |
|void | [addField(method, text, length, tooltip, enabled)](ToolBar.md#addfield-method-text-length-tooltip-enabled)                   | Add a Field to the toolbar..                                    |
|void | [addField(method, text, length, tooltip, enabled, visible)](ToolBar.md#addfield-method-text-length-tooltip-enabled-visible)                   | Add a Field to the toolbar..                                    |
|void | [addSeparator()](ToolBar.md#addseparator)                   | Add a Separator to the toolbar..                                    |
|void | [enableItem(index, enabled)](ToolBar.md#enableitem-index-enabled)                   | Enable/disable the item at the specified index..                                    |
|void | [removeAllItems()](ToolBar.md#removeallitems)                   | Remove all Buttons, Checkboxes etc..                                    |
|void | [removeItem(index)](ToolBar.md#removeitem-index)                   | Remove a Button, CheckBox, ComboBox from the toolbar..                                    |
|void | [selectCheckBox(index, selected)](ToolBar.md#selectcheckbox-index-selected)                   | Set the CheckBox selection..                                    |
|void | [selectComboBox(index, selection)](ToolBar.md#selectcombobox-index-selection)                   | Select a row of the ComboBox via the index..                                    |
|void | [setFieldText(index, text)](ToolBar.md#setfieldtext-index-text)                   | Set a (default) text of the field at the given index..                                    |
|void | [visibleItem(index, visible)](ToolBar.md#visibleitem-index-visible)                   | Make the item at the specified index visible/invisible..                                    |

## Methods Details

### addButton(text, method)

Add a Button to the toolbar.

**Parameters**\
[String](../../JSLib/String.md) text  ;\
[Function](../../JSLib/Function.md) method  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// create a new toolbar
var toolbar = plugins.window.addToolBar('toolbar_0');
// add a button with a text and a method
toolbar.addButton("button", feedback_button);
// add an input array to the button for feedback in the selected method
toolbar.addButton("button", feedback_button, [1, "2", "three"]);
// add an icon to the button
toolbar.addButton("button", feedback_button, [1, "2", "three"], "media:///yourimage.gif");
// add a tooltip to the button
toolbar.addButton("button", feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip");
// show only an icon on the button and disable the button
toolbar.addButton(null, feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip", false);
// make the button non visible
toolbar.addButton(null, feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip", true, false);
```
### addButton(text, method, arguments)

Add a Button to the toolbar.

**Parameters**\
[String](../../JSLib/String.md) text  ;\
[Function](../../JSLib/Function.md) method  ;\
[Array](../../JSLib/Array.md) arguments  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// create a new toolbar
var toolbar = plugins.window.addToolBar('toolbar_0');
// add a button with a text and a method
toolbar.addButton("button", feedback_button);
// add an input array to the button for feedback in the selected method
toolbar.addButton("button", feedback_button, [1, "2", "three"]);
// add an icon to the button
toolbar.addButton("button", feedback_button, [1, "2", "three"], "media:///yourimage.gif");
// add a tooltip to the button
toolbar.addButton("button", feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip");
// show only an icon on the button and disable the button
toolbar.addButton(null, feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip", false);
// make the button non visible
toolbar.addButton(null, feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip", true, false);
```
### addButton(text, method, arguments, icon)

Add a Button to the toolbar.

**Parameters**\
[String](../../JSLib/String.md) text  ;\
[Function](../../JSLib/Function.md) method  ;\
[Array](../../JSLib/Array.md) arguments  ;\
[Object](../../JSLib/Object.md) icon  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// create a new toolbar
var toolbar = plugins.window.addToolBar('toolbar_0');
// add a button with a text and a method
toolbar.addButton("button", feedback_button);
// add an input array to the button for feedback in the selected method
toolbar.addButton("button", feedback_button, [1, "2", "three"]);
// add an icon to the button
toolbar.addButton("button", feedback_button, [1, "2", "three"], "media:///yourimage.gif");
// add a tooltip to the button
toolbar.addButton("button", feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip");
// show only an icon on the button and disable the button
toolbar.addButton(null, feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip", false);
// make the button non visible
toolbar.addButton(null, feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip", true, false);
```
### addButton(text, method, arguments, icon, tooltip)

Add a Button to the toolbar.

**Parameters**\
[String](../../JSLib/String.md) text  ;\
[Function](../../JSLib/Function.md) method  ;\
[Array](../../JSLib/Array.md) arguments  ;\
[Object](../../JSLib/Object.md) icon  ;\
[String](../../JSLib/String.md) tooltip  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// create a new toolbar
var toolbar = plugins.window.addToolBar('toolbar_0');
// add a button with a text and a method
toolbar.addButton("button", feedback_button);
// add an input array to the button for feedback in the selected method
toolbar.addButton("button", feedback_button, [1, "2", "three"]);
// add an icon to the button
toolbar.addButton("button", feedback_button, [1, "2", "three"], "media:///yourimage.gif");
// add a tooltip to the button
toolbar.addButton("button", feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip");
// show only an icon on the button and disable the button
toolbar.addButton(null, feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip", false);
// make the button non visible
toolbar.addButton(null, feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip", true, false);
```
### addButton(text, method, arguments, icon, tooltip, enabled)

Add a Button to the toolbar.

**Parameters**\
[String](../../JSLib/String.md) text  ;\
[Function](../../JSLib/Function.md) method  ;\
[Array](../../JSLib/Array.md) arguments  ;\
[Object](../../JSLib/Object.md) icon  ;\
[String](../../JSLib/String.md) tooltip  ;\
[Boolean](../../JSLib/Boolean.md) enabled  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// create a new toolbar
var toolbar = plugins.window.addToolBar('toolbar_0');
// add a button with a text and a method
toolbar.addButton("button", feedback_button);
// add an input array to the button for feedback in the selected method
toolbar.addButton("button", feedback_button, [1, "2", "three"]);
// add an icon to the button
toolbar.addButton("button", feedback_button, [1, "2", "three"], "media:///yourimage.gif");
// add a tooltip to the button
toolbar.addButton("button", feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip");
// show only an icon on the button and disable the button
toolbar.addButton(null, feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip", false);
// make the button non visible
toolbar.addButton(null, feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip", true, false);
```
### addButton(text, method, arguments, icon, tooltip, enabled, visible)

Add a Button to the toolbar.

**Parameters**\
[String](../../JSLib/String.md) text  ;\
[Function](../../JSLib/Function.md) method  ;\
[Array](../../JSLib/Array.md) arguments  ;\
[Object](../../JSLib/Object.md) icon  ;\
[String](../../JSLib/String.md) tooltip  ;\
[Boolean](../../JSLib/Boolean.md) enabled  ;\
[Boolean](../../JSLib/Boolean.md) visible  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// create a new toolbar
var toolbar = plugins.window.addToolBar('toolbar_0');
// add a button with a text and a method
toolbar.addButton("button", feedback_button);
// add an input array to the button for feedback in the selected method
toolbar.addButton("button", feedback_button, [1, "2", "three"]);
// add an icon to the button
toolbar.addButton("button", feedback_button, [1, "2", "three"], "media:///yourimage.gif");
// add a tooltip to the button
toolbar.addButton("button", feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip");
// show only an icon on the button and disable the button
toolbar.addButton(null, feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip", false);
// make the button non visible
toolbar.addButton(null, feedback_button, [1, "2", "three"], "media:///yourimage.gif", "tooltip", true, false);
```
### addCheckBox(text, method)

Add a CheckBox to the toolbar.

**Parameters**\
[String](../../JSLib/String.md) text  ;\
[Function](../../JSLib/Function.md) method  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_1");
// add a checkbox with a text and a method
toolbar.addCheckBox("checkbox", feedback_checkbox);
// add an checkbox and set it's state to selected (not selected by default)
toolbar.addCheckBox("checkbox", feedback_checkbox, true);
// add a tooltip to the checkbox
toolbar.addCheckBox("checkbox", feedback_checkbox, false, "tooltip");
// disable the checkbox and select it
toolbar.addCheckBox("checkbox", feedback_checkbox, true, "tooltip", false);
// make the checkbox non visible
toolbar.addCheckBox("checkbox", feedback_checkbox, false, "tooltip", false, false);
```
### addCheckBox(text, method, selected)

Add a CheckBox to the toolbar.

**Parameters**\
[String](../../JSLib/String.md) text  ;\
[Function](../../JSLib/Function.md) method  ;\
[Boolean](../../JSLib/Boolean.md) selected  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_1");
// add a checkbox with a text and a method
toolbar.addCheckBox("checkbox", feedback_checkbox);
// add an checkbox and set it's state to selected (not selected by default)
toolbar.addCheckBox("checkbox", feedback_checkbox, true);
// add a tooltip to the checkbox
toolbar.addCheckBox("checkbox", feedback_checkbox, false, "tooltip");
// disable the checkbox and select it
toolbar.addCheckBox("checkbox", feedback_checkbox, true, "tooltip", false);
// make the checkbox non visible
toolbar.addCheckBox("checkbox", feedback_checkbox, false, "tooltip", false, false);
```
### addCheckBox(text, method, selected, tooltip)

Add a CheckBox to the toolbar.

**Parameters**\
[String](../../JSLib/String.md) text  ;\
[Function](../../JSLib/Function.md) method  ;\
[Boolean](../../JSLib/Boolean.md) selected  ;\
[String](../../JSLib/String.md) tooltip  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_1");
// add a checkbox with a text and a method
toolbar.addCheckBox("checkbox", feedback_checkbox);
// add an checkbox and set it's state to selected (not selected by default)
toolbar.addCheckBox("checkbox", feedback_checkbox, true);
// add a tooltip to the checkbox
toolbar.addCheckBox("checkbox", feedback_checkbox, false, "tooltip");
// disable the checkbox and select it
toolbar.addCheckBox("checkbox", feedback_checkbox, true, "tooltip", false);
// make the checkbox non visible
toolbar.addCheckBox("checkbox", feedback_checkbox, false, "tooltip", false, false);
```
### addCheckBox(text, method, selected, tooltip, enabled)

Add a CheckBox to the toolbar.

**Parameters**\
[String](../../JSLib/String.md) text  ;\
[Function](../../JSLib/Function.md) method  ;\
[Boolean](../../JSLib/Boolean.md) selected  ;\
[String](../../JSLib/String.md) tooltip  ;\
[Boolean](../../JSLib/Boolean.md) enabled  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_1");
// add a checkbox with a text and a method
toolbar.addCheckBox("checkbox", feedback_checkbox);
// add an checkbox and set it's state to selected (not selected by default)
toolbar.addCheckBox("checkbox", feedback_checkbox, true);
// add a tooltip to the checkbox
toolbar.addCheckBox("checkbox", feedback_checkbox, false, "tooltip");
// disable the checkbox and select it
toolbar.addCheckBox("checkbox", feedback_checkbox, true, "tooltip", false);
// make the checkbox non visible
toolbar.addCheckBox("checkbox", feedback_checkbox, false, "tooltip", false, false);
```
### addCheckBox(text, method, selected, tooltip, enabled, visible)

Add a CheckBox to the toolbar.

**Parameters**\
[String](../../JSLib/String.md) text  ;\
[Function](../../JSLib/Function.md) method  ;\
[Boolean](../../JSLib/Boolean.md) selected  ;\
[String](../../JSLib/String.md) tooltip  ;\
[Boolean](../../JSLib/Boolean.md) enabled  ;\
[Boolean](../../JSLib/Boolean.md) visible  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_1");
// add a checkbox with a text and a method
toolbar.addCheckBox("checkbox", feedback_checkbox);
// add an checkbox and set it's state to selected (not selected by default)
toolbar.addCheckBox("checkbox", feedback_checkbox, true);
// add a tooltip to the checkbox
toolbar.addCheckBox("checkbox", feedback_checkbox, false, "tooltip");
// disable the checkbox and select it
toolbar.addCheckBox("checkbox", feedback_checkbox, true, "tooltip", false);
// make the checkbox non visible
toolbar.addCheckBox("checkbox", feedback_checkbox, false, "tooltip", false, false);
```
### addComboBox(method, index, values)

Add a ComboBox to the toolbar.

**Parameters**\
[Function](../../JSLib/Function.md) method  ;\
[Number](../../JSLib/Number.md) index  ;\
[Array](../../JSLib/Array.md) values  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_2");
// add a combobox with the attached method, selected index and input (list) array
toolbar.addComboBox(feedback_combobox, 0, ["input","array","combobox",1]);
// add a tooltip to the combobox
toolbar.addComboBox(feedback_combobox, 1, ["input","array","combobox",2], "tooltip");
// disable the combobox
toolbar.addComboBox(feedback_combobox, 2, ["input","array","combobox",3], "tooltip", false);
// make the combobox non visible
toolbar.addComboBox(feedback_combobox, 3, ["input","array","combobox",4], "tooltip", false, false);
```
### addComboBox(method, index, values, tooltip)

Add a ComboBox to the toolbar.

**Parameters**\
[Function](../../JSLib/Function.md) method  ;\
[Number](../../JSLib/Number.md) index  ;\
[Array](../../JSLib/Array.md) values  ;\
[String](../../JSLib/String.md) tooltip  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_2");
// add a combobox with the attached method, selected index and input (list) array
toolbar.addComboBox(feedback_combobox, 0, ["input","array","combobox",1]);
// add a tooltip to the combobox
toolbar.addComboBox(feedback_combobox, 1, ["input","array","combobox",2], "tooltip");
// disable the combobox
toolbar.addComboBox(feedback_combobox, 2, ["input","array","combobox",3], "tooltip", false);
// make the combobox non visible
toolbar.addComboBox(feedback_combobox, 3, ["input","array","combobox",4], "tooltip", false, false);
```
### addComboBox(method, index, values, tooltip, enabled)

Add a ComboBox to the toolbar.

**Parameters**\
[Function](../../JSLib/Function.md) method  ;\
[Number](../../JSLib/Number.md) index  ;\
[Array](../../JSLib/Array.md) values  ;\
[String](../../JSLib/String.md) tooltip  ;\
[Boolean](../../JSLib/Boolean.md) enabled  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_2");
// add a combobox with the attached method, selected index and input (list) array
toolbar.addComboBox(feedback_combobox, 0, ["input","array","combobox",1]);
// add a tooltip to the combobox
toolbar.addComboBox(feedback_combobox, 1, ["input","array","combobox",2], "tooltip");
// disable the combobox
toolbar.addComboBox(feedback_combobox, 2, ["input","array","combobox",3], "tooltip", false);
// make the combobox non visible
toolbar.addComboBox(feedback_combobox, 3, ["input","array","combobox",4], "tooltip", false, false);
```
### addComboBox(method, index, values, tooltip, enabled, visible)

Add a ComboBox to the toolbar.

**Parameters**\
[Function](../../JSLib/Function.md) method  ;\
[Number](../../JSLib/Number.md) index  ;\
[Array](../../JSLib/Array.md) values  ;\
[String](../../JSLib/String.md) tooltip  ;\
[Boolean](../../JSLib/Boolean.md) enabled  ;\
[Boolean](../../JSLib/Boolean.md) visible  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_2");
// add a combobox with the attached method, selected index and input (list) array
toolbar.addComboBox(feedback_combobox, 0, ["input","array","combobox",1]);
// add a tooltip to the combobox
toolbar.addComboBox(feedback_combobox, 1, ["input","array","combobox",2], "tooltip");
// disable the combobox
toolbar.addComboBox(feedback_combobox, 2, ["input","array","combobox",3], "tooltip", false);
// make the combobox non visible
toolbar.addComboBox(feedback_combobox, 3, ["input","array","combobox",4], "tooltip", false, false);
```
### addField(method, text)

Add a Field to the toolbar.

**Parameters**\
[Function](../../JSLib/Function.md) method  ;\
[String](../../JSLib/String.md) text  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_3");
// add a field with the attached method and a default text
toolbar.addField(feedback_field, null);
// set the length of the field. 
// default length = 8 when length is not set or set to 0
toolbar.addField(feedback_field, "field", 0, "tooltip");
// add a tooltip to the field
toolbar.addField(feedback_field, null, 10, "tooltip");
// disable the field
toolbar.addField(feedback_field, "field", 5, "tooltip", false);
// make the field non visible
toolbar.addField(feedback_field, "field", 0, "tooltip", false, false);
```
### addField(method, text, length)

Add a Field to the toolbar.

**Parameters**\
[Function](../../JSLib/Function.md) method  ;\
[String](../../JSLib/String.md) text  ;\
[Number](../../JSLib/Number.md) length  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_3");
// add a field with the attached method and a default text
toolbar.addField(feedback_field, null);
// set the length of the field. 
// default length = 8 when length is not set or set to 0
toolbar.addField(feedback_field, "field", 0, "tooltip");
// add a tooltip to the field
toolbar.addField(feedback_field, null, 10, "tooltip");
// disable the field
toolbar.addField(feedback_field, "field", 5, "tooltip", false);
// make the field non visible
toolbar.addField(feedback_field, "field", 0, "tooltip", false, false);
```
### addField(method, text, length, tooltip)

Add a Field to the toolbar.

**Parameters**\
[Function](../../JSLib/Function.md) method  ;\
[String](../../JSLib/String.md) text  ;\
[Number](../../JSLib/Number.md) length  ;\
[String](../../JSLib/String.md) tooltip  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_3");
// add a field with the attached method and a default text
toolbar.addField(feedback_field, null);
// set the length of the field. 
// default length = 8 when length is not set or set to 0
toolbar.addField(feedback_field, "field", 0, "tooltip");
// add a tooltip to the field
toolbar.addField(feedback_field, null, 10, "tooltip");
// disable the field
toolbar.addField(feedback_field, "field", 5, "tooltip", false);
// make the field non visible
toolbar.addField(feedback_field, "field", 0, "tooltip", false, false);
```
### addField(method, text, length, tooltip, enabled)

Add a Field to the toolbar.

**Parameters**\
[Function](../../JSLib/Function.md) method  ;\
[String](../../JSLib/String.md) text  ;\
[Number](../../JSLib/Number.md) length  ;\
[String](../../JSLib/String.md) tooltip  ;\
[Boolean](../../JSLib/Boolean.md) enabled  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_3");
// add a field with the attached method and a default text
toolbar.addField(feedback_field, null);
// set the length of the field. 
// default length = 8 when length is not set or set to 0
toolbar.addField(feedback_field, "field", 0, "tooltip");
// add a tooltip to the field
toolbar.addField(feedback_field, null, 10, "tooltip");
// disable the field
toolbar.addField(feedback_field, "field", 5, "tooltip", false);
// make the field non visible
toolbar.addField(feedback_field, "field", 0, "tooltip", false, false);
```
### addField(method, text, length, tooltip, enabled, visible)

Add a Field to the toolbar.

**Parameters**\
[Function](../../JSLib/Function.md) method  ;\
[String](../../JSLib/String.md) text  ;\
[Number](../../JSLib/Number.md) length  ;\
[String](../../JSLib/String.md) tooltip  ;\
[Boolean](../../JSLib/Boolean.md) enabled  ;\
[Boolean](../../JSLib/Boolean.md) visible  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_3");
// add a field with the attached method and a default text
toolbar.addField(feedback_field, null);
// set the length of the field. 
// default length = 8 when length is not set or set to 0
toolbar.addField(feedback_field, "field", 0, "tooltip");
// add a tooltip to the field
toolbar.addField(feedback_field, null, 10, "tooltip");
// disable the field
toolbar.addField(feedback_field, "field", 5, "tooltip", false);
// make the field non visible
toolbar.addField(feedback_field, "field", 0, "tooltip", false, false);
```
### addSeparator()

Add a Separator to the toolbar.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_0");
// add a button 
toolbar.addButton("button", feedback_button);
// add a separator
toolbar.addSeparator();
// add a checkbox
toolbar.addCheckBox("checkbox", feedback_checkbox);
```
### enableItem(index, enabled)

Enable/disable the item at the specified index.

**Parameters**\
[Number](../../JSLib/Number.md) index  ;\
[Boolean](../../JSLib/Boolean.md) enabled  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_1");
// add a checkbox
toolbar.addCheckBox("checkbox", feedback_checkbox);
// disable the button
// REMARK: the pitfall here is that the indexes start at position 1 here
// position 0 is reserved for the toolbar handle!
toolbar.enableItem(1, false);
```
### removeAllItems()

Remove all Buttons, Checkboxes etc. from the toolbar.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_1");
// add a button
toolbar.addButton("button", feedback_button);
// add a checkbox
toolbar.addCheckBox("checkbox", feedback_checkbox);
// remove all items from the toolbar
toolbar.removeAllItems();
```
### removeItem(index)

Remove a Button, CheckBox, ComboBox from the toolbar.

**Parameters**\
[Number](../../JSLib/Number.md) index  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_1");
// add a button
toolbar.addButton("button", feedback_button);
// add a checkbox
toolbar.addCheckBox("checkbox", feedback_checkbox);
// remove the first item (the button in this case) from the toolbar
// REMARK: the pitfall here is that the indexes start at position 1 here
// position 0 is reserved for the toolbar handle!
toolbar.removeItem(1);
```
### selectCheckBox(index, selected)

Set the CheckBox selection.

**Parameters**\
[Number](../../JSLib/Number.md) index  ;\
[Boolean](../../JSLib/Boolean.md) selected  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_1");
// add a checkbox
toolbar.addCheckBox("checkbox 1", feedback_checkbox);
// add another checkbox
toolbar.addCheckBox("checkbox 2", feedback_checkbox);
// set the selection of the checkboxes
// REMARK: the pitfall here is that the indexes start at position 1 here
// position 0 is reserved for the toolbar handle!
toolbar.selectCheckBox(1, false);
toolbar.selectCheckBox(2, true);
```
### selectComboBox(index, selection)

Select a row of the ComboBox via the index.

**Parameters**\
[Number](../../JSLib/Number.md) index  ;\
[Number](../../JSLib/Number.md) selection  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_1");
// add a combobox
toolbar.addComboBox(feedback_combobox, 1, ["one", "two", "three"]);
// add another combobox
toolbar.addComboBox(feedback_combobox, 2, [1, 2, 3, 4, 5]);
// set the selection of the comboboxes
// REMARK: the pitfall here is that the indexes start at position 1 here
// position 0 is reserved for the toolbar handle!
toolbar.selectComboBox(1, 0); // entry "one" will be selected in the first combobox
toolbar.selectComboBox(2, 3); // entry 4 will be selected in the second combobox
```
### setFieldText(index, text)

Set a (default) text of the field at the given index.

**Parameters**\
[Number](../../JSLib/Number.md) index  ;\
[String](../../JSLib/String.md) text  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_1");
// add a field
toolbar.addField(feedback_field, "field one");
// add another field
toolbar.addField(feedback_field , "field_two");
// set the text of the fields
// REMARK: the pitfall here is that the indexes start at position 1 here
// position 0 is reserved for the toolbar handle!
toolbar.setFieldText(1, "new text 1");
toolbar.setFieldText(2, "new text 2");
```
### visibleItem(index, visible)

Make the item at the specified index visible/invisible.

**Parameters**\
[Number](../../JSLib/Number.md) index  ;\
[Boolean](../../JSLib/Boolean.md) visible  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
// add a toolbar
var toolbar = plugins.window.addToolBar("toolbar_1");
// add a button
toolbar.addButton("button", feedback_button);
// add a checkbox
toolbar.addCheckBox("checkbox", feedback_checkbox);
// make the first item (the button) invisible
// REMARK: the pitfall here is that the indexes start at position 1 here
// position 0 is reserved for the toolbar handle!
toolbar.visibleItem(1, false);
```

