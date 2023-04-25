#  BEVELTYPE

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [LOWERED](BEVELTYPE.md#LOWERED)                   | Lowered bevel border type..                                    |
| [Number](../JSLib/Number.md) | [RAISED](BEVELTYPE.md#RAISED)                   | Raised bevel border type..                                    |

## Constants Details

### LOWERED

Lowered bevel border type.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createBevelBorder(SM_BEVELTYPE.LOWERED, '#ff0000', '#00ff00','#f0000f', '#0000ff');
```
### RAISED

Raised bevel border type.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var form = solutionModel.getForm("someForm");
form.borderType = solutionModel.createBevelBorder(SM_BEVELTYPE.RAISED, '#ff0000', '#00ff00','#f0000f', '#0000ff');
```

