#  ViewRecord


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Exception](../Exception.md) | [exception](ViewRecord.md#exception)                   | Returns last occurred exception on this record (or null)..                                    |
| [JSFoundSet](./JSFoundSet.md) | [foundset](ViewRecord.md#foundset)                   | Returns parent foundset of the record..                                    |
| [JSRecordMarkers](./JSRecordMarkers.md) | [recordMarkers](ViewRecord.md#recordMarkers)                   | Returns the validation object if there where validation failures for this record Can be set to null again if you checked the problems, will also be set to null when a save was succesful..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSRecordMarkers](./JSRecordMarkers.md) | [createMarkers()](ViewRecord.md#createmarkers)                   | Creates and returns a new validation object for this record, which allows for markers to be used outside the validation flow..                                    |
| [JSDataSet](./JSDataSet.md) | [getChangedData()](ViewRecord.md#getchangeddata)                   | Returns a JSDataSet with outstanding (not saved) changed data of this record..                                    |
| [String](../JSLib/String.md) | [getDataSource()](ViewRecord.md#getdatasource)                   | Returns the records datasource string..                                    |
| [Array](../JSLib/Array.md) | [getPKs()](ViewRecord.md#getpks)                   | Returns an array with the primary key values of the record..                                    |
| [Boolean](../JSLib/Boolean.md) | [hasChangedData()](ViewRecord.md#haschangeddata)                   | Returns true if the current record has outstanding/changed data..                                    |
| [Boolean](../JSLib/Boolean.md) | [isEditing()](ViewRecord.md#isediting)                   | Returns true or false if the record has changes or not..                                    |
| [Boolean](../JSLib/Boolean.md) | [isNew()](ViewRecord.md#isnew)                   | Returns true if the current record is a new record or false otherwise..                                    |
| [Boolean](../JSLib/Boolean.md) | [isRelatedFoundSetLoaded(relationName)](ViewRecord.md#isrelatedfoundsetloaded-relationname)                   | Returns true or false if the related foundset is already loaded..                                    |
|void | [revertChanges()](ViewRecord.md#revertchanges)                   | Reverts the in memory outstanding (not saved) changes of the record..                                    |

## Properties Details

### exception

Returns last occurred exception on this record (or null).

**Returns**\
[Exception](../Exception.md) The occurred exception.


**Sample**

```javascript
var exception = record.exception;
```
### foundset

Returns parent foundset of the record.

**Returns**\
[JSFoundSet](./JSFoundSet.md) The parent foundset of the record.


**Sample**

```javascript
var parent = record.foundset;
```
### recordMarkers

Returns the validation object if there where validation failures for this record
Can be set to null again if you checked the problems, will also be set to null when a save was succesful.

**Returns**\
[JSRecordMarkers](./JSRecordMarkers.md) The last validtion object if the record was not validated.


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


**Sample**

```javascript
var recordMarkers = record.createMarkers();
```
### getChangedData()

Returns a JSDataSet with outstanding (not saved) changed data of this record.
column1 is the column name, colum2 is the old data and column3 is the new data.

NOTE: To return an array of records with outstanding changed data, see the function foundset.getEditedRecords().


**Returns**\
[JSDataSet](./JSDataSet.md) a JSDataSet with the changed data of this record.


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


**Sample**

```javascript
var ds = record.getDataSource();
```
### getPKs()

Returns an array with the primary key values of the record.


**Returns**\
[Array](../JSLib/Array.md) an Array with the pk values.


**Sample**

```javascript
var pks = foundset.getSelectedRecord().getPKs() // also foundset.getRecord can be used
```
### hasChangedData()

Returns true if the current record has outstanding/changed data.


**Returns**\
[Boolean](../JSLib/Boolean.md) true if the current record has outstanding/changed data.


**Sample**

```javascript
var hasChanged = record.hasChangedData();
```
### isEditing()

Returns true or false if the record has changes or not.

As opposed to isEditing() of regular records, this method actually returns whether there are unsaved changes
on this record, since there is no edit mode for view records.


**Returns**\
[Boolean](../JSLib/Boolean.md) true if unsaved changes are detected.


**Sample**

```javascript

```
### isNew()

Returns true if the current record is a new record or false otherwise. New record means not saved to database.
Because this record is part of a view foundset, this method will always return false.


**Returns**\
[Boolean](../JSLib/Boolean.md) true if the current record is a new record, false otherwise;


**Sample**

```javascript
var isNew = viewFoundset.getSelectedRecord().isNew();
```
### isRelatedFoundSetLoaded(relationName)

Returns true or false if the related foundset is already loaded. Will not load the related foundset.

**Parameters**\
[String](../JSLib/String.md) relationName name of the relation to check for

**Returns**\
[Boolean](../JSLib/Boolean.md) true if related foundset is loaded.


**Sample**

```javascript
var isLoaded = viewfoundset.getSelectedRecord().isRelatedFoundSetLoaded(relationName)
```
### revertChanges()

Reverts the in memory outstanding (not saved) changes of the record.


**Returns**\
void 


**Sample**

```javascript
var record= foundset.getSelectedRecord();
record.revertChanges();
```

