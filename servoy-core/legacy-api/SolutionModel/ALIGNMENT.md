#  ALIGNMENT

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [BOTTOM](ALIGNMENT.md#BOTTOM)                   | Constant used for setting vertical alignment for components..                                    |
| [Number](../JSLib/Number.md) | [CENTER](ALIGNMENT.md#CENTER)                   | Constant used for setting horizontal and vertical alignment for components..                                    |
| [Number](../JSLib/Number.md) | [DEFAULT](ALIGNMENT.md#DEFAULT)                   | Constant used for setting horizontal and vertical alignment..                                    |
| [Number](../JSLib/Number.md) | [LEFT](ALIGNMENT.md#LEFT)                   | Constant used for setting horizontal alignment for components..                                    |
| [Number](../JSLib/Number.md) | [RIGHT](ALIGNMENT.md#RIGHT)                   | Constant used for setting horizontal alignment for components..                                    |
| [Number](../JSLib/Number.md) | [TOP](ALIGNMENT.md#TOP)                   | Constant used for setting vertical alignment for components..                                    |

## Constants Details

### BOTTOM

Constant used for setting vertical alignment for components.
It makes the text inside the component be bottom aligned vertically.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var bottomAlignedLabel = form.newLabel('BOTTOM', 520, 10, 50, 300);
bottomAlignedLabel.verticalAlignment = SM_ALIGNMENT.BOTTOM;
```
### CENTER

Constant used for setting horizontal and vertical alignment
for components. If used for horizontal alignment,
then the text of the component will be horizontally centered.
Similarly, if used for vertical alignment, then the text
of the component will be vertically centered.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var hCenteredLabel = form.newLabel('CENTER', 10, 40, 300, 20);
hCenteredLabel.horizontalAlignment = SM_ALIGNMENT.CENTER;
var vCenterAlignedLabel = form.newLabel('CENTER', 460, 10, 50, 300);
vCenterAlignedLabel.verticalAlignment = SM_ALIGNMENT.CENTER
```
### DEFAULT

Constant used for setting horizontal and vertical alignment. DEFAULT value makes the alignment behave as if it was not changed before.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var hLabel = myJSForm.getLabel('label_name');
if (hLabel.horizontalAlignment == SM_ALIGNMENT.LEFT) hLabel.horizontalAlignment = SM_ALIGNMENT.DEFAULT;
```
### LEFT

Constant used for setting horizontal alignment for components.
It makes the text inside the component be left aligned horizontally.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var leftAlignedLabel = form.newLabel('LEFT', 10, 10, 300, 20);
leftAlignedLabel.horizontalAlignment = SM_ALIGNMENT.LEFT;
```
### RIGHT

Constant used for setting horizontal alignment for components.
It makes the text inside the component be right aligned vertically.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var rightAlignedLabel = form.newLabel('RIGHT', 10, 70, 300, 20);
rightAlignedLabel.horizontalAlignment = SM_ALIGNMENT.RIGHT;
```
### TOP

Constant used for setting vertical alignment for components.
It makes the text inside the component be top aligned vertically.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var topAlignedLabel = form.newLabel('TOP', 400, 10, 50, 300);
topAlignedLabel.verticalAlignment = SM_ALIGNMENT.TOP;
```

