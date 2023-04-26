# ViewRecord

## Property Summary

| Type                                                  | Name                                         | Summary                                                                                                                                                                                     |
| ----------------------------------------------------- | -------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Exception](../../../../servoy-core/api/Exception.md) | [exception](viewrecord.md#exception)         | Returns last occurred exception on this record (or null)..                                                                                                                                  |
| [JSFoundSet](jsfoundset.md)                           | [foundset](viewrecord.md#foundset)           | Returns parent foundset of the record..                                                                                                                                                     |
| [JSRecordMarkers](jsrecordmarkers.md)                 | [recordMarkers](viewrecord.md#recordMarkers) | Returns the validation object if there where validation failures for this record Can be set to null again if you checked the problems, will also be set to null when a save was succesful.. |

## Methods Summary

| Type                                  | Name                                                                                        | Summary                                                                                                                        |
| ------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| [JSRecordMarkers](jsrecordmarkers.md) | [createMarkers()](viewrecord.md#createmarkers)                                              | Creates and returns a new validation object for this record, which allows for markers to be used outside the validation flow.. |
| [JSDataSet](jsdataset.md)             | [getChangedData()](viewrecord.md#getchangeddata)                                            | Returns a JSDataSet with outstanding (not saved) changed data of this record..                                                 |
| [String](../js-lib/string.md)         | [getDataSource()](viewrecord.md#getdatasource)                                              | Returns the records datasource string..                                                                                        |
| [Array](../js-lib/array.md)           | [getPKs()](viewrecord.md#getpks)                                                            | Returns an array with the primary key values of the record..                                                                   |
| [Boolean](../js-lib/boolean.md)       | [hasChangedData()](viewrecord.md#haschangeddata)                                            | Returns true if the current record has outstanding/changed data..                                                              |
| [Boolean](../js-lib/boolean.md)       | [isEditing()](viewrecord.md#isediting)                                                      | Returns true or false if the record has changes or not..                                                                       |
| [Boolean](../js-lib/boolean.md)       | [isNew()](viewrecord.md#isnew)                                                              | Returns true if the current record is a new record or false otherwise..                                                        |
| [Boolean](../js-lib/boolean.md)       | [isRelatedFoundSetLoaded(relationName)](viewrecord.md#isrelatedfoundsetloaded-relationname) | Returns true or false if the related foundset is already loaded..                                                              |
| void                                  | [revertChanges()](viewrecord.md#revertchanges)                                              | Reverts the in memory outstanding (not saved) changes of the record..                                                          |

## Properties Details

### exception

Returns last occurred exception on this record (or null).

**Returns**\
[Exception](../../../../servoy-core/api/Exception.md) The occurred exception.

**Sample**

```javascript
var exception = record.exception;
```

### foundset

Returns parent foundset of the record.

**Returns**\
[JSFoundSet](jsfoundset.md) The parent foundset of the record.

**Sample**

```javascript
var parent = record.foundset;
```

### recordMarkers

Returns the validation object if there where validation failures for this record Can be set to null again if you checked the problems, will also be set to null when a save was succesful.

**Returns**\
[JSRecordMarkers](jsrecordmarkers.md) The last validtion object if the record was not validated.

**Sample**

```javascript
var recordMarkers = record.recordMarkers;
```

## Methods Details

### createMarkers()

Creates and returns a new validation object for this record, which allows for markers to be used outside the validation flow. Will overwrite the current markers if present. Can be set to null again if you checked the problems, will also be set to null when a save was successful.

**Returns**\
[JSRecordMarkers](jsrecordmarkers.md) A new validation object.

**Sample**

```javascript
var recordMarkers = record.createMarkers();
```

### getChangedData()

Returns a JSDataSet with outstanding (not saved) changed data of this record. column1 is the column name, colum2 is the old data and column3 is the new data.

NOTE: To return an array of records with outstanding changed data, see the function foundset.getEditedRecords().

**Returns**\
[JSDataSet](jsdataset.md) a JSDataSet with the changed data of this record.

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
[String](../js-lib/string.md) The datasource string of this record.

**Sample**

```javascript
var ds = record.getDataSource();
```

### getPKs()

Returns an array with the primary key values of the record.

**Returns**\
[Array](../js-lib/array.md) an Array with the pk values.

**Sample**

```javascript
var pks = foundset.getSelectedRecord().getPKs() // also foundset.getRecord can be used
```

### hasChangedData()

Returns true if the current record has outstanding/changed data.

**Returns**\
[Boolean](../js-lib/boolean.md) true if the current record has outstanding/changed data.

**Sample**

```javascript
var hasChanged = record.hasChangedData();
```

### isEditing()

Returns true or false if the record has changes or not.

As opposed to isEditing() of regular records, this method actually returns whether there are unsaved changes on this record, since there is no edit mode for view records.

**Returns**\
[Boolean](../js-lib/boolean.md) true if unsaved changes are detected.

**Sample**

```javascript
```

### isNew()

Returns true if the current record is a new record or false otherwise. New record means not saved to database. Because this record is part of a view foundset, this method will always return false.

**Returns**\
[Boolean](../js-lib/boolean.md) true if the current record is a new record, false otherwise;

**Sample**

```javascript
var isNew = viewFoundset.getSelectedRecord().isNew();
```

### isRelatedFoundSetLoaded(relationName)

Returns true or false if the related foundset is already loaded. Will not load the related foundset.

**Parameters**\
[String](../js-lib/string.md) relationName name of the relation to check for

**Returns**\
[Boolean](../js-lib/boolean.md) true if related foundset is loaded.

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
