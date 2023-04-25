#  JSComponent


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [anchors](JSComponent.md#anchors)                   | Enables a component to stick to a specific side of form and/or to  grow or shrink when a window is resized..                                    |
| [String](../JSLib/String.md) | [background](JSComponent.md#background)                   | The background color of the component..                                    |
| [String](../JSLib/String.md) | [borderType](JSComponent.md#borderType)                   | The type, color and style of border of the component..                                    |
| [CSSPosition](../Application/CSSPosition.md) | [cssPosition](JSComponent.md#cssPosition)                   | CSS position is a replacement for anchoring system making it more intuitive to place a component..                                    |
| [Boolean](../JSLib/Boolean.md) | [enabled](JSComponent.md#enabled)                   | The enable state of the component, default true..                                    |
| [String](../JSLib/String.md) | [fontType](JSComponent.md#fontType)                   | The font type of the component..                                    |
| [String](../JSLib/String.md) | [foreground](JSComponent.md#foreground)                   | The foreground color of the component..                                    |
| [Number](../JSLib/Number.md) | [formIndex](JSComponent.md#formIndex)                   | The Z index of this component..                                    |
| [String](../JSLib/String.md) | [groupID](JSComponent.md#groupID)                   | A String representing a group ID for this component..                                    |
| [Number](../JSLib/Number.md) | [height](JSComponent.md#height)                   | The height in pixels of the component..                                    |
| [String](../JSLib/String.md) | [name](JSComponent.md#name)                   | The name of the component..                                    |
| [String](../JSLib/String.md) | [styleClass](JSComponent.md#styleClass)                   | The name of the style class that should be applied to this component..                                    |
| [Boolean](../JSLib/Boolean.md) | [transparent](JSComponent.md#transparent)                   | Flag that tells if the component is transparent or not..                                    |
| [Boolean](../JSLib/Boolean.md) | [visible](JSComponent.md#visible)                   | The visible property of the component, default true..                                    |
| [Number](../JSLib/Number.md) | [width](JSComponent.md#width)                   | The width in pixels of the component..                                    |
| [Number](../JSLib/Number.md) | [x](JSComponent.md#x)                   | The x coordinate of the component on the form..                                    |
| [Number](../JSLib/Number.md) | [y](JSComponent.md#y)                   | The y coordinate of the component on the form..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Object](../JSLib/Object.md) | [getAttribute(name)](JSComponent.md#getattribute-name)                   | Get the value of an attribute of the element..                                    |
| [Array](../JSLib/Array.md) | [getAttributes()](JSComponent.md#getattributes)                   | Returns the attribute names of an element..                                    |
| [String](../JSLib/String.md) | [getComment()](JSComponent.md#getcomment)                   | Returns the comment of this component..                                    |
| [Object](../JSLib/Object.md) | [getDesignTimeProperty(key)](JSComponent.md#getdesigntimeproperty-key)                   | Get a design-time property of an element..                                    |
| [Array](../JSLib/Array.md) | [getDesignTimePropertyNames()](JSComponent.md#getdesigntimepropertynames)                   | Get the design-time properties of an element..                                    |
| [String](../JSLib/String.md) | [getFormName()](JSComponent.md#getformname)                   | Returns the name of the form..                                    |
| [UUID](../Application/UUID.md) | [getUUID()](JSComponent.md#getuuid)                   | Returns the UUID of this component..                                    |
| [Object](../JSLib/Object.md) | [putDesignTimeProperty(key, value)](JSComponent.md#putdesigntimeproperty-key-value)                   | Set a design-time property of an element..                                    |
| [String](../JSLib/String.md) | [removeAttribute(name)](JSComponent.md#removeattribute-name)                   | Remove the attribute of an element..                                    |
| [Object](../JSLib/Object.md) | [removeDesignTimeProperty(key)](JSComponent.md#removedesigntimeproperty-key)                   | Clear a design-time property of an element..                                    |
|void | [setAttribute(name, value)](JSComponent.md#setattribute-name-value)                   | Set the attribute value of an element..                                    |

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
### background

The background color of the component.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
// This property can be used on all types of components.
// Here it is illustrated only for labels and fields.
var greenLabel = form.newLabel('Green',10,10,100,50);
greenLabel.background = 'green'; // Use generic names for colors.
var redField = form.newField('parent_table_text',JSField.TEXT_FIELD,10,110,100,30);
redField.background = '#FF0000'; // Use RGB codes for colors.
```
### borderType

The type, color and style of border of the component.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
//HINT: To know exactly the notation of this property set it in the designer and then read it once out through the solution model.
var field = form.newField('my_table_text', JSField.TEXT_FIELD, 10, 10, 100, 20);
field.borderType = solutionModel.createLineBorder(1,'#ff0000');
```
### cssPosition

CSS position is a replacement for anchoring system making it more intuitive to place a component.
CSS position should be set on form, an absolute position form can either work with anchoring or with css position.
This is only working in NGClient.

**Returns**\
[CSSPosition](../Application/CSSPosition.md) 


**Sample**

```javascript
var label = form.newLabel('Label', -1);
label.cssPosition.r("10").b("10").w("20%").h("30px")
```
### enabled

The enable state of the component, default true.

**Returns**\
[Boolean](../JSLib/Boolean.md) 


**Sample**

```javascript
var form = solutionModel.newForm('printForm', 'db:/example_data/parent_table', null, false, 400, 300);
var field = form.newField('parent_table_text', JSField.TEXT_FIELD, 10, 10, 100, 20);
field.enabled = false;
```
### fontType

The font type of the component.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var label = form.newLabel('Text here', 10, 50, 100, 20);
label.fontType = solutionModel.createFont('Times New Roman',1,14);
```
### foreground

The foreground color of the component.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
// This property can be used on all types of components.
// Here it is illustrated only for labels and fields.
var labelWithBlueText = form.newLabel('Blue text', 10, 10, 100, 30);
labelWithBlueText.foreground = 'blue'; // Use generic names for colors.
var fieldWithYellowText = form.newField('parent_table_text', JSField.TEXT_FIELD, 10, 50, 100, 20);
fieldWithYellowText.foreground = '#FFFF00'; // Use RGB codes for colors.
```
### formIndex

The Z index of this component. If two components overlap,
then the component with higher Z index is displayed above
the component with lower Z index.

**Returns**\
[Number](../JSLib/Number.md) 


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


**Sample**

```javascript
var form = solutionModel.newForm('someForm', 'db:/example_data/parent_table', null, false, 620, 300);
var label = form.newLabel('Label', 10, 10, 150, 150);
label.name = 'myLabel'; // Give a name to the component.
forms['someForm'].controller.show()
// Now use the name to access the component.
forms['someForm'].elements['myLabel'].text = 'Updated text';
```
### styleClass

The name of the style class that should be applied to this component.

When defining style classes for specific component types, their names
must be prefixed according to the type of the component. For example 
in order to define a class names 'fancy' for fields, in the style
definition the class must be named 'field.fancy'. If it would be 
intended for labels, then it would be named 'label.fancy'. When specifying
the class name for a component, the prefix is dropped however. Thus the
field or the label will have its styleClass property set to 'fancy' only.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var form = solutionModel.newForm('printForm', 'db:/example_data/parent_table', null, false, 400, 300);
var field = form.newField('parent_table_text', JSField.TEXT_FIELD, 10, 10, 100, 20);
var style = solutionModel.newStyle('myStyle','field.fancy { background-color: yellow; }');
form.styleName = 'myStyle'; // First set the style on the form.
field.styleClass = 'fancy'; // Then set the style class on the field.
```
### transparent

Flag that tells if the component is transparent or not.

The default value is "false", that is the components
are not transparent.

**Returns**\
[Boolean](../JSLib/Boolean.md) 


**Sample**

```javascript
// Load an image from disk an create a Media object based on it.
var imageBytes = plugins.file.readFile('d:/ball.jpg');
var media = solutionModel.newMedia('ball.jpg', imageBytes);
// Put on the form a label with the image.
var image = form.newLabel('', 10, 10, 100, 100);
image.imageMedia = media;
// Put two fields over the image. The second one will be transparent and the
// image will shine through.
var nonTransparentField = form.newField('parent_table_text', JSField.TEXT_FIELD, 10, 20, 100, 20);
var transparentField = form.newField('parent_table_text', JSField.TEXT_FIELD, 10, 50, 100, 20);
transparentField.transparent = true;
```
### visible

The visible property of the component, default true.

**Returns**\
[Boolean](../JSLib/Boolean.md) 


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


**Sample**

```javascript
var name = %%elementName%%.getFormName();
```
### getUUID()

Returns the UUID of this component.


**Returns**\
[UUID](../Application/UUID.md) 


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


**Sample**

```javascript
var frm = solutionModel.getForm('orders')
var fld = frm.getField('fld')
fld.setAttribute('keylistener', 'callback')
```

