#  JSBean

## **Supported Clients**

    SmartClient
    WebClient
    MobileClient

## **Extends**
    JSComponent

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [anchors](JSBean.md#anchors)                   | Enables a component to stick to a specific side of form and/or to  grow or shrink when a window is resized..                                    |
| [String](../JSLib/String.md) | [className](JSBean.md#className)                   | The bean class name..                                    |
| [Boolean](../JSLib/Boolean.md) | [enabled](JSBean.md#enabled)                   | The enable state of the component, default true..                                    |
| [Number](../JSLib/Number.md) | [formIndex](JSBean.md#formIndex)                   | The Z index of this component..                                    |
| [String](../JSLib/String.md) | [groupID](JSBean.md#groupID)                   | A String representing a group ID for this component..                                    |
| [Number](../JSLib/Number.md) | [height](JSBean.md#height)                   | The height in pixels of the component..                                    |
| [String](../JSLib/String.md) | [name](JSBean.md#name)                   | The name of the component..                                    |
| [Boolean](../JSLib/Boolean.md) | [printable](JSBean.md#printable)                   | Flag that tells if the component should be printed or not when the form is printed..                                    |
| [Boolean](../JSLib/Boolean.md) | [visible](JSBean.md#visible)                   | The visible property of the component, default true..                                    |
| [Number](../JSLib/Number.md) | [width](JSBean.md#width)                   | The width in pixels of the component..                                    |
| [Number](../JSLib/Number.md) | [x](JSBean.md#x)                   | The x coordinate of the component on the form..                                    |
| [Number](../JSLib/Number.md) | [y](JSBean.md#y)                   | The y coordinate of the component on the form..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Object](../JSLib/Object.md) | [getAttribute(name)](JSBean.md#getattribute-name)                   | Get the value of an attribute of the element..                                    |
| [Array](../JSLib/Array.md) | [getAttributes()](JSBean.md#getattributes)                   | Returns the attribute names of an element..                                    |
| [String](../JSLib/String.md) | [getComment()](JSBean.md#getcomment)                   | Returns the comment of this component..                                    |
| [Object](../JSLib/Object.md) | [getDesignTimeProperty(key)](JSBean.md#getdesigntimeproperty-key)                   | Get a design-time property of an element..                                    |
| [Array](../JSLib/Array.md) | [getDesignTimePropertyNames()](JSBean.md#getdesigntimepropertynames)                   | Get the design-time properties of an element..                                    |
| [String](../JSLib/String.md) | [getFormName()](JSBean.md#getformname)                   | Returns the name of the form..                                    |
| [UUID](../Application/UUID.md) | [getUUID()](JSBean.md#getuuid)                   | Returns the UUID of this component..                                    |
| [Object](../JSLib/Object.md) | [putDesignTimeProperty(key, value)](JSBean.md#putdesigntimeproperty-key-value)                   | Set a design-time property of an element..                                    |
| [String](../JSLib/String.md) | [removeAttribute(name)](JSBean.md#removeattribute-name)                   | Remove the attribute of an element..                                    |
| [Object](../JSLib/Object.md) | [removeDesignTimeProperty(key)](JSBean.md#removedesigntimeproperty-key)                   | Clear a design-time property of an element..                                    |
|void | [setAttribute(name, value)](JSBean.md#setattribute-name-value)                   | Set the attribute value of an element..                                    |

## Properties Details

### anchors

Enables a component to stick to a specific side of form and/or to 
grow or shrink when a window is resized. 

If opposite anchors are activated then the component with grow or 
shrink with the window. For example if Top and Bottom are activated, 
then the component will grow/shrink when the window is vertically 
resized. If Left and Right are activated then the component
will grow/shrink when the window is horizontally resized. 

If opposite anchors are not activated, then the component will 
keep a constant distance from the sides of the window which
correspond to the activated anchors.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = solutionModel.newForm('mediaForm', 'db:/example_data/parent_table', null, false, 400, 300);
var strechAllDirectionsLabel = form.newLabel('Strech all directions', 10, 10, 380, 280);
strechAllDirectionsLabel.background = 'red';
strechAllDirectionsLabel.anchors = SM_ANCHOR.ALL;
var strechVerticallyLabel = form.newLabel('Strech vertically', 10, 10, 190, 280);
strechVerticallyLabel.background = 'green';
strechVerticallyLabel.anchors = SM_ANCHOR.WEST | SM_ANCHOR.NORTH | SM_ANCHOR.SOUTH;
var strechHorizontallyLabel = form.newLabel('Strech horizontally', 10, 10, 380, 140);
strechHorizontallyLabel.background = 'blue';
strechHorizontallyLabel.anchors = SM_ANCHOR.NORTH | SM_ANCHOR.WEST | SM_ANCHOR.EAST;
var stickToTopLeftCornerLabel = form.newLabel('Stick to top-left corner', 10, 10, 200, 100);
stickToTopLeftCornerLabel.background = 'orange';
stickToTopLeftCornerLabel.anchors = SM_ANCHOR.NORTH | SM_ANCHOR.WEST; // This is equivalent to SM_ANCHOR.DEFAULT
var stickToBottomRightCornerLabel = form.newLabel('Stick to bottom-right corner', 190, 190, 200, 100);
stickToBottomRightCornerLabel.background = 'pink';
stickToBottomRightCornerLabel.anchors = SM_ANCHOR.SOUTH | SM_ANCHOR.EAST;
```
### className

The bean class name.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var bean = form.getBean('mybean');
application.output(bean.className);
```
### enabled

The enable state of the component, default true.

**Returns**\
[Boolean](../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var form = solutionModel.newForm('printForm', 'db:/example_data/parent_table', null, false, 400, 300);
var field = form.newField('parent_table_text', JSField.TEXT_FIELD, 10, 10, 100, 20);
field.enabled = false;
```
### formIndex

The Z index of this component. If two components overlap,
then the component with higher Z index is displayed above
the component with lower Z index.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var labelBelow = form.newLabel('Green', 10, 10, 100, 50);
labelBelow.background = 'green';
labelBelow.formIndex = 10;
var fieldAbove = form.newField('parent_table_text', JSField.TEXT_FIELD, 10, 10, 100, 30);
fieldAbove.background = '#FF0000';
fieldAbove.formIndex = 20;
```
### groupID

A String representing a group ID for this component. If several
components have the same group ID then they belong to the same
group of components. Using the group itself, all components can
be disabled/enabled or made invisible/visible.
The group id should be a javascript compatible identifier to allow access of the group in scripting.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = solutionModel.newForm('someForm', 'db:/example_data/parent_table', null, false, 400, 300);
var label = form.newLabel('Green', 10, 10, 100, 20);
var field = form.newField('parent_table_text', JSField.TEXT_FIELD, 10, 40, 100, 20);
label.groupID = 'someGroup';
field.groupID = 'someGroup';
forms['someForm'].elements.someGroup.enabled = false;
```
### height

The height in pixels of the component.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var field = form.newField('parent_table_text', JSField.TEXT_FIELD, 10, 10, 100, 20);
application.output('original width: ' + field.width);
application.output('original height: ' + field.height);
field.width = 200;
field.height = 100;
application.output('modified width: ' + field.width);
application.output('modified height: ' + field.height);
```
### name

The name of the component. Through this name it can also accessed in methods.
Must be a valid javascript name. (no - in the name or start with number)

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var form = solutionModel.newForm('someForm', 'db:/example_data/parent_table', null, false, 620, 300);
var label = form.newLabel('Label', 10, 10, 150, 150);
label.name = 'myLabel'; // Give a name to the component.
forms['someForm'].controller.show()
// Now use the name to access the component.
forms['someForm'].elements['myLabel'].text = 'Updated text';
```
### printable

Flag that tells if the component should be printed or not when the form is printed.

By default components are printable.

**Returns**\
[Boolean](../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
var form = solutionModel.newForm('printForm', 'db:/example_data/parent_table', null, false, 400, 300);
var printedField = form.newField('parent_table_text', JSField.TEXT_FIELD, 10, 10, 100, 20);
var notPrintedField = form.newField('parent_table_id', JSField.TEXT_FIELD, 10, 40, 100, 20);
notPrintedField.printable = false; // This field won't show up in print preview and won't be printed.
forms['printForm'].controller.showPrintPreview()
```
### visible

The visible property of the component, default true.

**Returns**\
[Boolean](../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var form = solutionModel.newForm('printForm', 'db:/example_data/parent_table', null, false, 400, 300);
var field = form.newField('parent_table_text', JSField.TEXT_FIELD, 10, 10, 100, 20);
field.visible = false;
```
### width

The width in pixels of the component.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var field = form.newField('parent_table_text', JSField.TEXT_FIELD, 10, 10, 100, 20);
application.output('original width: ' + field.width);
application.output('original height: ' + field.height);
field.width = 200;
field.height = 100;
application.output('modified width: ' + field.width);
application.output('modified height: ' + field.height);
```
### x

The x coordinate of the component on the form.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var field = form.newField('parent_table_text', JSField.TEXT_FIELD, 10, 10, 100, 20);
application.output('original location: ' + field.x + ', ' + field.y);
field.x = 90;
field.y = 90;
application.output('changed location: ' + field.x + ', ' + field.y);
```
### y

The y coordinate of the component on the form.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var field = form.newField('parent_table_text', JSField.TEXT_FIELD, 10, 10, 100, 20);
application.output('original location: ' + field.x + ', ' + field.y);
field.x = 90;
field.y = 90;
application.output('changed location: ' + field.x + ', ' + field.y);
```

## Methods Details

### getAttribute(name)

Get the value of an attribute of the element.

**Parameters**\
[String](../JSLib/String.md) name the name of the attribute

**Returns**\
[Object](../JSLib/Object.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var frm = solutionModel.getForm('orders')
var fld = frm.getField('fld')
var attributes = fld.getAttributes();
for (var i = 0; i < attributes.length; i++)
{
		application.output(fld.getAttribute(attributes[i]));
}
```
### getAttributes()

Returns the attribute names of an element.


**Returns**\
[Array](../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var frm = solutionModel.getForm('orders')
var fld = frm.getField('fld')
var attributes = fld.getAttributes();
for (var i = 0; i < attributes.length; i++)
{
		application.output(fld.getAttribute(attributes[i]));
}
```
### getComment()

Returns the comment of this component.


**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var comment = solutionModel.getForm("my_form").getButton("my_button").getComment();
application.output(comment);
```
### getDesignTimeProperty(key)

Get a design-time property of an element.

**Parameters**\
[String](../JSLib/String.md) key the name of the property

**Returns**\
[Object](../JSLib/Object.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var frm = solutionModel.getForm('orders')
var fld = frm.getField('fld')
var prop = fld.getDesignTimeProperty('myprop')
```
### getDesignTimePropertyNames()

Get the design-time properties of an element.


**Returns**\
[Array](../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var frm = solutionModel.getForm('orders')
var fld = frm.getField('fld')
var propNames = fld.getDesignTimePropertyNames()
```
### getFormName()

Returns the name of the form. (may be empty string as well)


**Returns**\
[String](../JSLib/String.md) The name of the form.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var name = %%elementName%%.getFormName();
```
### getUUID()

Returns the UUID of this component.


**Returns**\
[UUID](../Application/UUID.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var button_uuid = solutionModel.getForm("my_form").getButton("my_button").getUUID();
application.output(button_uuid.toString());
```
### putDesignTimeProperty(key, value)

Set a design-time property of an element.

**Parameters**\
[String](../JSLib/String.md) key the name of the property\
[Object](../JSLib/Object.md) value the value to store

**Returns**\
[Object](../JSLib/Object.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var frm = solutionModel.getForm('orders')
var fld = frm.getField('fld')
fld.putDesignTimeProperty('myprop', 'strawberry')
```
### removeAttribute(name)

Remove the attribute of an element.

**Parameters**\
[String](../JSLib/String.md) name the name of the attribute

**Returns**\
[String](../JSLib/String.md) the deleted attribute value

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var frm = solutionModel.getForm('orders')
var fld = frm.getField('fld')
fld.removeAttribute('keylistener')
```
### removeDesignTimeProperty(key)

Clear a design-time property of an element.

**Parameters**\
[String](../JSLib/String.md) key the name of the property

**Returns**\
[Object](../JSLib/Object.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var frm = solutionModel.getForm('orders')
var fld = frm.getField('fld')
fld.removeDesignTimeProperty('myprop')
```
### setAttribute(name, value)

Set the attribute value of an element.

**Parameters**\
[String](../JSLib/String.md) name the name of the attribute\
[String](../JSLib/String.md) value the value of the attribute

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var frm = solutionModel.getForm('orders')
var fld = frm.getField('fld')
fld.setAttribute('keylistener', 'callback')
```

