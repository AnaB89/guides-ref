#  clientmanager

## **Return Types**
[Broadcaster](./Broadcaster.md),[JSClientInformation](./JSClientInformation.md),

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Broadcaster](./Broadcaster.md) | [getBroadcaster(name, channelName, callback)](clientmanager.md#getbroadcaster-name-channelname-callback)                   | Get a broadcast object giving it a (nick)name and on a specific channel, the callback is used for getting messages of other clients on that channel The function gets 3 arguments (nickName, message, channelName).                                    |
| [JSClientInformation](./JSClientInformation.md) | [getClientInformation()](clientmanager.md#getclientinformation)                   | Returns the current client JSClientInformation object..                                    |
| [Array](../../JSLib/Array.md) | [getConnectedClients()](clientmanager.md#getconnectedclients)                   | Returns an array of JSClientInformation elements describing the clients connected to the server..                                    |
| [Array](../../JSLib/Array.md) | [getConnectedClients(clientInfoFilter)](clientmanager.md#getconnectedclients-clientinfofilter)                   | /* Returns an array of JSClientInformation elements describing the clients connected to the server filtered by the a client info string..                                    |
| [JSClientInformation](./JSClientInformation.md) | [getLockedByClient(datasource, pks)](clientmanager.md#getlockedbyclient-datasource-pks)                   | Get client that locked the record from a specific datasource or null if record is not locked..                                    |
| [JSDataSet](../../Database%20Manager/JSDataSet.md) | [getLocks()](clientmanager.md#getlocks)                   | Get a dataset will all locks on the server..                                    |
| [Boolean](../../JSLib/Boolean.md) | [isInMaintenanceMode()](clientmanager.md#isinmaintenancemode)                   | Returns true if the server is in maintenance mode, false otherwise..                                    |
|void | [releaseLocks(clientId)](clientmanager.md#releaselocks-clientid)                   | Release all locks acquired by a client  WARNING: use with care.                                    |
|void | [sendMessageToAllClients(message)](clientmanager.md#sendmessagetoallclients-message)                   | Sends a message to all connected clients..                                    |
|void | [sendMessageToClient(clientId, message)](clientmanager.md#sendmessagetoclient-clientid-message)                   | Sends a message to a specific client, identified by its clientId..                                    |
|void | [shutDownAllClients()](clientmanager.md#shutdownallclients)                   | Shuts down all connected clients..                                    |
|void | [shutDownClient(clientId)](clientmanager.md#shutdownclient-clientid)                   | Shuts down a specific client, identified by its clientId..                                    |
|void | [shutDownClient(clientId, forceUnregister)](clientmanager.md#shutdownclient-clientid-forceunregister)                   | Shuts down a specific client, identified by its clientId..                                    |

## Methods Details

### getBroadcaster(name, channelName, callback)

Get a broadcast object giving it a (nick)name and on a specific channel, the callback is used for getting messages of other clients on that channel
The function gets 3 arguments (nickName, message, channelName)

**Parameters**\
[String](../../JSLib/String.md) name The nickname for this user on this channel\
[String](../../JSLib/String.md) channelName The channel name where should be listened to (and send messages to)\
[Function](../../JSLib/Function.md) callback The callback when for incomming messages

**Returns**\
[Broadcaster](./Broadcaster.md) BroadCaster


**Sample**

```javascript
function callback(nickName, message, channelName) {
   application.output('message received from ' + nickName + ' on channel ' + channelName + ': ' + message)
}
var broadcaster = plugins.clientmanager.getBroadcaster("nickname", "mychatchannel", callback);
broadcaster.broadcastMessage("Hallo");
```
### getClientInformation()

Returns the current client JSClientInformation object. Note this is snapshot information, client information will not get updated.


**Returns**\
[JSClientInformation](./JSClientInformation.md) 


**Sample**

```javascript

```
### getConnectedClients()

Returns an array of JSClientInformation elements describing the clients connected to the server. Note this is snapshot information on connected clients, client information will not get updated.


**Returns**\
[Array](../../JSLib/Array.md) JSClientInformation[]


**Sample**

```javascript
//Returns an array of JSClientInformation elements describing the clients connected to the server.
var clients = plugins.clientmanager.getConnectedClients();
application.output("There are " + clients.length + " connected clients.");
for (var i = 0; i < clients.length; i++)
	application.output("Client has clientId '" + clients[i].getClientID() + "' and has connected from host '" + clients[i].getHostAddress() + "'.");
```
### getConnectedClients(clientInfoFilter)

/*
Returns an array of JSClientInformation elements describing the clients connected to the server filtered by the a client info string.
This way you can ask for a specific set of clients that have a specific information added to there client information.
Note this is snapshot information on connected clients, client information will not get updated.

**Parameters**\
[String](../../JSLib/String.md) clientInfoFilter The filter string

**Returns**\
[Array](../../JSLib/Array.md) JSClientInformation[]


**Sample**

```javascript
//Returns an array of JSClientInformation elements describing the clients connected to the server.
var clients = plugins.clientmanager.getConnectedClients();
application.output("There are " + clients.length + " connected clients.");
for (var i = 0; i < clients.length; i++)
	application.output("Client has clientId '" + clients[i].getClientID() + "' and has connected from host '" + clients[i].getHostAddress() + "'.");
```
### getLockedByClient(datasource, pks)

Get client that locked the record from a specific datasource or null if record is not locked.

**Parameters**\
[String](../../JSLib/String.md) datasource  ;\
[Array](../../JSLib/Array.md) pks  ;

**Returns**\
[JSClientInformation](./JSClientInformation.md) Client information


**Sample**

```javascript
var client = plugins.clientmanager.getLockedByClient(foundset.getDataSource(),record.getPKs());
```
### getLocks()

Get a dataset will all locks on the server. The dataset will have four columns: datasource, acquireDate, clientId, pkHash.
	Each row in the dataset will be a lock.


**Returns**\
[JSDataSet](../../Database%20Manager/JSDataSet.md) 


**Sample**

```javascript
var locks = plugins.clientmanager.getLocks();
```
### isInMaintenanceMode()

Returns true if the server is in maintenance mode, false otherwise.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
//Returns true if the server is in maintenance mode, false otherwise.
if (plugins.maintenance.isInMaintenanceMode())
	application.output("Server is in maintenance mode.");
else
	application.output("Server is not in maintenance mode.");
```
### releaseLocks(clientId)

Release all locks acquired by a client

WARNING: use with care

**Parameters**\
[String](../../JSLib/String.md) clientId  ;

**Returns**\
void 


**Sample**

```javascript

```
### sendMessageToAllClients(message)

Sends a message to all connected clients.

**Parameters**\
[String](../../JSLib/String.md) message  ;

**Returns**\
void 


**Sample**

```javascript
//Sends a message to all connected clients.
plugins.clientmanager.sendMessageToAllClients("Hello, all clients!");
```
### sendMessageToClient(clientId, message)

Sends a message to a specific client, identified by its clientId. The clientIds are retrieved by calling the getConnectedClients method.

**Parameters**\
[String](../../JSLib/String.md) clientId  ;\
[String](../../JSLib/String.md) message  ;

**Returns**\
void 


**Sample**

```javascript
//Sends a message to a specific client, identified by its clientId. The clientIds are retrieved by calling the getConnectedClients method.
var clients = plugins.clientmanager.getConnectedClients();
for (var i=0; i<clients.length; i++)
	plugins.clientmanager.sendMessageToClient(clients[i].getClientId(), "Hello, client " + clients[i].getClientID() + "!");
```
### shutDownAllClients()

Shuts down all connected clients. This method returns immediately, it does not wait until the client shuts down.


**Returns**\
void 


**Sample**

```javascript
//Shuts down all connected clients. This method returns immediately, it does not wait until the client shuts down.
plugins.clientmanager.shutDownAllClients();
```
### shutDownClient(clientId)

Shuts down a specific client, identified by its clientId. The clientIds are retrieved by calling the getConnectedClients method. This method returns immediately, it does not wait until the client shuts down.

**Parameters**\
[String](../../JSLib/String.md) clientId  ;

**Returns**\
void 


**Sample**

```javascript
//Shuts down a specific client, identified by its clientId. The clientIds are retrieved by calling the getConnectedClients method. This method returns immediately, it does not wait until the client shuts down.
var clients = plugins.clientmanager.getConnectedClients();
for (var i=0; i<clients.length; i++)
	plugins.clientmanager.shutDownClient(clients[i].getClientId());
```
### shutDownClient(clientId, forceUnregister)

Shuts down a specific client, identified by its clientId. The clientIds are retrieved by calling the getConnectedClients method. This method returns immediately, it does not wait until the client shuts down.
If forceUnregister is true, the client will unregister itself from server. Beware this should be used only if you are sure client is already closed (cannot connect anymore)

**Parameters**\
[String](../../JSLib/String.md) clientId  ;\
[Boolean](../../JSLib/Boolean.md) forceUnregister client is forced to unregister from server

**Returns**\
void 


**Sample**

```javascript
//Shuts down a specific client, identified by its clientId. The clientIds are retrieved by calling the getConnectedClients method. This method returns immediately, it does not wait until the client shuts down.
var clients = plugins.clientmanager.getConnectedClients();
for (var i=0; i<clients.length; i++)
	plugins.clientmanager.shutDownClient(clients[i].getClientId());
```

