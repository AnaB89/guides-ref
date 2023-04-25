#  OptionsRequest


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../../JSLib/Boolean.md) | [addHeader(headerName, value)](OptionsRequest.md#addheader-headername-value)                   | Add a header to the request..                                    |
|void | [executeAsyncRequest(username, password, workstation, domain, successCallbackMethod, errorCallbackMethod)](OptionsRequest.md#executeasyncrequest-username-password-workstation-domain-successcallbackmethod-errorcallbackmethod)                   | Execute the request method asynchronous..                                    |
|void | [executeAsyncRequest(username, password, workstation, domain, successCallbackMethod, errorCallbackMethod, callbackExtraArgs)](OptionsRequest.md#executeasyncrequest-username-password-workstation-domain-successcallbackmethod-errorcallbackmethod-callbackextraargs)                   | Execute the request method asynchronous using windows authentication..                                    |
|void | [executeAsyncRequest(username, password, successCallbackMethod, errorCallbackMethod)](OptionsRequest.md#executeasyncrequest-username-password-successcallbackmethod-errorcallbackmethod)                   | Execute the request method asynchronous..                                    |
|void | [executeAsyncRequest(username, password, successCallbackMethod, errorCallbackMethod, callbackExtraArgs)](OptionsRequest.md#executeasyncrequest-username-password-successcallbackmethod-errorcallbackmethod-callbackextraargs)                   | Execute the request method asynchronous using windows authentication..                                    |
|void | [executeAsyncRequest(successCallbackMethod, errorCallbackMethod)](OptionsRequest.md#executeasyncrequest-successcallbackmethod-errorcallbackmethod)                   | Execute the request method asynchronous..                                    |
|void | [executeAsyncRequest(successCallbackMethod, errorCallbackMethod, callbackExtraArgs)](OptionsRequest.md#executeasyncrequest-successcallbackmethod-errorcallbackmethod-callbackextraargs)                   | Execute the request method asynchronous using windows authentication..                                    |
| [Response](./Response.md) | [executeRequest()](OptionsRequest.md#executerequest)                   | Execute the request method..                                    |
| [Response](./Response.md) | [executeRequest(userName, password)](OptionsRequest.md#executerequest-username-password)                   | Execute the request method..                                    |
| [Response](./Response.md) | [executeRequest(userName, password, workstation, domain)](OptionsRequest.md#executerequest-username-password-workstation-domain)                   | Execute a request method using windows authentication..                                    |
| [Array](../../JSLib/Array.md) | [getAllowedMethods(res)](OptionsRequest.md#getallowedmethods-res)                   | Returns the supported HTTP Request operations as a String Array.                                    |
|void | [usePreemptiveAuthentication(b)](OptionsRequest.md#usepreemptiveauthentication-b)                   | Whatever to use preemptive authentication (sending the credentials in the header, avoiding the server request to the client - useful when uploading files, as some http servers would cancel the first request from the client, if too big, as the authentication request to the client was not yet sent).                                    |

## Methods Details

### addHeader(headerName, value)

Add a header to the request.

**Parameters**\
[String](../../JSLib/String.md) headerName  ;\
[String](../../JSLib/String.md) value  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
method.addHeader('Content-type','text/xml; charset=ISO-8859-1')
```
### executeAsyncRequest(username, password, workstation, domain, successCallbackMethod, errorCallbackMethod)

Execute the request method asynchronous. Success callback method will be called when response is received.
Response is sent as parameter in callback.
This Response can be a response with a different status code then just 200, it could also be 500, which is still a valid response from the server, this won't go into the error callback.
So you need to test the Reponse.getStatusCode() for that to know if everything did go OK.
If no response is received (request errors out), the errorCallbackMethod is called with exception message as parameter.

**Parameters**\
[String](../../JSLib/String.md) username the user name\
[String](../../JSLib/String.md) password the password\
[String](../../JSLib/String.md) workstation The workstation the authentication request is originating from.\
[String](../../JSLib/String.md) domain The domain to authenticate within.\
[Function](../../JSLib/Function.md) successCallbackMethod callbackMethod to be called after response is received\
[Function](../../JSLib/Function.md) errorCallbackMethod callbackMethod to be called if request errors out

**Returns**\
void 


**Sample**

```javascript
method.executeAsyncRequest('username','password','mycomputername','domain',globals.successCallback,globals.errorCallback)
```
### executeAsyncRequest(username, password, workstation, domain, successCallbackMethod, errorCallbackMethod, callbackExtraArgs)

Execute the request method asynchronous using windows authentication.
Success callback method will be called when response is received. Response is sent as parameter in callback followed by any 'callbackExtraArgs' that were given.
This Response can be a response with a different status code then just 200, it could also be 500, which is still a valid response from the server, this won't go into the error callback.
So you need to test the Reponse.getStatusCode() for that to know if everything did go OK.
If no response is received (request errors out, network errors), the errorCallbackMethod is called with exception message as parameter followed by any 'callbackExtraArgs' that were given.

**Parameters**\
[String](../../JSLib/String.md) username the user name\
[String](../../JSLib/String.md) password the password\
[String](../../JSLib/String.md) workstation The workstation the authentication request is originating from.\
[String](../../JSLib/String.md) domain The domain to authenticate within.\
[Function](../../JSLib/Function.md) successCallbackMethod callbackMethod to be called after response is received\
[Function](../../JSLib/Function.md) errorCallbackMethod callbackMethod to be called if request errors out\
[Array](../../JSLib/Array.md) callbackExtraArgs extra arguments that will be passed to the callback methods; can be used to identify from which request the response arrived when
using the same callback method for multiple requests. Please use only simple JSON arguments (primitive types or array/objects of primitive types)

**Returns**\
void 


**Sample**

```javascript
method.executeAsyncRequest('username','password','mycomputername','domain',globals.successCallback,globals.errorCallback, [callIDInt])
```
### executeAsyncRequest(username, password, successCallbackMethod, errorCallbackMethod)

Execute the request method asynchronous. Success callback method will be called when response is received.
Response is sent as parameter in callback.
This Response can be a response with a different status code then just 200, it could also be 500, which is still a valid response from the server, this won't go into the error callback.
So you need to test the Reponse.getStatusCode() for that to know if everything did go OK.
If no response is received (request errors out), the errorCallbackMethod is called with exception message as parameter.

**Parameters**\
[String](../../JSLib/String.md) username the user name\
[String](../../JSLib/String.md) password the password\
[Function](../../JSLib/Function.md) successCallbackMethod callbackMethod to be called after response is received\
[Function](../../JSLib/Function.md) errorCallbackMethod callbackMethod to be called if request errors out

**Returns**\
void 


**Sample**

```javascript
method.executeAsyncRequest(globals.successCallback,globals.errorCallback)
```
### executeAsyncRequest(username, password, successCallbackMethod, errorCallbackMethod, callbackExtraArgs)

Execute the request method asynchronous using windows authentication.
Success callback method will be called when response is received. Response is sent as parameter in callback followed by any 'callbackExtraArgs' that were given.
This Response can be a response with a different status code then just 200, it could also be 500, which is still a valid response from the server, this won't go into the error callback.
So you need to test the Reponse.getStatusCode() for that to know if everything did go OK.
If no response is received (request errors out, network errors), the errorCallbackMethod is called with exception message as parameter followed by any 'callbackExtraArgs' that were given.

**Parameters**\
[String](../../JSLib/String.md) username the user name\
[String](../../JSLib/String.md) password the password\
[Function](../../JSLib/Function.md) successCallbackMethod callbackMethod to be called after response is received\
[Function](../../JSLib/Function.md) errorCallbackMethod callbackMethod to be called if request errors out\
[Array](../../JSLib/Array.md) callbackExtraArgs extra arguments that will be passed to the callback methods; can be used to identify from which request the response arrived when
using the same callback method for multiple requests. Please use only simple JSON arguments (primitive types or array/objects of primitive types)

**Returns**\
void 


**Sample**

```javascript
method.executeAsyncRequest(globals.successCallback,globals.errorCallback, [callIDInt])
```
### executeAsyncRequest(successCallbackMethod, errorCallbackMethod)

Execute the request method asynchronous. Success callback method will be called when response is received.
Response is sent as parameter in callback.
This Response can be a response with a different status code then just 200, it could also be 500, which is still a valid response from the server, this won't go into the error callback.
So you need to test the Reponse.getStatusCode() for that to know if everything did go OK.
If no response is received (request errors out), the errorCallbackMethod is called with exception message as parameter.

**Parameters**\
[Function](../../JSLib/Function.md) successCallbackMethod callbackMethod to be called after response is received\
[Function](../../JSLib/Function.md) errorCallbackMethod callbackMethod to be called if request errors out

**Returns**\
void 


**Sample**

```javascript
method.executeAsyncRequest(globals.successCallback,globals.errorCallback)
```
### executeAsyncRequest(successCallbackMethod, errorCallbackMethod, callbackExtraArgs)

Execute the request method asynchronous using windows authentication.
Success callback method will be called when response is received. Response is sent as parameter in callback followed by any 'callbackExtraArgs' that were given.
This Response can be a response with a different status code then just 200, it could also be 500, which is still a valid response from the server, this won't go into the error callback.
So you need to test the Reponse.getStatusCode() for that to know if everything did go OK.
If no response is received (request errors out, network errors), the errorCallbackMethod is called with exception message as parameter followed by any 'callbackExtraArgs' that were given.

**Parameters**\
[Function](../../JSLib/Function.md) successCallbackMethod callbackMethod to be called after response is received\
[Function](../../JSLib/Function.md) errorCallbackMethod callbackMethod to be called if request errors out\
[Array](../../JSLib/Array.md) callbackExtraArgs extra arguments that will be passed to the callback methods; can be used to identify from which request the response arrived when
using the same callback method for multiple requests. Please use only simple JSON arguments (primitive types or array/objects of primitive types)

**Returns**\
void 


**Sample**

```javascript
method.executeAsyncRequest(globals.successCallback,globals.errorCallback, [callIDInt])
```
### executeRequest()

Execute the request method.


**Returns**\
[Response](./Response.md) 


**Sample**

```javascript
var response = method.executeRequest()

To be able to reuse the client, the response must be
closed if the content is not read via getResponseBody
 or getMediaData:

response.close()
```
### executeRequest(userName, password)

Execute the request method.

**Parameters**\
[String](../../JSLib/String.md) userName the user name\
[String](../../JSLib/String.md) password the password

**Returns**\
[Response](./Response.md) 


**Sample**

```javascript
var response = method.executeRequest()

To be able to reuse the client, the response must be
closed if the content is not read via getResponseBody
 or getMediaData:

response.close()
```
### executeRequest(userName, password, workstation, domain)

Execute a request method using windows authentication.

**Parameters**\
[String](../../JSLib/String.md) userName the user name\
[String](../../JSLib/String.md) password the password\
[String](../../JSLib/String.md) workstation The workstation the authentication request is originating from.\
[String](../../JSLib/String.md) domain The domain to authenticate within.

**Returns**\
[Response](./Response.md) 


**Sample**

```javascript
var response = method.executeRequest('username','password','mycomputername','domain');
```
### getAllowedMethods(res)

Returns the supported HTTP Request operations as a String Array

**Parameters**\
[Response](./Response.md) res The response request to get the allowed methods from.

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
var supportedOperations = request.getAllowedMethods()
application.output(supportedOperations.join(','));
```
### usePreemptiveAuthentication(b)

Whatever to use preemptive authentication (sending the credentials in the header, avoiding the server request to
the client - useful when uploading files, as some http servers would cancel the first request from the client, if too big,
as the authentication request to the client was not yet sent)

**Parameters**\
[Boolean](../../JSLib/Boolean.md) b  ;

**Returns**\
void 


**Sample**

```javascript

```

