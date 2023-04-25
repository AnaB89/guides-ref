#  Form


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [borderType](Form.md#borderType)                   | The type, color and style of border..                                    |
| [String](../JSLib/String.md) | [comment](Form.md#comment)                   | .                                    |
| [String](../JSLib/String.md) | [dataSource](Form.md#dataSource)                   | The names of the database server and table that this form is linked to..                                    |
| [String](../JSLib/String.md) | [deprecated](Form.md#deprecated)                   | Gets the deprecate info for this element.                                    |
| [Object](../JSLib/Object.md) | [designTimeProperties](Form.md#designTimeProperties)                   | Property to get and add design-time properties for a component..                                    |
| [Number](../JSLib/Number.md) | [encapsulation](Form.md#encapsulation)                   | The encapsulation mode of this persist..                                    |
| [Number](../JSLib/Number.md) | [extendsForm](Form.md#extendsForm)                   | The selected parent (extended element) for the element (form)..                                    |
| [Boolean](../JSLib/Boolean.md) | [formComponent](Form.md#formComponent)                   | .                                    |
| [String](../JSLib/String.md) | [initialSort](Form.md#initialSort)                   | The default sort order only when the form loads..                                    |
| [String](../JSLib/String.md) | [name](Form.md#name)                   | The name of the form..                                    |
| [String](../JSLib/String.md) | [namedFoundSet](Form.md#namedFoundSet)                   | Property that tells the form to use a named foundset instead of the default foundset..                                    |
| [Number](../JSLib/Number.md) | [navigator](Form.md#navigator)                   | The navigator (previously named "controller") that is used to control/navigate to the form..                                    |
| [String](../JSLib/String.md) | [rowBGColorCalculation](Form.md#rowBGColorCalculation)                   | The calculation dataprovider used to add background color and highlight selected or alternate rows..                                    |
| [Number](../JSLib/Number.md) | [scrollbars](Form.md#scrollbars)                   | Scrollbar options for the vertical and horizontal scrollbars..                                    |
| [Number](../JSLib/Number.md) | [selectionMode](Form.md#selectionMode)                   | Returns the value of the selectionMode property..                                    |
| [String](../JSLib/String.md) | [styleClass](Form.md#styleClass)                   | The Cascading Style Sheet (CSS) class name applied to the form..                                    |
| [String](../JSLib/String.md) | [titleText](Form.md#titleText)                   | The text that displays in the title bar of the form window..                                    |
| [Boolean](../JSLib/Boolean.md) | [transparent](Form.md#transparent)                   | When set, the form is transparent..                                    |
| [Number](../JSLib/Number.md) | [view](Form.md#view)                   | The default form view mode..                                    |
| [Number](../JSLib/Number.md) | [width](Form.md#width)                   | The width of the form in pixels..                                    |

## Commands Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [void](../void.md) | [onSort](Form.md#onSort)                   | The method that overrides the Servoy menu item Select > Sort..                                    |

## Events Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../JSLib/Boolean.md) | [onBeforeHide(event)](Form.md#onbeforehide-event)                   | This method is triggered when the form wants to hide; this will be called before onHide, and should be used to return if this form can be hidden or not..                                    |
| [Boolean](../JSLib/Boolean.md) | [onElementDataChange(oldValue, newValue, event)](Form.md#onelementdatachange-oldvalue-newvalue-event)                   | Method that is executed when the data in one of the form's component is successfully changed and the onDataChange callback from the component does not exist or exists and returned true.                                    |
| [Boolean](../JSLib/Boolean.md) | [onElementFocusGained(event)](Form.md#onelementfocusgained-event)                   | The method that is triggered when focus is gained by a component inside the form..                                    |
| [Boolean](../JSLib/Boolean.md) | [onElementFocusLost(event)](Form.md#onelementfocuslost-event)                   | The method that gets triggered when focus is lost by a component inside the form..                                    |
| [void](../void.md) | [onHide(event)](Form.md#onhide-event)                   | This method is triggered when the form gets hidden..                                    |
| [void](../void.md) | [onLoad(event)](Form.md#onload-event)                   | The method that is triggered when a form is loaded/reloaded from the repository; used to alter elements, set globals, hide toolbars, etc; onShow method can also be assigned..                                    |
| [Boolean](../JSLib/Boolean.md) | [onRecordEditStart(event)](Form.md#onrecordeditstart-event)                   | The method that is triggered when a user clicks into a column on the form..                                    |
| [Boolean](../JSLib/Boolean.md) | [onRecordEditStop(record, event)](Form.md#onrecordeditstop-record-event)                   | The method that is triggered when a record is being saved..                                    |
| [void](../void.md) | [onRecordSelection(event)](Form.md#onrecordselection-event)                   | The method that is triggered each time a record is selected..                                    |
| [void](../void.md) | [onResize(event)](Form.md#onresize-event)                   | The method that gets triggered when resize occurs..                                    |
| [void](../void.md) | [onShow(firstShow, event)](Form.md#onshow-firstshow-event)                   | The method that is triggered EVERY TIME the form is displayed; an argument must be passed to the method if this is the first time the form is displayed..                                    |
| [void](../void.md) | [onUnLoad(event)](Form.md#onunload-event)                   | The method that is triggered when a form is unloaded from the repository..                                    |

## Properties Details

### borderType

The type, color and style of border.
This property is automatically set to "DEFAULT" when a new form is created.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### comment



**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### dataSource

The names of the database server and table that this form is linked to.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### deprecated

Gets the deprecate info for this element

**Returns**\
[String](../JSLib/String.md) the deprecate info for this element or null if it is not deprecated


**Sample**

```javascript

```
### designTimeProperties

Property to get and add design-time properties for a component.

**Returns**\
[Object](../JSLib/Object.md) map of the design-time properties


**Sample**

```javascript

```
### encapsulation

The encapsulation mode of this persist. The following can be used/checked:

- Public (not a separate option - if none of the below options are selected)
- Hide in scripting; Module Scope - not available in scripting from any other context except the form itself. Available in designer for the same module.
- Module Scope - available in both scripting and designer but only in the same module.
- Hide Dataproviders (checked by default)
- Hide Foundset (checked by default)
- Hide Controller (checked by default)
- Hide Elements (checked by default)

**Returns**\
[Number](../JSLib/Number.md) the encapsulation mode/level of the persist.


**Sample**

```javascript

```
### extendsForm

The selected parent (extended element) for the element (form).

**Returns**\
[Number](../JSLib/Number.md) the parent


**Sample**

```javascript

```
### formComponent



**Returns**\
[Boolean](../JSLib/Boolean.md) 


**Sample**

```javascript

```
### initialSort

The default sort order only when the form loads.
This is applied each time an internal SQL query is being executed (find, find-all, open form); and is only executed when no other manual sort has been performed on the foundset.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### name

The name of the form.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### namedFoundSet

Property that tells the form to use a named foundset instead of the default foundset.
When "separate" as special value is specified the form will always create a copy of assigned foundset and therefor become separated from other foundsets.
When "empty" it will initially load an empty foundset.
When a global relation name it will load the a related foundset.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### navigator

The navigator (previously named "controller")
that is used to control/navigate to the form. The navigator is shown at
the left or at the right side of the form, depending on the page orientation.

The following options are available:
-none- - no navigator is assigned.
DEFAULT - the Servoy default navigator is assigned.
IGNORE - the navigator last assigned to a previous form.
Custom - a custom navigator based on a selected form.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```
### rowBGColorCalculation

The calculation dataprovider used to add background color and highlight selected or alternate rows.
The default is -none-.

NOTE: This property has been deprecated and is kept visible for legacy purposes. Use CSS Row Styling & onRender event instead.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### scrollbars

Scrollbar options for the vertical and horizontal scrollbars. Each of the
vertical and horizontal scrollbars can be configured to display all the time,
to display only when needed or to never display.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```
### selectionMode

Returns the value of the selectionMode property.

**Returns**\
[Number](../JSLib/Number.md) one of IForm#SELECTION_MODE_DEFAULT, IForm#SELECTION_MODE_SINGLE and IForm#SELECTION_MODE_MULTI.


**Sample**

```javascript

```
### styleClass

The Cascading Style Sheet (CSS) class name applied to the form.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### titleText

The text that displays in the title bar of the form window.
NOTE: Data tags and Servoy tags can be used as part of the title text.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### transparent

When set, the form is transparent.

**Returns**\
[Boolean](../JSLib/Boolean.md) 


**Sample**

```javascript

```
### view

The default form view mode.

The view can be changed using a method at runtime. The following views are available:
- Record view
- List view
- Record view (locked)
- List view (locked)
- Table View (locked)

NOTE: Only Table View (locked) uses asynchronized related data loading.
This feature defers all related foundset data loading to the background - enhancing
the visual display of a related foundset.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```
### width

The width of the form in pixels.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```

