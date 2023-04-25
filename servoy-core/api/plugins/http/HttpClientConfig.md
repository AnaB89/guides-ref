#  HttpClientConfig


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../../JSLib/Boolean.md) | [enableRedirects](HttpClientConfig.md#enableRedirects)                   | Sets whether client should follow redirects or you want to do it manually..                                    |
| [Boolean](../../JSLib/Boolean.md) | [forceHttp1](HttpClientConfig.md#forceHttp1)                   | Force the use of http1, use this if there are problems connecting to a server that does use http/2 but uses old cipher suites or if there are other problems like http/2 not setting the content length and the server still wants it..                                    |
| [Number](../../JSLib/Number.md) | [keepAliveDuration](HttpClientConfig.md#keepAliveDuration)                   | Gets/Sets keep alive duration in seconds for a connection, default is -1 (no duration specified)..                                    |
| [Number](../../JSLib/Number.md) | [maxIOThreadCount](HttpClientConfig.md#maxIOThreadCount)                   | Gets/Sets maximum number of input/output threads per client, default value is 2..                                    |
| [String](../../JSLib/String.md) | [protocol](HttpClientConfig.md#protocol)                   | Gets/Sets which TLS protocol to use, default value is TLS..                                    |
| [String](../../JSLib/String.md) | [userAgent](HttpClientConfig.md#userAgent)                   | Gets/Sets custom userAgent to use..                                    |

## Properties Details

### enableRedirects

Sets whether client should follow redirects or you want to do it manually. Default value is true.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var config = plugins.http.createNewHttpClientConfig();
config.enableRedirects = false;
var client = plugins.http.createNewHttpClient(config);
```
### forceHttp1

Force the use of http1, use this if there are problems connecting to a server that does use http/2 but uses old cipher suites
or if there are other problems like http/2 not setting the content length and the server still wants it.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var config = plugins.http.createNewHttpClientConfig();
config.maxIOThreadCount = 5;
var client = plugins.http.createNewHttpClient(config);
```
### keepAliveDuration

Gets/Sets keep alive duration in seconds for a connection, default is -1 (no duration specified).

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var config = plugins.http.createNewHttpClientConfig();
config.keepAliveDuration = 5;
var client = plugins.http.createNewHttpClient(config);
```
### maxIOThreadCount

Gets/Sets maximum number of input/output threads per client, default value is 2.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var config = plugins.http.createNewHttpClientConfig();
config.maxIOThreadCount = 5;
var client = plugins.http.createNewHttpClient(config);
```
### protocol

Gets/Sets which TLS protocol to use, default value is TLS.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var config = plugins.http.createNewHttpClientConfig();
config.protocol = "TLSv1.2";
var client = plugins.http.createNewHttpClient(config);
```
### userAgent

Gets/Sets custom userAgent to use.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var config = plugins.http.createNewHttpClientConfig();
config.userAgent = "Mozilla/5.0 Firefox/26.0";
var client = plugins.http.createNewHttpClient(config);
```

