#  JSMaintenanceClientInformation


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](../../JSLib/Number.md) | [getApplicationType()](JSMaintenanceClientInformation.md#getapplicationtype)                   | The type of the application started by this client..                                    |
| [String](../../JSLib/String.md) | [getClientID()](JSMaintenanceClientInformation.md#getclientid)                   | The ID of this client..                                    |
| [String](../../JSLib/String.md) | [getHostAddress()](JSMaintenanceClientInformation.md#gethostaddress)                   | The host address of this client..                                    |
| [String](../../JSLib/String.md) | [getHostIdentifier()](JSMaintenanceClientInformation.md#gethostidentifier)                   | The host identifier of this client..                                    |
| [String](../../JSLib/String.md) | [getHostName()](JSMaintenanceClientInformation.md#gethostname)                   | The host name of this client..                                    |
| [Date](../../JSLib/Date.md) | [getIdleTime()](JSMaintenanceClientInformation.md#getidletime)                   | The time and date since the user has been idle..                                    |
| [Date](../../JSLib/Date.md) | [getLastAccessedTime()](JSMaintenanceClientInformation.md#getlastaccessedtime)                   | Gets the last date and time when a user has physically accessed the application..                                    |
| [Date](../../JSLib/Date.md) | [getLoginTime()](JSMaintenanceClientInformation.md#getlogintime)                   | The time and date the user logged into the system..                                    |
| [String](../../JSLib/String.md) | [getOpenSolutionName()](JSMaintenanceClientInformation.md#getopensolutionname)                   | The name of the solution that is currently open by the client..                                    |
| [String](../../JSLib/String.md) | [getStatusLine()](JSMaintenanceClientInformation.md#getstatusline)                   | This returns the status line of a NGClient (other clients don't have a value for this).                                    |
| [String](../../JSLib/String.md) | [getUserName()](JSMaintenanceClientInformation.md#getusername)                   | The name of the user who is logged in at this client..                                    |
| [String](../../JSLib/String.md) | [getUserUID()](JSMaintenanceClientInformation.md#getuseruid)                   | The ID of the user who is logged in at this client..                                    |

## Methods Details

### getApplicationType()

The type of the application started by this client.


**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var clients = plugins.maintenance.getConnectedClients();
application.output('There are ' + clients.length + ' connected clients.');
for (var i = 0; i < clients.length; i++)
{
	var client = clients[i];
	application.output('Client details:');
	application.output('	ID: ' + client.getClientID());
	application.output('	Application type: ' + client.getApplicationType());
	application.output('	Host address: ' + client.getHostAddress());
	application.output('	Host identifier: ' + client.getHostIdentifier());
	application.output('	Host name: ' + client.getHostName());
	application.output('	User name: ' + client.getUserName());
	application.output('	Used UID: ' + client.getUserUID());
	application.output('	Open solution: ' + client.getOpenSolutionName());
	application.output('	User login time and date: ' + client.getLoginTime());
	application.output('	User idle since: ' + client.getIdleTime());
	application.output('	Status line: ' + client.getStatusLine());
}
```
### getClientID()

The ID of this client.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var clients = plugins.maintenance.getConnectedClients();
application.output('There are ' + clients.length + ' connected clients.');
for (var i = 0; i < clients.length; i++)
{
	var client = clients[i];
	application.output('Client details:');
	application.output('	ID: ' + client.getClientID());
	application.output('	Application type: ' + client.getApplicationType());
	application.output('	Host address: ' + client.getHostAddress());
	application.output('	Host identifier: ' + client.getHostIdentifier());
	application.output('	Host name: ' + client.getHostName());
	application.output('	User name: ' + client.getUserName());
	application.output('	Used UID: ' + client.getUserUID());
	application.output('	Open solution: ' + client.getOpenSolutionName());
	application.output('	User login time and date: ' + client.getLoginTime());
	application.output('	User idle since: ' + client.getIdleTime());
	application.output('	Status line: ' + client.getStatusLine());
}
```
### getHostAddress()

The host address of this client.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var clients = plugins.maintenance.getConnectedClients();
application.output('There are ' + clients.length + ' connected clients.');
for (var i = 0; i < clients.length; i++)
{
	var client = clients[i];
	application.output('Client details:');
	application.output('	ID: ' + client.getClientID());
	application.output('	Application type: ' + client.getApplicationType());
	application.output('	Host address: ' + client.getHostAddress());
	application.output('	Host identifier: ' + client.getHostIdentifier());
	application.output('	Host name: ' + client.getHostName());
	application.output('	User name: ' + client.getUserName());
	application.output('	Used UID: ' + client.getUserUID());
	application.output('	Open solution: ' + client.getOpenSolutionName());
	application.output('	User login time and date: ' + client.getLoginTime());
	application.output('	User idle since: ' + client.getIdleTime());
	application.output('	Status line: ' + client.getStatusLine());
}
```
### getHostIdentifier()

The host identifier of this client.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var clients = plugins.maintenance.getConnectedClients();
application.output('There are ' + clients.length + ' connected clients.');
for (var i = 0; i < clients.length; i++)
{
	var client = clients[i];
	application.output('Client details:');
	application.output('	ID: ' + client.getClientID());
	application.output('	Application type: ' + client.getApplicationType());
	application.output('	Host address: ' + client.getHostAddress());
	application.output('	Host identifier: ' + client.getHostIdentifier());
	application.output('	Host name: ' + client.getHostName());
	application.output('	User name: ' + client.getUserName());
	application.output('	Used UID: ' + client.getUserUID());
	application.output('	Open solution: ' + client.getOpenSolutionName());
	application.output('	User login time and date: ' + client.getLoginTime());
	application.output('	User idle since: ' + client.getIdleTime());
	application.output('	Status line: ' + client.getStatusLine());
}
```
### getHostName()

The host name of this client.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var clients = plugins.maintenance.getConnectedClients();
application.output('There are ' + clients.length + ' connected clients.');
for (var i = 0; i < clients.length; i++)
{
	var client = clients[i];
	application.output('Client details:');
	application.output('	ID: ' + client.getClientID());
	application.output('	Application type: ' + client.getApplicationType());
	application.output('	Host address: ' + client.getHostAddress());
	application.output('	Host identifier: ' + client.getHostIdentifier());
	application.output('	Host name: ' + client.getHostName());
	application.output('	User name: ' + client.getUserName());
	application.output('	Used UID: ' + client.getUserUID());
	application.output('	Open solution: ' + client.getOpenSolutionName());
	application.output('	User login time and date: ' + client.getLoginTime());
	application.output('	User idle since: ' + client.getIdleTime());
	application.output('	Status line: ' + client.getStatusLine());
}
```
### getIdleTime()

The time and date since the user has been idle.


**Returns**\
[Date](../../JSLib/Date.md) 


**Sample**

```javascript
var clients = plugins.maintenance.getConnectedClients();
application.output('There are ' + clients.length + ' connected clients.');
for (var i = 0; i < clients.length; i++)
{
	var client = clients[i];
	application.output('Client details:');
	application.output('	ID: ' + client.getClientID());
	application.output('	Application type: ' + client.getApplicationType());
	application.output('	Host address: ' + client.getHostAddress());
	application.output('	Host identifier: ' + client.getHostIdentifier());
	application.output('	Host name: ' + client.getHostName());
	application.output('	User name: ' + client.getUserName());
	application.output('	Used UID: ' + client.getUserUID());
	application.output('	Open solution: ' + client.getOpenSolutionName());
	application.output('	User login time and date: ' + client.getLoginTime());
	application.output('	User idle since: ' + client.getIdleTime());
	application.output('	Status line: ' + client.getStatusLine());
}
```
### getLastAccessedTime()

Gets the last date and time when a user has physically accessed the application. NGClient only!


**Returns**\
[Date](../../JSLib/Date.md) a date object or null if the client doesn't support this


**Sample**

```javascript
var clients = plugins.maintenance.getConnectedClients();
application.output('There are ' + clients.length + ' connected clients.');
for (var i = 0; i < clients.length; i++)
{
	var client = clients[i];
	application.output('Client details:');
	application.output('	ID: ' + client.getClientID());
	application.output('	Application type: ' + client.getApplicationType());
	application.output('	Host address: ' + client.getHostAddress());
	application.output('	Host identifier: ' + client.getHostIdentifier());
	application.output('	Host name: ' + client.getHostName());
	application.output('	User name: ' + client.getUserName());
	application.output('	Used UID: ' + client.getUserUID());
	application.output('	Open solution: ' + client.getOpenSolutionName());
	application.output('	User login time and date: ' + client.getLoginTime());
	application.output('	User idle since: ' + client.getIdleTime());
	application.output('	Status line: ' + client.getStatusLine());
}
```
### getLoginTime()

The time and date the user logged into the system.


**Returns**\
[Date](../../JSLib/Date.md) 


**Sample**

```javascript
var clients = plugins.maintenance.getConnectedClients();
application.output('There are ' + clients.length + ' connected clients.');
for (var i = 0; i < clients.length; i++)
{
	var client = clients[i];
	application.output('Client details:');
	application.output('	ID: ' + client.getClientID());
	application.output('	Application type: ' + client.getApplicationType());
	application.output('	Host address: ' + client.getHostAddress());
	application.output('	Host identifier: ' + client.getHostIdentifier());
	application.output('	Host name: ' + client.getHostName());
	application.output('	User name: ' + client.getUserName());
	application.output('	Used UID: ' + client.getUserUID());
	application.output('	Open solution: ' + client.getOpenSolutionName());
	application.output('	User login time and date: ' + client.getLoginTime());
	application.output('	User idle since: ' + client.getIdleTime());
	application.output('	Status line: ' + client.getStatusLine());
}
```
### getOpenSolutionName()

The name of the solution that is currently open by the client.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var clients = plugins.maintenance.getConnectedClients();
application.output('There are ' + clients.length + ' connected clients.');
for (var i = 0; i < clients.length; i++)
{
	var client = clients[i];
	application.output('Client details:');
	application.output('	ID: ' + client.getClientID());
	application.output('	Application type: ' + client.getApplicationType());
	application.output('	Host address: ' + client.getHostAddress());
	application.output('	Host identifier: ' + client.getHostIdentifier());
	application.output('	Host name: ' + client.getHostName());
	application.output('	User name: ' + client.getUserName());
	application.output('	Used UID: ' + client.getUserUID());
	application.output('	Open solution: ' + client.getOpenSolutionName());
	application.output('	User login time and date: ' + client.getLoginTime());
	application.output('	User idle since: ' + client.getIdleTime());
	application.output('	Status line: ' + client.getStatusLine());
}
```
### getStatusLine()

This returns the status line of a NGClient (other clients don't have a value for this)


**Returns**\
[String](../../JSLib/String.md) a string that is the status line as reported on the admin page.


**Sample**

```javascript
var clients = plugins.maintenance.getConnectedClients();
application.output('There are ' + clients.length + ' connected clients.');
for (var i = 0; i < clients.length; i++)
{
	var client = clients[i];
	application.output('Client details:');
	application.output('	ID: ' + client.getClientID());
	application.output('	Application type: ' + client.getApplicationType());
	application.output('	Host address: ' + client.getHostAddress());
	application.output('	Host identifier: ' + client.getHostIdentifier());
	application.output('	Host name: ' + client.getHostName());
	application.output('	User name: ' + client.getUserName());
	application.output('	Used UID: ' + client.getUserUID());
	application.output('	Open solution: ' + client.getOpenSolutionName());
	application.output('	User login time and date: ' + client.getLoginTime());
	application.output('	User idle since: ' + client.getIdleTime());
	application.output('	Status line: ' + client.getStatusLine());
}
```
### getUserName()

The name of the user who is logged in at this client.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var clients = plugins.maintenance.getConnectedClients();
application.output('There are ' + clients.length + ' connected clients.');
for (var i = 0; i < clients.length; i++)
{
	var client = clients[i];
	application.output('Client details:');
	application.output('	ID: ' + client.getClientID());
	application.output('	Application type: ' + client.getApplicationType());
	application.output('	Host address: ' + client.getHostAddress());
	application.output('	Host identifier: ' + client.getHostIdentifier());
	application.output('	Host name: ' + client.getHostName());
	application.output('	User name: ' + client.getUserName());
	application.output('	Used UID: ' + client.getUserUID());
	application.output('	Open solution: ' + client.getOpenSolutionName());
	application.output('	User login time and date: ' + client.getLoginTime());
	application.output('	User idle since: ' + client.getIdleTime());
	application.output('	Status line: ' + client.getStatusLine());
}
```
### getUserUID()

The ID of the user who is logged in at this client.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var clients = plugins.maintenance.getConnectedClients();
application.output('There are ' + clients.length + ' connected clients.');
for (var i = 0; i < clients.length; i++)
{
	var client = clients[i];
	application.output('Client details:');
	application.output('	ID: ' + client.getClientID());
	application.output('	Application type: ' + client.getApplicationType());
	application.output('	Host address: ' + client.getHostAddress());
	application.output('	Host identifier: ' + client.getHostIdentifier());
	application.output('	Host name: ' + client.getHostName());
	application.output('	User name: ' + client.getUserName());
	application.output('	Used UID: ' + client.getUserUID());
	application.output('	Open solution: ' + client.getOpenSolutionName());
	application.output('	User login time and date: ' + client.getLoginTime());
	application.output('	User idle since: ' + client.getIdleTime());
	application.output('	Status line: ' + client.getStatusLine());
}
```

