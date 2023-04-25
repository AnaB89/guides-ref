#  JSTab

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSForm](./JSForm.md) | [containsForm](JSTab.md#containsForm)                   | The name of the form displayed in the tab..                                    |
| [String](../JSLib/String.md) | [foreground](JSTab.md#foreground)                   | The foreground color of the tab..                                    |
| [JSMedia](./JSMedia.md) | [imageMedia](JSTab.md#imageMedia)                   | The name of the image Media file used..                                    |
| [String](../JSLib/String.md) | [mnemonic](JSTab.md#mnemonic)                   | Mnemonic used to switch to tab..                                    |
| [String](../JSLib/String.md) | [name](JSTab.md#name)                   | The name of the tab..                                    |
| [String](../JSLib/String.md) | [relationName](JSTab.md#relationName)                   | The name of the relation that links the form which contains the tab  with the form displayed in the tab..                                    |
| [String](../JSLib/String.md) | [text](JSTab.md#text)                   | The text on the tab..                                    |
| [String](../JSLib/String.md) | [toolTipText](JSTab.md#toolTipText)                   | The text displayed when hovering over the component with a mouse cursor..                                    |
| [Number](../JSLib/Number.md) | [x](JSTab.md#x)                   | The X coordinate of the tab..                                    |
| [Number](../JSLib/Number.md) | [y](JSTab.md#y)                   | The Y coordinate of the tab..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [getComment()](JSTab.md#getcomment)                   | Returns the comment of this component..                                    |
| [UUID](../Application/UUID.md) | [getUUID()](JSTab.md#getuuid)                   | Returns the UUID of this component..                                    |

## Properties Details

### containsForm

The name of the form displayed in the tab.

**Returns**\
[JSForm](./JSForm.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var childForm = solutionModel.newForm('childForm', 'db:/example_data/child_table', null, false, 400, 300);
var anotherChildForm = solutionModel.newForm('anotherChildForm', 'db:/example_data/child_table', null, false, 400, 300);
var firstTab = tabs.newTab('firstTab', 'Child Form', childForm, relation);
firstTab.containsForm = anotherChildForm;
```
### foreground

The foreground color of the tab.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var firstTab = tabs.newTab('firstTab', 'Child Form', childForm, relation);
firstTab.foreground = '#FF0000';
```
### imageMedia

The name of the image Media file used.

**Returns**\
[JSMedia](./JSMedia.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var bytes = plugins.file.readFile('d:/ball.jpg');
var ballImage = solutionModel.newMedia('ball.jpg', bytes);
var firstTab = tabs.newTab('firstTab', 'Child Form', childForm, relation);
firstTab.imageMedia = ballImage;
```
### mnemonic

Mnemonic used to switch to tab.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var childForm = solutionModel.newForm('childForm', 'db:/example_data/child_table', null, false, 400, 300);
var anotherChildForm = solutionModel.newForm('anotherChildForm', 'db:/example_data/child_table', null, false, 400, 300);
var firstTab = tabs.newTab('firstTab', 'Child Form', childForm, relation);
firstTab.mnemonic = 'a';
```
### name

The name of the tab.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var firstTab = tabs.newTab('firstTab', 'Child Form', childForm, relation);
firstTab.name = 'firstTabRenamed';
```
### relationName

The name of the relation that links the form which contains the tab 
with the form displayed in the tab.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var firstTab = tabs.newTab('firstTab', 'Child Form', childForm);
firstTab.relationName = 'parent_table_to_child_table';
```
### text

The text on the tab.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var firstTab = tabs.newTab('firstTab', 'Child Form', childForm, relation);
firstTab.text = 'Better Title';
```
### toolTipText

The text displayed when hovering over the component with a mouse cursor.

NOTE:
HTML should be used for multi-line tooltips; you can also use any
valid HTML tags to format tooltip text. For example:
<html>This includes<b>bolded text</b> and
<font color='blue'>BLUE</font> text as well.</html>

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var firstTab = tabs.newTab('firstTab', 'Child Form', childForm, relation);
firstTab.toolTipText = 'Tooltip';
```
### x

The X coordinate of the tab. This influences the order in which the tabs are displayed. 
The tabs are displayed in increasing order of the X coordinate. If two tabs have the 
same X coordinate, then they are displayed in increasing order of the Y coordinate.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Create two tabs, then make the second one be displayed to the left of the first
// by setting their X coordinates in the needed order.
var firstTab = tabs.newTab('firstTab', 'Child Form', childForm, relation);
firstTab.x = 10;
var secondTab = tabs.newTab('secondTab', 'Another Child Form', anotherChildForm);
secondTab.x = 0;
```
### y

The Y coordinate of the tab. Together with the X coordinate, this influences the order 
in which the tabs are displayed. The tabs are displayed in increasing order of the X coordinate,
and if two tabs have the same X coordinate, then they are displayed in increasing order 
of the Y coordinate.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Create two tabs, then make the second one be displayed to the left of the first
// by setting their X to the same value and Y coordinates in the needed order. 
var firstTab = tabs.newTab('firstTab', 'Child Form', childForm, relation);
firstTab.x = 0;
firstTab.y = 10;
var secondTab = tabs.newTab('secondTab', 'Another Child Form', anotherChildForm);
secondTab.x = 0;
secondTab.y = 0;
```

## Methods Details

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

