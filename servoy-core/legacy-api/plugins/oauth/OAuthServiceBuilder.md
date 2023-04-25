#  OAuthServiceBuilder

## **Supported Clients**

    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [OAuthServiceBuilder](../../OAuthServiceBuilder.md) | [additionalParameters(params)](OAuthServiceBuilder.md#additionalparameters-params)                   | Add some more parameters to the authorization url..                                    |
| [OAuthService](../../OAuthService.md) | [build(api)](OAuthServiceBuilder.md#build-api)                   | Creates an OAuth service that can be used to obtain an access token and access protected data..                                    |
| [OAuthService](../../OAuthService.md) | [build(api)](OAuthServiceBuilder.md#build-api)                   | Creates an OAuth service that can be used to obtain an access token and access protected data..                                    |
| [OAuthServiceBuilder](../../OAuthServiceBuilder.md) | [callback(callback, timeout)](OAuthServiceBuilder.md#callback-callback-timeout)                   | Configure the service with a callback function to be executed when the service is ready to use..                                    |
| [OAuthServiceBuilder](../../OAuthServiceBuilder.md) | [clientSecret(clientSecret)](OAuthServiceBuilder.md#clientsecret-clientsecret)                   | Set the client secret of the application..                                    |
| [OAuthServiceBuilder](../../OAuthServiceBuilder.md) | [deeplink(deeplink)](OAuthServiceBuilder.md#deeplink-deeplink)                   | OPTIONAL This is a way to override the default deeplink method name, which is 'deeplink_svy_oauth'..                                    |
| [OAuthServiceBuilder](../../OAuthServiceBuilder.md) | [defaultScope(scope)](OAuthServiceBuilder.md#defaultscope-scope)                   | Request always the same scope..                                    |
| [OAuthServiceBuilder](../../OAuthServiceBuilder.md) | [domain(domain)](OAuthServiceBuilder.md#domain-domain)                   | Set the domain if the API supports it (e..                                    |
| [String](../../JSLib/String.md) | [getUsedAuthorizationURL(api)](OAuthServiceBuilder.md#getusedauthorizationurl-api)                   | Get the authorization url..                                    |
| [String](../../JSLib/String.md) | [getUsedAuthorizationURL(api)](OAuthServiceBuilder.md#getusedauthorizationurl-api)                   | Get the authorization url..                                    |
| [OAuthServiceBuilder](../../OAuthServiceBuilder.md) | [responseMode(mode)](OAuthServiceBuilder.md#responsemode-mode)                   | Configure if the code/tokens are going to be received as a query or as a url fragment..                                    |
| [OAuthServiceBuilder](../../OAuthServiceBuilder.md) | [responseType(response_type)](OAuthServiceBuilder.md#responsetype-response_type)                   | Configures the OAuth flow..                                    |
| [OAuthServiceBuilder](../../OAuthServiceBuilder.md) | [scope(scope)](OAuthServiceBuilder.md#scope-scope)                   | Request any unique scope per each access token request..                                    |
| [OAuthServiceBuilder](../../OAuthServiceBuilder.md) | [state(state)](OAuthServiceBuilder.md#state-state)                   | Configures the anti forgery session state..                                    |
| [OAuthServiceBuilder](../../OAuthServiceBuilder.md) | [tenant(tenant)](OAuthServiceBuilder.md#tenant-tenant)                   | Set the tenant identifiers/organization if the API supports it (e..                                    |
| [OAuthServiceBuilder](../../OAuthServiceBuilder.md) | [withPKCE()](OAuthServiceBuilder.md#withpkce)                   | Configures the service with Proof Key for Code Exchange, which prevents authorization code interception attacks..                                    |

## Methods Details

### additionalParameters(params)

Add some more parameters to the authorization url.

**Parameters**\
[Object](../../JSLib/Object.md) params a json containing the parameters and their values
		e.g. {'param1': 'value1', 'param2': 'value2'}

**Returns**\
[OAuthServiceBuilder](../../OAuthServiceBuilder.md) the service builder for method chaining

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### build(api)

Creates an OAuth service that can be used to obtain an access token and access protected data.

**Parameters**\
[CustomApiBuilder](../../CustomApiBuilder.md) api a custom api, see plugins.oauth.customApi

**Returns**\
[OAuthService](../../OAuthService.md) an OAuthService object that can be used to make signed requests to the api

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### build(api)

Creates an OAuth service that can be used to obtain an access token and access protected data.

**Parameters**\
[String](../../JSLib/String.md) api an OAuth provider id, see plugins.oauth.OAuthProviders

**Returns**\
[OAuthService](../../OAuthService.md) an OAuthService object that can be used to make signed requests to the api

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### callback(callback, timeout)

Configure the service with a callback function to be executed when the service is ready to use.
After the access token is returned by the server, this callback function is executed.

**Parameters**\
[Function](../../JSLib/Function.md) callback a function in a scope or form\
[Number](../../JSLib/Number.md) timeout max number of seconds in which the callback method should be executed (with success or error message)
			Please note that the timeout should be enough for the user to login and accept permissions.

**Returns**\
[OAuthServiceBuilder](../../OAuthServiceBuilder.md) the service builder for method chaining

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### clientSecret(clientSecret)

Set the client secret of the application.

**Parameters**\
[String](../../JSLib/String.md) clientSecret a secret known only to the application and the authorization server

**Returns**\
[OAuthServiceBuilder](../../OAuthServiceBuilder.md) the service builder for method chaining

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### deeplink(deeplink)

OPTIONAL This is a way to override the default deeplink method name, which is 'deeplink_svy_oauth'.
The deeplink method is a global method that receives the code needed to obtain the access token from the OAuth provider.

NOTE: The deeplink method name is strongly related to the redirect url configured for the application.
If the OAuth provider (eg. Microsoft AD, Likedin) requires to configure a full redirect url then it should be of the form:
https://example.com/<solution_name>/m/<deeplinkmethod> - where <deeplinkmethod> is the name configured with the service builder
https://example.com/<solution_name>/m/deeplink_svy_oauth - if the deeplink method name was not overridden

If the deeplink method with the provided name does not exist in the solution,
then a default deeplink method is generated under the hood with the solution model.
If a global method with the provided name already exists in the solution, then it should set the access
token on the service and handle possible errors.

**Parameters**\
[String](../../JSLib/String.md) deeplink a global scope method name

**Returns**\
[OAuthServiceBuilder](../../OAuthServiceBuilder.md) the service builder for method chaining

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### defaultScope(scope)

Request always the same scope.
Scope is a mechanism in OAuth 2.0 to limit an application's access to a user's account.
An application can request one or more scopes, separated by space.
This information is then presented to the user in the consent screen, and the access token issued
to the application will be limited to the scopes granted.

**Parameters**\
[String](../../JSLib/String.md) scope the default scope

**Returns**\
[OAuthServiceBuilder](../../OAuthServiceBuilder.md) the service builder for method chaining

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### domain(domain)

Set the domain if the API supports it (e.g.Okta)

**Parameters**\
[String](../../JSLib/String.md) domain  ;

**Returns**\
[OAuthServiceBuilder](../../OAuthServiceBuilder.md) the service builder for method chaining

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### getUsedAuthorizationURL(api)

Get the authorization url. This is for DEBUGGING PURPOSES ONLY.

**Parameters**\
[CustomApiBuilder](../../CustomApiBuilder.md) api a custom api builder

**Returns**\
[String](../../JSLib/String.md) the used authorization url

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### getUsedAuthorizationURL(api)

Get the authorization url. This is for DEBUGGING PURPOSES ONLY.

**Parameters**\
[String](../../JSLib/String.md) api an OAuth provider id, see plugins.oauth.OAuthProviders

**Returns**\
[String](../../JSLib/String.md) the used authorization url

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### responseMode(mode)

Configure if the code/tokens are going to be received as a query or as a url fragment.
Will be ignored if the response type is token/id_token or if the oauth provider does not support it.

For the "fragment" response mode the redirect url configured for the oauth app needs to be of the following form
https://example.com/servoy-service/oauth/solutions/<solution_name>/m/<deeplinkmethod> - where <deeplinkmethod> is the name configured with the service builder

**Parameters**\
[String](../../JSLib/String.md) mode can be "query" or "fragment"

**Returns**\
[OAuthServiceBuilder](../../OAuthServiceBuilder.md) the service builder for method chaining

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### responseType(response_type)

Configures the OAuth flow. Defaults to "code" (authorization code flow) if not set.
Use response type "token" for the implicit grant flow.
Use response type "id_token" for OpenID Connect sign-in. In this case the response is a JWT token which can be used to verify the identity of a user.
OAuth providers may allow combinations of "code" "id_token" "token".

**Parameters**\
[String](../../JSLib/String.md) response_type one or a combination of "code" "id_token" "token"

**Returns**\
[OAuthServiceBuilder](../../OAuthServiceBuilder.md) the service builder for method chaining

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### scope(scope)

Request any unique scope per each access token request.
Scope is a mechanism in OAuth 2.0 to limit an application's access to a user's account.
An application can request one or more scopes, separated by space.
This information is then presented to the user in the consent screen, and the access token issued
to the application will be limited to the scopes granted.

**Parameters**\
[String](../../JSLib/String.md) scope one or multiple scopes separated by space

**Returns**\
[OAuthServiceBuilder](../../OAuthServiceBuilder.md) the service builder for method chaining

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### state(state)

Configures the anti forgery session state. This is required in some APIs (like Facebook's).

**Parameters**\
[String](../../JSLib/String.md) state  ;

**Returns**\
[OAuthServiceBuilder](../../OAuthServiceBuilder.md) the service builder for method chaining

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### tenant(tenant)

Set the tenant identifiers/organization if the API supports it (e.g.Microsoft AD)

**Parameters**\
[String](../../JSLib/String.md) tenant  ;

**Returns**\
[OAuthServiceBuilder](../../OAuthServiceBuilder.md) the service builder for method chaining

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### withPKCE()

Configures the service with Proof Key for Code Exchange, which prevents authorization code interception attacks.
See more at https://datatracker.ietf.org/doc/html/rfc7636.


**Returns**\
[OAuthServiceBuilder](../../OAuthServiceBuilder.md) the service builder for method chaining

**Supported Clients**\
NGClient

**Sample**

```javascript

```

