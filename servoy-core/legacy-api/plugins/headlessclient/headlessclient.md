#  headlessclient

## **Return Types**
[JSClient](./JSClient.md),
## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSClient](./JSClient.md) | [createClient(solutionName, username, password, solutionOpenMethodArgs)](headlessclient.md#createclient-solutionname-username-password-solutionopenmethodargs)                   | Creates a headless client on the server that will open the given solution..                                    |
| [JSClient](./JSClient.md) | [getClient(clientID)](headlessclient.md#getclient-clientid)                   | Gets an existing headless client for the given client uuid..                                    |
| [JSClient](./JSClient.md) | [getOrCreateClient(clientId, solutionname, username, password, solutionOpenMethodArgs)](headlessclient.md#getorcreateclient-clientid-solutionname-username-password-solutionopenmethodargs)                   | This will try to get a existing client by the given id if that client is already created for that specific solution; it will create a headless client on the server that will open the given solution if it didn't exists yet..                                    |

## Methods Details

### createClient(solutionName, username, password, solutionOpenMethodArgs)

Creates a headless client on the server that will open the given solution.
The clientId of this client can be stored in the database to be shared between clients so that that specific client can be used
over multiply clients later on or picked up later on by this client. (Even after restart of this client)

NOTE: in the developer this will only load one solution in debug mode when it is the current active solution or a module of the active solution.
So calling createClient with the same or another solution/module will replace the existig debug client.
You can load any solution (and have multily  JSClient instances) from the workspace when you pass "nodebug" as last argument in the arguments list (it should still use the same resources project).
But then you won't be able to debug it, breakpoints won't hit.

**Parameters**\
[String](../../JSLib/String.md) solutionName  ;\
[String](../../JSLib/String.md) username  ;\
[String](../../JSLib/String.md) password  ;\
[Array](../../JSLib/Array.md) solutionOpenMethodArgs  ;

**Returns**\
[JSClient](./JSClient.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Creates a headless client that will open the given solution.
var headlessClient = plugins.headlessclient.createClient("someSolution", "user", "pass", null);
if (headlessClient != null && headlessClient.isValid()) {
	var x = new Object();
	x.name = 'remote1';
	x.number = 10;
	headlessClient.queueMethod(null, "remoteMethod", [x], callback);
}
```
### getClient(clientID)

Gets an existing headless client for the given client uuid.

**Parameters**\
[String](../../JSLib/String.md) clientID  ;

**Returns**\
[JSClient](./JSClient.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Gets an existing headless client for the given client uuid.
var headlessClient = plugins.headlessclient.getClient("clientID");
if (headlessClient != null && headlessClient.isValid()) {
	 headlessClient.queueMethod(null, "someRemoteMethod", null, callback);
}
```
### getOrCreateClient(clientId, solutionname, username, password, solutionOpenMethodArgs)

This will try to get a existing client by the given id if that client is already created for that specific solution;
it will create a headless client on the server that will open the given solution if it didn't exists yet.

If the client does exist but it is not loaded with that solution an exception will be thrown.

NOTE: in the developer this will only load the solution in debug mode when it is the current active solution or a module of the active solution;
you can load any solution from the workspace when you pass "nodebug" as last argument in the arguments list (it should still use the same resources project).
But then you won't be able to debug it, breakpoints won't hit.

**Parameters**\
[String](../../JSLib/String.md) clientId The client to lookup by id, if not found a new headless client is created with this id.\
[String](../../JSLib/String.md) solutionname The solution to load\
[String](../../JSLib/String.md) username The user name that is used to login to the solution\
[String](../../JSLib/String.md) password The password for the user\
[Array](../../JSLib/Array.md) solutionOpenMethodArgs The arguments that will be passed to the solution open method.

**Returns**\
[JSClient](./JSClient.md) An existing JSClient or the JSClient that is created.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Creates a headless client that will open the given solution.
var storedSolutionSpecificID = "aaaabbbbccccc1111";
var headlessClient = plugins.headlessclient.getOrCreateClient(storedSolutionSpecificID, "someSolution", "user", "pass", null);
if (headlessClient != null && headlessClient.isValid()) {
	var x = new Object();
	x.name = 'remote1';
	x.number = 10;
	headlessClient.queueMethod(null, "remoteMethod", [x], callback);
}
```

