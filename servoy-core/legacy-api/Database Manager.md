#  Database Manager

## **Return Types**
[SQL_ACTION_TYPES](Database%20Manager/SQL_ACTION_TYPES.md),[JSColumn](Database%20Manager/JSColumn.md),[JSDataSet](Database%20Manager/JSDataSet.md),[JSFoundSetUpdater](Database%20Manager/JSFoundSetUpdater.md),[JSRecordMarker](Database%20Manager/JSRecordMarker.md),[JSRecordMarkers](Database%20Manager/JSRecordMarkers.md),[JSRecord](Database%20Manager/JSRecord.md),[JSFoundSet](Database%20Manager/JSFoundSet.md),[JSTable](Database%20Manager/JSTable.md),[QBSelect](Database%20Manager/QBSelect.md),[QBColumn](Database%20Manager/QBColumn.md),[QBCase](Database%20Manager/QBCase.md),[QBCaseWhen](Database%20Manager/QBCaseWhen.md),[QBColumn](Database%20Manager/QBColumn.md),[QBColumns](Database%20Manager/QBColumns.md),[QBCondition](Database%20Manager/QBCondition.md),[QBColumn](Database%20Manager/QBColumn.md),[QBGroupBy](Database%20Manager/QBGroupBy.md),[QBJoin](Database%20Manager/QBJoin.md),[QBJoins](Database%20Manager/QBJoins.md),[QBLogicalCondition](Database%20Manager/QBLogicalCondition.md),[QBLogicalCondition](Database%20Manager/QBLogicalCondition.md),[QBResult](Database%20Manager/QBResult.md),[QBColumn](Database%20Manager/QBColumn.md),[QBSort](Database%20Manager/QBSort.md),[QBSorts](Database%20Manager/QBSorts.md),[QBTableClause](Database%20Manager/QBTableClause.md),[QBPart](Database%20Manager/QBPart.md),[QBParameter](Database%20Manager/QBParameter.md),[QBParameters](Database%20Manager/QBParameters.md),[QBFunctions](Database%20Manager/QBFunctions.md),[QUERY_COLUMN_TYPES](Database%20Manager/QUERY_COLUMN_TYPES.md),[JSFoundSet](Database%20Manager/JSFoundSet.md),[JSRecord](Database%20Manager/JSRecord.md),[JSTableFilter](Database%20Manager/JSTableFilter.md),
## **Supported Clients**

    SmartClient
    WebClient
    NGClient
    MobileClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](JSLib/Boolean.md) | [alwaysFollowPkSelection](Database%20Manager.md#alwaysFollowPkSelection)                   | Enable/disable the foundset behaviour to keep selection to the first row always, even if updates from other clients are received that add new records before the current first record..                                    |
| [Boolean](JSLib/Boolean.md) | [disableRelatedSiblingsPrefetch](Database%20Manager.md#disableRelatedSiblingsPrefetch)                   | Enable/disable the automatic prefetching of related foundsets for sibling records..                                    |
| [Boolean](JSLib/Boolean.md) | [nullColumnValidatorEnabled](Database%20Manager.md#nullColumnValidatorEnabled)                   | Enable/disable the default null validator for non null columns, makes it possible to do the checks later on when saving, when for example autosave is disabled..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](JSLib/Boolean.md) | [acquireLock(foundset, recordIndex)](Database%20Manager.md#acquirelock-foundset-recordindex)                   | Request lock(s) for a foundset, can be a normal or related foundset..                                    |
| [Boolean](JSLib/Boolean.md) | [acquireLock(foundset, recordIndex, lockName)](Database%20Manager.md#acquirelock-foundset-recordindex-lockname)                   | Request lock(s) for a foundset, can be a normal or related foundset..                                    |
| [Boolean](JSLib/Boolean.md) | [addTableFilterParam(query)](Database%20Manager.md#addtablefilterparam-query)                   | Adds a filter based on a query to all the foundsets based on a table..                                    |
| [Boolean](JSLib/Boolean.md) | [addTableFilterParam(query, filterName)](Database%20Manager.md#addtablefilterparam-query-filtername)                   | Adds a filter based on a query to all the foundsets based on a table..                                    |
| [Boolean](JSLib/Boolean.md) | [addTableFilterParam(datasource, dataprovider, operator, value)](Database%20Manager.md#addtablefilterparam-datasource-dataprovider-operator-value)                   | Adds a filter to all the foundsets based on a table..                                    |
| [Boolean](JSLib/Boolean.md) | [addTableFilterParam(datasource, dataprovider, operator, value, filterName)](Database%20Manager.md#addtablefilterparam-datasource-dataprovider-operator-value-filtername)                   | Adds a filter to all the foundsets based on a table..                                    |
| [Boolean](JSLib/Boolean.md) | [addTableFilterParam(serverName, tableName, dataprovider, operator, value)](Database%20Manager.md#addtablefilterparam-servername-tablename-dataprovider-operator-value)                   | Adds a filter to all the foundsets based on a table..                                    |
| [Boolean](JSLib/Boolean.md) | [addTableFilterParam(serverName, tableName, dataprovider, operator, value, filterName)](Database%20Manager.md#addtablefilterparam-servername-tablename-dataprovider-operator-value-filtername)                   | Adds a filter to all the foundsets based on a table..                                    |
|void | [addTrackingInfo(columnName, value)](Database%20Manager.md#addtrackinginfo-columnname-value)                   | Add tracking info used in the log table..                                    |
| [Boolean](JSLib/Boolean.md) | [commitTransaction()](Database%20Manager.md#committransaction)                   | Returns true if a transaction is committed; rollback if commit fails..                                    |
| [Boolean](JSLib/Boolean.md) | [commitTransaction(saveFirst)](Database%20Manager.md#committransaction-savefirst)                   | Returns true if a transaction is committed; rollback if commit fails..                                    |
| [Boolean](JSLib/Boolean.md) | [commitTransaction(saveFirst, revertSavedRecords)](Database%20Manager.md#committransaction-savefirst-revertsavedrecords)                   | Returns true if a transaction is committed; rollback if commit fails..                                    |
| [JSFoundSet](Database%20Manager/JSFoundSet.md) | [convertFoundSet(foundset, related)](Database%20Manager.md#convertfoundset-foundset-related)                   | Creates a foundset that combines all the records of the specified one-to-many relation seen from the given parent/primary foundset..                                    |
| [JSFoundSet](Database%20Manager/JSFoundSet.md) | [convertFoundSet(foundset, related)](Database%20Manager.md#convertfoundset-foundset-related)                   | Creates a foundset that combines all the records of the specified one-to-many relation seen from the given parent/primary foundset..                                    |
| [JSDataSet](Database%20Manager/JSDataSet.md) | [convertToDataSet(foundset)](Database%20Manager.md#converttodataset-foundset)                   | Converts the argument to a JSDataSet, possible use in controller..                                    |
| [JSDataSet](Database%20Manager/JSDataSet.md) | [convertToDataSet(foundset, dataproviderNames)](Database%20Manager.md#converttodataset-foundset-dataprovidernames)                   | Converts the argument to a JSDataSet, possible use in controller..                                    |
| [JSDataSet](Database%20Manager/JSDataSet.md) | [convertToDataSet(values)](Database%20Manager.md#converttodataset-values)                   | Converts the argument to a JSDataSet, possible use in controller..                                    |
| [JSDataSet](Database%20Manager/JSDataSet.md) | [convertToDataSet(values, dataproviderNames)](Database%20Manager.md#converttodataset-values-dataprovidernames)                   | Converts the argument to a JSDataSet, possible use in controller..                                    |
| [JSDataSet](Database%20Manager/JSDataSet.md) | [convertToDataSet(ids)](Database%20Manager.md#converttodataset-ids)                   | Converts the argument to a JSDataSet, possible use in controller..                                    |
| [Boolean](JSLib/Boolean.md) | [copyMatchingFields(source, destination)](Database%20Manager.md#copymatchingfields-source-destination)                   | Copies all matching non empty columns (if overwrite boolean is given all columns except pk/ident, if array then all columns except pk and array names)..                                    |
| [Boolean](JSLib/Boolean.md) | [copyMatchingFields(source, destination, overwrite)](Database%20Manager.md#copymatchingfields-source-destination-overwrite)                   | Copies all matching non empty columns (if overwrite boolean is given all columns except pk/ident, if array then all columns except pk and array names)..                                    |
| [Boolean](JSLib/Boolean.md) | [copyMatchingFields(source, destination, names)](Database%20Manager.md#copymatchingfields-source-destination-names)                   | Copies all matching non empty columns (if overwrite boolean is given all columns except pk/ident, if array then all columns except pk and array names)..                                    |
| [String](JSLib/String.md) | [createDataSourceByQuery(name, query, useTableFilters, max_returned_rows, types, pkNames)](Database%20Manager.md#createdatasourcebyquery-name-query-usetablefilters-max_returned_rows-types-pknames)                   | Performs a query and saves the result in a datasource..                                    |
| [String](JSLib/String.md) | [createDataSourceByQuery(name, query, max_returned_rows)](Database%20Manager.md#createdatasourcebyquery-name-query-max_returned_rows)                   | Performs a query and saves the result in a datasource..                                    |
| [String](JSLib/String.md) | [createDataSourceByQuery(name, query, max_returned_rows, types)](Database%20Manager.md#createdatasourcebyquery-name-query-max_returned_rows-types)                   | Performs a query and saves the result in a datasource..                                    |
| [String](JSLib/String.md) | [createDataSourceByQuery(name, query, max_returned_rows, types, pkNames)](Database%20Manager.md#createdatasourcebyquery-name-query-max_returned_rows-types-pknames)                   | Performs a query and saves the result in a datasource..                                    |
| [String](JSLib/String.md) | [createDataSourceByQuery(name, server_name, sql_query, arguments, max_returned_rows)](Database%20Manager.md#createdatasourcebyquery-name-server_name-sql_query-arguments-max_returned_rows)                   | Performs a sql query on the specified server, saves the the result in a datasource..                                    |
| [String](JSLib/String.md) | [createDataSourceByQuery(name, server_name, sql_query, arguments, max_returned_rows, types)](Database%20Manager.md#createdatasourcebyquery-name-server_name-sql_query-arguments-max_returned_rows-types)                   | Performs a sql query on the specified server, saves the the result in a datasource..                                    |
| [String](JSLib/String.md) | [createDataSourceByQuery(name, server_name, sql_query, arguments, max_returned_rows, columnTypes, pkNames)](Database%20Manager.md#createdatasourcebyquery-name-server_name-sql_query-arguments-max_returned_rows-columntypes-pknames)                   | Performs a sql query on the specified server, saves the the result in a datasource..                                    |
| [JSDataSet](Database%20Manager/JSDataSet.md) | [createEmptyDataSet()](Database%20Manager.md#createemptydataset)                   | Returns an empty dataset object..                                    |
| [JSDataSet](Database%20Manager/JSDataSet.md) | [createEmptyDataSet(rowCount, columnCount)](Database%20Manager.md#createemptydataset-rowcount-columncount)                   | Returns an empty dataset object..                                    |
| [JSDataSet](Database%20Manager/JSDataSet.md) | [createEmptyDataSet(rowCount, columnNames)](Database%20Manager.md#createemptydataset-rowcount-columnnames)                   | Returns an empty dataset object..                                    |
| [QBSelect](Database%20Manager/QBSelect.md) | [createSelect(dataSource)](Database%20Manager.md#createselect-datasource)                   | Create a QueryBuilder object for a datasource..                                    |
| [QBSelect](Database%20Manager/QBSelect.md) | [createSelect(dataSource, tableAlias)](Database%20Manager.md#createselect-datasource-tablealias)                   | Create a QueryBuilder object for a datasource with given table alias..                                    |
| [JSTableFilter](Database%20Manager/JSTableFilter.md) | [createTableFilterParam(query)](Database%20Manager.md#createtablefilterparam-query)                   | Create a table filter that can be applied to all the foundsets based on a table..                                    |
| [JSTableFilter](Database%20Manager/JSTableFilter.md) | [createTableFilterParam(datasource, dataprovider, operator, value)](Database%20Manager.md#createtablefilterparam-datasource-dataprovider-operator-value)                   | Create a table filter that can be applied to all the foundsets based on a table..                                    |
| [JSTableFilter](Database%20Manager/JSTableFilter.md) | [createTableFilterParam(serverName, tableName, dataprovider, operator, value)](Database%20Manager.md#createtablefilterparam-servername-tablename-dataprovider-operator-value)                   | Create a table filter that can be applied to all the foundsets based on a table..                                    |
| [Boolean](JSLib/Boolean.md) | [dataSourceExists(dataSource)](Database%20Manager.md#datasourceexists-datasource)                   | Check wether a data source exists..                                    |
|void | [flushCalculations(datasource, onlyUnstored)](Database%20Manager.md#flushcalculations-datasource-onlyunstored)                   | This method differences for recalculate() that it only works on a datasource rows/records that are loaded in memory..                                    |
|void | [flushCalculations(datasource, onlyUnstored, calcnames)](Database%20Manager.md#flushcalculations-datasource-onlyunstored-calcnames)                   | This method differences for recalculate() that it only works on a datasource rows/records that are loaded in memory..                                    |
| [Boolean](JSLib/Boolean.md) | [getAutoSave()](Database%20Manager.md#getautosave)                   | Returns true or false if autosave is enabled or disabled..                                    |
| [Array](JSLib/Array.md) | [getDataModelClonesFrom(serverName)](Database%20Manager.md#getdatamodelclonesfrom-servername)                   | Retrieves a list with names of all database servers that have property DataModelCloneFrom equal to the server name parameter..                                    |
| [JSDataSet](Database%20Manager/JSDataSet.md) | [getDataSetByQuery(query, useTableFilters, max_returned_rows)](Database%20Manager.md#getdatasetbyquery-query-usetablefilters-max_returned_rows)                   | Performs a sql query with a query builder object..                                    |
| [JSDataSet](Database%20Manager/JSDataSet.md) | [getDataSetByQuery(query, max_returned_rows)](Database%20Manager.md#getdatasetbyquery-query-max_returned_rows)                   | Performs a sql query with a query builder object..                                    |
| [JSDataSet](Database%20Manager/JSDataSet.md) | [getDataSetByQuery(server_name, sql_query, arguments, max_returned_rows)](Database%20Manager.md#getdatasetbyquery-server_name-sql_query-arguments-max_returned_rows)                   | Performs a sql query on the specified server, returns the result in a dataset..                                    |
| [String](JSLib/String.md) | [getDataSource(serverName, tableName)](Database%20Manager.md#getdatasource-servername-tablename)                   | Returns the datasource corresponding to the given server/table..                                    |
| [String](JSLib/String.md) | [getDataSourceServerName(dataSource)](Database%20Manager.md#getdatasourceservername-datasource)                   | Returns the server name from the datasource, or null if not a database datasource..                                    |
| [String](JSLib/String.md) | [getDataSourceTableName(dataSource)](Database%20Manager.md#getdatasourcetablename-datasource)                   | Returns the table name from the datasource, or null if not a database datasource..                                    |
| [String](JSLib/String.md) | [getDatabaseProductName(serverName)](Database%20Manager.md#getdatabaseproductname-servername)                   | Returns the database product name as supplied by the driver for a server..                                    |
| [Array](JSLib/Array.md) | [getEditedRecords()](Database%20Manager.md#geteditedrecords)                   | Returns an array of edited records with outstanding (unsaved) data..                                    |
| [Array](JSLib/Array.md) | [getEditedRecords(foundset)](Database%20Manager.md#geteditedrecords-foundset)                   | Returns an array of edited records with outstanding (unsaved) data..                                    |
| [Array](JSLib/Array.md) | [getEditedRecords(datasource)](Database%20Manager.md#geteditedrecords-datasource)                   | Returns an array of edited records with outstanding (unsaved) data..                                    |
| [Array](JSLib/Array.md) | [getEditedRecords(datasource, filter)](Database%20Manager.md#geteditedrecords-datasource-filter)                   | Returns an array of edited records with outstanding (unsaved) data for a datasource with a filter..                                    |
| [Array](JSLib/Array.md) | [getFailedRecords()](Database%20Manager.md#getfailedrecords)                   | Returns an array of records that fail after a save..                                    |
| [Array](JSLib/Array.md) | [getFailedRecords(foundset)](Database%20Manager.md#getfailedrecords-foundset)                   | Returns an array of records that fail after a save..                                    |
| [JSFoundSet](Database%20Manager/JSFoundSet.md) | [getFoundSet(query)](Database%20Manager.md#getfoundset-query)                   | Returns a foundset object for a specified pk query..                                    |
| [JSFoundSet](Database%20Manager/JSFoundSet.md) | [getFoundSet(dataSource)](Database%20Manager.md#getfoundset-datasource)                   | Returns a foundset object for a specified datasource or server and tablename..                                    |
| [JSFoundSet](Database%20Manager/JSFoundSet.md) | [getFoundSet(serverName, tableName)](Database%20Manager.md#getfoundset-servername-tablename)                   | Returns a foundset object for a specified datasource or server and tablename..                                    |
| [Number](JSLib/Number.md) | [getFoundSetCount(foundset)](Database%20Manager.md#getfoundsetcount-foundset)                   | Returns the total number of records in a foundset..                                    |
| [JSFoundSetUpdater](Database%20Manager/JSFoundSetUpdater.md) | [getFoundSetUpdater(foundset)](Database%20Manager.md#getfoundsetupdater-foundset)                   | Returns a JSFoundsetUpdater object that can be used to update all or a specific number of rows in the specified foundset..                                    |
| [JSFoundSet](Database%20Manager/JSFoundSet.md) | [getNamedFoundSet(name)](Database%20Manager.md#getnamedfoundset-name)                   | An existing foundset under that name will be returned, or created if there is a definition (there is a form with a named foundset property with that name)..                                    |
| [Object](JSLib/Object.md) | [getNextSequence(dataSource, columnName)](Database%20Manager.md#getnextsequence-datasource-columnname)                   | Gets the next sequence for a column which has a sequence defined in its column dataprovider properties..                                    |
| [String](JSLib/String.md) | [getSQL(foundsetOrQBSelect)](Database%20Manager.md#getsql-foundsetorqbselect)                   | Returns the internal SQL which defines the specified (related)foundset..                                    |
| [String](JSLib/String.md) | [getSQL(foundsetOrQBSelect, includeFilters)](Database%20Manager.md#getsql-foundsetorqbselect-includefilters)                   | Returns the internal SQL which defines the specified (related)foundset..                                    |
| [Array](JSLib/Array.md) | [getSQLParameters(foundsetOrQBSelect)](Database%20Manager.md#getsqlparameters-foundsetorqbselect)                   | Returns the internal SQL parameters, as an array, that are used to define the specified (related)foundset..                                    |
| [Array](JSLib/Array.md) | [getSQLParameters(foundsetOrQBSelect, includeFilters)](Database%20Manager.md#getsqlparameters-foundsetorqbselect-includefilters)                   | Returns the internal SQL parameters, as an array, that are used to define the specified (related)foundset..                                    |
| [Array](JSLib/Array.md) | [getServerNames()](Database%20Manager.md#getservernames)                   | Returns an array with all the server names used in the solution..                                    |
| [JSTable](Database%20Manager/JSTable.md) | [getTable(foundset)](Database%20Manager.md#gettable-foundset)                   | Returns the JSTable object from which more info can be obtained (like columns)..                                    |
| [JSTable](Database%20Manager/JSTable.md) | [getTable(record)](Database%20Manager.md#gettable-record)                   | Returns the JSTable object from which more info can be obtained (like columns)..                                    |
| [JSTable](Database%20Manager/JSTable.md) | [getTable(dataSource)](Database%20Manager.md#gettable-datasource)                   | Returns the JSTable object from which more info can be obtained (like columns)..                                    |
| [JSTable](Database%20Manager/JSTable.md) | [getTable(serverName, tableName)](Database%20Manager.md#gettable-servername-tablename)                   | Returns the JSTable object from which more info can be obtained (like columns)..                                    |
| [Number](JSLib/Number.md) | [getTableCount(dataSource)](Database%20Manager.md#gettablecount-datasource)                   | Returns the total number of records(rows) in a table..                                    |
| [Array](JSLib/Array.md) | [getTableFilterParams(serverName)](Database%20Manager.md#gettablefilterparams-servername)                   | Returns a two dimensional array object containing the table filter information currently applied to the servers tables..                                    |
| [Array](JSLib/Array.md) | [getTableFilterParams(serverName, filterName)](Database%20Manager.md#gettablefilterparams-servername-filtername)                   | Returns a two dimensional array object containing the table filter information currently applied to the servers tables..                                    |
| [Array](JSLib/Array.md) | [getTableNames(serverName)](Database%20Manager.md#gettablenames-servername)                   | Returns an array of all table names for a specified server..                                    |
| [JSFoundSet](Database%20Manager/JSFoundSet.md) | [getViewFoundSet(name)](Database%20Manager.md#getviewfoundset-name)                   | Returns a ViewFoundSet that was created by getViewFoundSet(name,query,register) with the registerd boolean "true"..                                    |
| [JSFoundSet](Database%20Manager/JSFoundSet.md) | [getViewFoundSet(name, query)](Database%20Manager.md#getviewfoundset-name-query)                   | Returns a foundset object for a specified query..                                    |
| [JSFoundSet](Database%20Manager/JSFoundSet.md) | [getViewFoundSet(name, query, register)](Database%20Manager.md#getviewfoundset-name-query-register)                   | Returns a foundset object for a specified query..                                    |
| [Array](JSLib/Array.md) | [getViewNames(serverName)](Database%20Manager.md#getviewnames-servername)                   | Returns an array of all view names for a specified server..                                    |
| [Boolean](JSLib/Boolean.md) | [hasLocks()](Database%20Manager.md#haslocks)                   | Returns true if the current client has any or the specified lock(s) acquired..                                    |
| [Boolean](JSLib/Boolean.md) | [hasLocks(lockName)](Database%20Manager.md#haslocks-lockname)                   | Returns true if the current client has any or the specified lock(s) acquired..                                    |
| [Boolean](JSLib/Boolean.md) | [hasNewRecords(foundset)](Database%20Manager.md#hasnewrecords-foundset)                   | Returns true if the argument (foundSet / record) has at least one row that was not yet saved in the database..                                    |
| [Boolean](JSLib/Boolean.md) | [hasNewRecords(foundset, index)](Database%20Manager.md#hasnewrecords-foundset-index)                   | Returns true if the argument (foundSet / record) has at least one row that was not yet saved in the database..                                    |
| [Boolean](JSLib/Boolean.md) | [hasRecordChanges(foundset)](Database%20Manager.md#hasrecordchanges-foundset)                   | Returns true if the specified foundset, on a specific index or in any of its records, or the specified record has changes or is new unsaved record..                                    |
| [Boolean](JSLib/Boolean.md) | [hasRecordChanges(foundset, index)](Database%20Manager.md#hasrecordchanges-foundset-index)                   | Returns true if the specified foundset, on a specific index or in any of its records, or the specified record has changes or is new unsaved record..                                    |
| [Boolean](JSLib/Boolean.md) | [hasRecords(foundset)](Database%20Manager.md#hasrecords-foundset)                   | Returns true if the (related)foundset exists and has records..                                    |
| [Boolean](JSLib/Boolean.md) | [hasRecords(record, relationString)](Database%20Manager.md#hasrecords-record-relationstring)                   | Returns true if the (related)foundset exists and has records..                                    |
| [Boolean](JSLib/Boolean.md) | [hasTransaction()](Database%20Manager.md#hastransaction)                   | Returns true if there is an transaction active for this client..                                    |
| [Boolean](JSLib/Boolean.md) | [mergeRecords(sourceRecord, combinedDestinationRecord)](Database%20Manager.md#mergerecords-sourcerecord-combineddestinationrecord)                   | Merge records from the same foundset, updates entire datamodel (via foreign type on columns) with destination record pk, deletes source record..                                    |
| [Boolean](JSLib/Boolean.md) | [mergeRecords(sourceRecord, combinedDestinationRecord, columnNames)](Database%20Manager.md#mergerecords-sourcerecord-combineddestinationrecord-columnnames)                   | Merge records from the same foundset, updates entire datamodel (via foreign type on columns) with destination record pk, deletes source record..                                    |
|void | [recalculate(foundsetOrRecord)](Database%20Manager.md#recalculate-foundsetorrecord)                   | Can be used to recalculate a specified record or all rows in the specified foundset..                                    |
| [Boolean](JSLib/Boolean.md) | [refreshRecordFromDatabase(foundset, index)](Database%20Manager.md#refreshrecordfromdatabase-foundset-index)                   | Flushes the client data cache and requeries the data for a record (based on the record index) in a foundset or all records in the foundset..                                    |
| [Boolean](JSLib/Boolean.md) | [releaseAllLocks()](Database%20Manager.md#releasealllocks)                   | Release all current locks the client has (optionally limited to named locks)..                                    |
| [Boolean](JSLib/Boolean.md) | [releaseAllLocks(lockName)](Database%20Manager.md#releasealllocks-lockname)                   | Release all current locks the client has (optionally limited to named locks)..                                    |
| [Boolean](JSLib/Boolean.md) | [removeDataSource(uri)](Database%20Manager.md#removedatasource-uri)                   | Free resources allocated for a previously created data source..                                    |
| [Boolean](JSLib/Boolean.md) | [removeTableFilterParam(serverName, filterName)](Database%20Manager.md#removetablefilterparam-servername-filtername)                   | Removes a previously defined table filter..                                    |
|void | [revertEditedRecords()](Database%20Manager.md#reverteditedrecords)                   | Reverts outstanding (not saved) in memory changes from edited records..                                    |
|void | [revertEditedRecords(foundset)](Database%20Manager.md#reverteditedrecords-foundset)                   | Reverts outstanding (not saved) in memory changes from edited records..                                    |
|void | [rollbackTransaction()](Database%20Manager.md#rollbacktransaction)                   | Rollback a transaction started by databaseManager..                                    |
|void | [rollbackTransaction(rollbackEdited)](Database%20Manager.md#rollbacktransaction-rollbackedited)                   | Rollback a transaction started by databaseManager..                                    |
|void | [rollbackTransaction(rollbackEdited, revertSavedRecords)](Database%20Manager.md#rollbacktransaction-rollbackedited-revertsavedrecords)                   | Rollback a transaction started by databaseManager..                                    |
| [Boolean](JSLib/Boolean.md) | [saveData()](Database%20Manager.md#savedata)                   | Saves all outstanding (unsaved) data and exits the current record..                                    |
| [Boolean](JSLib/Boolean.md) | [saveData(foundset)](Database%20Manager.md#savedata-foundset)                   | Saves all outstanding (unsaved) data and exits the current record..                                    |
| [Boolean](JSLib/Boolean.md) | [saveData(record)](Database%20Manager.md#savedata-record)                   | Saves all outstanding (unsaved) data and exits the current record..                                    |
| [Boolean](JSLib/Boolean.md) | [saveData(records)](Database%20Manager.md#savedata-records)                   | Saves all outstanding (unsaved) data and exits the current record..                                    |
| [Boolean](JSLib/Boolean.md) | [setAutoSave(autoSave)](Database%20Manager.md#setautosave-autosave)                   | Set autosave, if false then no saves will happen by the ui (not including deletes!)..                                    |
|void | [setCreateEmptyFormFoundsets()](Database%20Manager.md#setcreateemptyformfoundsets)                   | Turnoff the initial form foundset record loading, set this in the solution open method..                                    |
| [Boolean](JSLib/Boolean.md) | [setTableFilters(filterName, tableFilters)](Database%20Manager.md#settablefilters-filtername-tablefilters)                   | Apply multiples table filters to all the foundsets that arte affected by the filters..                                    |
|void | [startTransaction()](Database%20Manager.md#starttransaction)                   | Start a database transaction..                                    |
| [Boolean](JSLib/Boolean.md) | [switchServer(sourceName, destinationName)](Database%20Manager.md#switchserver-sourcename-destinationname)                   | Switches a named server to another named server with the same datamodel (recommended to be used in an onOpen method for a solution)..                                    |
| [JSRecordMarkers](Database%20Manager/JSRecordMarkers.md) | [validate(record)](Database%20Manager.md#validate-record)                   | Validates the given record, it runs first the method that is attached to the entity event "onValidate"..                                    |
| [JSRecordMarkers](Database%20Manager/JSRecordMarkers.md) | [validate(record, customObject)](Database%20Manager.md#validate-record-customobject)                   | Validates the given record, it runs first the method that is attached to the entity event "onValidate"..                                    |

## Properties Details

### alwaysFollowPkSelection

Enable/disable the foundset behaviour to keep selection to the first row always, even if updates from other clients are received that add new records before the current first record.

If set to false [default], a foundset with selection on first record will keep the selected index to 1, but may change the selected record when a new record is received from another client.
If set to true, the selected index may change but the selected record will be kept if possible.

**Returns**\
[Boolean](JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
databaseManager.alwaysFollowPkSelection = true; // enable

// test if enabled
if(databaseManager.alwaysFollowPkSelection) application.output('alwaysFollowPkSelection enabled')
```
### disableRelatedSiblingsPrefetch

Enable/disable the automatic prefetching of related foundsets for sibling records.
<p>
For example, when orders from a record in a customer foundset are retrieved, already the orders of a few sibling records are also prefetched.
This is the default behaviour and in most situations this better for performance in user interfaces.
<p>
In some situations performance can be better if this property is set to false to prevent queries for data that is never used.

**Returns**\
[Boolean](JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
databaseManager.disableRelatedSiblingsPrefetch = true; // disable

// test if enabled
if(databaseManager.disableRelatedSiblingsPrefetch) application.output('prefetching of sibling related foundsets is enabled')
```
### nullColumnValidatorEnabled

Enable/disable the default null validator for non null columns, makes it possible to do the checks later on when saving, when for example autosave is disabled.

**Returns**\
[Boolean](JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
databaseManager.nullColumnValidatorEnabled = false;//disable

//test if enabled
if(databaseManager.nullColumnValidatorEnabled) application.output('null validation enabled')
```

## Methods Details

### acquireLock(foundset, recordIndex)

Request lock(s) for a foundset, can be a normal or related foundset.
The record_index can be -1 to lock all rows, 0 to lock the current row, or a specific row of > 0
Optionally name the lock(s) so that it can be referenced it in releaseAllLocks()

By default this call doesn't try to lock records in the database itself. But the locks are tracked  in the Servoy Server itself.
If you need database locking because of others applications that can also read the table or you use the Broadcaster plugin for more then 1 servoy server on the same database,
you need to set the property 'servoy.record.lock.lockInDB' in the servoy.properties file to true. This will try to do a 'select for update no wait' on databases that supports this.
This can only be used together with a transaction, so before you aquire the lock a transaction must be started so the database lock is held on to the transaction connection.

Do not change the record data before that, because aquirelock will make sure with a select from the database that it really has the latest data.
If there are changes to columns that you changed before calling aquireLock these changes will be reverted, so you don't change something again that you didn't see really the value of first.

returns true if the lock could be acquired.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset The JSFoundset to get the lock for\
[Number](JSLib/Number.md) recordIndex The record index which should be locked.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the lock could be acquired.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//locks the complete foundset
databaseManager.acquireLock(foundset,-1);

//locks the current row
databaseManager.acquireLock(foundset,0);

//locks all related orders for the current Customer
var success = databaseManager.acquireLock(Cust_to_Orders,-1);
if(!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to get a lock','OK');
}
```
### acquireLock(foundset, recordIndex, lockName)

Request lock(s) for a foundset, can be a normal or related foundset.
The record_index can be -1 to lock all rows, 0 to lock the current row, or a specific row of > 0
Optionally name the lock(s) so that it can be referenced it in releaseAllLocks()

By default this call doesn't try to lock records in the database itself. But the locks are tracked  in the Servoy Server itself.
If you need database locking because of others applications that can also read the table or you use the Broadcaster plugin for more then 1 servoy server on the same database,
you need to set the property 'servoy.record.lock.lockInDB' in the servoy.properties file to true. This will try to do a 'select for update no wait' on databases that supports this.
This can only be used together with a transaction, so before you aquire the lock a transaction must be started so the database lock is held on to the transaction connection.

Do not change the record data before that, because aquirelock will make sure with a select from the database that it really has the latest data.
If there are changes to columns that you changed before calling aquireLock these changes will be reverted, so you don't change something again that you didn't see really the value of first.

returns true if the lock could be acquired.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset The JSFoundset to get the lock for\
[Number](JSLib/Number.md) recordIndex The record index which should be locked.\
[String](JSLib/String.md) lockName The name of the lock.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the lock could be acquired.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//locks the complete foundset
databaseManager.acquireLock(foundset,-1);

//locks the current row
databaseManager.acquireLock(foundset,0);

//locks all related orders for the current Customer
var success = databaseManager.acquireLock(Cust_to_Orders,-1);
if(!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to get a lock','OK');
}
```
### addTableFilterParam(query)

Adds a filter based on a query to all the foundsets based on a table.

Filters on tables touched in the query will not be applied to the query filter.
For example, when a table filter exists on the order_details table,
a query filter with a join from orders to order_details will be applied to queries on the orders table,
but the filter condition on the orders_details table will not be included.

returns true if the table filter could be applied.

**Parameters**\
[QBSelect](Database%20Manager/QBSelect.md) query condition to filter on.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the table filter could be applied.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Best way to call this in a global solution startup method, but filters may be added/removed at any time.
// Note that

var query = datasources.db.example_data.orders.createSelect();
query.where.add(
   query.or.add(
            query.columns.shipcity.eq('Amersfoort'))
   .add(    query.columns.shipcity.eq('Amsterdam')));

var success = databaseManager.addTableFilterParam(query, 'cityFilter')
```
### addTableFilterParam(query, filterName)

Adds a filter based on a query to all the foundsets based on a table.

Filters on tables touched in the query will not be applied to the query filter.
For example, when a table filter exists on the order_details table,
a query filter with a join from orders to order_details will be applied to queries on the orders table,
but the filter condition on the orders_details table will not be included.

returns true if the table filter could be applied.

**Parameters**\
[QBSelect](Database%20Manager/QBSelect.md) query condition to filter on.\
[String](JSLib/String.md) filterName The specified name of the database table filter.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the table filter could be applied.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Best way to call this in a global solution startup method, but filters may be added/removed at any time.
// Note that

var query = datasources.db.example_data.orders.createSelect();
query.where.add(
   query.or.add(
            query.columns.shipcity.eq('Amersfoort'))
   .add(    query.columns.shipcity.eq('Amsterdam')));

var success = databaseManager.addTableFilterParam(query, 'cityFilter')
```
### addTableFilterParam(datasource, dataprovider, operator, value)

Adds a filter to all the foundsets based on a table.
Note: if null is provided as the tablename the filter will be applied on all tables with the dataprovider name.
A dataprovider can have multiple filters defined, they will all be applied.
returns true if the table filter could be applied.

**Parameters**\
[String](JSLib/String.md) datasource The datasource\
[String](JSLib/String.md) dataprovider A specified dataprovider column name.\
[String](JSLib/String.md) operator One of "=, <, >, >=, <=, !=, LIKE, or IN" optionally augmented with modifiers "#" (ignore case) or "^||" (or-is-null), prefix with "sql:" to allow the value to be interpreted as a custom query.\
[Object](JSLib/Object.md) value The specified filter value.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the table filter could be applied.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Best way to call this in a global solution startup method, but filters may be added/removed at any time.
// Note that multiple filters can be added to the same dataprovider, they will all be applied.

// filter on messages table where messagesid>10, the filter has a name so it can be removed using databaseManager.removeTableFilterParam()
var success = databaseManager.addTableFilterParam('admin', 'messages', 'messagesid', '>', 10, 'higNumberedMessagesRule')

// a filter can be created based on a query
var query = datasources.db.admin.messages.createSelect()
query.where.add(query.columns.messagesid.gt(10))
var success = databaseManager.addTableFilterParam(query, 'higNumberedMessagesRule')

// all tables that have the companyid column should be filtered
var success = databaseManager.addTableFilterParam('crm', null, 'companyidid', '=', currentcompanyid)

// some filters with in-conditions
var success = databaseManager.addTableFilterParam('crm', 'products', 'productcode', 'in', [120, 144, 200])
// use "sql:in" in stead of "in" to allow the value to be interpreted as a custom query
var success = databaseManager.addTableFilterParam('crm', 'orders', 'countrycode', 'sql:in', 'select country code from countries where region = "Europe"')

// you can use modifiers in the operator as well, filter on companies where companyname is null or equals-ignore-case 'servoy'
var success = databaseManager.addTableFilterParam('crm', 'companies', 'companyname', '#^||=', 'servoy')

// the value may be null, this will result in 'column is null' sql condition.
var success = databaseManager.addTableFilterParam('crm', 'companies', 'verified', '=', null)

//if you want to add a filter for a column (created by you) in the i18n table
databaseManager.addTableFilterParam('database', 'your_i18n_table', 'message_variant', 'in', [1, 2])
```
### addTableFilterParam(datasource, dataprovider, operator, value, filterName)

Adds a filter to all the foundsets based on a table.
Note: if null is provided as the tablename the filter will be applied on all tables with the dataprovider name.
A dataprovider can have multiple filters defined, they will all be applied.
returns true if the table filter could be applied.

**Parameters**\
[String](JSLib/String.md) datasource The datasource\
[String](JSLib/String.md) dataprovider A specified dataprovider column name.\
[String](JSLib/String.md) operator One of "=, <, >, >=, <=, !=, LIKE, or IN" optionally augmented with modifiers "#" (ignore case) or "^||" (or-is-null), prefix with "sql:" to allow the value to be interpreted as a custom query.\
[Object](JSLib/Object.md) value The specified filter value.\
[String](JSLib/String.md) filterName The specified name of the database table filter.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the table filter could be applied.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Best way to call this in a global solution startup method, but filters may be added/removed at any time.
// Note that multiple filters can be added to the same dataprovider, they will all be applied.

// filter on messages table where messagesid>10, the filter has a name so it can be removed using databaseManager.removeTableFilterParam()
var success = databaseManager.addTableFilterParam('admin', 'messages', 'messagesid', '>', 10, 'higNumberedMessagesRule')

// a filter can be created based on a query
var query = datasources.db.admin.messages.createSelect()
query.where.add(query.columns.messagesid.gt(10))
var success = databaseManager.addTableFilterParam(query, 'higNumberedMessagesRule')

// all tables that have the companyid column should be filtered
var success = databaseManager.addTableFilterParam('crm', null, 'companyidid', '=', currentcompanyid)

// some filters with in-conditions
var success = databaseManager.addTableFilterParam('crm', 'products', 'productcode', 'in', [120, 144, 200])
// use "sql:in" in stead of "in" to allow the value to be interpreted as a custom query
var success = databaseManager.addTableFilterParam('crm', 'orders', 'countrycode', 'sql:in', 'select country code from countries where region = "Europe"')

// you can use modifiers in the operator as well, filter on companies where companyname is null or equals-ignore-case 'servoy'
var success = databaseManager.addTableFilterParam('crm', 'companies', 'companyname', '#^||=', 'servoy')

// the value may be null, this will result in 'column is null' sql condition.
var success = databaseManager.addTableFilterParam('crm', 'companies', 'verified', '=', null)

//if you want to add a filter for a column (created by you) in the i18n table
databaseManager.addTableFilterParam('database', 'your_i18n_table', 'message_variant', 'in', [1, 2])
```
### addTableFilterParam(serverName, tableName, dataprovider, operator, value)

Adds a filter to all the foundsets based on a table.
Note: if null is provided as the tablename the filter will be applied on all tables with the dataprovider name.
A dataprovider can have multiple filters defined, they will all be applied.
returns true if the table filter could be applied.

**Parameters**\
[String](JSLib/String.md) serverName The name of the database server connection for the specified table name.\
[String](JSLib/String.md) tableName The name of the specified table.\
[String](JSLib/String.md) dataprovider A specified dataprovider column name.\
[String](JSLib/String.md) operator One of "=, <, >, >=, <=, !=, LIKE, or IN" optionally augmented with modifiers "#" (ignore case) or "^||" (or-is-null), prefix with "sql:" to allow the value to be interpreted as a custom query.\
[Object](JSLib/Object.md) value The specified filter value.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the table filter could be applied.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Best way to call this in a global solution startup method, but filters may be added/removed at any time.
// Note that multiple filters can be added to the same dataprovider, they will all be applied.

// filter on messages table where messagesid>10, the filter has a name so it can be removed using databaseManager.removeTableFilterParam()
var success = databaseManager.addTableFilterParam('admin', 'messages', 'messagesid', '>', 10, 'higNumberedMessagesRule')

// a filter can be created based on a query
var query = datasources.db.admin.messages.createSelect()
query.where.add(query.columns.messagesid.gt(10))
var success = databaseManager.addTableFilterParam(query, 'higNumberedMessagesRule')

// all tables that have the companyid column should be filtered
var success = databaseManager.addTableFilterParam('crm', null, 'companyidid', '=', currentcompanyid)

// some filters with in-conditions
var success = databaseManager.addTableFilterParam('crm', 'products', 'productcode', 'in', [120, 144, 200])
// use "sql:in" in stead of "in" to allow the value to be interpreted as a custom query
var success = databaseManager.addTableFilterParam('crm', 'orders', 'countrycode', 'sql:in', 'select country code from countries where region = "Europe"')

// you can use modifiers in the operator as well, filter on companies where companyname is null or equals-ignore-case 'servoy'
var success = databaseManager.addTableFilterParam('crm', 'companies', 'companyname', '#^||=', 'servoy')

// the value may be null, this will result in 'column is null' sql condition.
var success = databaseManager.addTableFilterParam('crm', 'companies', 'verified', '=', null)

//if you want to add a filter for a column (created by you) in the i18n table
databaseManager.addTableFilterParam('database', 'your_i18n_table', 'message_variant', 'in', [1, 2])
```
### addTableFilterParam(serverName, tableName, dataprovider, operator, value, filterName)

Adds a filter to all the foundsets based on a table.
Note: if null is provided as the tablename the filter will be applied on all tables with the dataprovider name.
A dataprovider can have multiple filters defined, they will all be applied.
returns true if the table filter could be applied.

**Parameters**\
[String](JSLib/String.md) serverName The name of the database server connection for the specified table name.\
[String](JSLib/String.md) tableName The name of the specified table.\
[String](JSLib/String.md) dataprovider A specified dataprovider column name.\
[String](JSLib/String.md) operator One of "=, <, >, >=, <=, !=, LIKE, or IN" optionally augmented with modifiers "#" (ignore case) or "^||" (or-is-null), prefix with "sql:" to allow the value to be interpreted as a custom query..\
[Object](JSLib/Object.md) value The specified filter value.\
[String](JSLib/String.md) filterName The specified name of the database table filter.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the table filter could be applied.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Best way to call this in a global solution startup method, but filters may be added/removed at any time.
// Note that multiple filters can be added to the same dataprovider, they will all be applied.

// filter on messages table where messagesid>10, the filter has a name so it can be removed using databaseManager.removeTableFilterParam()
var success = databaseManager.addTableFilterParam('admin', 'messages', 'messagesid', '>', 10, 'higNumberedMessagesRule')

// a filter can be created based on a query
var query = datasources.db.admin.messages.createSelect()
query.where.add(query.columns.messagesid.gt(10))
var success = databaseManager.addTableFilterParam(query, 'higNumberedMessagesRule')

// all tables that have the companyid column should be filtered
var success = databaseManager.addTableFilterParam('crm', null, 'companyidid', '=', currentcompanyid)

// some filters with in-conditions
var success = databaseManager.addTableFilterParam('crm', 'products', 'productcode', 'in', [120, 144, 200])
// use "sql:in" in stead of "in" to allow the value to be interpreted as a custom query
var success = databaseManager.addTableFilterParam('crm', 'orders', 'countrycode', 'sql:in', 'select country code from countries where region = "Europe"')

// you can use modifiers in the operator as well, filter on companies where companyname is null or equals-ignore-case 'servoy'
var success = databaseManager.addTableFilterParam('crm', 'companies', 'companyname', '#^||=', 'servoy')

// the value may be null, this will result in 'column is null' sql condition.
var success = databaseManager.addTableFilterParam('crm', 'companies', 'verified', '=', null)

//if you want to add a filter for a column (created by you) in the i18n table
databaseManager.addTableFilterParam('database', 'your_i18n_table', 'message_variant', 'in', [1, 2])
```
### addTrackingInfo(columnName, value)

Add tracking info used in the log table.
When tracking is enabled and a new row is inserted in the log table,
if it has a column named 'columnName', its value will be set with 'value'

**Parameters**\
[String](JSLib/String.md) columnName The name of the column in the log table, used for tracking info\
[Object](JSLib/Object.md) value The value to be set when inserting a new row in the log table, for the 'columnName' column

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
databaseManager.addTrackingInfo('log_column_name', 'trackingInfo')
```
### commitTransaction()

Returns true if a transaction is committed; rollback if commit fails.
Saves all edited records and commits the data.


**Returns**\
[Boolean](JSLib/Boolean.md) if the transaction could be committed.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// starts a database transaction
databaseManager.startTransaction()
// Now let users input data

// when data has been entered do a commit or rollback if the data entry is canceled or the the commit did fail.
if (cancel || !databaseManager.commitTransaction())
{
	databaseManager.rollbackTransaction();
}
```
### commitTransaction(saveFirst)

Returns true if a transaction is committed; rollback if commit fails.

**Parameters**\
[Boolean](JSLib/Boolean.md) saveFirst save edited records to the database first (default true)

**Returns**\
[Boolean](JSLib/Boolean.md) if the transaction could be committed.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// starts a database transaction
databaseManager.startTransaction()
// Now let users input data

// when data has been entered do a commit or rollback if the data entry is canceled or the the commit did fail.
if (cancel || !databaseManager.commitTransaction())
{
	databaseManager.rollbackTransaction();
}
```
### commitTransaction(saveFirst, revertSavedRecords)

Returns true if a transaction is committed; rollback if commit fails.

**Parameters**\
[Boolean](JSLib/Boolean.md) saveFirst save edited records to the database first (default true)\
[Boolean](JSLib/Boolean.md) revertSavedRecords if a commit fails and a rollback is done, the when given false the records are not reverted to the database state (and are in edited records again)

**Returns**\
[Boolean](JSLib/Boolean.md) if the transaction could be committed.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// starts a database transaction
databaseManager.startTransaction()
// Now let users input data

// when data has been entered do a commit or rollback if the data entry is canceled or the the commit did fail.
if (cancel || !databaseManager.commitTransaction())
{
	databaseManager.rollbackTransaction();
}
```
### convertFoundSet(foundset, related)

Creates a foundset that combines all the records of the specified one-to-many relation seen from the given parent/primary foundset.
The created foundset will not contain records that have not been saved in the database, because the records in the foundset will be the
result of a select query to the database.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset The JSFoundset to convert.\
[JSFoundSet](Database%20Manager/JSFoundSet.md) related can be a one-to-many relation object or the name of a one-to-many relation

**Returns**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) The converted JSFoundset.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Convert in the order form a orders foundset into a orderdetails foundset,
// that has all the orderdetails from all the orders in the foundset.
var convertedFoundSet = databaseManager.convertFoundSet(foundset,order_to_orderdetails);
// or var convertedFoundSet = databaseManager.convertFoundSet(foundset,"order_to_orderdetails");
forms.orderdetails.controller.showRecords(convertedFoundSet);
```
### convertFoundSet(foundset, related)

Creates a foundset that combines all the records of the specified one-to-many relation seen from the given parent/primary foundset.
The created foundset will not contain records that have not been saved in the database, because the records in the foundset will be the
result of a select query to the database.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset The JSFoundset to convert.\
[String](JSLib/String.md) related the name of a one-to-many relation

**Returns**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) The converted JSFoundset.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Convert in the order form a orders foundset into a orderdetails foundset,
// that has all the orderdetails from all the orders in the foundset.
var convertedFoundSet = databaseManager.convertFoundSet(foundset,order_to_orderdetails);
// or var convertedFoundSet = databaseManager.convertFoundSet(foundset,"order_to_orderdetails");
forms.orderdetails.controller.showRecords(convertedFoundSet);
```
### convertToDataSet(foundset)

Converts the argument to a JSDataSet, possible use in controller.loadRecords(dataset).
The optional array of dataprovider names is used (only) to add the specified dataprovider names as columns to the dataset.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset The foundset to be converted.

**Returns**\
[JSDataSet](Database%20Manager/JSDataSet.md) JSDataSet with the data.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// converts a foundset pks to a dataset
var dataset = databaseManager.convertToDataSet(foundset);
// converts a foundset to a dataset
//var dataset = databaseManager.convertToDataSet(foundset,['product_id','product_name']);
// converts an object array to a dataset
//var dataset = databaseManager.convertToDataSet(files,['name','path']);
// converts an array to a dataset
//var dataset = databaseManager.convertToDataSet(new Array(1,2,3,4,5,6));
// converts an string list to a dataset
//var dataset = databaseManager.convertToDataSet('4,5,6');
```
### convertToDataSet(foundset, dataproviderNames)

Converts the argument to a JSDataSet, possible use in controller.loadRecords(dataset).
The optional array of dataprovider names is used (only) to add the specified dataprovider names as columns to the dataset.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset The foundset to be converted.\
[Array](JSLib/Array.md) dataproviderNames Array with column names.

**Returns**\
[JSDataSet](Database%20Manager/JSDataSet.md) JSDataSet with the data.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// converts a foundset pks to a dataset
var dataset = databaseManager.convertToDataSet(foundset);
// converts a foundset to a dataset
//var dataset = databaseManager.convertToDataSet(foundset,['product_id','product_name']);
// converts an object array to a dataset
//var dataset = databaseManager.convertToDataSet(files,['name','path']);
// converts an array to a dataset
//var dataset = databaseManager.convertToDataSet(new Array(1,2,3,4,5,6));
// converts an string list to a dataset
//var dataset = databaseManager.convertToDataSet('4,5,6');
```
### convertToDataSet(values)

Converts the argument to a JSDataSet, possible use in controller.loadRecords(dataset).
The optional array of dataprovider names is used (only) to add the specified dataprovider names as columns to the dataset.

**Parameters**\
[Array](JSLib/Array.md) values The values array.

**Returns**\
[JSDataSet](Database%20Manager/JSDataSet.md) JSDataSet with the data.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// converts a foundset pks to a dataset
var dataset = databaseManager.convertToDataSet(foundset);
// converts a foundset to a dataset
//var dataset = databaseManager.convertToDataSet(foundset,['product_id','product_name']);
// converts an object array to a dataset
//var dataset = databaseManager.convertToDataSet(files,['name','path']);
// converts an array to a dataset
//var dataset = databaseManager.convertToDataSet(new Array(1,2,3,4,5,6));
// converts an string list to a dataset
//var dataset = databaseManager.convertToDataSet('4,5,6');
```
### convertToDataSet(values, dataproviderNames)

Converts the argument to a JSDataSet, possible use in controller.loadRecords(dataset).
The optional array of dataprovider names is used (only) to add the specified dataprovider names as columns to the dataset.

**Parameters**\
[Array](JSLib/Array.md) values The values array.\
[Array](JSLib/Array.md) dataproviderNames The property names array.

**Returns**\
[JSDataSet](Database%20Manager/JSDataSet.md) JSDataSet with the data.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// converts a foundset pks to a dataset
var dataset = databaseManager.convertToDataSet(foundset);
// converts a foundset to a dataset
//var dataset = databaseManager.convertToDataSet(foundset,['product_id','product_name']);
// converts an object array to a dataset
//var dataset = databaseManager.convertToDataSet(files,['name','path']);
// converts an array to a dataset
//var dataset = databaseManager.convertToDataSet(new Array(1,2,3,4,5,6));
// converts an string list to a dataset
//var dataset = databaseManager.convertToDataSet('4,5,6');
```
### convertToDataSet(ids)

Converts the argument to a JSDataSet, possible use in controller.loadRecords(dataset).
The optional array of dataprovider names is used (only) to add the specified dataprovider names as columns to the dataset.

**Parameters**\
[String](JSLib/String.md) ids Concatenated values to be put into dataset.

**Returns**\
[JSDataSet](Database%20Manager/JSDataSet.md) JSDataSet with the data.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// converts a foundset pks to a dataset
var dataset = databaseManager.convertToDataSet(foundset);
// converts a foundset to a dataset
//var dataset = databaseManager.convertToDataSet(foundset,['product_id','product_name']);
// converts an object array to a dataset
//var dataset = databaseManager.convertToDataSet(files,['name','path']);
// converts an array to a dataset
//var dataset = databaseManager.convertToDataSet(new Array(1,2,3,4,5,6));
// converts an string list to a dataset
//var dataset = databaseManager.convertToDataSet('4,5,6');
```
### copyMatchingFields(source, destination)

Copies all matching non empty columns (if overwrite boolean is given all columns except pk/ident, if array then all columns except pk and array names).
The matching requires the properties and getter functions of the source to match those of the destination; for the getter functions,
the 'get' will be removed and the remaining name will be converted to lowercase before attempting to match.
Returns true if no error occurred.

NOTE: This function could be used to store a copy of records in an archive table. Use the getRecord() function to get the record as an object.
Before trying this example, please make sure that the foundsets have some records loaded:

**Parameters**\
[Object](JSLib/Object.md) source The source record or (java/javascript)object to be copied.\
[JSRecord](Database%20Manager/JSRecord.md) destination The destination record to copy to.

**Returns**\
[Boolean](JSLib/Boolean.md) true if no errors happened.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
otherfoundset.loadAllRecords();
for( var i = 1 ; i <= foundset.getSize() ; i++ )
{
	var srcRecord = foundset.getRecord(i);
	var destRecord = otherfoundset.getRecord(i);
	if (srcRecord == null || destRecord == null) break;
	databaseManager.copyMatchingFields(srcRecord,destRecord,true)
}
//saves any outstanding changes to the dest foundset
databaseManager.saveData();

//copying from a MailMessage JavaScript object
//var _msg = plugins.mail.receiveMail(login, password, true, 0, null, properties);
//if (_msg != null)
//{
//	controller.newRecord();
//	var srcObject = _msg[0];
//	var destRecord = foundset.getSelectedRecord();
//	databaseManager.copyMatchingFields(srcObject, destRecord, true);
//	databaseManager.saveData();
//}
```
### copyMatchingFields(source, destination, overwrite)

Copies all matching non empty columns (if overwrite boolean is given all columns except pk/ident, if array then all columns except pk and array names).
The matching requires the properties and getter functions of the source to match those of the destination; for the getter functions,
the 'get' will be removed and the remaining name will be converted to lowercase before attempting to match.
Returns true if no error occurred.

NOTE: This function could be used to store a copy of records in an archive table. Use the getRecord() function to get the record as an object.
Before trying this example, please make sure that the foundsets have some records loaded:

**Parameters**\
[Object](JSLib/Object.md) source The source record or (java/javascript)object to be copied.\
[JSRecord](Database%20Manager/JSRecord.md) destination The destination record to copy to.\
[Boolean](JSLib/Boolean.md) overwrite Boolean values to overwrite all values. If overwrite is false/not provided, then the non empty values are not overwritten in the destination record.

**Returns**\
[Boolean](JSLib/Boolean.md) true if no errors happened.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
otherfoundset.loadAllRecords();
for( var i = 1 ; i <= foundset.getSize() ; i++ )
{
	var srcRecord = foundset.getRecord(i);
	var destRecord = otherfoundset.getRecord(i);
	if (srcRecord == null || destRecord == null) break;
	databaseManager.copyMatchingFields(srcRecord,destRecord,true)
}
//saves any outstanding changes to the dest foundset
databaseManager.saveData();

//copying from a MailMessage JavaScript object
//var _msg = plugins.mail.receiveMail(login, password, true, 0, null, properties);
//if (_msg != null)
//{
//	controller.newRecord();
//	var srcObject = _msg[0];
//	var destRecord = foundset.getSelectedRecord();
//	databaseManager.copyMatchingFields(srcObject, destRecord, true);
//	databaseManager.saveData();
//}
```
### copyMatchingFields(source, destination, names)

Copies all matching non empty columns (if overwrite boolean is given all columns except pk/ident, if array then all columns except pk and array names).
The matching requires the properties and getter functions of the source to match those of the destination; for the getter functions,
the 'get' will be removed and the remaining name will be converted to lowercase before attempting to match.
Returns true if no error occurred.

NOTE: This function could be used to store a copy of records in an archive table. Use the getRecord() function to get the record as an object.
Before trying this example, please make sure that the foundsets have some records loaded:

**Parameters**\
[Object](JSLib/Object.md) source The source record or (java/javascript)object to be copied.\
[JSRecord](Database%20Manager/JSRecord.md) destination The destination record to copy to.\
[Array](JSLib/Array.md) names The property names that shouldn't be overriden.

**Returns**\
[Boolean](JSLib/Boolean.md) true if no errors happened.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
otherfoundset.loadAllRecords();
for( var i = 1 ; i <= foundset.getSize() ; i++ )
{
	var srcRecord = foundset.getRecord(i);
	var destRecord = otherfoundset.getRecord(i);
	if (srcRecord == null || destRecord == null) break;
	databaseManager.copyMatchingFields(srcRecord,destRecord,true)
}
//saves any outstanding changes to the dest foundset
databaseManager.saveData();

//copying from a MailMessage JavaScript object
//var _msg = plugins.mail.receiveMail(login, password, true, 0, null, properties);
//if (_msg != null)
//{
//	controller.newRecord();
//	var srcObject = _msg[0];
//	var destRecord = foundset.getSelectedRecord();
//	databaseManager.copyMatchingFields(srcObject, destRecord, true);
//	databaseManager.saveData();
//}
```
### createDataSourceByQuery(name, query, useTableFilters, max_returned_rows, types, pkNames)

Performs a query and saves the result in a datasource.
Will throw an exception if anything went wrong when executing the query.
Column types in the datasource are inferred from the query result or can be explicitly specified.

A datasource can be reused if the data has the same signature (column names and types).
A new createDataSourceByQuery() call will clear the datasource contents from a previous call and insert the current data.

**Parameters**\
[String](JSLib/String.md) name Data source name\
[QBSelect](Database%20Manager/QBSelect.md) query The query builder to be executed.\
[Boolean](JSLib/Boolean.md) useTableFilters use table filters (default true).\
[Number](JSLib/Number.md) max_returned_rows The maximum number of rows returned by the query.\
[Array](JSLib/Array.md) types The column types, when null the types are inferred from the query.\
[Array](JSLib/Array.md) pkNames array of pk names, when null a hidden pk-column will be added

**Returns**\
[String](JSLib/String.md) datasource containing the results of the query or null if the parameters are wrong.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// select customer data for order 1234
var q = datasources.db.example_data.customers.createSelect()
q.result.add(q.columns.customer_id).add(q.columns.city).add(q.columns.country);
q.where.add(q.joins.customers_to_orders.columns.orderid.eq(1234));
var uri = databaseManager.createDataSourceByQuery('mydata', q, true, 999, null, ['customer_id']);
//var uri = databaseManager.createDataSourceByQuery('mydata', q, true, 999, [JSColumn.TEXT, JSColumn.TEXT, JSColumn.TEXT], ['customer_id']);

// the uri can be used to create a form using solution model
var myForm = solutionModel.newForm('newForm', uri, 'myStyleName', false, 800, 600);
myForm.newTextField('city', 140, 20, 140,20);

// the uri can be used to acces a foundset directly
var fs = databaseManager.getFoundSet(uri);
fs.loadAllRecords();
```
### createDataSourceByQuery(name, query, max_returned_rows)

Performs a query and saves the result in a datasource.
Will throw an exception if anything went wrong when executing the query.
Column types in the datasource are inferred from the query result or can be explicitly specified.

A datasource can be reused if the data has the same signature (column names and types).
A new createDataSourceByQuery() call will clear the datasource contents from a previous call and insert the current data.

**Parameters**\
[String](JSLib/String.md) name data source name\
[QBSelect](Database%20Manager/QBSelect.md) query The query builder to be executed.\
[Number](JSLib/Number.md) max_returned_rows The maximum number of rows returned by the query.

**Returns**\
[String](JSLib/String.md) datasource containing the results of the query or null if the parameters are wrong.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// select customer data for order 1234
var q = datasources.db.example_data.customers.createSelect()
q.result.add(q.columns.customer_id).add(q.columns.city).add(q.columns.country);
q.where.add(q.joins.customers_to_orders.columns.orderid.eq(1234));
var uri = databaseManager.createDataSourceByQuery('mydata', q, true, 999, null, ['customer_id']);
//var uri = databaseManager.createDataSourceByQuery('mydata', q, true, 999, [JSColumn.TEXT, JSColumn.TEXT, JSColumn.TEXT], ['customer_id']);

// the uri can be used to create a form using solution model
var myForm = solutionModel.newForm('newForm', uri, 'myStyleName', false, 800, 600);
myForm.newTextField('city', 140, 20, 140,20);

// the uri can be used to acces a foundset directly
var fs = databaseManager.getFoundSet(uri);
fs.loadAllRecords();
```
### createDataSourceByQuery(name, query, max_returned_rows, types)

Performs a query and saves the result in a datasource.
Will throw an exception if anything went wrong when executing the query.
Column types in the datasource are inferred from the query result or can be explicitly specified.

Using this variation of createDataSourceByQuery any Tablefilter on the involved tables will be taken into account.

A datasource can be reused if the data has the same signature (column names and types).
A new createDataSourceByQuery() call will clear the datasource contents from a previous call and insert the current data.

**Parameters**\
[String](JSLib/String.md) name Data source name\
[QBSelect](Database%20Manager/QBSelect.md) query The query builder to be executed.\
[Number](JSLib/Number.md) max_returned_rows The maximum number of rows returned by the query.\
[Array](JSLib/Array.md) types The column types

**Returns**\
[String](JSLib/String.md) datasource containing the results of the query or null if the parameters are wrong.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// select customer data for order 1234
var q = datasources.db.example_data.customers.createSelect();
q.result.add(q.columns.address).add(q.columns.city).add(q.columns.country);
q.where.add(q.joins.customers_to_orders.columns.orderid.eq(1234));
var uri = databaseManager.createDataSourceByQuery('mydata', q, 999);
//var uri = databaseManager.createDataSourceByQuery('mydata', q, 999, [JSColumn.TEXT, JSColumn.TEXT, JSColumn.TEXT]);

// the uri can be used to create a form using solution model
var myForm = solutionModel.newForm('newForm', uri, 'myStyleName', false, 800, 600);
myForm.newTextField('city', 140, 20, 140,20);

// the uri can be used to acces a foundset directly
var fs = databaseManager.getFoundSet(uri);
fs.loadAllRecords();
```
### createDataSourceByQuery(name, query, max_returned_rows, types, pkNames)

Performs a query and saves the result in a datasource.
Will throw an exception if anything went wrong when executing the query.
Column types in the datasource are inferred from the query result or can be explicitly specified.

Using this variation of createDataSourceByQuery any Tablefilter on the involved tables will be taken into account.

A datasource can be reused if the data has the same signature (column names and types).
A new createDataSourceByQuery() call will clear the datasource contents from a previous call and insert the current data.

**Parameters**\
[String](JSLib/String.md) name Data source name\
[QBSelect](Database%20Manager/QBSelect.md) query The query builder to be executed.\
[Number](JSLib/Number.md) max_returned_rows The maximum number of rows returned by the query.\
[Array](JSLib/Array.md) types The column types\
[Array](JSLib/Array.md) pkNames array of pk names, when null a hidden pk-column will be added

**Returns**\
[String](JSLib/String.md) datasource containing the results of the query or null if the parameters are wrong.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// select customer data for order 1234
var q = datasources.db.example_data.customers.createSelect();
q.result.add(q.columns.customer_id).add(q.columns.city).add(q.columns.country);
q.where.add(q.joins.customers_to_orders.columns.orderid.eq(1234));
var uri = databaseManager.createDataSourceByQuery('mydata', q, 999, null, ['customer_id']);
//var uri = databaseManager.createDataSourceByQuery('mydata', q, 999, [JSColumn.TEXT, JSColumn.TEXT, JSColumn.TEXT], ['customer_id']);

// the uri can be used to create a form using solution model
var myForm = solutionModel.newForm('newForm', uri, 'myStyleName', false, 800, 600);
myForm.newTextField('city', 140, 20, 140,20);

// the uri can be used to acces a foundset directly
var fs = databaseManager.getFoundSet(uri);
fs.loadAllRecords();
```
### createDataSourceByQuery(name, server_name, sql_query, arguments, max_returned_rows)

Performs a sql query on the specified server, saves the the result in a datasource.
Will throw an exception if anything went wrong when executing the query.
Column types in the datasource are inferred from the query result or can be explicitly specified.

Using this variation of createDataSourceByQuery any Tablefilter on the involved tables will be disregarded.

A datasource can be reused if the data has the same signature (column names and types).
A new createDataSourceByQuery() call will clear the datasource contents from a previous call and insert the current data.

**Parameters**\
[String](JSLib/String.md) name data source name\
[String](JSLib/String.md) server_name The name of the server where the query should be executed.\
[String](JSLib/String.md) sql_query The custom sql, must start with 'select', 'call', 'with' or 'declare'.\
[Array](JSLib/Array.md) arguments Specified arguments or null if there are no arguments.\
[Number](JSLib/Number.md) max_returned_rows The maximum number of rows returned by the query.

**Returns**\
[String](JSLib/String.md) datasource containing the results of the query or null if the parameters are wrong.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var query = 'select address, city, country  from customers';
var uri = databaseManager.createDataSourceByQuery('mydata', 'example_data', query, null, 999);
//var uri = databaseManager.createDataSourceByQuery('mydata', 'example_data', query, null, 999, [JSColumn.TEXT, JSColumn.TEXT, JSColumn.TEXT]);

// the uri can be used to create a form using solution model
var myForm = solutionModel.newForm('newForm', uri, 'myStyleName', false, 800, 600)
myForm.newTextField('city', 140, 20, 140,20)

// the uri can be used to acces a foundset directly
var fs = databaseManager.getFoundSet(uri)
fs.loadAllRecords();
```
### createDataSourceByQuery(name, server_name, sql_query, arguments, max_returned_rows, types)

Performs a sql query on the specified server, saves the the result in a datasource.
Will throw an exception if anything went wrong when executing the query.
Column types in the datasource are inferred from the query result or can be explicitly specified.

Using this variation of createDataSourceByQuery any Tablefilter on the involved tables will be disregarded.

A datasource can be reused if the data has the same signature (column names and types).
A new createDataSourceByQuery() call will clear the datasource contents from a previous call and insert the current data.

**Parameters**\
[String](JSLib/String.md) name data source name\
[String](JSLib/String.md) server_name The name of the server where the query should be executed.\
[String](JSLib/String.md) sql_query The custom sql, must start with 'select', 'call', 'with' or 'declare'.\
[Array](JSLib/Array.md) arguments Specified arguments or null if there are no arguments.\
[Number](JSLib/Number.md) max_returned_rows The maximum number of rows returned by the query.\
[Array](JSLib/Array.md) types The column types

**Returns**\
[String](JSLib/String.md) datasource containing the results of the query or null if the parameters are wrong.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var query = 'select address, city, country  from customers';
var uri = databaseManager.createDataSourceByQuery('mydata', 'example_data', query, null, 999);
//var uri = databaseManager.createDataSourceByQuery('mydata', 'example_data', query, null, 999, [JSColumn.TEXT, JSColumn.TEXT, JSColumn.TEXT]);

// the uri can be used to create a form using solution model
var myForm = solutionModel.newForm('newForm', uri, 'myStyleName', false, 800, 600)
myForm.newTextField('city', 140, 20, 140,20)

// the uri can be used to acces a foundset directly
var fs = databaseManager.getFoundSet(uri)
fs.loadAllRecords();
```
### createDataSourceByQuery(name, server_name, sql_query, arguments, max_returned_rows, columnTypes, pkNames)

Performs a sql query on the specified server, saves the the result in a datasource.
Will throw an exception if anything went wrong when executing the query.
Column types in the datasource are inferred from the query result or can be explicitly specified.

Using this variation of createDataSourceByQuery any Tablefilter on the involved tables will be disregarded.

A datasource can be reused if the data has the same signature (column names and types).
A new createDataSourceByQuery() call will clear the datasource contents from a previous call and insert the current data.

**Parameters**\
[String](JSLib/String.md) name data source name\
[String](JSLib/String.md) server_name The name of the server where the query should be executed.\
[String](JSLib/String.md) sql_query The custom sql, must start with 'select', 'call', 'with' or 'declare'.\
[Array](JSLib/Array.md) arguments Specified arguments or null if there are no arguments.\
[Number](JSLib/Number.md) max_returned_rows The maximum number of rows returned by the query.\
[Object](JSLib/Object.md) columnTypes The column types\
[Array](JSLib/Array.md) pkNames array of pk names, when null a hidden pk-column will be added

**Returns**\
[String](JSLib/String.md) datasource containing the results of the query or null if the parameters are wrong.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var query = 'select customer_id, address, city, country  from customers';
var uri = databaseManager.createDataSourceByQuery('mydata', 'example_data', query, null, 999);
//var uri = databaseManager.createDataSourceByQuery('mydata', 'example_data', query, null, 999, [JSColumn.TEXT, JSColumn.TEXT, JSColumn.TEXT], ['customer_id']);

// the uri can be used to create a form using solution model
var myForm = solutionModel.newForm('newForm', uri, 'myStyleName', false, 800, 600)
myForm.newTextField('city', 140, 20, 140,20)

// the uri can be used to acces a foundset directly
var fs = databaseManager.getFoundSet(uri)
fs.loadAllRecords();
```
### createEmptyDataSet()

Returns an empty dataset object.


**Returns**\
[JSDataSet](Database%20Manager/JSDataSet.md) An empty JSDataSet with the initial sizes.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// gets an empty dataset with a specifed row and column count
var dataset = databaseManager.createEmptyDataSet(10,10)
// gets an empty dataset with a specifed row count and column array
var dataset2 = databaseManager.createEmptyDataSet(10,new Array ('a','b','c','d'))
```
### createEmptyDataSet(rowCount, columnCount)

Returns an empty dataset object.

**Parameters**\
[Number](JSLib/Number.md) rowCount The number of rows in the DataSet object.\
[Number](JSLib/Number.md) columnCount Number of columns.

**Returns**\
[JSDataSet](Database%20Manager/JSDataSet.md) An empty JSDataSet with the initial sizes.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// gets an empty dataset with a specifed row and column count
var dataset = databaseManager.createEmptyDataSet(10,10)
// gets an empty dataset with a specifed row count and column array
var dataset2 = databaseManager.createEmptyDataSet(10,new Array ('a','b','c','d'))
```
### createEmptyDataSet(rowCount, columnNames)

Returns an empty dataset object.

**Parameters**\
[Number](JSLib/Number.md) rowCount  ;\
[Array](JSLib/Array.md) columnNames  ;

**Returns**\
[JSDataSet](Database%20Manager/JSDataSet.md) An empty JSDataSet with the initial sizes.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// gets an empty dataset with a specifed row and column count
var dataset = databaseManager.createEmptyDataSet(10,10)
// gets an empty dataset with a specifed row count and column array
var dataset2 = databaseManager.createEmptyDataSet(10,new Array ('a','b','c','d'))
```
### createSelect(dataSource)

Create a QueryBuilder object for a datasource.

**Parameters**\
[String](JSLib/String.md) dataSource The data source to build a query for.

**Returns**\
[QBSelect](Database%20Manager/QBSelect.md) query builder

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
/** @type {QBSelect<db:/example_data/book_nodes>} */
var q = databaseManager.createSelect('db:/example_data/book_nodes');
q.result.addPk()
q.where.add(q.columns.label_text.not.isin(null))
datasources.db.example_data.book_nodes.getFoundSet().loadRecords(q)
```
### createSelect(dataSource, tableAlias)

Create a QueryBuilder object for a datasource with given table alias.
The alias can be used inside custom queries to bind to the outer table.

**Parameters**\
[String](JSLib/String.md) dataSource The data source to build a query for.\
[String](JSLib/String.md) tableAlias The alias for the main table.

**Returns**\
[QBSelect](Database%20Manager/QBSelect.md) query builder

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
/** @type {QBSelect<db:/example_data/book_nodes>} */
var q = databaseManager.createSelect('db:/example_data/book_nodes', 'b');
q.result.addPk()
q.where.add(q.columns.label_text.isin('select comment_text from book_text t where t.note_text = ? and t.node_id = b.node_id', ['test']))
datasources.db.example_data.book_nodes.getFoundSet().loadRecords(q)
```
### createTableFilterParam(query)

Create a table filter that can be applied to all the foundsets based on a table.
Multiple filters can be applied at the same time using databaseManager.setTableFilters().

Filters on tables touched in the query will not be applied to the query filter.
For example, when a table filter exists on the order_details table,
a query filter with a join from orders to order_details will be applied to queries on the orders table,
but the filter condition on the orders_details table will not be included.

**Parameters**\
[QBSelect](Database%20Manager/QBSelect.md) query condition to filter on.

**Returns**\
[JSTableFilter](Database%20Manager/JSTableFilter.md) table filter.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Best way to call this in a global solution startup method, but filters may be added/removed at any time.
// Note that multiple filters can be added to the same dataprovider, they will all be applied.

// filter on messages table where messagesid>10, the filter has a name so it can be removed using databaseManager.removeTableFilterParam()
var filter = databaseManager.createTableFilterParam('admin', 'messages', 'messagesid', '>', 10)

// a filter can be created based on a query
var query = datasources.db.admin.messages.createSelect()
query.where.add(query.columns.messagesid.gt(10))
var filter = databaseManager.createTableFilterParam(query)

// all tables that have the companyid column should be filtered
var filter = databaseManager.createTableFilterParam('crm', null, 'companyidid', '=', currentcompanyid)

// some filters with in-conditions
var filter = databaseManager.createTableFilterParam('crm', 'products', 'productcode', 'in', [120, 144, 200])
// use "sql:in" in stead of "in" to allow the value to be interpreted as a custom query
var filter = databaseManager.createTableFilterParam('crm', 'orders', 'countrycode', 'sql:in', 'select country code from countries where region = "Europe"')

// you can use modifiers in the operator as well, filter on companies where companyname is null or equals-ignore-case 'servoy'
var filter = databaseManager.createTableFilterParam('crm', 'companies', 'companyname', '#^||=', 'servoy')

// the value may be null, this will result in 'column is null' sql condition.
var filter = databaseManager.createTableFilterParam('crm', 'companies', 'verified', '=', null)

// if you want to add a filter for a column (created by you) in the i18n table
var filter = databaseManager.createTableFilterParam('database', 'your_i18n_table', 'message_variant', 'in', [1, 2])

// apply multiple filters at the same time, previous filters with the same name are removed:
var success = databaseManager.setTableFilters('myfilters', [filter1, filter2])
```
### createTableFilterParam(datasource, dataprovider, operator, value)

Create a table filter that can be applied to all the foundsets based on a table.
Multiple filters can be applied at the same time using databaseManager.setTableFilters().

Note: if null is provided as the tablename the filter will be applied on all tables with the dataprovider name.
A dataprovider can have multiple filters defined, they will all be applied.

**Parameters**\
[String](JSLib/String.md) datasource The datasource\
[String](JSLib/String.md) dataprovider A specified dataprovider column name.\
[String](JSLib/String.md) operator One of "=, <, >, >=, <=, !=, LIKE, or IN" optionally augmented with modifiers "#" (ignore case) or "^||" (or-is-null), prefix with "sql:" to allow the value to be interpreted as a custom query.\
[Object](JSLib/Object.md) value The specified filter value.

**Returns**\
[JSTableFilter](Database%20Manager/JSTableFilter.md) table filter.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Best way to call this in a global solution startup method, but filters may be added/removed at any time.
// Note that multiple filters can be added to the same dataprovider, they will all be applied.

// filter on messages table where messagesid>10, the filter has a name so it can be removed using databaseManager.removeTableFilterParam()
var filter = databaseManager.createTableFilterParam('admin', 'messages', 'messagesid', '>', 10)

// a filter can be created based on a query
var query = datasources.db.admin.messages.createSelect()
query.where.add(query.columns.messagesid.gt(10))
var filter = databaseManager.createTableFilterParam(query)

// all tables that have the companyid column should be filtered
var filter = databaseManager.createTableFilterParam('crm', null, 'companyidid', '=', currentcompanyid)

// some filters with in-conditions
var filter = databaseManager.createTableFilterParam('crm', 'products', 'productcode', 'in', [120, 144, 200])
// use "sql:in" in stead of "in" to allow the value to be interpreted as a custom query
var filter = databaseManager.createTableFilterParam('crm', 'orders', 'countrycode', 'sql:in', 'select country code from countries where region = "Europe"')

// you can use modifiers in the operator as well, filter on companies where companyname is null or equals-ignore-case 'servoy'
var filter = databaseManager.createTableFilterParam('crm', 'companies', 'companyname', '#^||=', 'servoy')

// the value may be null, this will result in 'column is null' sql condition.
var filter = databaseManager.createTableFilterParam('crm', 'companies', 'verified', '=', null)

// if you want to add a filter for a column (created by you) in the i18n table
var filter = databaseManager.createTableFilterParam('database', 'your_i18n_table', 'message_variant', 'in', [1, 2])

// apply multiple filters at the same time, previous filters with the same name are removed:
var success = databaseManager.setTableFilters('myfilters', [filter1, filter2])
```
### createTableFilterParam(serverName, tableName, dataprovider, operator, value)

Create a table filter that can be applied to all the foundsets based on a table.
Multiple filters can be applied at the same time using databaseManager.setTableFilters().

Note: if null is provided as the tablename the filter will be applied on all tables with the dataprovider name.
A dataprovider can have multiple filters defined, they will all be applied.

**Parameters**\
[String](JSLib/String.md) serverName The name of the database server connection for the specified table name.\
[String](JSLib/String.md) tableName The name of the specified table.\
[String](JSLib/String.md) dataprovider A specified dataprovider column name.\
[String](JSLib/String.md) operator One of "=, <, >, >=, <=, !=, LIKE, or IN" optionally augmented with modifiers "#" (ignore case) or "^||" (or-is-null), prefix with "sql:" to allow the value to be interpreted as a custom query.\
[Object](JSLib/Object.md) value The specified filter value.

**Returns**\
[JSTableFilter](Database%20Manager/JSTableFilter.md) table filter.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Best way to call this in a global solution startup method, but filters may be added/removed at any time.
// Note that multiple filters can be added to the same dataprovider, they will all be applied.

// filter on messages table where messagesid>10, the filter has a name so it can be removed using databaseManager.removeTableFilterParam()
var filter = databaseManager.createTableFilterParam('admin', 'messages', 'messagesid', '>', 10)

// a filter can be created based on a query
var query = datasources.db.admin.messages.createSelect()
query.where.add(query.columns.messagesid.gt(10))
var filter = databaseManager.createTableFilterParam(query)

// all tables that have the companyid column should be filtered
var filter = databaseManager.createTableFilterParam('crm', null, 'companyidid', '=', currentcompanyid)

// some filters with in-conditions
var filter = databaseManager.createTableFilterParam('crm', 'products', 'productcode', 'in', [120, 144, 200])
// use "sql:in" in stead of "in" to allow the value to be interpreted as a custom query
var filter = databaseManager.createTableFilterParam('crm', 'orders', 'countrycode', 'sql:in', 'select country code from countries where region = "Europe"')

// you can use modifiers in the operator as well, filter on companies where companyname is null or equals-ignore-case 'servoy'
var filter = databaseManager.createTableFilterParam('crm', 'companies', 'companyname', '#^||=', 'servoy')

// the value may be null, this will result in 'column is null' sql condition.
var filter = databaseManager.createTableFilterParam('crm', 'companies', 'verified', '=', null)

// if you want to add a filter for a column (created by you) in the i18n table
var filter = databaseManager.createTableFilterParam('database', 'your_i18n_table', 'message_variant', 'in', [1, 2])

// apply multiple filters at the same time, previous filters with the same name are removed:
var success = databaseManager.setTableFilters('myfilters', [filter1, filter2])
```
### dataSourceExists(dataSource)

Check wether a data source exists. This function can be used for any type of data source (db-based, in-memory).

**Parameters**\
[String](JSLib/String.md) dataSource the datasource string to check.

**Returns**\
[Boolean](JSLib/Boolean.md) boolean exists

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (!databaseManager.dataSourceExists(dataSource))
{
   // does not exist
}
```
### flushCalculations(datasource, onlyUnstored)

This method differences for recalculate() that it only works on a datasource rows/records that are loaded in memory.
It will not cause extra rows of that datasource to be loaded in memory (except if a calc itself would do that)

if onlyUnstored is true, then only unstored calculations will be flushed. (so also not causing any saves to the database)

**Parameters**\
[String](JSLib/String.md) datasource The datasource to flush all calculations of\
[Boolean](JSLib/Boolean.md) onlyUnstored to only go over the unstore cals of this datasource

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// flushed all unstored caclulations of the foundsets datasource.
databaseManager.flushCalculations(datasource, true);
```
### flushCalculations(datasource, onlyUnstored, calcnames)

This method differences for recalculate() that it only works on a datasource rows/records that are loaded in memory.
It will not cause extra rows of that datasource to be loaded in memory (except if a calc itself would do that)

if onlyUnstored is true, then only unstored calculations will be flushed. (so also not causing any saves to the database)

**Parameters**\
[String](JSLib/String.md) datasource The datasource to flush all calculations of\
[Boolean](JSLib/Boolean.md) onlyUnstored to only go over the unstore cals of this datasource\
[Array](JSLib/Array.md) calcnames A string array of calculation names that need to be flushed, if null then all unstored (or all depending on the boolean)

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// flushed all unstored caclulations of the foundsets datasource.
databaseManager.flushCalculations(datasource, true);
```
### getAutoSave()

Returns true or false if autosave is enabled or disabled.


**Returns**\
[Boolean](JSLib/Boolean.md) true if autosave if enabled.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//Set autosave, if false then no saves will happen by the ui (not including deletes!). Until you call saveData or setAutoSave(true)
//Rollbacks in mem the records that were edited and not yet saved. Best used in combination with autosave false.
databaseManager.setAutoSave(false)
//Now let users input data

//On save or cancel, when data has been entered:
if (cancel) databaseManager.rollbackEditedRecords()
databaseManager.setAutoSave(true)
```
### getDataModelClonesFrom(serverName)

Retrieves a list with names of all database servers that have property DataModelCloneFrom equal to the server name parameter.

**Parameters**\
[String](JSLib/String.md) serverName  ;

**Returns**\
[Array](JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var serverNames = databaseManager.getDataModelClonesFrom('myServerName');
```
### getDataSetByQuery(query, useTableFilters, max_returned_rows)

Performs a sql query with a query builder object.
Will throw an exception if anything did go wrong when executing the query.

**Parameters**\
[QBSelect](Database%20Manager/QBSelect.md) query QBSelect query.\
[Boolean](JSLib/Boolean.md) useTableFilters use table filters (default true).\
[Number](JSLib/Number.md) max_returned_rows The maximum number of rows returned by the query.

**Returns**\
[JSDataSet](Database%20Manager/JSDataSet.md) The JSDataSet containing the results of the query.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// use the query from a foundset and add a condition
/** @type {QBSelect<db:/example_data/orders>} */
var q = foundset.getQuery()
q.where.add(q.joins.orders_to_order_details.columns.discount.eq(2))
var maxReturnedRows = 10;//useful to limit number of rows
var ds = databaseManager.getDataSetByQuery(q, true, maxReturnedRows);

// query: select PK from example.book_nodes where parent = 111 and(note_date is null or note_date > now)
var query = datasources.db.example_data.book_nodes.createSelect().result.addPk().root
query.where.add(query.columns.parent_id.eq(111))
	.add(query.or
	.add(query.columns.note_date.isNull)
	.add(query.columns.note_date.gt(new Date())))
databaseManager.getDataSetByQuery(q, true, max_returned_rows)
```
### getDataSetByQuery(query, max_returned_rows)

Performs a sql query with a query builder object.
Will throw an exception if anything did go wrong when executing the query.

Using this variation of getDataSetByQuery any Tablefilter on the involved tables will be taken into account.

**Parameters**\
[QBSelect](Database%20Manager/QBSelect.md) query QBSelect query.\
[Number](JSLib/Number.md) max_returned_rows The maximum number of rows returned by the query.

**Returns**\
[JSDataSet](Database%20Manager/JSDataSet.md) The JSDataSet containing the results of the query.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// use the query froma foundset and add a condition
/** @type {QBSelect<db:/example_data/orders>} */
var q = foundset.getQuery()
q.where.add(q.joins.orders_to_order_details.columns.discount.eq(2))
var maxReturnedRows = 10;//useful to limit number of rows
var ds = databaseManager.getDataSetByQuery(q, maxReturnedRows);

// query: select PK from example.book_nodes where parent = 111 and(note_date is null or note_date > now)
var query = datasources.db.example_data.book_nodes.createSelect().result.addPk().root
query.where.add(query.columns.parent_id.eq(111))
	.add(query.or
	.add(query.columns.note_date.isNull)
	.add(query.columns.note_date.gt(new Date())))
databaseManager.getDataSetByQuery(q, max_returned_rows)
```
### getDataSetByQuery(server_name, sql_query, arguments, max_returned_rows)

Performs a sql query on the specified server, returns the result in a dataset.
Will throw an exception if query is not a select statement or anything did go wrong when executing the query.

Using this variation of getDataSetByQuery any Tablefilter on the involved tables will be disregarded.

**Parameters**\
[String](JSLib/String.md) server_name The name of the server where the query should be executed.\
[String](JSLib/String.md) sql_query The custom sql, must start with 'select', 'call', 'with' or 'declare'.\
[Array](JSLib/Array.md) arguments Specified arguments or null if there are no arguments.\
[Number](JSLib/Number.md) max_returned_rows The maximum number of rows returned by the query.

**Returns**\
[JSDataSet](Database%20Manager/JSDataSet.md) The JSDataSet containing the results of the query.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//finds duplicate records in a specified foundset
var vQuery =" SELECT companiesid from companies where company_name IN (SELECT company_name from companies group bycompany_name having count(company_name)>1 )";
var vDataset = databaseManager.getDataSetByQuery(databaseManager.getDataSourceServerName(controller.getDataSource()), vQuery, null, 1000);
controller.loadRecords(vDataset);

var maxReturnedRows = 10;//useful to limit number of rows
var query = 'select c1,c2,c3 from test_table where start_date = ?';//do not use '.' or special chars in names or aliases if you want to access data by name
var args = new Array();
args[0] = order_date //or  new Date()
var dataset = databaseManager.getDataSetByQuery(databaseManager.getDataSourceServerName(controller.getDataSource()), query, args, maxReturnedRows);

// place in label:
// elements.myLabel.text = '<html>'+dataset.getAsHTML()+'</html>';

//example to calc a strange total
global_total = 0;
for( var i = 1 ; i <= dataset.getMaxRowIndex() ; i++ )
{
	dataset.rowIndex = i;
	global_total = global_total + dataset.c1 + dataset.getValue(i,3);
}
//example to assign to dataprovider
//employee_salary = dataset.getValue(row,column)
```
### getDataSource(serverName, tableName)

Returns the datasource corresponding to the given server/table.

**Parameters**\
[String](JSLib/String.md) serverName The name of the table's server.\
[String](JSLib/String.md) tableName The table's name.

**Returns**\
[String](JSLib/String.md) The datasource of the given table/server.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var datasource = databaseManager.getDataSource('example_data', 'categories');
```
### getDataSourceServerName(dataSource)

Returns the server name from the datasource, or null if not a database datasource.

**Parameters**\
[String](JSLib/String.md) dataSource The datasource string to get the server name from.

**Returns**\
[String](JSLib/String.md) The servername of the datasource.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var servername = databaseManager.getDataSourceServerName(datasource);
```
### getDataSourceTableName(dataSource)

Returns the table name from the datasource, or null if not a database datasource.

**Parameters**\
[String](JSLib/String.md) dataSource The datasource string to get the tablename from.

**Returns**\
[String](JSLib/String.md) The tablename of the datasource.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var tablename = databaseManager.getDataSourceTableName(datasource);
```
### getDatabaseProductName(serverName)

Returns the database product name as supplied by the driver for a server.

NOTE: For more detail on named server connections, see the chapter on Database Connections, beginning with the Introduction to database connections in the Servoy Developer User's Guide.

**Parameters**\
[String](JSLib/String.md) serverName The specified name of the database server connection.

**Returns**\
[String](JSLib/String.md) A database product name.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var databaseProductName = databaseManager.getDatabaseProductName(servername)
```
### getEditedRecords()

Returns an array of edited records with outstanding (unsaved) data.

This is different form JSRecord.isEditing() because this call actually checks if there are changes between the current
record data and the stored data in the database. If there are no changes then the record is removed from the edited records
list (so after this call JSRecord.isEditing() can return false when it returned true just before this call)

NOTE: To return a dataset of outstanding (unsaved) edited data for each record, see JSRecord.getChangedData();
NOTE2: The fields focus may be lost in user interface in order to determine the edits.


**Returns**\
[Array](JSLib/Array.md) Array of outstanding/unsaved JSRecords.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//This method can be used to loop through all outstanding changes,
//the application.output line contains all the changed data, their tablename and primary key
var editr = databaseManager.getEditedRecords()
for (x=0;x<editr.length;x++)
{
	var ds = editr[x].getChangedData();
	var jstable = databaseManager.getTable(editr[x]);
	var tableSQLName = jstable.getSQLName();
	var pkrec = jstable.getRowIdentifierColumnNames().join(',');
	var pkvals = new Array();
	for (var j = 0; j < jstable.getRowIdentifierColumnNames().length; j++)
	{
		pkvals[j] = editr[x][jstable.getRowIdentifierColumnNames()[j]];
	}
	application.output('Table: '+tableSQLName +', PKs: '+ pkvals.join(',') +' ('+pkrec +')');
	// Get a dataset with outstanding changes on a record
	for( var i = 1 ; i <= ds.getMaxRowIndex() ; i++ )
	{
		application.output('Column: '+ ds.getValue(i,1) +', oldValue: '+ ds.getValue(i,2) +', newValue: '+ ds.getValue(i,3));
	}
}
//in most cases you will want to set autoSave back on now
databaseManager.setAutoSave(true);
```
### getEditedRecords(foundset)

Returns an array of edited records with outstanding (unsaved) data.

NOTE: To return a dataset of outstanding (unsaved) edited data for each record, see JSRecord.getChangedData();
NOTE2: The fields focus may be lost in user interface in order to determine the edits.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset return edited records in the foundset only.

**Returns**\
[Array](JSLib/Array.md) Array of outstanding/unsaved JSRecords.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//This method can be used to loop through all outstanding changes in a foundset,
//the application.output line contains all the changed data, their tablename and primary key
var editr = databaseManager.getEditedRecords(foundset)
for (x=0;x<editr.length;x++)
{
	var ds = editr[x].getChangedData();
	var jstable = databaseManager.getTable(editr[x]);
	var tableSQLName = jstable.getSQLName();
	var pkrec = jstable.getRowIdentifierColumnNames().join(',');
	var pkvals = new Array();
	for (var j = 0; j < jstable.getRowIdentifierColumnNames().length; j++)
	{
		pkvals[j] = editr[x][jstable.getRowIdentifierColumnNames()[j]];
	}
	application.output('Table: '+tableSQLName +', PKs: '+ pkvals.join(',') +' ('+pkrec +')');
	// Get a dataset with outstanding changes on a record
	for( var i = 1 ; i <= ds.getMaxRowIndex() ; i++ )
	{
		application.output('Column: '+ ds.getValue(i,1) +', oldValue: '+ ds.getValue(i,2) +', newValue: '+ ds.getValue(i,3));
	}
}
databaseManager.saveData(foundset);//save all records from foundset
```
### getEditedRecords(datasource)

Returns an array of edited records with outstanding (unsaved) data.

**Parameters**\
[String](JSLib/String.md) datasource the datasource for which to get the edited records

**Returns**\
[Array](JSLib/Array.md) Array of outstanding/unsaved JSRecords

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// This method can be used to loop through all outstanding changes for a specific datasource.
// The application.output line contains all the changed data, their tablename and primary key
var edits = databaseManager.getEditedRecords(datasources.db.mydb.mytable.getDataSource())

var jsTable = databaseManager.getTable('mydb', 'mytable');
var tableSQLName = jstable.getSQLName();
var pkColumnNames = jstable.getRowIdentifierColumnNames().join(',');
var pkValues [];

var x;
var ds;
var i;

for (x = 0; x < edits.length; x++) {
	ds = edits[x].getChangedData();
	pkValues.length = 0;

	for (i = 0; i < jsTable.getRowIdentifierColumnNames().length; i++) {
		pkValues[i] = edits[x][jsTable.getRowIdentifierColumnNames()[i]];
	}

	application.output('Table: ' + tableSQLName + ', PKs: ' + pkValues.join(',') + ' (' + pkColumnNames + ')');

	// Output the outstanding changes on each record
	for (i = 1; i <= ds.getMaxRowIndex(); i++) {
		application.output('Column: ' + ds.getValue(i, 1) + ', oldValue: ' + ds.getValue(i, 2) + ', newValue: ' + ds.getValue(i, 3));
	}
}
databaseManager.saveData(edits); //save all edited records in the datasource
```
### getEditedRecords(datasource, filter)

Returns an array of edited records with outstanding (unsaved) data for a datasource with a filter.

**Parameters**\
[String](JSLib/String.md) datasource the datasource for which to get the edited records\
[Object](JSLib/Object.md) filter criteria against which the edited record must match to be included

**Returns**\
[Array](JSLib/Array.md) Array of outstanding/unsaved JSRecords

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// This method can be used to loop through all outstanding changes for a specific datasource.
// The application.output line contains all the changed data, their tablename and primary key.
// Filter on records that match certain criteria.
// The criteria can be specified in a javascript object, for example get edited records for country NL or DE and currency EUR.
var edits = databaseManager.getEditedRecords(datasources.db.mydb.mytable.getDataSource(), {currency: 'EUR', country: ['NL', 'DE']})

var jsTable = databaseManager.getTable('mydb', 'mytable');
var tableSQLName = jstable.getSQLName();
var pkColumnNames = jstable.getRowIdentifierColumnNames().join(',');
var pkValues [];

var x;
var ds;
var i;

for (x = 0; x < edits.length; x++) {
	ds = edits[x].getChangedData();
	pkValues.length = 0;

	for (i = 0; i < jsTable.getRowIdentifierColumnNames().length; i++) {
		pkValues[i] = edits[x][jsTable.getRowIdentifierColumnNames()[i]];
	}

	application.output('Table: ' + tableSQLName + ', PKs: ' + pkValues.join(',') + ' (' + pkColumnNames + ')');

	// Output the outstanding changes on each record
	for (i = 1; i <= ds.getMaxRowIndex(); i++) {
		application.output('Column: ' + ds.getValue(i, 1) + ', oldValue: ' + ds.getValue(i, 2) + ', newValue: ' + ds.getValue(i, 3));
	}
}
databaseManager.saveData(edits); //save all edited records in the datasource
```
### getFailedRecords()

Returns an array of records that fail after a save.


**Returns**\
[Array](JSLib/Array.md) Array of failed JSRecords

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var array = databaseManager.getFailedRecords()
for( var i = 0 ; i < array.length ; i++ )
{
	var record = array[i];
	application.output(record.exception);
	if (record.exception.getErrorCode() === ServoyException.RECORD_VALIDATION_FAILED)
	{
		// exception thrown in pre-insert/update/delete event method
		var thrown = record.exception.getValue()
		application.output("Record validation failed: "+thrown)
	}
	else if (record.exception.getErrorCode() !== ServoyException.MUST_ROLLBACK)
	{
		// some other exception (ServoyException.MUST_ROLLBACK are records that were not saved because of previous errors in the transaction)
	}
	// find out the table of the record (similar to getEditedRecords)
	var jstable = databaseManager.getTable(record);
	var tableSQLName = jstable.getSQLName();
	application.output('Table:'+tableSQLName+' in server:'+jstable.getServerName()+' failed to save.')
}
```
### getFailedRecords(foundset)

Returns an array of records that fail after a save.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset return failed records in the foundset only.

**Returns**\
[Array](JSLib/Array.md) Array of failed JSRecords

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var array = databaseManager.getFailedRecords(foundset)
for( var i = 0 ; i < array.length ; i++ )
{
	var record = array[i];
	application.output(record.exception);
	if (record.exception.getErrorCode() == ServoyException.RECORD_VALIDATION_FAILED)
	{
		// exception thrown in pre-insert/update/delete event method
		var thrown = record.exception.getValue()
		application.output("Record validation failed: "+thrown)
	}
	// find out the table of the record (similar to getEditedRecords)
	var jstable = databaseManager.getTable(record);
	var tableSQLName = jstable.getSQLName();
	application.output('Table:'+tableSQLName+' in server:'+jstable.getServerName()+' failed to save.')
}
```
### getFoundSet(query)

Returns a foundset object for a specified pk query.

**Parameters**\
[QBSelect](Database%20Manager/QBSelect.md) query The query to get the JSFoundset for.

**Returns**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) A new JSFoundset for that query.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// type the foundset returned from the call with JSDoc, fill in the right server/tablename
/** @type {JSFoundset<db:/servername/tablename>} */
var fs = databaseManager.getFoundSet(controller.getDataSource())
// same as datasources.db.example_data.orders.getFoundSet() or datasources.mem['myds'].getFoundSet()
var ridx = fs.newRecord()
var record = fs.getRecord(ridx)
record.emp_name = 'John'
databaseManager.saveData()
```
### getFoundSet(dataSource)

Returns a foundset object for a specified datasource or server and tablename.
Alternative method: datasources.db.server_name.table_name.getFoundSet() or datasources.mem['ds'].getFoundSet()

**Parameters**\
[String](JSLib/String.md) dataSource The datasource to get a JSFoundset for.

**Returns**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) A new JSFoundset for that datasource.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
// type the foundset returned from the call with JSDoc, fill in the right server/tablename
/** @type {JSFoundset<db:/servername/tablename>} */
var fs = databaseManager.getFoundSet(controller.getDataSource())
// same as datasources.db.example_data.orders.getFoundSet() or datasources.mem['myds'].getFoundSet()
var ridx = fs.newRecord()
var record = fs.getRecord(ridx)
record.emp_name = 'John'
databaseManager.saveData()
```
### getFoundSet(serverName, tableName)

Returns a foundset object for a specified datasource or server and tablename.

**Parameters**\
[String](JSLib/String.md) serverName The servername to get a JSFoundset for.\
[String](JSLib/String.md) tableName The tablename for that server

**Returns**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) A new JSFoundset for that datasource.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// type the foundset returned from the call with JSDoc, fill in the right server/tablename
/** @type {JSFoundset<db:/servername/tablename>} */
var fs = databaseManager.getFoundSet(controller.getDataSource())
// same as datasources.db.example_data.orders.getFoundSet() or datasources.mem['myds'].getFoundSet()
var ridx = fs.newRecord()
var record = fs.getRecord(ridx)
record.emp_name = 'John'
databaseManager.saveData()
```
### getFoundSetCount(foundset)

Returns the total number of records in a foundset.

NOTE: This can be an expensive operation (time-wise) if your resultset is large.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset The JSFoundset to get the count for.

**Returns**\
[Number](JSLib/Number.md) the foundset count

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//return the total number of records in a foundset.
databaseManager.getFoundSetCount(foundset);
```
### getFoundSetUpdater(foundset)

Returns a JSFoundsetUpdater object that can be used to update all or a specific number of rows in the specified foundset.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset The foundset to update.

**Returns**\
[JSFoundSetUpdater](Database%20Manager/JSFoundSetUpdater.md) The JSFoundsetUpdater for the specified JSFoundset.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//1) update entire foundset
var fsUpdater = databaseManager.getFoundSetUpdater(foundset)
fsUpdater.setColumn('customer_type',1)
fsUpdater.setColumn('my_flag',0)
fsUpdater.performUpdate()

//2) update part of foundset, for example the first 4 row (starts with selected row)
var fsUpdater = databaseManager.getFoundSetUpdater(foundset)
fsUpdater.setColumn('customer_type',new Array(1,2,3,4))
fsUpdater.setColumn('my_flag',new Array(1,0,1,0))
fsUpdater.performUpdate()

//3) safely loop through foundset (starts with selected row)
controller.setSelectedIndex(1)
var count = 0
var fsUpdater = databaseManager.getFoundSetUpdater(foundset)
while(fsUpdater.next())
{
	fsUpdater.setColumn('my_flag',count++)
}
```
### getNamedFoundSet(name)

An existing foundset under that name will be returned, or created if there is a definition (there is a form with a named foundset property with that name).
Alternative method: datasources.db.server_name.table_name.getFoundSet(name)

**Parameters**\
[String](JSLib/String.md) name The named foundset name

**Returns**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) An existing named(separate) foundset.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// type the foundset returned from the call with JSDoc, fill in the right server/tablename
/** @type {JSFoundset<db:/servername/tablename>} */
var fs = databaseManager.getNamedFoundSet('myname')
// same as datasources.db.example_data.orders.getFoundSet('myname')
var ridx = fs.newRecord()
var record = fs.getRecord(ridx)
record.emp_name = 'John'
databaseManager.saveData()
```
### getNextSequence(dataSource, columnName)

Gets the next sequence for a column which has a sequence defined in its column dataprovider properties.

NOTE: For more infomation on configuring the sequence for a column, see the section Auto enter options for a column from the Dataproviders chapter in the Servoy Developer User's Guide.

**Parameters**\
[String](JSLib/String.md) dataSource The datasource that points to the table which has the column with the sequence,
								or the name of the server where the table can be found. If the name of the server
								is specified, then a second optional parameter specifying the name of the table
								must be used. If the datasource is specified, then the name of the table is not needed
								as the second argument.\
[String](JSLib/String.md) columnName The name of the column that has a sequence defined in its properties.

**Returns**\
[Object](JSLib/Object.md) The next sequence for the column, null if there was no sequence for that column
        or if there is no column with the given name.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var seqDataSource = forms.seq_table.controller.getDataSource();
var nextValue = databaseManager.getNextSequence(seqDataSource, 'seq_table_value');
application.output(nextValue);

nextValue = databaseManager.getNextSequence(databaseManager.getDataSourceServerName(seqDataSource), databaseManager.getDataSourceTableName(seqDataSource), 'seq_table_value')
application.output(nextValue);
```
### getSQL(foundsetOrQBSelect)

Returns the internal SQL which defines the specified (related)foundset.
Table filters are on by default.
Make sure to set the applicable filters when the sql is used in a loadRecords() call.

**Parameters**\
[Object](JSLib/Object.md) foundsetOrQBSelect The JSFoundset or QBSelect to get the sql for.

**Returns**\
[String](JSLib/String.md) String representing the sql of the JSFoundset.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var sql = databaseManager.getSQL(foundset)
```
### getSQL(foundsetOrQBSelect, includeFilters)

Returns the internal SQL which defines the specified (related)foundset.
Optionally, the foundset and table filter params can be excluded in the sql (includeFilters=false).
Make sure to set the applicable filters when the sql is used in a loadRecords() call.
When the founset is in find mode, the find conditions are included in the resulting query.

**Parameters**\
[Object](JSLib/Object.md) foundsetOrQBSelect The JSFoundset or QBSelect to get the sql for.\
[Boolean](JSLib/Boolean.md) includeFilters include the foundset and table filters.

**Returns**\
[String](JSLib/String.md) String representing the sql of the JSFoundset.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var sql = databaseManager.getSQL(foundset)
```
### getSQLParameters(foundsetOrQBSelect)

Returns the internal SQL parameters, as an array, that are used to define the specified (related)foundset.
Parameters for the filters are included.

**Parameters**\
[Object](JSLib/Object.md) foundsetOrQBSelect The JSFoundset or QBSelect to get the sql parameters for.

**Returns**\
[Array](JSLib/Array.md) An Array with the sql parameter values.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var sqlParameterArray = databaseManager.getSQLParameters(foundset,false)
```
### getSQLParameters(foundsetOrQBSelect, includeFilters)

Returns the internal SQL parameters, as an array, that are used to define the specified (related)foundset.
When the founset is in find mode, the arguments for the find conditions are included in the result.

**Parameters**\
[Object](JSLib/Object.md) foundsetOrQBSelect The JSFoundset or QBSelect to get the sql parameters for.\
[Boolean](JSLib/Boolean.md) includeFilters include the parameters for the filters.

**Returns**\
[Array](JSLib/Array.md) An Array with the sql parameter values.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var sqlParameterArray = databaseManager.getSQLParameters(foundset,false)
```
### getServerNames()

Returns an array with all the server names used in the solution.

NOTE: For more detail on named server connections, see the chapter on Database Connections, beginning with the Introduction to database connections in the Servoy Developer User's Guide.


**Returns**\
[Array](JSLib/Array.md) An Array of servernames.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var array = databaseManager.getServerNames()
```
### getTable(foundset)

Returns the JSTable object from which more info can be obtained (like columns).
The parameter can be a JSFoundset,JSRecord,datasource string or server/tablename combination.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset The foundset where the JSTable can be get from.

**Returns**\
[JSTable](Database%20Manager/JSTable.md) the JSTable get from the input.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var jstable = databaseManager.getTable(controller.getDataSource());
//var jstable = databaseManager.getTable(foundset);
//var jstable = databaseManager.getTable(record);
//var jstable = databaseManager.getTable(datasource);
var tableSQLName = jstable.getSQLName();
var columnNamesArray = jstable.getColumnNames();
var firstColumnName = columnNamesArray[0];
var jscolumn = jstable.getColumn(firstColumnName);
var columnLength = jscolumn.getLength();
var columnType = jscolumn.getTypeAsString();
var columnSQLName = jscolumn.getSQLName();
var isPrimaryKey = jscolumn.isRowIdentifier();
```
### getTable(record)

Returns the JSTable object from which more info can be obtained (like columns).
The parameter can be a JSFoundset,JSRecord,datasource string or server/tablename combination.

**Parameters**\
[JSRecord](Database%20Manager/JSRecord.md) record The record where the table can be get from.

**Returns**\
[JSTable](Database%20Manager/JSTable.md) the JSTable get from the input.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var jstable = databaseManager.getTable(controller.getDataSource());
//var jstable = databaseManager.getTable(foundset);
//var jstable = databaseManager.getTable(record);
//var jstable = databaseManager.getTable(datasource);
var tableSQLName = jstable.getSQLName();
var columnNamesArray = jstable.getColumnNames();
var firstColumnName = columnNamesArray[0];
var jscolumn = jstable.getColumn(firstColumnName);
var columnLength = jscolumn.getLength();
var columnType = jscolumn.getTypeAsString();
var columnSQLName = jscolumn.getSQLName();
var isPrimaryKey = jscolumn.isRowIdentifier();
```
### getTable(dataSource)

Returns the JSTable object from which more info can be obtained (like columns).
The parameter can be a JSFoundset,JSRecord,datasource string or server/tablename combination.

**Parameters**\
[String](JSLib/String.md) dataSource The datasource where the table can be get from.

**Returns**\
[JSTable](Database%20Manager/JSTable.md) the JSTable get from the input.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var jstable = databaseManager.getTable(controller.getDataSource());
//var jstable = databaseManager.getTable(foundset);
//var jstable = databaseManager.getTable(record);
//var jstable = databaseManager.getTable(datasource);
var tableSQLName = jstable.getSQLName();
var columnNamesArray = jstable.getColumnNames();
var firstColumnName = columnNamesArray[0];
var jscolumn = jstable.getColumn(firstColumnName);
var columnLength = jscolumn.getLength();
var columnType = jscolumn.getTypeAsString();
var columnSQLName = jscolumn.getSQLName();
var isPrimaryKey = jscolumn.isRowIdentifier();
```
### getTable(serverName, tableName)

Returns the JSTable object from which more info can be obtained (like columns).
The parameter can be a JSFoundset,JSRecord,datasource string or server/tablename combination.

**Parameters**\
[String](JSLib/String.md) serverName Server name.\
[String](JSLib/String.md) tableName Table name.

**Returns**\
[JSTable](Database%20Manager/JSTable.md) the JSTable get from the input.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var jstable = databaseManager.getTable(controller.getDataSource());
//var jstable = databaseManager.getTable(foundset);
//var jstable = databaseManager.getTable(record);
//var jstable = databaseManager.getTable(datasource);
var tableSQLName = jstable.getSQLName();
var columnNamesArray = jstable.getColumnNames();
var firstColumnName = columnNamesArray[0];
var jscolumn = jstable.getColumn(firstColumnName);
var columnLength = jscolumn.getLength();
var columnType = jscolumn.getTypeAsString();
var columnSQLName = jscolumn.getSQLName();
var isPrimaryKey = jscolumn.isRowIdentifier();
```
### getTableCount(dataSource)

Returns the total number of records(rows) in a table.

NOTE: This can be an expensive operation (time-wise) if your resultset is large

**Parameters**\
[Object](JSLib/Object.md) dataSource Data where a server table can be get from. Can be a foundset, a datasource name or a JSTable.

**Returns**\
[Number](JSLib/Number.md) the total table count.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//return the total number of rows in a table.
var count = databaseManager.getTableCount(foundset);
```
### getTableFilterParams(serverName)

Returns a two dimensional array object containing the table filter information currently applied to the servers tables.
For column-based table filters, a row of 5 fields per filter are returned.
The "columns" of a row from this array are: tablename, dataprovider, operator, value, filtername

For query-based filters, a row of 2 fields per filter are returned.
The "columns" of a row from this array are: query, filtername

**Parameters**\
[String](JSLib/String.md) serverName The name of the database server connection.

**Returns**\
[Array](JSLib/Array.md) Two dimensional array.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var params = databaseManager.getTableFilterParams(databaseManager.getDataSourceServerName(controller.getDataSource()))
for (var i = 0; params != null && i < params.length; i++)
{
 if (params[i].length() == 5) {
		application.output('Table filter on table ' + params[i][0] + ': '+ params[i][1] + ' '+params[i][2] + ' '+params[i][3] + (params[i][4] == null ? ' [no name]' : ' ['+params[i][4]+']'))
	}
 if (params[i].length() == 2) {
		application.output('Table filter with query ' + params[i][0]+ ': ' + (params[i][1] == null ? ' [no name]' : ' ['+params[i][1]+']'))
	}
}
```
### getTableFilterParams(serverName, filterName)

Returns a two dimensional array object containing the table filter information currently applied to the servers tables.
For column-based table filters, a row of 5 fields per filter are returned.
The "columns" of a row from this array are: tablename, dataprovider, operator, value, filtername

For query-based filters, a row of 2 fields per filter are returned.
The "columns" of a row from this array are: query, filtername

**Parameters**\
[String](JSLib/String.md) serverName The name of the database server connection.\
[String](JSLib/String.md) filterName The filter name for which to get the array.

**Returns**\
[Array](JSLib/Array.md) Two dimensional array.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var params = databaseManager.getTableFilterParams(databaseManager.getDataSourceServerName(controller.getDataSource()))
for (var i = 0; params != null && i < params.length; i++)
{
 if (params[i].length() == 5) {
		application.output('Table filter on table ' + params[i][0] + ': '+ params[i][1] + ' '+params[i][2] + ' '+params[i][3] + (params[i][4] == null ? ' [no name]' : ' ['+params[i][4]+']'))
	}
 if (params[i].length() == 2) {
		application.output('Table filter with query ' + params[i][0]+ ': ' + (params[i][1] == null ? ' [no name]' : ' ['+params[i][1]+']'))
	}
}
```
### getTableNames(serverName)

Returns an array of all table names for a specified server.

**Parameters**\
[String](JSLib/String.md) serverName The server name to get the table names from.

**Returns**\
[Array](JSLib/Array.md) An Array with the tables names of that server.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//return all the table names as array
var tableNamesArray = databaseManager.getTableNames('user_data');
var firstTableName = tableNamesArray[0];
```
### getViewFoundSet(name)

Returns a ViewFoundSet that was created by getViewFoundSet(name,query,register) with the registerd boolean "true".
So it is registered and remembered by the system to use in Forms.
You can't get ViewFounSet back that are not registered to the system, those are not remembered.

**Parameters**\
[String](JSLib/String.md) name The name to lookup a ViewFoundSet for

**Returns**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) A new ViewFoundSet for that query.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### getViewFoundSet(name, query)

Returns a foundset object for a specified query.
This just creates one without keeping any reference to it, you have to use the getViewFoundSet(name,query,true) for registering it to the system.
ViewFoundSets are different then normal foundsets because they have a lot less methods, stuff like newRecord/deleteRecord don't work.

If you query the pk with the columns that you display for the main or join tables then those columns can be updated and through ViewFoundSet#save(ViewRecord) they can be saved.
If there are changes in ViewRecords of this ViewFoundSet then databroadcast configurations that need to load new data won't do the query right away (only after the save)
Also loading more (the next chunksize) will not be done. This is because the ViewRecord on an index can be completely changed. We can't track those.

Also databroadcast can be enabled by calling one of the ViewFoundSet#enableDatabroadcastFor(QBTableClause) to listen for that specific table (main or joins).
Flags can be used to control what exactly should be monitored, some don't cost a lot of overhead others have to do a full re-query to see the changes.

**Parameters**\
[String](JSLib/String.md) name The name given to this foundset (will create a datasource url like view:[name])\
[QBSelect](Database%20Manager/QBSelect.md) query The query to get the ViewFoundSet for.

**Returns**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) A new ViewFoundSet for that query.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// create a new view foundset and also directly register it to the system so they can be picked up by forms if a form has the view datasource.
/** @type {ViewFoundSet<view:myname>} */
var vfs = databaseManager.getViewFoundSet('myname', query, true)
```
### getViewFoundSet(name, query, register)

Returns a foundset object for a specified query. If the boolean register is true then the system will register it to the system so it can be used in Forms.
Also getViewFoundSet(name) will then return that instance.
ViewFoundSets are different then normal foundsets because they have a lot less methods, stuff like newRecord/deleteRecord don't work.

If you query the pk with the columns that you display for the main or join tables then those columns can be updated and through ViewFoundSet#save(ViewRecord) they can be saved.
If there are changes in ViewRecords of this ViewFoundSet then databroadcast configurations that need to load new data won't do the query right away (only after the save)
Also loading more (the next chunksize) will not be done. This is because the ViewRecord on an index can be completely changed. We can't track those.

Also databroadcast can be enabled by calling one of the ViewFoundSet#enableDatabroadcastFor(QBTableClause) to listen for that specific table (main or joins).
Flags can be used to control what exactly should be monitored, some don't cost a lot of overhead others have to do a full re-query to see the changes.

if the register boolean is true, then the given ViewFoundSet is registered to the system so it is picked up by forms that have this datasource (see viewFoundset.getDatasource() for the actual datasource string) assigned.
The form's foundset will then have a much more limited API, so a lot of things can't be done with it - e.g. newRecord() or deleteRecords().
Also records can be updated in memory, so they are not fully read-only, but the developer is responsible for saving these changes to a persisted store. See also viewFoundset.save(...).

If the solution doesn't need this ViewFoundSet anymore and you did use register is true, please use ViewFoundSet.dispose() to clear and remove it from the system, because otherwise this
register call will keep/hold this foundset in memory (for that datasource string to work) forever.

**Parameters**\
[String](JSLib/String.md) name The name given to this foundset (will create a datasource url like view:[name])\
[QBSelect](Database%20Manager/QBSelect.md) query The query to get the ViewFoundSet for.\
[Boolean](JSLib/Boolean.md) register Register the created ViewFoundSet to the system so it can be used by forms.

**Returns**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) A new JSFoundset for that query.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// create a new view foundset and also directly register it to the system so they can be picked up by forms if a form has the view datasource.
/** @type {ViewFoundSet<view:myname>} */
var vfs = databaseManager.getViewFoundSet('myname', query, true)
```
### getViewNames(serverName)

Returns an array of all view names for a specified server.

**Parameters**\
[String](JSLib/String.md) serverName The server name to get the view names from.

**Returns**\
[Array](JSLib/Array.md) An Array with the view names of that server.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//return all the view names as array
var viewNamesArray = databaseManager.getViewNames('user_data');
var firstViewName = viewNamesArray[0];
```
### hasLocks()

Returns true if the current client has any or the specified lock(s) acquired.


**Returns**\
[Boolean](JSLib/Boolean.md) true if the current client has locks or the lock.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var hasLocks = databaseManager.hasLocks('mylock')
```
### hasLocks(lockName)

Returns true if the current client has any or the specified lock(s) acquired.

**Parameters**\
[String](JSLib/String.md) lockName The lock name to check.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the current client has locks or the lock.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var hasLocks = databaseManager.hasLocks('mylock')
```
### hasNewRecords(foundset)

Returns true if the argument (foundSet / record) has at least one row that was not yet saved in the database.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset The JSFoundset to test.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the JSFoundset has new records or JSRecord is a new record.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var fs = databaseManager.getFoundSet(databaseManager.getDataSourceServerName(controller.getDataSource()),'employees');
databaseManager.startTransaction();
var ridx = fs.newRecord();
var record = fs.getRecord(ridx);
record.emp_name = 'John';
if (databaseManager.hasNewRecords(fs)) {
	application.output("new records");
} else {
	application.output("no new records");
}
databaseManager.saveData();
databaseManager.commitTransaction();
```
### hasNewRecords(foundset, index)

Returns true if the argument (foundSet / record) has at least one row that was not yet saved in the database.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset The JSFoundset to test.\
[Number](JSLib/Number.md) index The record index in the foundset to test (not specified means has the foundset any new records)

**Returns**\
[Boolean](JSLib/Boolean.md) true if the JSFoundset has new records or JSRecord is a new record.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var fs = databaseManager.getFoundSet(databaseManager.getDataSourceServerName(controller.getDataSource()),'employees');
databaseManager.startTransaction();
var ridx = fs.newRecord();
var record = fs.getRecord(ridx);
record.emp_name = 'John';
if (databaseManager.hasNewRecords(fs)) {
	application.output("new records");
} else {
	application.output("no new records");
}
databaseManager.saveData();
databaseManager.commitTransaction();
```
### hasRecordChanges(foundset)

Returns true if the specified foundset, on a specific index or in any of its records, or the specified record has changes or is new unsaved record.

NOTE: The fields focus may be lost in user interface in order to determine the edits.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset The JSFoundset to test if it has changes.

**Returns**\
[Boolean](JSLib/Boolean.md) true if there are changes in the JSFoundset or JSRecord.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (databaseManager.hasRecordChanges(foundset,2))
{
	//do save or something else
}
```
### hasRecordChanges(foundset, index)

Returns true if the specified foundset, on a specific index or in any of its records, or the specified record has changes or is new unsaved record.

NOTE: The fields focus may be lost in user interface in order to determine the edits.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset The JSFoundset to test if it has changes.\
[Number](JSLib/Number.md) index The record index in the foundset to test (not specified means has the foundset any changed records)

**Returns**\
[Boolean](JSLib/Boolean.md) true if there are changes in the JSFoundset or JSRecord.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
if (databaseManager.hasRecordChanges(foundset,2))
{
	//do save or something else
}
```
### hasRecords(foundset)

Returns true if the (related)foundset exists and has records.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset A JSFoundset to test.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the foundset/relation has records.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
if (%%elementName%%.hasRecords(orders_to_orderitems))
{
	//do work on relatedFoundSet
}
//if (%%elementName%%.hasRecords(foundset.getSelectedRecord(),'orders_to_orderitems.orderitems_to_products'))
//{
//	//do work on deeper relatedFoundSet
//}
```
### hasRecords(record, relationString)

Returns true if the (related)foundset exists and has records.

**Parameters**\
[JSRecord](Database%20Manager/JSRecord.md) record A JSRecord to test.\
[String](JSLib/String.md) relationString The relation name.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the foundset/relation has records.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
if (%%elementName%%.hasRecords(orders_to_orderitems))
{
	//do work on relatedFoundSet
}
//if (%%elementName%%.hasRecords(foundset.getSelectedRecord(),'orders_to_orderitems.orderitems_to_products'))
//{
//	//do work on deeper relatedFoundSet
//}
```
### hasTransaction()

Returns true if there is an transaction active for this client.


**Returns**\
[Boolean](JSLib/Boolean.md) true if the client has a transaction.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var hasTransaction = databaseManager.hasTransaction()
```
### mergeRecords(sourceRecord, combinedDestinationRecord)

Merge records from the same foundset, updates entire datamodel (via foreign type on columns) with destination
record pk, deletes source record. Do use a transaction!

This function is very handy in situations where duplicate data exists. It allows you to merge the two records
and move all related records in one go. Say the source_record is "Ikea" and the combined_destination_record is "IKEA", the
"Ikea" record is deleted and all records related to it (think of contacts and orders, for instance) will be related
to the "IKEA" record.

The function takes an optional array of column names. If provided, the data in the named columns will be copied
from source_record to combined_destination_record.

Note that it is essential for both records to originate from the same foundset, as shown in the sample code.

**Parameters**\
[JSRecord](Database%20Manager/JSRecord.md) sourceRecord The source JSRecord to copy from.\
[JSRecord](Database%20Manager/JSRecord.md) combinedDestinationRecord The target/destination JSRecord to copy into.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the records could me merged.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
databaseManager.mergeRecords(foundset.getRecord(1),foundset.getRecord(2));
```
### mergeRecords(sourceRecord, combinedDestinationRecord, columnNames)

Merge records from the same foundset, updates entire datamodel (via foreign type on columns) with destination
record pk, deletes source record. Do use a transaction!

This function is very handy in situations where duplicate data exists. It allows you to merge the two records
and move all related records in one go. Say the source_record is "Ikea" and the combined_destination_record is "IKEA", the
"Ikea" record is deleted and all records related to it (think of contacts and orders, for instance) will be related
to the "IKEA" record.

The function takes an optional array of column names. If provided, the data in the named columns will be copied
from source_record to combined_destination_record.

Note that it is essential for both records to originate from the same foundset, as shown in the sample code.

**Parameters**\
[JSRecord](Database%20Manager/JSRecord.md) sourceRecord The source JSRecord to copy from.\
[JSRecord](Database%20Manager/JSRecord.md) combinedDestinationRecord The target/destination JSRecord to copy into.\
[Array](JSLib/Array.md) columnNames The column names array that should be copied.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the records could me merged.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
databaseManager.mergeRecords(foundset.getRecord(1),foundset.getRecord(2));
```
### recalculate(foundsetOrRecord)

Can be used to recalculate a specified record or all rows in the specified foundset.
May be necessary when data is changed from outside of servoy, or when there is data changed inside servoy
but records with calculations depending on that data where not loaded so not updated and you need to update
the stored calculation values because you are depending on that with queries or aggregates.

**Parameters**\
[Object](JSLib/Object.md) foundsetOrRecord JSFoundset or JSRecord to recalculate.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// recalculate one record from a foundset.
databaseManager.recalculate(foundset.getRecord(1));
// recalculate all records from the foundset.
// please use with care, this can be expensive!
//databaseManager.recalculate(foundset);
```
### refreshRecordFromDatabase(foundset, index)

Flushes the client data cache and requeries the data for a record (based on the record index) in a foundset or all records in the foundset.
Used where a program external to Servoy has modified the database record.
Giving 0 as the index will just refresh he selected record.

If the index is -1 then this method will refresh all the records of the datasource of the foundset, it does this by flusing all the records and the row data of the full datasource
So everything is reloaded fully fresh when the foundsets will requery for there data.
WARNING: Don't hold any references to JSRecord objects from before this call with -1 index. Those records objects are all in an invalid state because of the underlying data flush.

**Parameters**\
[Object](JSLib/Object.md) foundset The JSFoundset to refresh\
[Number](JSLib/Number.md) index The index of the JSRecord that must be refreshed (or -1 for all).

**Returns**\
[Boolean](JSLib/Boolean.md) true if the refresh was done.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//refresh the second record from the foundset.
databaseManager.refreshRecordFromDatabase(foundset,2)
//flushes all records in the related foundset datasource (so the whole table, so -1 is an expensive operation)
databaseManager.refreshRecordFromDatabase(order_to_orderdetails,-1);
```
### releaseAllLocks()

Release all current locks the client has (optionally limited to named locks).
return true if the locks are released.


**Returns**\
[Boolean](JSLib/Boolean.md) true if all locks or the lock is released.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
databaseManager.releaseAllLocks('mylock')
```
### releaseAllLocks(lockName)

Release all current locks the client has (optionally limited to named locks).
return true if the locks are released.

**Parameters**\
[String](JSLib/String.md) lockName The lock name to release.

**Returns**\
[Boolean](JSLib/Boolean.md) true if all locks or the lock is released.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
databaseManager.releaseAllLocks('mylock')
```
### removeDataSource(uri)

Free resources allocated for a previously created data source.
NOTE: make sure this datasource is not using anymore in forms or components!
because the inmemory table and the foundset build on that table are all just removed.

Normally this will be automatically done if a client is removed/shutdown, but if constantly new stuff is created
or you don't need it anymore from what the client currently is using or seeing, then removing this will clean up memory.

**Parameters**\
[String](JSLib/String.md) uri  ;

**Returns**\
[Boolean](JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
databaseManager.removeDataSource(uri);
```
### removeTableFilterParam(serverName, filterName)

Removes a previously defined table filter.

**Parameters**\
[String](JSLib/String.md) serverName The name of the database server connection.\
[String](JSLib/String.md) filterName The name of the filter that should be removed.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the filter could be removed.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var success = databaseManager.removeTableFilterParam('admin', 'higNumberedMessagesRule')
```
### revertEditedRecords()

Reverts outstanding (not saved) in memory changes from edited records.
Can specify a record or foundset as parameter to rollback.
Best used in combination with the function databaseManager.setAutoSave()
This does not include deletes, they do not honor the autosafe false flag so they cant be rollbacked by this call.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//Set autosave, if false then no saves will happen by the ui (not including deletes!). Until you call saveData or setAutoSave(true)
//reverts in mem the records that were edited and not yet saved. Best used in combination with autosave false.
databaseManager.setAutoSave(false)
//Now let users input data

//On save or cancel, when data has been entered:
if (cancel) databaseManager.revertEditedRecords()
//databaseManager.revertEditedRecords(foundset); // rollback all records from foundset
//databaseManager.revertEditedRecords(foundset.getSelectedRecord()); // rollback only one record
databaseManager.setAutoSave(true)
```
### revertEditedRecords(foundset)

Reverts outstanding (not saved) in memory changes from edited records.
Can specify a record or foundset as parameter to rollback.
Best used in combination with the function databaseManager.setAutoSave()
This does not include deletes, they do not honor the autosafe false flag so they cant be rollbacked by this call.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset A JSFoundset to revert.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//Set autosave, if false then no saves will happen by the ui (not including deletes!). Until you call saveData or setAutoSave(true)
//reverts in mem the records that were edited and not yet saved. Best used in combination with autosave false.
databaseManager.setAutoSave(false)
//Now let users input data

//On save or cancel, when data has been entered:
if (cancel) databaseManager.revertEditedRecords()
//databaseManager.revertEditedRecords(foundset); // rollback all records from foundset
//databaseManager.revertEditedRecords(foundset.getSelectedRecord()); // rollback only one record
databaseManager.setAutoSave(true)
```
### rollbackTransaction()

Rollback a transaction started by databaseManager.startTransaction().
Note that when autosave is false, revertEditedRecords() will not handle deleted records, while rollbackTransaction() does.
Also, rollbackEditedRecords() is called before rolling back the transaction see rollbackTransaction(boolean) to control that behavior
and saved records within the transactions are restored to the database values, so user input is lost, to control this see rollbackTransaction(boolean,boolean)


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// starts a database transaction
databaseManager.startTransaction()
// Now let users input data

// when data has been entered do a commit or rollback if the data entry is canceled or the the commit did fail.
if (cancel || !databaseManager.commitTransaction())
{
	databaseManager.rollbackTransaction();
}
```
### rollbackTransaction(rollbackEdited)

Rollback a transaction started by databaseManager.startTransaction().
Note that when autosave is false, revertEditedRecords() will not handle deleted records, while rollbackTransaction() does.
Also, saved records within the transactions are restored to the database values, so user input is lost, to controll this see rollbackTransaction(boolean,boolean)

**Parameters**\
[Boolean](JSLib/Boolean.md) rollbackEdited call rollbackEditedRecords() before rolling back the transaction

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// starts a database transaction
databaseManager.startTransaction()
// Now let users input data

// when data has been entered do a commit or rollback if the data entry is canceled or the the commit did fail.
if (cancel || !databaseManager.commitTransaction())
{
	databaseManager.rollbackTransaction();
}
```
### rollbackTransaction(rollbackEdited, revertSavedRecords)

Rollback a transaction started by databaseManager.startTransaction().
Note that when autosave is false, revertEditedRecords() will not handle deleted records, while rollbackTransaction() does.

**Parameters**\
[Boolean](JSLib/Boolean.md) rollbackEdited call rollbackEditedRecords() before rolling back the transaction\
[Boolean](JSLib/Boolean.md) revertSavedRecords if false then all records in the transaction do keep the user input and are back in the edited records list.
Note that if the pks of such a record are no longer used by it's foundset (find/search or load by query or ...) it will just be rolled-back as
it can't be put in editing records list.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// starts a database transaction
databaseManager.startTransaction()
// Now let users input data

// when data has been entered do a commit or rollback if the data entry is canceled or the the commit did fail.
if (cancel || !databaseManager.commitTransaction())
{
	databaseManager.rollbackTransaction();
}
```
### saveData()

Saves all outstanding (unsaved) data and exits the current record.

Optionally, by specifying a record or foundset, can save a single record or all records from foundset instead of all the data.
Since Servoy 8.3 saveData with null parameter does not call saveData() as fallback, it just returns false.
<p>
<b>NOTE</b>: The fields focus may be lost in user interface in order to determine the edits.
		 saveData() called from table events (like afterRecordInsert) is only partially supported depending on how first saveData() (that triggers the event) is called.
		 If first saveData() is called with no arguments, all saveData() from table events are returning immediately with true value and records will be saved as part of first save.
      If first saveData() is called with record(s) as arguments, saveData() from table event will try to save record(s) from arguments that are different than those in first call.
      saveData() with no arguments inside table events will always return true without saving anything.
<p>
<b>NOTE</b>: When saveData() is called within a transaction, records after a record that fails with some sql-exception will not be saved, but moved to the failed records.
      record.exception.getErrorCode() will return ServoyException.MUST_ROLLBACK for these records.


**Returns**\
[Boolean](JSLib/Boolean.md) true if the save was done without an error.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var saved = databaseManager.saveData()
// var saved = databaseManager.saveData(foundset.getRecord(1)) // save specific record
// var saved = databaseManager.saveData(foundset) // save all records from foundset

// when creating many records in a loop do a batch save on an interval as every 10 records (to save on memory and roundtrips)
var success = true
for (var recordIndex = 1; success && recordIndex <= 5000; recordIndex++)
{
	foundset.newRecord()
	someColumn = recordIndex
	anotherColumn = "Index is: " + recordIndex
	if (recordIndex % 10 == 0) success = databaseManager.saveData()
}

// check the failed records
if (!success) {
  var failedRecords = databaseManager.getFailedRecords();
  for (var i = 0; i < failedRecords.length; i++) {
     var failedRecord = failedRecords[i]
     // failed[i].exception shows the error, failed[i].exception.getErrorCode() is one of the ServoyException.* values
  }
}
```
### saveData(foundset)

Saves all outstanding (unsaved) data and exits the current record.

Optionally, by specifying a record or foundset, can save a single record or all records from foundset instead of all the data.
Since Servoy 8.3 saveData with null parameter does not call saveData() as fallback, it just returns false.
<p>
<b>NOTE</b>: The fields focus may be lost in user interface in order to determine the edits.
		 saveData() called from table events (like afterRecordInsert) is only partially supported depending on how first saveData() (that triggers the event) is called.
		 If first saveData() is called with no arguments, all saveData() from table events are returning immediately with true value and records will be saved as part of first save.
      If first saveData() is called with record(s) as arguments, saveData() from table event will try to save record(s) from arguments that are different than those in first call.
      saveData() with no arguments inside table events will always return true without saving anything.
<p>
<b>NOTE</b>: When saveData() is called within a transaction, records after a record that fails with some sql-exception will not be saved, but moved to the failed records.
      record.exception.getErrorCode() will return ServoyException.MUST_ROLLBACK for these records.

**Parameters**\
[JSFoundSet](Database%20Manager/JSFoundSet.md) foundset The JSFoundset to save.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the save was done without an error.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var saved = databaseManager.saveData()
// var saved = databaseManager.saveData(foundset.getRecord(1)) // save specific record
// var saved = databaseManager.saveData(foundset) // save all records from foundset

// when creating many records in a loop do a batch save on an interval as every 10 records (to save on memory and roundtrips)
var success = true
for (var recordIndex = 1; success && recordIndex <= 5000; recordIndex++)
{
	foundset.newRecord()
	someColumn = recordIndex
	anotherColumn = "Index is: " + recordIndex
	if (recordIndex % 10 == 0) success = databaseManager.saveData()
}

// check the failed records
if (!success) {
  var failedRecords = databaseManager.getFailedRecords();
  for (var i = 0; i < failedRecords.length; i++) {
     var failedRecord = failedRecords[i]
     // failed[i].exception shows the error, failed[i].exception.getErrorCode() is one of the ServoyException.* values
  }
}
```
### saveData(record)

Saves all outstanding (unsaved) data and exits the current record.

Optionally, by specifying a record or foundset, can save a single record or all records from foundset instead of all the data.
Since Servoy 8.3 saveData with null parameter does not call saveData() as fallback, it just returns false.
<p>
<b>NOTE</b>: The fields focus may be lost in user interface in order to determine the edits.
		 saveData() called from table events (like afterRecordInsert) is only partially supported depending on how first saveData() (that triggers the event) is called.
		 If first saveData() is called with no arguments, all saveData() from table events are returning immediately with true value and records will be saved as part of first save.
      If first saveData() is called with record(s) as arguments, saveData() from table event will try to save record(s) from arguments that are different than those in first call.
      saveData() with no arguments inside table events will always return true without saving anything.
<p>
<b>NOTE</b>: When saveData() is called within a transaction, records after a record that fails with some sql-exception will not be saved, but moved to the failed records.
      record.exception.getErrorCode() will return ServoyException.MUST_ROLLBACK for these records.

**Parameters**\
[JSRecord](Database%20Manager/JSRecord.md) record The JSRecord to save.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the save was done without an error.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var saved = databaseManager.saveData()
// var saved = databaseManager.saveData(foundset.getRecord(1)) // save specific record
// var saved = databaseManager.saveData(foundset) // save all records from foundset

// when creating many records in a loop do a batch save on an interval as every 10 records (to save on memory and roundtrips)
var success = true
for (var recordIndex = 1; success && recordIndex <= 5000; recordIndex++)
{
	foundset.newRecord()
	someColumn = recordIndex
	anotherColumn = "Index is: " + recordIndex
	if (recordIndex % 10 == 0) success = databaseManager.saveData()
}

// check the failed records
if (!success) {
  var failedRecords = databaseManager.getFailedRecords();
  for (var i = 0; i < failedRecords.length; i++) {
     var failedRecord = failedRecords[i]
     // failed[i].exception shows the error, failed[i].exception.getErrorCode() is one of the ServoyException.* values
  }
}
```
### saveData(records)

Saves all outstanding (unsaved) data and exits the current record.

Optionally, by specifying a record or foundset, can save a single record or all records from foundset instead of all the data.
Since Servoy 8.3 saveData with null parameter does not call saveData() as fallback, it just returns false.
<p>
<b>NOTE</b>: The fields focus may be lost in user interface in order to determine the edits.
		 saveData() called from table events (like afterRecordInsert) is only partially supported depending on how first saveData() (that triggers the event) is called.
		 If first saveData() is called with no arguments, all saveData() from table events are returning immediately with true value and records will be saved as part of first save.
      If first saveData() is called with record(s) as arguments, saveData() from table event will try to save record(s) from arguments that are different than those in first call.
      saveData() with no arguments inside table events will always return true without saving anything.
<p>
<b>NOTE</b>: When saveData() is called within a transaction, records after a record that fails with some sql-exception will not be saved, but moved to the failed records.
      record.exception.getErrorCode() will return ServoyException.MUST_ROLLBACK for these records.

**Parameters**\
[Array](JSLib/Array.md) records The array of JSRecord to save.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the save was done without an error.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var saved = databaseManager.saveData()
// var saved = databaseManager.saveData(foundset.getRecord(1)) // save specific record
// var saved = databaseManager.saveData(foundset) // save all records from foundset

// when creating many records in a loop do a batch save on an interval as every 10 records (to save on memory and roundtrips)
var success = true
for (var recordIndex = 1; success && recordIndex <= 5000; recordIndex++)
{
	foundset.newRecord()
	someColumn = recordIndex
	anotherColumn = "Index is: " + recordIndex
	if (recordIndex % 10 == 0) success = databaseManager.saveData()
}

// check the failed records
if (!success) {
  var failedRecords = databaseManager.getFailedRecords();
  for (var i = 0; i < failedRecords.length; i++) {
     var failedRecord = failedRecords[i]
     // failed[i].exception shows the error, failed[i].exception.getErrorCode() is one of the ServoyException.* values
  }
}
```
### setAutoSave(autoSave)

Set autosave, if false then no saves will happen by the ui (not including deletes!).
Until you call databaseManager.saveData() or setAutoSave(true)

If you also want to be able to rollback deletes then you have to use databaseManager.startTransaction().
Because even if autosave is false deletes of records will be done.

**Parameters**\
[Boolean](JSLib/Boolean.md) autoSave Boolean to enable or disable autosave.

**Returns**\
[Boolean](JSLib/Boolean.md) false if the current edited record could not be saved.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//Rollbacks in mem the records that were edited and not yet saved. Best used in combination with autosave false.
databaseManager.setAutoSave(false)
//Now let users input data

//On save or cancel, when data has been entered:
if (cancel) databaseManager.rollbackEditedRecords()
databaseManager.setAutoSave(true)
```
### setCreateEmptyFormFoundsets()

Turnoff the initial form foundset record loading, set this in the solution open method.
Simular to calling foundset.clear() in the form's onload event.

NOTE: When the foundset record loading is turned off, controller.find or controller.loadAllRecords must be called to display the records


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this has to be called in the solution open method
databaseManager.setCreateEmptyFormFoundsets()
```
### setTableFilters(filterName, tableFilters)

Apply multiples table filters to all the foundsets that arte affected by the filters.
After all filters have been applied / updated, foundset changes will be applied in the client.

The filters that have been applied with the same filter name will be removed and replaced with the new set of filters.

**Parameters**\
[String](JSLib/String.md) filterName The name of the filter that should be removed.\
[Array](JSLib/Array.md) tableFilters list of filters to be applied.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the table filters could be applied.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Create a number of filters
var query1_nl = datasources.db.crm.companies.createSelect()
query.where.add(query1_nl.columns.countrycode.eq('nl'))
var filter1_nl = databaseManager.createTableFilterParam(query1_nl)

// apply multiple filters at the same time, previous filters with the same name are removed:
var success = databaseManager.setTableFilters('myfilters', [filter1, filter2])

// update one of the filters:
var query1_us = datasources.db.crm.companies.createSelect()
query1_us.where.add(query1_us.columns.countrycode.eq('us'))
var filter1_2 = databaseManager.createTableFilterParam(query1_us)

var success = databaseManager.setTableFilters('myfilters', [filter1_2, filter2])

// filters can be removed by setting them to an empty list:
var success = databaseManager.setTableFilters('myfilters', [])

// use the databroadCast flag on a filter to reduce databroadcast events
// for clients having a databroadcast filter set for the same column with a different value.
// Note that the dataBroadcast flag is *only* supported for simple filters, only for operator 'in' or '='.
var filter = databaseManager.createTableFilterParam('example', 'orders', 'clusterid', '=', 10).dataBroadcast(true)
var success = databaseManager.setTableFilters('clusterfilter', [filter])
```
### startTransaction()

Start a database transaction.
If you want to avoid round trips to the server or avoid the possibility of blocking other clients
because of your pending changes, you can use databaseManager.setAutoSave(false/true) and databaseManager.rollbackEditedRecords().

startTransaction, commit/rollbackTransacton() does support rollback of record deletes which autoSave = false doesn't support.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// starts a database transaction
databaseManager.startTransaction()
// Now let users input data

// when data has been entered do a commit or rollback if the data entry is canceled or the the commit did fail.
if (cancel || !databaseManager.commitTransaction())
{
	databaseManager.rollbackTransaction();
}
```
### switchServer(sourceName, destinationName)

Switches a named server to another named server with the same datamodel (recommended to be used in an onOpen method for a solution).
return true if successful.
Note that this only works if source and destination server are of the same database type.

**Parameters**\
[String](JSLib/String.md) sourceName The name of the source database server connection\
[String](JSLib/String.md) destinationName The name of the destination database server connection.

**Returns**\
[Boolean](JSLib/Boolean.md) true if the switch could be done.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//dynamically changes a server for the entire solution, destination database server must contain the same tables/columns!
//will fail if there is a lock, transaction , if repository_server is used or if destination server is invalid
//in the solution keep using the sourceName every where to reference the server!
var success = databaseManager.switchServer('crm', 'crm1')
```
### validate(record)

Validates the given record, it runs first the method that is attached to the entity event "onValidate".
Then it will call also the entity events "onInsert" or "onUpdate" depending if the record is new or an update.
All those methods do get a parameter JSRecordMarkers where the problems can be reported against.

All columns are then also null/empty checked and if they are and the Column is marked as "not null" an error will be
added with the message key "servoy.record.error.null.not.allowed" for that column.

All changed columns are length checked and if the record values is bigger then what the database column can handle and
error will be added with the message key "servoy.record.error.columnSizeTooSmall" for that column.
Then all the column validators will be run over all the changed columns, The validators will also get the same JSRecordMarkers
to report problems to. So the global method validator now also has more parameters then just the value.

These 3 validations (null, length and column validators) are not by default done any more on change of the dataprovider itself.
This is controlled by the servoy property "servoy.execute.column.validators.only.on.validate_and_save" which can also be seen at
the TableEditor column validators page.

An extra state object can be given that will also be passed around if you want to have more state in the validation objects
(like giving some ui state so the entity methods know where you come from)

It will return a JSRecordMarkers when the record had validation problems


**Parameters**\
[JSRecord](Database%20Manager/JSRecord.md) record The record to validate.

**Returns**\
[JSRecordMarkers](Database%20Manager/JSRecordMarkers.md) Returns a JSRecordMarkers if the record has validation problems

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### validate(record, customObject)

Validates the given record, it runs first the method that is attached to the entity event "onValidate".
Then it will call also the entity events "onInsert" or "onUpdate" depending if the record is new or an update.
All those methods do get a parameter JSRecordMarkers where the problems can be reported against.

All columns are then also null/empty checked and if they are and the Column is marked as "not null" an error will be
added with the message key "servoy.record.error.null.not.allowed" for that column.

All changed columns are length checked and if the record values is bigger then what the database column can handle and
error will be added with the message key "servoy.record.error.columnSizeTooSmall" for that column.
Then all the column validators will be run over all the changed columns, The validators will also get the same JSRecordMarkers
to report problems to. So the global method validator now also has more parameters then just the value.

These 3 validations (null, length and column validators) are not by default done any more on change of the dataprovider itself.
This is controlled by the servoy property "servoy.execute.column.validators.only.on.validate_and_save" which can also be seen at
the TableEditor column validators page.

An extra state object can be given that will also be passed around if you want to have more state in the validation objects
(like giving some ui state so the entity methods know where you come from)

It will return a JSRecordMarkers when the record had validation problems


**Parameters**\
[JSRecord](Database%20Manager/JSRecord.md) record The record to validate.\
[Object](JSLib/Object.md) customObject The extra customObject that is passed on the the validation methods.

**Returns**\
[JSRecordMarkers](Database%20Manager/JSRecordMarkers.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```

