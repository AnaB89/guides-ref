#  JSRecord

## **Supported Clients**

    SmartClient
    WebClient
    NGClient
    MobileClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Exception](../Exception.md) | [exception](JSRecord.md#exception)                   | Returns last occurred exception on this record (or null)..                                    |
| [JSFoundSet](./JSFoundSet.md) | [foundset](JSRecord.md#foundset)                   | Returns parent foundset of the record..                                    |
| [JSRecordMarkers](./JSRecordMarkers.md) | [recordMarkers](JSRecord.md#recordMarkers)                   | Returns the validation object if there where validation failures for this record Can be set to null again if you checked the problems, will also be set to null when a save was successful..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSRecordMarkers](./JSRecordMarkers.md) | [createMarkers()](JSRecord.md#createmarkers)                   | Creates and returns a new validation object for this record, which allows for markers to be used outside the validation flow..                                    |
| [JSDataSet](./JSDataSet.md) | [getChangedData()](JSRecord.md#getchangeddata)                   | Returns a JSDataSet with outstanding (not saved) changed data of this record..                                    |
| [String](../JSLib/String.md) | [getDataSource()](JSRecord.md#getdatasource)                   | Returns the records datasource string..                                    |
| [Array](../JSLib/Array.md) | [getPKs()](JSRecord.md#getpks)                   | Returns an array with the primary key values of the record..                                    |
| [Boolean](../JSLib/Boolean.md) | [hasChangedData()](JSRecord.md#haschangeddata)                   | Returns true if the current record has outstanding/changed data..                                    |
| [Boolean](../JSLib/Boolean.md) | [isEditing()](JSRecord.md#isediting)                   | Returns true or false if the record is being edited or not..                                    |
| [Boolean](../JSLib/Boolean.md) | [isNew()](JSRecord.md#isnew)                   | Returns true if the current record is a new record or false otherwise..                                    |
| [Boolean](../JSLib/Boolean.md) | [isRelatedFoundSetLoaded(relationName)](JSRecord.md#isrelatedfoundsetloaded-relationname)                   | Returns true or false if the related foundset is already loaded..                                    |
|void | [revertChanges()](JSRecord.md#revertchanges)                   | Reverts the in memory outstanding (not saved) changes of the record..                                    |

## Properties Details

### exception

Returns last occurred exception on this record (or null).

**Returns**\
[Exception](../Exception.md) The occurred exception.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var exception = record.exception;
```
### foundset

Returns parent foundset of the record.

**Returns**\
[JSFoundSet](./JSFoundSet.md) The parent foundset of the record.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var parent = record.foundset;
```
### recordMarkers

Returns the validation object if there where validation failures for this record
Can be set to null again if you checked the problems, will also be set to null when a save was successful.

**Returns**\
[JSRecordMarkers](./JSRecordMarkers.md) The last validation object if the record was not validated.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var recordMarkers = record.recordMarkers;
```

## Methods Details

### createMarkers()

Creates and returns a new validation object for this record, which allows for markers to be used outside the validation flow.
Will overwrite the current markers if present.
Can be set to null again if you checked the problems, will also be set to null when a save was successful.


**Returns**\
[JSRecordMarkers](./JSRecordMarkers.md) A new validation object.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var recordMarkers = record.createMarkers();
```
### getChangedData()

Returns a JSDataSet with outstanding (not saved) changed data of this record.
column1 is the column name, colum2 is the old data and column3 is the new data.

NOTE: To return an array of records with outstanding changed data, see the function databaseManager.getEditedRecords().


**Returns**\
[JSDataSet](./JSDataSet.md) a JSDataSet with the changed data of this record.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
/** @type {JSDataSet} */
var dataset = record.getChangedData()
for( var i = 1 ; i <= dataset.getMaxRowIndex() ; i++ )
{
	application.output(dataset.getValue(i,1) +' '+ dataset.getValue(i,2) +' '+ dataset.getValue(i,3));
}
```
### getDataSource()

Returns the records datasource string.


**Returns**\
[String](../JSLib/String.md) The datasource string of this record.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var ds = record.getDataSource();
```
### getPKs()

Returns an array with the primary key values of the record.


**Returns**\
[Array](../JSLib/Array.md) an Array with the pk values.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var pks = foundset.getSelectedRecord().getPKs() // also foundset.getRecord can be used
```
### hasChangedData()

Returns true if the current record has outstanding/changed data.


**Returns**\
[Boolean](../JSLib/Boolean.md) true if the current record has outstanding/changed data.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var hasChanged = record.hasChangedData();
```
### isEditing()

Returns true or false if the record is being edited or not.

This will not check if the record doesn't really have any changes, it just returns the edit state.
So this can return true but databaseManager.getEditedRecord() will not return this record because that
call will check if the record has really any changed values compared to the stored database values.
Record can be in edit mode without changes when some field is focused (so edit is started) but no changes are done yet
or when changes were done in such a way that record data is the same as database data.


**Returns**\
[Boolean](../JSLib/Boolean.md) a boolean when in edit.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var isEditing = foundset.getSelectedRecord().isEditing() // also foundset.getRecord can be used
```
### isNew()

Returns true if the current record is a new record or false otherwise. New record means not saved to database.


**Returns**\
[Boolean](../JSLib/Boolean.md) true if the current record is a new record, false otherwise;

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var isNew = foundset.getSelectedRecord().isNew();
```
### isRelatedFoundSetLoaded(relationName)

Returns true or false if the related foundset is already loaded. Will not load the related foundset.

**Parameters**\
[String](../JSLib/String.md) relationName name of the relation to check for

**Returns**\
[Boolean](../JSLib/Boolean.md) a boolean when loaded.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var isLoaded = foundset.getSelectedRecord().isRelatedFoundSetLoaded(relationName)
```
### revertChanges()

Reverts the in memory outstanding (not saved) changes of the record.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var record= foundset.getSelectedRecord();
record.revertChanges();
```

