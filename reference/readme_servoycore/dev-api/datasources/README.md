# Datasources

## **Return Types**

[DBDataSource](dbdatasource.md),[MemDataSource](memdatasource.md),[JSDataSource](jsdatasource.md),[JSConnectionDefinition](jsconnectiondefinition.md),[DBDataSourceServer](dbdatasourceserver.md),[ViewDataSource](../../../../servoy-core/api/Datasources/ViewDataSource.md),

## Property Summary

| Type                                                                        | Name            | Summary                                              |
| --------------------------------------------------------------------------- | --------------- | ---------------------------------------------------- |
| [DBDataSource](dbdatasource.md)                                             | [db](./#db)     | Scope property for server/table based data sources.. |
| [MemDataSource](memdatasource.md)                                           | [mem](./#mem)   | Scope property for in-memory data sources..          |
| [SPDataSource](../../../../servoy-core/api/SPDataSource.md)                 | [sp](./#sp)     | Scope property for stored procedures..               |
| [ViewDataSource](../../../../servoy-core/api/Datasources/ViewDataSource.md) | [view](./#view) | Scope property for view foundset data sources..      |

## Methods Summary

| Type                            | Name                                 | Summary                                                         |
| ------------------------------- | ------------------------------------ | --------------------------------------------------------------- |
| [JSDataSource](jsdatasource.md) | [get(datasource)](./#get-datasource) | Scope getter for a datasource node based on datasource string.. |

## Properties Details

### db

Scope property for server/table based data sources.

**Returns**\
[DBDataSource](dbdatasource.md)

**Sample**

```javascript
datasources.db.example_data.orders
```

### mem

Scope property for in-memory data sources.

**Returns**\
[MemDataSource](memdatasource.md)

**Sample**

```javascript
datasources.mem['myds']
```

### sp

Scope property for stored procedures. This will list the stored procedures of server that have this property enabled (see server editor).

**Returns**\
[SPDataSource](../../../../servoy-core/api/SPDataSource.md)

**Sample**

```javascript
datasources.sp.servername.mystoredproc();
```

### view

Scope property for view foundset data sources.

**Returns**\
[ViewDataSource](../../../../servoy-core/api/Datasources/ViewDataSource.md)

**Sample**

```javascript
datasources.view['myds']
```

## Methods Details

### get(datasource)

Scope getter for a datasource node based on datasource string.

**Parameters**\
[String](../js-lib/string.md) datasource ;

**Returns**\
[JSDataSource](jsdatasource.md) a JSDataSource based on parameter

**Sample**

```javascript
datasources.get(datasource)
```
