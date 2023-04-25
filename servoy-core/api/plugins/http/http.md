#  http

## **Return Types**
[PatchRequest](./PatchRequest.md),[PostRequest](./PostRequest.md),[PutRequest](./PutRequest.md),[GetRequest](./GetRequest.md),[DeleteRequest](./DeleteRequest.md),[OptionsRequest](./OptionsRequest.md),[HeadRequest](./HeadRequest.md),[TraceRequest](./TraceRequest.md),[Cookie](./Cookie.md),[Response](./Response.md),[HttpClient](./HttpClient.md),[HttpClientConfig](./HttpClientConfig.md),[HTTP_STATUS](./HTTP_STATUS.md),

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [HttpClient](./HttpClient.md) | [createNewHttpClient()](http.md#createnewhttpclient)                   | Create an http client (like a web browser with session binding) usable todo multiple request/posts in same server session ..                                    |
| [HttpClient](./HttpClient.md) | [createNewHttpClient(config)](http.md#createnewhttpclient-config)                   | Create an http client (like a web browser with session binding) usable todo multiple request/posts in same server session..                                    |
| [HttpClientConfig](./HttpClientConfig.md) | [createNewHttpClientConfig()](http.md#createnewhttpclientconfig)                   | Create a http client config.                                    |
| [Array](../../JSLib/Array.md) | [getMediaData(url)](http.md#getmediadata-url)                   | Get media (binary data) such as images in a variable..                                    |
| [String](../../JSLib/String.md) | [getPageData(url)](http.md#getpagedata-url)                   | Get all page html in a variable, if this url is an https url that uses certificates unknown to Java then you have to use the HttpClient so that smart client users will get the unknown certificate dialog that they then can accept or you must make sure that those server certificates are stored in the cacerts of the java vm that is used (this is required for a web or headless client).                                    |

## Methods Details

### createNewHttpClient()

Create an http client (like a web browser with session binding) usable todo multiple request/posts in same server session
.
WARNING: Make sure you call client.close() on it after you used this client object to clean up resources.
Starting a HTTPClient is the same as starting an actual browser without UI!


**Returns**\
[HttpClient](./HttpClient.md) 


**Sample**

```javascript
var client = plugins.http.createNewHttpClient();
```
### createNewHttpClient(config)

Create an http client (like a web browser with session binding) usable todo multiple request/posts in same server session.

WARNING: Make sure you call client.close() on it after you used this client object to clean up resources.
Starting a HTTPClient is the same as starting an actual browser without UI!

**Parameters**\
[HttpClientConfig](./HttpClientConfig.md) config httpclient config

**Returns**\
[HttpClient](./HttpClient.md) 


**Sample**

```javascript
var client = plugins.http.createNewHttpClient(config);
```
### createNewHttpClientConfig()

Create a http client config


**Returns**\
[HttpClientConfig](./HttpClientConfig.md) 


**Sample**

```javascript
var config = plugins.http.createNewHttpClientConfig();
```
### getMediaData(url)

Get media (binary data) such as images in a variable. It also supports gzip-ed content.
If this url is an https url that uses certificates unknown to Java
then you have to use the HttpClient so that smart client users will get the unknown certificate dialog that they then can accept
or you must make sure that those server certificates are stored in the cacerts of the java vm that is used (this is required for a web or headless client)

**Parameters**\
[String](../../JSLib/String.md) url  ;

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
var image_byte_array = plugins.http.getMediaData('http://www.cnn.com/cnn.gif');
```
### getPageData(url)

Get all page html in a variable, if this url is an https url that uses certificates unknown to Java
then you have to use the HttpClient so that smart client users will get the unknown certificate dialog that they then can accept
or you must make sure that those server certificates are stored in the cacerts of the java vm that is used (this is required for a web or headless client)

**Parameters**\
[String](../../JSLib/String.md) url  ;

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
// get data using a default connection
var pageData = plugins.http.getPageData('http://www.cnn.com');
```

