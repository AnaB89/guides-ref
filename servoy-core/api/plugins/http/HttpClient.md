#  HttpClient


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [close()](HttpClient.md#close)                   | releases all resources that this client has, should be called after usage..                                    |
| [DeleteRequest](./DeleteRequest.md) | [createDeleteRequest(url)](HttpClient.md#createdeleterequest-url)                   | Creates a new delete request (a request to delete a resource on server)..                                    |
| [GetRequest](./GetRequest.md) | [createGetRequest(url)](HttpClient.md#creategetrequest-url)                   | Creates a new get request (retrieves whatever information is stored on specified url)..                                    |
| [HeadRequest](./HeadRequest.md) | [createHeadRequest(url)](HttpClient.md#createheadrequest-url)                   | Creates a new head request (similar to get request, must not contain body content)..                                    |
| [OptionsRequest](./OptionsRequest.md) | [createOptionsRequest(url)](HttpClient.md#createoptionsrequest-url)                   | Creates a new options request (a request for information about communication options)..                                    |
| [PatchRequest](./PatchRequest.md) | [createPatchRequest(url)](HttpClient.md#createpatchrequest-url)                   | Creates a new patch request (used for granular updates)..                                    |
| [PostRequest](./PostRequest.md) | [createPostRequest(url)](HttpClient.md#createpostrequest-url)                   | Create a new post request ( Origin server should accept/process the submitted data..                                    |
| [PutRequest](./PutRequest.md) | [createPutRequest(url)](HttpClient.md#createputrequest-url)                   | Creates a new put request (similar to post request, contains information to be submitted)..                                    |
| [TraceRequest](./TraceRequest.md) | [createTraceRequest(url)](HttpClient.md#createtracerequest-url)                   | Creates a new trace request (debug request, server will just echo back)..                                    |
| [Cookie](./Cookie.md) | [getCookie(cookieName)](HttpClient.md#getcookie-cookiename)                   | Get a cookie by name..                                    |
| [Array](../../JSLib/Array.md) | [getCookies()](HttpClient.md#getcookies)                   | Get all cookies from this client..                                    |
|void | [setClientProxyCredentials(userName, password)](HttpClient.md#setclientproxycredentials-username-password)                   | Set proxy credentials..                                    |
|void | [setClientProxyServer(hostname, port)](HttpClient.md#setclientproxyserver-hostname-port)                   | Set proxy server..                                    |
| [Boolean](../../JSLib/Boolean.md) | [setCookie(cookieName, cookieValue)](HttpClient.md#setcookie-cookiename-cookievalue)                   | Add cookie to the this client..                                    |
| [Boolean](../../JSLib/Boolean.md) | [setCookie(cookieName, cookieValue, domain)](HttpClient.md#setcookie-cookiename-cookievalue-domain)                   | Add cookie to the this client..                                    |
| [Boolean](../../JSLib/Boolean.md) | [setCookie(cookieName, cookieValue, domain, path)](HttpClient.md#setcookie-cookiename-cookievalue-domain-path)                   | Add cookie to the this client..                                    |
| [Boolean](../../JSLib/Boolean.md) | [setCookie(cookieName, cookieValue, domain, path, maxAge)](HttpClient.md#setcookie-cookiename-cookievalue-domain-path-maxage)                   | Add cookie to the this client..                                    |
| [Boolean](../../JSLib/Boolean.md) | [setCookie(cookieName, cookieValue, domain, path, maxAge, secure)](HttpClient.md#setcookie-cookiename-cookievalue-domain-path-maxage-secure)                   | Add cookie to the this client..                                    |
|void | [setTimeout(msTimeout)](HttpClient.md#settimeout-mstimeout)                   | Sets a timeout in milliseconds for retrieving of data (when 0 there is no timeout)..                                    |

## Methods Details

### close()

releases all resources that this client has, should be called after usage.


**Returns**\
void 


**Sample**

```javascript

```
### createDeleteRequest(url)

Creates a new delete request (a request to delete a resource on server).

**Parameters**\
[String](../../JSLib/String.md) url  ;

**Returns**\
[DeleteRequest](./DeleteRequest.md) 


**Sample**

```javascript
var client = plugins.http.createNewHttpClient();
var request = client.createDeleteRequest('http://www.servoy.com/delete.me');
var response = request.executeRequest();
var httpCode = response.getStatusCode(); // httpCode 200 is ok"
var content = response.getResponseBody();
```
### createGetRequest(url)

Creates a new get request (retrieves whatever information is stored on specified url).
If this url is a https ssl encrypted url which certificates are not in the java certificate store.
(Like a self signed certificate or a none existing root certificate)
Then for a smart client a dialog will be given, to give the user the ability to accept this certificate for the next time.
For a Web or Headless client the system administrator does have to add that certificate (chain) to the java install on the server.
See http://wiki.servoy.com/display/tutorials/Import+a+%28Root%29+certificate+in+the+java+cacerts+file

**Parameters**\
[String](../../JSLib/String.md) url  ;

**Returns**\
[GetRequest](./GetRequest.md) 


**Sample**

```javascript
var client = plugins.http.createNewHttpClient();
var request = client.createGetRequest('http://www.servoy.com');
var response = request.executeRequest();
var httpCode = response.getStatusCode(); // httpCode 200 is ok"
var content = response.getResponseBody();
```
### createHeadRequest(url)

Creates a new head request (similar to get request, must not contain body content).

**Parameters**\
[String](../../JSLib/String.md) url  ;

**Returns**\
[HeadRequest](./HeadRequest.md) 


**Sample**

```javascript
var client = plugins.http.createNewHttpClient();
var request = client.createHeadRequest('http://www.servoy.com');
var response = request.executeRequest();
var httpCode = response.getStatusCode(); // httpCode 200 is ok
var header = response.getResponseHeaders('last-modified');
```
### createOptionsRequest(url)

Creates a new options request (a request for information about communication options).

**Parameters**\
[String](../../JSLib/String.md) url  ;

**Returns**\
[OptionsRequest](./OptionsRequest.md) 


**Sample**

```javascript
var client = plugins.http.createNewHttpClient();
var request = client.createOptionsRequest('http://www.servoy.com');
var methods = request.getAllowedMethods(request.executeRequest());
```
### createPatchRequest(url)

Creates a new patch request (used for granular updates).

**Parameters**\
[String](../../JSLib/String.md) url  ;

**Returns**\
[PatchRequest](./PatchRequest.md) 


**Sample**

```javascript
var client = plugins.http.createNewHttpClient();
var request = client.createPatchRequest('http://jakarta.apache.org');
request.setBodyContent('{"email": "newemail@newdomain.com"}','application/json');
var httpCode = request.executeRequest().getStatusCode() // httpCode 200 is ok
```
### createPostRequest(url)

Create a new post request ( Origin server should accept/process the submitted data.)
If this url is a https ssl encrypted url which certificates are not in the java certificate store.
(Like a self signed certificate or a none existing root certificate)
Then for a smart client a dialog will be given, to give the user the ability to accept this certificate for the next time.
For a Web or Headless client the system administrator does have to add that certificate (chain) to the java install on the server.
See http://wiki.servoy.com/display/tutorials/Import+a+%28Root%29+certificate+in+the+java+cacerts+file

**Parameters**\
[String](../../JSLib/String.md) url  ;

**Returns**\
[PostRequest](./PostRequest.md) 


**Sample**

```javascript
var client = plugins.http.createNewHttpClient();
var poster = client.createPostRequest('https://twitter.com/statuses/update.json');
poster.addParameter('status',globals.textToPost);
poster.addParameter('source','Test Source');
poster.setCharset('UTF-8');
var httpCode = poster.executeRequest(globals.twitterUserName, globals.twitterPassword).getStatusCode(); // httpCode 200 is ok
```
### createPutRequest(url)

Creates a new put request (similar to post request, contains information to be submitted).

**Parameters**\
[String](../../JSLib/String.md) url  ;

**Returns**\
[PutRequest](./PutRequest.md) 


**Sample**

```javascript
var client = plugins.http.createNewHttpClient();
var request = client.createPutRequest('http://jakarta.apache.org');
request.setFile('UploadMe.gif');
var httpCode = putRequest.executeRequest().getStatusCode() // httpCode 200 is ok
```
### createTraceRequest(url)

Creates a new trace request (debug request, server will just echo back).

**Parameters**\
[String](../../JSLib/String.md) url  ;

**Returns**\
[TraceRequest](./TraceRequest.md) 


**Sample**

```javascript
var client = plugins.http.createNewHttpClient();
var response = request.executeRequest();
var httpCode = response.getStatusCode(); // httpCode 200 is ok"
var content = response.getResponseBody();
```
### getCookie(cookieName)

Get a cookie by name.

**Parameters**\
[String](../../JSLib/String.md) cookieName  ;

**Returns**\
[Cookie](./Cookie.md) 


**Sample**

```javascript
var cookie = client.getCookie('JSESSIONID');
if (cookie != null)
{
	// do something
}
else
	client.setCookie('JSESSIONID', 'abc', 'localhost', '/', -1, false)
```
### getCookies()

Get all cookies from this client.


**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
var cookies = client.getHttpClientCookies()
```
### setClientProxyCredentials(userName, password)

Set proxy credentials.

**Parameters**\
[String](../../JSLib/String.md) userName  ;\
[String](../../JSLib/String.md) password  ;

**Returns**\
void 


**Sample**

```javascript
client.setClientProxyCredentials('my_proxy_username','my_proxy_password');
```
### setClientProxyServer(hostname, port)

Set proxy server.

**Parameters**\
[String](../../JSLib/String.md) hostname - proxy host // null value will clear proxyHost settings;\
[Number](../../JSLib/Number.md) port - proxy port //null value will clear proxyHost settings;

**Returns**\
void 


**Sample**

```javascript
client.setClientProxyServer('server',port);
```
### setCookie(cookieName, cookieValue)

Add cookie to the this client.

**Parameters**\
[String](../../JSLib/String.md) cookieName the name of the cookie\
[String](../../JSLib/String.md) cookieValue the value of the cookie

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var cookieSet = client.setCookie('JSESSIONID', 'abc', 'localhost', '/', -1, false)
if (cookieSet)
{
	//do something
}
```
### setCookie(cookieName, cookieValue, domain)

Add cookie to the this client.

**Parameters**\
[String](../../JSLib/String.md) cookieName the name of the cookie\
[String](../../JSLib/String.md) cookieValue the value of the cookie\
[String](../../JSLib/String.md) domain the domain

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var cookieSet = client.setCookie('JSESSIONID', 'abc', 'localhost', '/', -1, false)
if (cookieSet)
{
	//do something
}
```
### setCookie(cookieName, cookieValue, domain, path)

Add cookie to the this client.

**Parameters**\
[String](../../JSLib/String.md) cookieName the name of the cookie\
[String](../../JSLib/String.md) cookieValue the value of the cookie\
[String](../../JSLib/String.md) domain the domain\
[String](../../JSLib/String.md) path the path

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var cookieSet = client.setCookie('JSESSIONID', 'abc', 'localhost', '/', -1, false)
if (cookieSet)
{
	//do something
}
```
### setCookie(cookieName, cookieValue, domain, path, maxAge)

Add cookie to the this client.

**Parameters**\
[String](../../JSLib/String.md) cookieName the name of the cookie\
[String](../../JSLib/String.md) cookieValue the value of the cookie\
[String](../../JSLib/String.md) domain the domain\
[String](../../JSLib/String.md) path the path\
[Number](../../JSLib/Number.md) maxAge maximum age of cookie

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var cookieSet = client.setCookie('JSESSIONID', 'abc', 'localhost', '/', -1, false)
if (cookieSet)
{
	//do something
}
```
### setCookie(cookieName, cookieValue, domain, path, maxAge, secure)

Add cookie to the this client.

**Parameters**\
[String](../../JSLib/String.md) cookieName the name of the cookie\
[String](../../JSLib/String.md) cookieValue the value of the cookie\
[String](../../JSLib/String.md) domain the domain\
[String](../../JSLib/String.md) path the path\
[Number](../../JSLib/Number.md) maxAge maximum age of cookie\
[Boolean](../../JSLib/Boolean.md) secure true if it is a secure cookie, false otherwise

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var cookieSet = client.setCookie('JSESSIONID', 'abc', 'localhost', '/', -1, false)
if (cookieSet)
{
	//do something
}
```
### setTimeout(msTimeout)

Sets a timeout in milliseconds for retrieving of data (when 0 there is no timeout).

**Parameters**\
[Object](../../JSLib/Object.md) msTimeout  ;

**Returns**\
void 


**Sample**

```javascript
client.setTimeout(1000)
```

