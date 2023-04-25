#  CustomApiBuilder


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [CustomApiBuilder](../../CustomApiBuilder.md) | [withAccessTokenExtractor(accessTokenExtractor)](CustomApiBuilder.md#withaccesstokenextractor-accesstokenextractor)                   | Configures the api with a token extractor which parses the concrete type of token from the response string..                                    |
| [CustomApiBuilder](../../CustomApiBuilder.md) | [withAccessTokenMethod(tokenRequestMethod)](CustomApiBuilder.md#withaccesstokenmethod-tokenrequestmethod)                   | The request method used for the access token endpoint (defaults to POST)..                                    |
| [CustomApiBuilder](../../CustomApiBuilder.md) | [withClientAuthentication(clientAuthentication)](CustomApiBuilder.md#withclientauthentication-clientauthentication)                   | Configures the api with a client authentication method which specifies how the client credentials are sent..                                    |
| [CustomApiBuilder](../../CustomApiBuilder.md) | [withRefreshTokenEndpoint(refreshTokenEndpoint)](CustomApiBuilder.md#withrefreshtokenendpoint-refreshtokenendpoint)                   | Configure the api with the URL that receives the refresh token requests..                                    |
| [CustomApiBuilder](../../CustomApiBuilder.md) | [withRevokeTokenEndpoint(revokeTokenEndpoint)](CustomApiBuilder.md#withrevoketokenendpoint-revoketokenendpoint)                   | Configure the api with the URL that receives the revoke token requests..                                    |

## Methods Details

### withAccessTokenExtractor(accessTokenExtractor)

Configures the api with a token extractor which parses the concrete type of token from the response string.

**Parameters**\
[String](../../JSLib/String.md) accessTokenExtractor see plugins.oauth.OAuthTokenExtractors

**Returns**\
[CustomApiBuilder](../../CustomApiBuilder.md) the api builder for method chaining


**Sample**

```javascript

```
### withAccessTokenMethod(tokenRequestMethod)

The request method used for the access token endpoint (defaults to POST).

**Parameters**\
[String](../../JSLib/String.md) tokenRequestMethod can be 'post' or 'get'

**Returns**\
[CustomApiBuilder](../../CustomApiBuilder.md) the api builder for method chaining


**Sample**

```javascript

```
### withClientAuthentication(clientAuthentication)

Configures the api with a client authentication method which specifies how the client credentials are sent.
They can be sent as basic Auth header or in the request body.

**Parameters**\
[String](../../JSLib/String.md) clientAuthentication see plugins.oauth.ClientAuthentication

**Returns**\
[CustomApiBuilder](../../CustomApiBuilder.md) the api builder for method chaining


**Sample**

```javascript

```
### withRefreshTokenEndpoint(refreshTokenEndpoint)

Configure the api with the URL that receives the refresh token requests.

**Parameters**\
[String](../../JSLib/String.md) refreshTokenEndpoint  ;

**Returns**\
[CustomApiBuilder](../../CustomApiBuilder.md) the api builder for method chaining


**Sample**

```javascript

```
### withRevokeTokenEndpoint(revokeTokenEndpoint)

Configure the api with the URL that receives the revoke token requests.

**Parameters**\
[String](../../JSLib/String.md) revokeTokenEndpoint  ;

**Returns**\
[CustomApiBuilder](../../CustomApiBuilder.md) the api builder for method chaining


**Sample**

```javascript

```

