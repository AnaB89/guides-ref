#  PAGEORIENTATION

## **Supported Clients**

    SmartClient
    WebClient

## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [LANDSCAPE](PAGEORIENTATION.md#LANDSCAPE)                   | Landscape page orientation..                                    |
| [Number](../JSLib/Number.md) | [PORTRAIT](PAGEORIENTATION.md#PORTRAIT)                   | Portrait page orientation..                                    |
| [Number](../JSLib/Number.md) | [REVERSE_LANDSCAPE](PAGEORIENTATION.md#REVERSE_LANDSCAPE)                   | Reverse landscape page orientation..                                    |

## Constants Details

### LANDSCAPE

Landscape page orientation.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
var form = solutionModel.getForm("some_form");
form.defaultPageFormat = solutionModel.createPageFormat(792,612,72,72,72,72,SM_ORIENTATION.LANDSCAPE,SM_UNITS.PIXELS);
```
### PORTRAIT

Portrait page orientation.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
var form = solutionModel.getForm("some_form");
form.defaultPageFormat = solutionModel.createPageFormat(612,792,72,72,72,72,SM_ORIENTATION.PORTRAIT,SM_UNITS.PIXELS);
```
### REVERSE_LANDSCAPE

Reverse landscape page orientation.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
var form = solutionModel.getForm("some_form");
form.defaultPageFormat = solutionModel.createPageFormat(792,612,72,72,72,72,SM_ORIENTATION.REVERSE_LANDSCAPE,SM_UNITS.PIXELS);
```

