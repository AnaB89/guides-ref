# CLIENTDESIGN

## Constants Summary

| Type                          | Name                                     | Summary                                                  |
| ----------------------------- | ---------------------------------------- | -------------------------------------------------------- |
| [String](../js-lib/string.md) | [HANDLES](clientdesign.md#HANDLES)       | Property that can be set using elements\['element\_1'].. |
| [String](../js-lib/string.md) | [SELECTABLE](clientdesign.md#SELECTABLE) | Property that can be set using elements\['element\_1'].. |

## Constants Details

### HANDLES

Property that can be set using elements\['element\_1'].putClientProperty(...), it sets the available handles in clientdesign

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
//by default all are present. ('l' stands for left, 't' stands for top, etc.)
elements['element_1'].putClientProperty(CLIENTDESIGN.HANDLES, new Array('r', 'l')); // other options are 't', 'b', 'r', 'l', 'bl', 'br', 'tl', 'tr'
```

### SELECTABLE

Property that can be set using elements\['element\_1'].putClientProperty(...), it sets the selectable flag in clientdesign

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
//by default an element with an name is selectable in client design
elements['element_1'].putClientProperty(CLIENTDESIGN.SELECTABLE, false);
```
