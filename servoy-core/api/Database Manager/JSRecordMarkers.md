#  JSRecordMarkers


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../JSLib/Boolean.md) | [hasErrors](JSRecordMarkers.md#hasErrors)                   | .                                    |
| [Boolean](../JSLib/Boolean.md) | [onBeforeInsertFailed](JSRecordMarkers.md#onBeforeInsertFailed)                   | .                                    |
| [Boolean](../JSLib/Boolean.md) | [onBeforeUpdateFailed](JSRecordMarkers.md#onBeforeUpdateFailed)                   | .                                    |
| [JSRecord](./JSRecord.md) | [record](JSRecordMarkers.md#record)                   | The record for which this JSRecordMarkers is for..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Array](../JSLib/Array.md) | [getGenericExceptions()](JSRecordMarkers.md#getgenericexceptions)                   | Returns a list of all the generic exceptions that did happen when the various methods where called..                                    |
| [Array](../JSLib/Array.md) | [getMarkers()](JSRecordMarkers.md#getmarkers)                   | This returns all the problems found when validation the record..                                    |
| [Array](../JSLib/Array.md) | [getMarkers(level)](JSRecordMarkers.md#getmarkers-level)                   | This returns the problems found when validation the record filtered by the given level.                                    |
|void | [report(message)](JSRecordMarkers.md#report-message)                   | Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n') Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use and a array of message keys if the message was an i18n key with variables..                                    |
|void | [report(message, dataprovider)](JSRecordMarkers.md#report-message-dataprovider)                   | Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n') Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use and a array of message keys if the message was an i18n key with variables..                                    |
|void | [report(message, dataprovider, level)](JSRecordMarkers.md#report-message-dataprovider-level)                   | Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n') Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use and a array of message keys if the message was an i18n key with variables..                                    |
|void | [report(message, dataprovider, level, customObject)](JSRecordMarkers.md#report-message-dataprovider-level-customobject)                   | Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n') Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use and a array of message keys if the message was an i18n key with variables..                                    |
|void | [report(message, dataprovider, level, customObject, messageKeyParams)](JSRecordMarkers.md#report-message-dataprovider-level-customobject-messagekeyparams)                   | Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n') Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use and a array of message keys if the message was an i18n key with variables..                                    |

## Properties Details

### hasErrors



**Returns**\
[Boolean](../JSLib/Boolean.md) If this validation object has errors or only warnings which don't block the save.


**Sample**

```javascript

```
### onBeforeInsertFailed



**Returns**\
[Boolean](../JSLib/Boolean.md) the onBeforeInsertFailed


**Sample**

```javascript

```
### onBeforeUpdateFailed



**Returns**\
[Boolean](../JSLib/Boolean.md) the onBeforeUpdateFailed


**Sample**

```javascript

```
### record

The record for which this JSRecordMarkers is for.

**Returns**\
[JSRecord](./JSRecord.md) the record


**Sample**

```javascript

```

## Methods Details

### getGenericExceptions()

Returns a list of all the generic exceptions that did happen when the various methods where called.


**Returns**\
[Array](../JSLib/Array.md) the genericExceptions


**Sample**

```javascript

```
### getMarkers()

This returns all the problems found when validation the record.


**Returns**\
[Array](../JSLib/Array.md) all the problems that where reported by a report() call.


**Sample**

```javascript

```
### getMarkers(level)

This returns the problems found when validation the record filtered by the given level

**Parameters**\
[Number](../JSLib/Number.md) level a level of a marker that should be returned.

**Returns**\
[Array](../JSLib/Array.md) all the problems that where reported by a report() call.


**Sample**

```javascript

```
### report(message)

Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n')
Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use
and a array of message keys if the message was an i18n key with variables.

**Parameters**\
[String](../JSLib/String.md) message The message (can be i18n)

**Returns**\
void 


**Sample**

```javascript

```
### report(message, dataprovider)

Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n')
Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use
and a array of message keys if the message was an i18n key with variables.

**Parameters**\
[String](../JSLib/String.md) message The message (can be i18n)\
[String](../JSLib/String.md) dataprovider The dataprovider for which this marker is for.

**Returns**\
void 


**Sample**

```javascript

```
### report(message, dataprovider, level)

Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n')
Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use
and a array of message keys if the message was an i18n key with variables.

**Parameters**\
[String](../JSLib/String.md) message The message (can be i18n)\
[String](../JSLib/String.md) dataprovider The dataprovider for which this marker is for.\
[Number](../JSLib/Number.md) level The LOGGINGLEVEL like ERROR or WARNING

**Returns**\
void 


**Sample**

```javascript

```
### report(message, dataprovider, level, customObject)

Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n')
Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use
and a array of message keys if the message was an i18n key with variables.

**Parameters**\
[String](../JSLib/String.md) message The message (can be i18n)\
[String](../JSLib/String.md) dataprovider The dataprovider for which this marker is for.\
[Number](../JSLib/Number.md) level The LOGGINGLEVEL like ERROR or WARNING\
[Object](../JSLib/Object.md) customObject A custom object is default the customObject of the validate() call.

**Returns**\
void 


**Sample**

```javascript

```
### report(message, dataprovider, level, customObject, messageKeyParams)

Create a new JSMarker by reporting a message, this message can be an i18n key (should then start with 'i18n')
Optionally you can give a dataprovider for which this marker is reported, a LOGGINGLEVEL for this marker, some custom javascript object for later use
and a array of message keys if the message was an i18n key with variables.

**Parameters**\
[String](../JSLib/String.md) message The message (can be i18n)\
[String](../JSLib/String.md) dataprovider The dataprovider for which this marker is for.\
[Number](../JSLib/Number.md) level The LOGGINGLEVEL like ERROR or WARNING\
[Object](../JSLib/Object.md) customObject A custom object is default the customObject of the validate() call.\
[Array](../JSLib/Array.md) messageKeyParams Some variables if he message is an i18n key that has place holders.

**Returns**\
void 


**Sample**

```javascript

```

