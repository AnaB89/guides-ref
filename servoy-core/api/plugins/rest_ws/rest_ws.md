#  rest_ws


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [WsCookie](../../WsCookie.md) | [createCookie(name, value)](rest_ws.md#createcookie-name-value)                   | Create a http cookie..                                    |
| [WsRequest](../../WsRequest.md) | [getRequest()](rest_ws.md#getrequest)                   | Get the currently running REST-WS request..                                    |
| [WsResponse](../../WsResponse.md) | [getResponse()](rest_ws.md#getresponse)                   | Get the response for the currently running REST-WS request..                                    |
| [Boolean](../../JSLib/Boolean.md) | [isRunningRequest()](rest_ws.md#isrunningrequest)                   | Check whether the client is currently running a REST-WS request..                                    |
|void | [sendResponseUserPropertiesHeaders(send)](rest_ws.md#sendresponseuserpropertiesheaders-send)                   | Allow or block sending the user properties as response header values..                                    |

## Methods Details

### createCookie(name, value)

Create a http cookie.
The cookie name and value allows only a sequence of non-special, non-white space characters, see
the cookie spec https://tools.ietf.org/html/rfc2965

**Parameters**\
[String](../../JSLib/String.md) name The name of the cookie\
[String](../../JSLib/String.md) value The value of the cookie

**Returns**\
[WsCookie](../../WsCookie.md) 


**Sample**

```javascript
var cookie = plugins.rest_ws.createCookie('chocolate', 'chip');
var response = plugins.rest_ws.getResponse();
response.addCookie(cookie);
```
### getRequest()

Get the currently running REST-WS request.
 If the client is not currently running in REST-WS, an exception is thrown.


**Returns**\
[WsRequest](../../WsRequest.md) 


**Sample**

```javascript

```
### getResponse()

Get the response for the currently running REST-WS request.
If the client is not currently running in REST-WS, an exception is thrown.


**Returns**\
[WsResponse](../../WsResponse.md) 


**Sample**

```javascript
var response = plugins.rest_ws.getResponse();
resp.setHeader("My-Custom-Header", "42");
```
### isRunningRequest()

Check whether the client is currently running a REST-WS request.
 If false, the rest-ws client-plugin features are not available.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript

```
### sendResponseUserPropertiesHeaders(send)

Allow or block sending the user properties as response header values.
By default the response headers contain the user properties.

**Parameters**\
[Boolean](../../JSLib/Boolean.md) send  ;

**Returns**\
void 


**Sample**

```javascript

```

