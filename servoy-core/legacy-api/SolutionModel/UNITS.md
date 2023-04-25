#  UNITS

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [INCH](UNITS.md#INCH)                   | Inch length unit..                                    |
| [Number](../JSLib/Number.md) | [MM](UNITS.md#MM)                   | Millimeters length unit..                                    |
| [Number](../JSLib/Number.md) | [PIXELS](UNITS.md#PIXELS)                   | Pixels length unit..                                    |

## Constants Details

### INCH

Inch length unit.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.defaultPageFormat = solutionModel.createPageFormat(8.5,11,1,1,1,1,SM_ORIENTATION.PORTRAIT,SM_UNITS.INCH);
```
### MM

Millimeters length unit.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.defaultPageFormat = solutionModel.createPageFormat(215,279,25,25,25,25,SM_ORIENTATION.PORTRAIT,SM_UNITS.MM);
```
### PIXELS

Pixels length unit.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.defaultPageFormat = solutionModel.createPageFormat(612,792,72,72,72,72,SM_ORIENTATION.PORTRAIT,SM_UNITS.PIXELS);
```

