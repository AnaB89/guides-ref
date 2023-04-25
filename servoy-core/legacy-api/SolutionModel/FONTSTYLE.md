#  FONTSTYLE

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [BOLD](FONTSTYLE.md#BOLD)                   | Bold font style..                                    |
| [Number](../JSLib/Number.md) | [BOLD_ITALIC](FONTSTYLE.md#BOLD_ITALIC)                   | Bold and italic font style..                                    |
| [Number](../JSLib/Number.md) | [ITALIC](FONTSTYLE.md#ITALIC)                   | Italic font style..                                    |
| [Number](../JSLib/Number.md) | [PLAIN](FONTSTYLE.md#PLAIN)                   | Plain(normal) font style..                                    |

## Constants Details

### BOLD

Bold font style.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
var component = form.getComponent("someComponent")
component.fontType = solutionModel.createFont('Arial',SM_FONTSTYLE.BOLD,12);
```
### BOLD_ITALIC

Bold and italic font style.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
var component = form.getComponent("someComponent")
component.fontType = solutionModel.createFont('Arial',SM_FONTSTYLE.BOLD_ITALIC,20);
```
### ITALIC

Italic font style.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
var component = form.getComponent("someComponent")
component.fontType = solutionModel.createFont('Arial',SM_FONTSTYLE.ITALIC,14);
```
### PLAIN

Plain(normal) font style.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
var component = form.getComponent("someComponent")
component.fontType = solutionModel.createFont('Arial',SM_FONTSTYLE.PLAIN,10);
```

