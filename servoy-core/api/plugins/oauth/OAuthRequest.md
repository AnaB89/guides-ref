#  OAuthRequest


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [addBodyParameter(key, value)](OAuthRequest.md#addbodyparameter-key-value)                   | Add a body parameter to the request..                                    |
|void | [addHeader(header, value)](OAuthRequest.md#addheader-header-value)                   | Allows setting a header on the request object..                                    |
|void | [addOAuthParameter(key, value)](OAuthRequest.md#addoauthparameter-key-value)                   | Add an OAuth parameter, like 'scope', 'realm' or with the 'oauth_' prefix.                                    |
|void | [addParameter(key, value)](OAuthRequest.md#addparameter-key-value)                   | Add a body or a query string parameter, depending on the request type..                                    |
|void | [addQuerystringParameter(key, value)](OAuthRequest.md#addquerystringparameter-key-value)                   | Add a query string parameter..                                    |
| [OAuthResponse](../../OAuthResponse.md) | [execute()](OAuthRequest.md#execute)                   | Execute a request that was created with the OAuth service..                                    |
|void | [setPayload(data)](OAuthRequest.md#setpayload-data)                   | Set body payload..                                    |

## Methods Details

### addBodyParameter(key, value)

Add a body parameter to the request.

**Parameters**\
[String](../../JSLib/String.md) key the parameter name\
[String](../../JSLib/String.md) value the parameter value

**Returns**\
void 


**Sample**

```javascript
var postRequest = service.createPostRequest("https://.....");
postRequest.addBodyParameter("param1", "value1");
```
### addHeader(header, value)

Allows setting a header on the request object.

**Parameters**\
[String](../../JSLib/String.md) header the header name\
[String](../../JSLib/String.md) value the header value

**Returns**\
void 


**Sample**

```javascript
var getRequest = service.createGetRequest("https://api.linkedin.com/v2/me");
getRequest.addHeader("Accept", "application/json");
```
### addOAuthParameter(key, value)

Add an OAuth parameter, like 'scope', 'realm' or with the 'oauth_' prefix

**Parameters**\
[String](../../JSLib/String.md) key one of 'scope', 'realm' or starting with 'oauth_'\
[String](../../JSLib/String.md) value the oauth parameter value

**Returns**\
void 


**Sample**

```javascript

```
### addParameter(key, value)

Add a body or a query string parameter, depending on the request type.
If the request allows a body (POST, PUT, DELETE, PATCH) then it adds it as a body parameter.
Otherwise it is added as a query string parameter.

**Parameters**\
[String](../../JSLib/String.md) key the parameter name\
[String](../../JSLib/String.md) value the parameter value

**Returns**\
void 


**Sample**

```javascript

```
### addQuerystringParameter(key, value)

Add a query string parameter.

**Parameters**\
[String](../../JSLib/String.md) key the query string parameter name\
[String](../../JSLib/String.md) value the parameter value

**Returns**\
void 


**Sample**

```javascript

```
### execute()

Execute a request that was created with the OAuth service.


**Returns**\
[OAuthResponse](../../OAuthResponse.md) the OAuthResponse object


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
### setPayload(data)

Set body payload.

**Parameters**\
[String](../../JSLib/String.md) data  ;

**Returns**\
void 


**Sample**

```javascript
var putRequest = service.createPutRequest("https://graph.microsoft.com/v1.0/me/drive/root:/FolderAA/FileBB.txt:/content");
putRequest.addHeader("Content-Type", "text/plain");
putRequest.setPayload("ABC");
```

