# JSRecordMarker

## Property Summary

| Type                          | Name                                           | Summary                                                                                   |
| ----------------------------- | ---------------------------------------------- | ----------------------------------------------------------------------------------------- |
| [Object](../js-lib/object.md) | [customObject](jsrecordmarker.md#customObject) | The custom object the users did give the the JSRecordMarkers..                            |
| [String](../js-lib/string.md) | [dataprovider](jsrecordmarker.md#dataprovider) | The column of this record where this problem is reported for..                            |
| [String](../js-lib/string.md) | [i18NMessage](jsrecordmarker.md#i18NMessage)   | The the resolved i19n message if the message was an i18n key..                            |
| [Number](../js-lib/number.md) | [level](jsrecordmarker.md#level)               | The LOGGINGLEVEL the users did give the the JSRecordMarkers..                             |
| [String](../js-lib/string.md) | [message](jsrecordmarker.md#message)           | The message of this problem, can be a i18n key, see getI18NMessage() for a resolved one.. |
| [JSRecord](jsrecord.md)       | [record](jsrecordmarker.md#record)             | The record for which this problem is generated..                                          |

## Properties Details

### customObject

The custom object the users did give the the JSRecordMarkers.report() method.

**Returns**\
[Object](../js-lib/object.md) the customObject

**Sample**

```javascript
```

### dataprovider

The column of this record where this problem is reported for.

**Returns**\
[String](../js-lib/string.md) the column

**Sample**

```javascript
```

### i18NMessage

The the resolved i19n message if the message was an i18n key.

**Returns**\
[String](../js-lib/string.md) the resolved message

**Sample**

```javascript
```

### level

The LOGGINGLEVEL the users did give the the JSRecordMarkers.report() method.

**Returns**\
[Number](../js-lib/number.md) the level

**Sample**

```javascript
```

### message

The message of this problem, can be a i18n key, see getI18NMessage() for a resolved one.

**Returns**\
[String](../js-lib/string.md) the message

**Sample**

```javascript
```

### record

The record for which this problem is generated.

**Returns**\
[JSRecord](jsrecord.md) the record

**Sample**

```javascript
```
