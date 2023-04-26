# JSRecordMarkers

## Property Summary

| Type                            | Name                                                            | Summary                                            |
| ------------------------------- | --------------------------------------------------------------- | -------------------------------------------------- |
| [Boolean](../js-lib/boolean.md) | [hasErrors](jsrecordmarkers.md#hasErrors)                       | .                                                  |
| [Boolean](../js-lib/boolean.md) | [onBeforeInsertFailed](jsrecordmarkers.md#onBeforeInsertFailed) | .                                                  |
| [Boolean](../js-lib/boolean.md) | [onBeforeUpdateFailed](jsrecordmarkers.md#onBeforeUpdateFailed) | .                                                  |
| [JSRecord](jsrecord.md)         | [record](jsrecordmarkers.md#record)                             | The record for which this JSRecordMarkers is for.. |

## Methods Summary

| Type                        | Name                                                                                                                                                       | Summary                                                                                                                                                                                                                                                                                                                                         |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Array](../js-lib/array.md) | [getGenericExceptions()](jsrecordmarkers.md#getgenericexceptions)                                                                                          | Returns a list of all the generic exceptions that did happen when the various methods where called..                                                                                                                                                                                                                                            |
| [Array](../js-lib/array.md) | [getMarkers()](jsrecordmarkers.md#getmarkers)                                                                                                              | This returns all the problems found when validation the record..                                                                                                                                                                                                                                                                                |
| [Array](../js-lib/array.md) | [getMarkers(level)](jsrecordmarkers.md#getmarkers-level)                                                                                                   | This returns the problems found when validation the record filtered by the given level.                                                                                                                                                                                                                                                         |
| void                        | [report(message)](jsrecordmarkers.md#report-message)                                                                                                       | Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n') Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use and a array of message keys if the message was an i18n key with variables.. |
| void                        | [report(message, dataprovider)](jsrecordmarkers.md#report-message-dataprovider)                                                                            | Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n') Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use and a array of message keys if the message was an i18n key with variables.. |
| void                        | [report(message, dataprovider, level)](jsrecordmarkers.md#report-message-dataprovider-level)                                                               | Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n') Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use and a array of message keys if the message was an i18n key with variables.. |
| void                        | [report(message, dataprovider, level, customObject)](jsrecordmarkers.md#report-message-dataprovider-level-customobject)                                    | Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n') Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use and a array of message keys if the message was an i18n key with variables.. |
| void                        | [report(message, dataprovider, level, customObject, messageKeyParams)](jsrecordmarkers.md#report-message-dataprovider-level-customobject-messagekeyparams) | Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n') Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use and a array of message keys if the message was an i18n key with variables.. |

## Properties Details

### hasErrors

**Returns**\
[Boolean](../js-lib/boolean.md) If this validation object has errors or only warnings which don't block the save.

**Sample**

```javascript
```

### onBeforeInsertFailed

**Returns**\
[Boolean](../js-lib/boolean.md) the onBeforeInsertFailed

**Sample**

```javascript
```

### onBeforeUpdateFailed

**Returns**\
[Boolean](../js-lib/boolean.md) the onBeforeUpdateFailed

**Sample**

```javascript
```

### record

The record for which this JSRecordMarkers is for.

**Returns**\
[JSRecord](jsrecord.md) the record

**Sample**

```javascript
```

## Methods Details

### getGenericExceptions()

Returns a list of all the generic exceptions that did happen when the various methods where called.

**Returns**\
[Array](../js-lib/array.md) the genericExceptions

**Sample**

```javascript
```

### getMarkers()

This returns all the problems found when validation the record.

**Returns**\
[Array](../js-lib/array.md) all the problems that where reported by a report() call.

**Sample**

```javascript
```

### getMarkers(level)

This returns the problems found when validation the record filtered by the given level

**Parameters**\
[Number](../js-lib/number.md) level a level of a marker that should be returned.

**Returns**\
[Array](../js-lib/array.md) all the problems that where reported by a report() call.

**Sample**

```javascript
```

### report(message)

Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n') Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use and a array of message keys if the message was an i18n key with variables.

**Parameters**\
[String](../js-lib/string.md) message The message (can be i18n)

**Returns**\
void

**Sample**

```javascript
```

### report(message, dataprovider)

Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n') Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use and a array of message keys if the message was an i18n key with variables.

**Parameters**\
[String](../js-lib/string.md) message The message (can be i18n)\
[String](../js-lib/string.md) dataprovider The dataprovider for which this marker is for.

**Returns**\
void

**Sample**

```javascript
```

### report(message, dataprovider, level)

Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n') Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use and a array of message keys if the message was an i18n key with variables.

**Parameters**\
[String](../js-lib/string.md) message The message (can be i18n)\
[String](../js-lib/string.md) dataprovider The dataprovider for which this marker is for.\
[Number](../js-lib/number.md) level The LOGGINGLEVEL like ERROR or WARNING

**Returns**\
void

**Sample**

```javascript
```

### report(message, dataprovider, level, customObject)

Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n') Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use and a array of message keys if the message was an i18n key with variables.

**Parameters**\
[String](../js-lib/string.md) message The message (can be i18n)\
[String](../js-lib/string.md) dataprovider The dataprovider for which this marker is for.\
[Number](../js-lib/number.md) level The LOGGINGLEVEL like ERROR or WARNING\
[Object](../js-lib/object.md) customObject A custom object is default the customObject of the validate() call.

**Returns**\
void

**Sample**

```javascript
```

### report(message, dataprovider, level, customObject, messageKeyParams)

Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n') Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use and a array of message keys if the message was an i18n key with variables.

**Parameters**\
[String](../js-lib/string.md) message The message (can be i18n)\
[String](../js-lib/string.md) dataprovider The dataprovider for which this marker is for.\
[Number](../js-lib/number.md) level The LOGGINGLEVEL like ERROR or WARNING\
[Object](../js-lib/object.md) customObject A custom object is default the customObject of the validate() call.\
[Array](../js-lib/array.md) messageKeyParams Some variables if he message is an i18n key that has place holders.

**Returns**\
void

**Sample**

```javascript
```
