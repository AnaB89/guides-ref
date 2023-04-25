#  CLIENTDESIGN

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [String](../JSLib/String.md) | [HANDLES](CLIENTDESIGN.md#HANDLES)                   | Property that can be set using elements['element_1']..                                    |
| [String](../JSLib/String.md) | [SELECTABLE](CLIENTDESIGN.md#SELECTABLE)                   | Property that can be set using elements['element_1']..                                    |

## Constants Details

### HANDLES

Property that can be set using elements['element_1'].putClientProperty(...), it sets the available handles in clientdesign

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//by default all are present. ('l' stands for left, 't' stands for top, etc.)
elements['element_1'].putClientProperty(CLIENTDESIGN.HANDLES, new Array('r', 'l')); // other options are 't', 'b', 'r', 'l', 'bl', 'br', 'tl', 'tr'
```
### SELECTABLE

Property that can be set using elements['element_1'].putClientProperty(...), it sets the selectable flag in clientdesign

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//by default an element with an name is selectable in client design
elements['element_1'].putClientProperty(CLIENTDESIGN.SELECTABLE, false);
```

