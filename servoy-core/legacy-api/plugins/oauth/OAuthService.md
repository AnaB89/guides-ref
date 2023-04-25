#  OAuthService

## **Supported Clients**

    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [OAuthRequest](../../OAuthRequest.md) | [createDeleteRequest(resourceURL)](OAuthService.md#createdeleterequest-resourceurl)                   | Create a DELETE request..                                    |
| [OAuthRequest](../../OAuthRequest.md) | [createGetRequest(resourceURL)](OAuthService.md#creategetrequest-resourceurl)                   | Create a GET request for a resource..                                    |
| [OAuthRequest](../../OAuthRequest.md) | [createPostRequest(resourceURL)](OAuthService.md#createpostrequest-resourceurl)                   | Create a POST request..                                    |
| [OAuthRequest](../../OAuthRequest.md) | [createPutRequest(resourceURL)](OAuthService.md#createputrequest-resourceurl)                   | Create a PUT request..                                    |
| [OAuthRequest](../../OAuthRequest.md) | [createRequest(requestType, resourceURL)](OAuthService.md#createrequest-requesttype-resourceurl)                   | Creates a JSOAuthRequest for with the enum of RequestType (GET, PUT, DELETE, etc) for a resource url..                                    |
| [OAuthResponse](../../OAuthResponse.md) | [executeGetRequest(resourceURL)](OAuthService.md#executegetrequest-resourceurl)                   | This is quick method by executing a GET request and returning right away the OAuthResponse So it would be the same as executeRequest(createRequest(RequestType..                                    |
| [OAuthResponse](../../OAuthResponse.md) | [executeRequest(request)](OAuthService.md#executerequest-request)                   | Method to execute requests that are made, and configured by  #createRequest(Verb,String).                                    |
| [Number](../../JSLib/Number.md) | [getAccessExpiresIn()](OAuthService.md#getaccessexpiresin)                   | Returns the number of seconds left until the access token expires..                                    |
| [String](../../JSLib/String.md) | [getAccessToken()](OAuthService.md#getaccesstoken)                   | Get the access token currently set on the service..                                    |
| [Number](../../JSLib/Number.md) | [getAccessTokenLifetime()](OAuthService.md#getaccesstokenlifetime)                   | Return the token lifetime in seconds..                                    |
| [String](../../JSLib/String.md) | [getAuthorizationURL()](OAuthService.md#getauthorizationurl)                   | .                                    |
| [String](../../JSLib/String.md) | [getAuthorizationURL(params)](OAuthService.md#getauthorizationurl-params)                   | Get the authorization url with some additional parameters..                                    |
| [String](../../JSLib/String.md) | [getIdToken()](OAuthService.md#getidtoken)                   | Obtain the Openid token if it is available..                                    |
| [String](../../JSLib/String.md) | [getRefreshToken()](OAuthService.md#getrefreshtoken)                   | Return the refresh token..                                    |
| [Boolean](../../JSLib/Boolean.md) | [isAccessTokenExpired()](OAuthService.md#isaccesstokenexpired)                   | Checks if the access token is expired..                                    |
| [String](../../JSLib/String.md) | [refreshToken()](OAuthService.md#refreshtoken)                   | Obtains a new access token if the OAuth api supports it..                                    |
|void | [revokeToken(token)](OAuthService.md#revoketoken-token)                   | Revoke the provided access token..                                    |
|void | [setAccessToken(code)](OAuthService.md#setaccesstoken-code)                   | Configure the oauth service with an access token using the scope that was initially set when creating the service..                                    |
|void | [setAccessToken(code, scope)](OAuthService.md#setaccesstoken-code-scope)                   | Configure the oauth service with an access token for the specified scope..                                    |

## Methods Details

### createDeleteRequest(resourceURL)

Create a DELETE request.

**Parameters**\
[String](../../JSLib/String.md) resourceURL the url of the resource to be deleted

**Returns**\
[OAuthRequest](../../OAuthRequest.md) the request object

**Supported Clients**\
NGClient

**Sample**

```javascript
var putRequest = service.createDeleteRequest("https://graph.microsoft.com/v1.0/me/drive/root:/FolderAA/FileBB.txt:/content");
var response = putRequest.execute();
if (response.getCode() == 204) {
		application.output("File was deleted "+response.getBody());
	}
else
{
		application.output('http status '+response.getCode());
		application.output("File could not be deleted: "+response.getBody())
}
```
### createGetRequest(resourceURL)

Create a GET request for a resource.

**Parameters**\
[String](../../JSLib/String.md) resourceURL the url of the resource which you want to get

**Returns**\
[OAuthRequest](../../OAuthRequest.md) the request object

**Supported Clients**\
NGClient

**Sample**

```javascript
var getRequest = service.createGetRequest("https://api.linkedin.com/v2/me");
getRequest.addHeader("Accept", "application/json");

var response = getRequest.execute();
if (response.getCode() == 200) {
		var json = response.getAsJSON();
		application.output("Name is "+json.firstName);
	}
else
{
		application.output("ERROR http status "+response.getCode());
		application.output(response.getBody())
}
```
### createPostRequest(resourceURL)

Create a POST request.

**Parameters**\
[String](../../JSLib/String.md) resourceURL the url where the enclosed entity will be stored

**Returns**\
[OAuthRequest](../../OAuthRequest.md) the request object

**Supported Clients**\
NGClient

**Sample**

```javascript
var postRequest = service.createPostRequest("https://.....");
postRequest.addHeader("Content-Type", "text/plain");
postRequest.addBodyParameter("param1", "value1");
var response = postRequest.execute();
```
### createPutRequest(resourceURL)

Create a PUT request.

**Parameters**\
[String](../../JSLib/String.md) resourceURL the url where the enclosed entity will be stored

**Returns**\
[OAuthRequest](../../OAuthRequest.md) the request object

**Supported Clients**\
NGClient

**Sample**

```javascript
var putRequest = service.createPutRequest("https://graph.microsoft.com/v1.0/me/drive/root:/FolderAA/FileBB.txt:/content");
putRequest.addHeader("Content-Type", "text/plain");
putRequest.setPayload("ABC");
var response = putRequest.execute();
if (response.getCode() == 201) {
		application.output("New file was created "+response.getBody());
	}
else
{
		application.output("ERROR http status "+response.getCode());
		application.output("File could not be created: "+response.getBody())
}
```
### createRequest(requestType, resourceURL)

Creates a JSOAuthRequest for with the enum of RequestType (GET, PUT, DELETE, etc) for a resource url.

**Parameters**\
[enum](../../enum.md) requestType one of the types of plugins.oauth.RequestType\
[String](../../JSLib/String.md) resourceURL the url of the resource you want to access

**Returns**\
[OAuthRequest](../../OAuthRequest.md) a JSOAuthRequest object

**Supported Clients**\
NGClient

**Sample**

```javascript
var request = service.createRequest(plugins.oauth.RequestType.GET, "https://api.linkedin.com/v2/me");
request.addHeader("Accept", "application/json");

var response = request.execute();
if (response.getCode() == 200) {
		var json = response.getAsJSON();
		application.output("Name is "+json.firstName);
	}
else
{
		application.output("ERROR http status "+response.getCode());
		application.output(response.getBody())
}
```
### executeGetRequest(resourceURL)

This is quick method by executing a GET request and returning right away the OAuthResponse
So it would be the same as executeRequest(createRequest(RequestType.GET, url))

**Parameters**\
[String](../../JSLib/String.md) resourceURL  ;

**Returns**\
[OAuthResponse](../../OAuthResponse.md) the OAuthResponse object

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### executeRequest(request)

Method to execute requests that are made, and configured by  #createRequest(Verb,String)

**Parameters**\
[OAuthRequest](../../OAuthRequest.md) request the JSOAuthRequest object that was created by #createRequest(Verb,String)

**Returns**\
[OAuthResponse](../../OAuthResponse.md) the OAuthResponse object

**Supported Clients**\
NGClient

**Sample**

```javascript
var request = service.createRequest(plugins.oauth.RequestType.GET, "https://api.linkedin.com/v2/me");
request.addHeader("Accept", "application/json");

var response = service.executeRequest(request);
if (response.getCode() == 200) {
		var json = response.getAsJSON();
		application.output("Name is "+json.firstName);
	}
else
{
		application.output("ERROR http status "+response.getCode());
		application.output(response.getBody())
}
```
### getAccessExpiresIn()

Returns the number of seconds left until the access token expires.


**Returns**\
[Number](../../JSLib/Number.md) seconds left untol the access token expires.

**Supported Clients**\
NGClient

**Sample**

```javascript
var seconds = service.getAccessExpiresIn();
 if (seconds < 60)
 {
 	application.output("The access token is going to expire in less than 1 minute! Use service.refreshToken() to get a new one");
 }
 else
 {
 	application.output("Make some requests");
 }
```
### getAccessToken()

Get the access token currently set on the service.


**Returns**\
[String](../../JSLib/String.md) the access token or null if it was not set

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### getAccessTokenLifetime()

Return the token lifetime in seconds.


**Returns**\
[Number](../../JSLib/Number.md) the token lifetime as it was retrieved by the OAuth provider with the access token

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### getAuthorizationURL()




**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### getAuthorizationURL(params)

Get the authorization url with some additional parameters.

**Parameters**\
[Object](../../JSLib/Object.md) params a json containing the parameters and their values
		e.g. {'param1': 'value1', 'param2': 'value2'}

**Returns**\
[String](../../JSLib/String.md) the authorization url with the provided parameters appended to the query string.

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### getIdToken()

Obtain the Openid token if it is available.


**Returns**\
[String](../../JSLib/String.md) the id token, or null if was not set on the service.

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### getRefreshToken()

Return the refresh token.


**Returns**\
[String](../../JSLib/String.md) the refresh token or null if it is not present

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### isAccessTokenExpired()

Checks if the access token is expired. Returns false if the access token expire information is not set.


**Returns**\
[Boolean](../../JSLib/Boolean.md) true if the access token is expired, false otherwise

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### refreshToken()

Obtains a new access token if the OAuth api supports it.


**Returns**\
[String](../../JSLib/String.md) The new access token issued by the authorization server

**Supported Clients**\
NGClient

**Sample**

```javascript
accessToken = service.refreshToken();
```
### revokeToken(token)

Revoke the provided access token.

**Parameters**\
[String](../../JSLib/String.md) token to revoke

**Returns**\
void 

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### setAccessToken(code)

Configure the oauth service with an access token using the scope that was initially set when creating the service.

**Parameters**\
[String](../../JSLib/String.md) code the authorization code used to request and access token

**Returns**\
void 

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### setAccessToken(code, scope)

Configure the oauth service with an access token for the specified scope.

**Parameters**\
[String](../../JSLib/String.md) code the authorization code used to request an access token\
[String](../../JSLib/String.md) scope the scope for which to obtain an access token

**Returns**\
void 

**Supported Clients**\
NGClient

**Sample**

```javascript

```

