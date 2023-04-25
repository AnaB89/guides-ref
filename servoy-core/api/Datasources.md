#  Datasources

## **Return Types**
[DBDataSource](Datasources/DBDataSource.md),[MemDataSource](Datasources/MemDataSource.md),[JSDataSource](Datasources/JSDataSource.md),[JSConnectionDefinition](Datasources/JSConnectionDefinition.md),[DBDataSourceServer](Datasources/DBDataSourceServer.md),[ViewDataSource](Datasources/ViewDataSource.md),

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [DBDataSource](Datasources/DBDataSource.md) | [db](Datasources.md#db)                   | Scope property for server/table based data sources..                                    |
| [MemDataSource](Datasources/MemDataSource.md) | [mem](Datasources.md#mem)                   | Scope property for in-memory data sources..                                    |
| [SPDataSource](./SPDataSource.md) | [sp](Datasources.md#sp)                   | Scope property for stored procedures..                                    |
| [ViewDataSource](Datasources/ViewDataSource.md) | [view](Datasources.md#view)                   | Scope property for view foundset data sources..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSDataSource](Datasources/JSDataSource.md) | [get(datasource)](Datasources.md#get-datasource)                   | Scope getter for a datasource node based on datasource string..                                    |

## Properties Details

### db

Scope property for server/table based data sources.

**Returns**\
[DBDataSource](Datasources/DBDataSource.md) 


**Sample**

```javascript
datasources.db.example_data.orders
```
### mem

Scope property for in-memory data sources.

**Returns**\
[MemDataSource](Datasources/MemDataSource.md) 


**Sample**

```javascript
datasources.mem['myds']
```
### sp

Scope property for stored procedures.
This will list the stored procedures of server that have this property enabled (see server editor).

**Returns**\
[SPDataSource](./SPDataSource.md) 


**Sample**

```javascript
datasources.sp.servername.mystoredproc();
```
### view

Scope property for view foundset data sources.

**Returns**\
[ViewDataSource](Datasources/ViewDataSource.md) 


**Sample**

```javascript
datasources.view['myds']
```

## Methods Details

### get(datasource)

Scope getter for a datasource node based on datasource string.

**Parameters**\
[String](JSLib/String.md) datasource  ;

**Returns**\
[JSDataSource](Datasources/JSDataSource.md) a JSDataSource based on parameter


**Sample**

```javascript
datasources.get(datasource)
```

