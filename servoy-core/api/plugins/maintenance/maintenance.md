#  maintenance

## **Return Types**
[JSMaintenanceClientInformation](./JSMaintenanceClientInformation.md),[JSServer](./JSServer.md),[JSTableObject](./JSTableObject.md),[JSColumnObject](./JSColumnObject.md),

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSServer](./JSServer.md) | [getServer(serverName)](maintenance.md#getserver-servername)                   | Retrieves an instance of JSServer corresponding to the server with the name specified through the "serverName" argument..                                    |
| [JSServer](./JSServer.md) | [getServer(serverName, mustBeEnabled)](maintenance.md#getserver-servername-mustbeenabled)                   | Retrieves an instance of JSServer corresponding to the server with the name specified through the "serverName" argument..                                    |
| [JSServer](./JSServer.md) | [getServer(serverName, mustBeEnabled, mustBeValid)](maintenance.md#getserver-servername-mustbeenabled-mustbevalid)                   | Retrieves an instance of JSServer corresponding to the server with the name specified through the "serverName" argument..                                    |
| [Array](../../JSLib/Array.md) | [getServerNames()](maintenance.md#getservernames)                   | Retrieves a list with the names of all available database servers..                                    |
| [Array](../../JSLib/Array.md) | [getServerNames(mustBeEnabled)](maintenance.md#getservernames-mustbeenabled)                   | Retrieves a list with the names of all available database servers..                                    |
| [Array](../../JSLib/Array.md) | [getServerNames(mustBeEnabled, mustBeValid)](maintenance.md#getservernames-mustbeenabled-mustbevalid)                   | Retrieves a list with the names of all available database servers..                                    |
| [Array](../../JSLib/Array.md) | [getServerNames(mustBeEnabled, mustBeValid, sort)](maintenance.md#getservernames-mustbeenabled-mustbevalid-sort)                   | Retrieves a list with the names of all available database servers..                                    |
| [Array](../../JSLib/Array.md) | [getServerNames(mustBeEnabled, mustBeValid, sort, includeDuplicates)](maintenance.md#getservernames-mustbeenabled-mustbevalid-sort-includeduplicates)                   | Retrieves a list with the names of all available database servers..                                    |
| [Boolean](../../JSLib/Boolean.md) | [isInMaintenanceMode()](maintenance.md#isinmaintenancemode)                   | Returns true if the server is in maintenance mode, false otherwise..                                    |
|void | [setMaintenanceMode(maintenanceMode)](maintenance.md#setmaintenancemode-maintenancemode)                   | Puts the server into/out of maintenance mode, depending on the boolean parameter that is specified (if the parameter is true, then the server will be put into maintenance mode; if the parameter is false, then the server will be put out of maintenance mode)..                                    |

## Methods Details

### getServer(serverName)

Retrieves an instance of JSServer corresponding to the server with the name specified through the "serverName" argument.
If the optional argument "mustBeEnabled" is set to true, then the JSServer instance is returned only if the server is active.
Similarly, if the "mustBeValid" optional argument is set to true, then the JSServer instance is returned only if the server is valid.
If the specified server is not found, or if it does not meet the requirements imposed by the optional arguments, then null is returned.
By default both optional arguments have the value false.

**Parameters**\
[String](../../JSLib/String.md) serverName  ;

**Returns**\
[JSServer](./JSServer.md) 


**Sample**

```javascript
// WARNING: maintenance plugin is only meant to run during solution import using before or after import hook(so not from Smart/Web client)
//Retrieves an instance of JSServer corresponding to the server with the name specified through the "serverName" argument.
//If the optional argument "mustBeEnabled" is set to true, then the JSServer instance is returned only if the server is active.
//Similarly, if the "mustBeValid" optional argument is set to true, then the JSServer instance is returned only if the server is valid.
//If the specified server is not found, or if it does not meet the requirements imposed by the optional arguments, then null is returned.
//By default both optional arguments have the value false.
var server = plugins.maintenance.getServer("example_data");
if (server) {
	var tableNames = server.getTableNames();
	application.output("There are " + tableNames.length + " tables.");
	for (var i=0; i<tableNames.length; i++)
		application.output("Table " + i + ": " + tableNames[i]);
}
else {
	plugins.dialogs.showInfoDialog("Attention","Server 'example_data' cannot be found.","OK");
}
```
### getServer(serverName, mustBeEnabled)

Retrieves an instance of JSServer corresponding to the server with the name specified through the "serverName" argument.
If the optional argument "mustBeEnabled" is set to true, then the JSServer instance is returned only if the server is active.
Similarly, if the "mustBeValid" optional argument is set to true, then the JSServer instance is returned only if the server is valid.
If the specified server is not found, or if it does not meet the requirements imposed by the optional arguments, then null is returned.
By default both optional arguments have the value false.

**Parameters**\
[String](../../JSLib/String.md) serverName  ;\
[Boolean](../../JSLib/Boolean.md) mustBeEnabled  ;

**Returns**\
[JSServer](./JSServer.md) 


**Sample**

```javascript
// WARNING: maintenance plugin is only meant to run during solution import using before or after import hook(so not from Smart/Web client)
//Retrieves an instance of JSServer corresponding to the server with the name specified through the "serverName" argument.
//If the optional argument "mustBeEnabled" is set to true, then the JSServer instance is returned only if the server is active.
//Similarly, if the "mustBeValid" optional argument is set to true, then the JSServer instance is returned only if the server is valid.
//If the specified server is not found, or if it does not meet the requirements imposed by the optional arguments, then null is returned.
//By default both optional arguments have the value false.
var server = plugins.maintenance.getServer("example_data");
if (server) {
	var tableNames = server.getTableNames();
	application.output("There are " + tableNames.length + " tables.");
	for (var i=0; i<tableNames.length; i++)
		application.output("Table " + i + ": " + tableNames[i]);
}
else {
	plugins.dialogs.showInfoDialog("Attention","Server 'example_data' cannot be found.","OK");
}
```
### getServer(serverName, mustBeEnabled, mustBeValid)

Retrieves an instance of JSServer corresponding to the server with the name specified through the "serverName" argument.
If the optional argument "mustBeEnabled" is set to true, then the JSServer instance is returned only if the server is active.
Similarly, if the "mustBeValid" optional argument is set to true, then the JSServer instance is returned only if the server is valid.
If the specified server is not found, or if it does not meet the requirements imposed by the optional arguments, then null is returned.
By default both optional arguments have the value false.

**Parameters**\
[String](../../JSLib/String.md) serverName  ;\
[Boolean](../../JSLib/Boolean.md) mustBeEnabled  ;\
[Boolean](../../JSLib/Boolean.md) mustBeValid  ;

**Returns**\
[JSServer](./JSServer.md) 


**Sample**

```javascript
// WARNING: maintenance plugin is only meant to run during solution import using before or after import hook(so not from Smart/Web client)
//Retrieves an instance of JSServer corresponding to the server with the name specified through the "serverName" argument.
//If the optional argument "mustBeEnabled" is set to true, then the JSServer instance is returned only if the server is active.
//Similarly, if the "mustBeValid" optional argument is set to true, then the JSServer instance is returned only if the server is valid.
//If the specified server is not found, or if it does not meet the requirements imposed by the optional arguments, then null is returned.
//By default both optional arguments have the value false.
var server = plugins.maintenance.getServer("example_data");
if (server) {
	var tableNames = server.getTableNames();
	application.output("There are " + tableNames.length + " tables.");
	for (var i=0; i<tableNames.length; i++)
		application.output("Table " + i + ": " + tableNames[i]);
}
else {
	plugins.dialogs.showInfoDialog("Attention","Server 'example_data' cannot be found.","OK");
}
```
### getServerNames()

Retrieves a list with the names of all available database servers. The returned list will contain only enabled servers if the "mustBeEnabled"
optional argument is set to true. The list will contain only valid servers if the "mustBeValid" argument is set to true. If the "sort" optional
argument is set to true, then the list will be sorted alphabetically. If the "includeDuplicates" optional argument is set to false, then duplicate
servers will appear only once in the list. By default, the "mustBeEnabled" and the "mustBeValid" arguments have the value false, while the "sort"
and "includeDuplicates" arguments have the value true.


**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
// WARNING: maintenance plugin is only meant to run during solution import using before or after import hook(so not from Smart/Web client)
//Retrieves a list with the names of all available database servers. The returned list will contain only enabled servers if the "mustBeEnabled"
//optional argument is set to true. The list will contain only valid servers if the "mustBeValid" argument is set to true. If the "sort" optional
//argument is set to true, then the list will be sorted alphabetically. If the "includeDuplicates" optional argument is set to false, then duplicate
//servers will appear only once in the list. By default, the "mustBeEnabled" and the "mustBeValid" arguments have the value false, while the "sort"
//and "includeDuplicates" arguments have the value true.
var serverNames = plugins.maintenance.getServerNames();
application.output("There are " + serverNames.length + " servers.");
for (var i=0; i<serverNames.length; i++)
	application.output("Server " + i + ": " + serverNames[i]);
```
### getServerNames(mustBeEnabled)

Retrieves a list with the names of all available database servers. The returned list will contain only enabled servers if the "mustBeEnabled"
optional argument is set to true. The list will contain only valid servers if the "mustBeValid" argument is set to true. If the "sort" optional
argument is set to true, then the list will be sorted alphabetically. If the "includeDuplicates" optional argument is set to false, then duplicate
servers will appear only once in the list. By default, the "mustBeEnabled" and the "mustBeValid" arguments have the value false, while the "sort"
and "includeDuplicates" arguments have the value true.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) mustBeEnabled  ;

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
// WARNING: maintenance plugin is only meant to run during solution import using before or after import hook(so not from Smart/Web client)
//Retrieves a list with the names of all available database servers. The returned list will contain only enabled servers if the "mustBeEnabled"
//optional argument is set to true. The list will contain only valid servers if the "mustBeValid" argument is set to true. If the "sort" optional
//argument is set to true, then the list will be sorted alphabetically. If the "includeDuplicates" optional argument is set to false, then duplicate
//servers will appear only once in the list. By default, the "mustBeEnabled" and the "mustBeValid" arguments have the value false, while the "sort"
//and "includeDuplicates" arguments have the value true.
var serverNames = plugins.maintenance.getServerNames();
application.output("There are " + serverNames.length + " servers.");
for (var i=0; i<serverNames.length; i++)
	application.output("Server " + i + ": " + serverNames[i]);
```
### getServerNames(mustBeEnabled, mustBeValid)

Retrieves a list with the names of all available database servers. The returned list will contain only enabled servers if the "mustBeEnabled"
optional argument is set to true. The list will contain only valid servers if the "mustBeValid" argument is set to true. If the "sort" optional
argument is set to true, then the list will be sorted alphabetically. If the "includeDuplicates" optional argument is set to false, then duplicate
servers will appear only once in the list. By default, the "mustBeEnabled" and the "mustBeValid" arguments have the value false, while the "sort"
and "includeDuplicates" arguments have the value true.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) mustBeEnabled  ;\
[Boolean](../../JSLib/Boolean.md) mustBeValid  ;

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
// WARNING: maintenance plugin is only meant to run during solution import using before or after import hook(so not from Smart/Web client)
//Retrieves a list with the names of all available database servers. The returned list will contain only enabled servers if the "mustBeEnabled"
//optional argument is set to true. The list will contain only valid servers if the "mustBeValid" argument is set to true. If the "sort" optional
//argument is set to true, then the list will be sorted alphabetically. If the "includeDuplicates" optional argument is set to false, then duplicate
//servers will appear only once in the list. By default, the "mustBeEnabled" and the "mustBeValid" arguments have the value false, while the "sort"
//and "includeDuplicates" arguments have the value true.
var serverNames = plugins.maintenance.getServerNames();
application.output("There are " + serverNames.length + " servers.");
for (var i=0; i<serverNames.length; i++)
	application.output("Server " + i + ": " + serverNames[i]);
```
### getServerNames(mustBeEnabled, mustBeValid, sort)

Retrieves a list with the names of all available database servers. The returned list will contain only enabled servers if the "mustBeEnabled"
optional argument is set to true. The list will contain only valid servers if the "mustBeValid" argument is set to true. If the "sort" optional
argument is set to true, then the list will be sorted alphabetically. If the "includeDuplicates" optional argument is set to false, then duplicate
servers will appear only once in the list. By default, the "mustBeEnabled" and the "mustBeValid" arguments have the value false, while the "sort"
and "includeDuplicates" arguments have the value true.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) mustBeEnabled  ;\
[Boolean](../../JSLib/Boolean.md) mustBeValid  ;\
[Boolean](../../JSLib/Boolean.md) sort  ;

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
// WARNING: maintenance plugin is only meant to run during solution import using before or after import hook(so not from Smart/Web client)
//Retrieves a list with the names of all available database servers. The returned list will contain only enabled servers if the "mustBeEnabled"
//optional argument is set to true. The list will contain only valid servers if the "mustBeValid" argument is set to true. If the "sort" optional
//argument is set to true, then the list will be sorted alphabetically. If the "includeDuplicates" optional argument is set to false, then duplicate
//servers will appear only once in the list. By default, the "mustBeEnabled" and the "mustBeValid" arguments have the value false, while the "sort"
//and "includeDuplicates" arguments have the value true.
var serverNames = plugins.maintenance.getServerNames();
application.output("There are " + serverNames.length + " servers.");
for (var i=0; i<serverNames.length; i++)
	application.output("Server " + i + ": " + serverNames[i]);
```
### getServerNames(mustBeEnabled, mustBeValid, sort, includeDuplicates)

Retrieves a list with the names of all available database servers. The returned list will contain only enabled servers if the "mustBeEnabled"
optional argument is set to true. The list will contain only valid servers if the "mustBeValid" argument is set to true. If the "sort" optional
argument is set to true, then the list will be sorted alphabetically. If the "includeDuplicates" optional argument is set to false, then duplicate
servers will appear only once in the list. By default, the "mustBeEnabled" and the "mustBeValid" arguments have the value false, while the "sort"
and "includeDuplicates" arguments have the value true.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) mustBeEnabled  ;\
[Boolean](../../JSLib/Boolean.md) mustBeValid  ;\
[Boolean](../../JSLib/Boolean.md) sort  ;\
[Boolean](../../JSLib/Boolean.md) includeDuplicates  ;

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
// WARNING: maintenance plugin is only meant to run during solution import using before or after import hook(so not from Smart/Web client)
//Retrieves a list with the names of all available database servers. The returned list will contain only enabled servers if the "mustBeEnabled"
//optional argument is set to true. The list will contain only valid servers if the "mustBeValid" argument is set to true. If the "sort" optional
//argument is set to true, then the list will be sorted alphabetically. If the "includeDuplicates" optional argument is set to false, then duplicate
//servers will appear only once in the list. By default, the "mustBeEnabled" and the "mustBeValid" arguments have the value false, while the "sort"
//and "includeDuplicates" arguments have the value true.
var serverNames = plugins.maintenance.getServerNames();
application.output("There are " + serverNames.length + " servers.");
for (var i=0; i<serverNames.length; i++)
	application.output("Server " + i + ": " + serverNames[i]);
```
### isInMaintenanceMode()

Returns true if the server is in maintenance mode, false otherwise.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
// WARNING: maintenance plugin is only meant to run during solution import using before or after import hook(so not from Smart/Web client)
//Returns true if the server is in maintenance mode, false otherwise.
if (plugins.maintenance.isInMaintenanceMode())
	application.output("Server is in maintenance mode.");
else
	application.output("Server is not in maintenance mode.");
```
### setMaintenanceMode(maintenanceMode)

Puts the server into/out of maintenance mode, depending on the boolean parameter that is specified (if the parameter is true, then the server will be put into maintenance mode; if the parameter is false, then the server will be put out of maintenance mode).

**Parameters**\
[Boolean](../../JSLib/Boolean.md) maintenanceMode  ;

**Returns**\
void 


**Sample**

```javascript
// WARNING: maintenance plugin is only meant to run during solution import using before or after import hook(so not from Smart/Web client)
//Puts the server into/out of maintenance mode, depending on the boolean parameter that is specified (if the parameter is true, then the server will be put into maintenance mode; if the parameter is false, then the server will be put out of maintenance mode).
plugins.maintenance.setMaintenanceMode(!plugins.maintenance.isInMaintenanceMode());
```

