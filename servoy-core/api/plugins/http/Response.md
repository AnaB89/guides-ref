#  Response


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../../JSLib/String.md) | [getCharset()](Response.md#getcharset)                   | Get the charset of the response body..                                    |
| [String](../../JSLib/String.md) | [getException()](Response.md#getexception)                   | Getter for the exception message..                                    |
| [Array](../../JSLib/Array.md) | [getMediaData()](Response.md#getmediadata)                   | Get the content of response as binary data..                                    |
| [String](../../JSLib/String.md) | [getResponseBody()](Response.md#getresponsebody)                   | Get the content of the response as String..                                    |
| [Object](../../JSLib/Object.md) | [getResponseHeaders()](Response.md#getresponseheaders)                   | Gets the headers of the response as name/value arrays..                                    |
| [Object](../../JSLib/Object.md) | [getResponseHeaders(headerName)](Response.md#getresponseheaders-headername)                   | Gets the headers of the response as name/value arrays..                                    |
| [Number](../../JSLib/Number.md) | [getStatusCode()](Response.md#getstatuscode)                   | Gets the status code of the response, the list of the possible values is in HTTP_STATUS constants..                                    |
| [String](../../JSLib/String.md) | [getStatusReasonPhrase()](Response.md#getstatusreasonphrase)                   | Gets the status code's reason phrase..                                    |

## Methods Details

### getCharset()

Get the charset of the response body.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var charset = response.getCharset();
```
### getException()

Getter for the exception message.


**Returns**\
[String](../../JSLib/String.md) the exception message


**Sample**

```javascript
var exception = response.getException();
```
### getMediaData()

Get the content of response as binary data. It also supports gzip-ed content.


**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
var mediaData = response.getMediaData();
```
### getResponseBody()

Get the content of the response as String.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var pageData = response.getResponseBody();
```
### getResponseHeaders()

Gets the headers of the response as name/value arrays.


**Returns**\
[Object](../../JSLib/Object.md) 


**Sample**

```javascript
var allHeaders = response.getResponseHeaders();
var header;

for (header in allHeaders) application.output(header + ': ' + allHeaders[header]);
```
### getResponseHeaders(headerName)

Gets the headers of the response as name/value arrays.

**Parameters**\
[String](../../JSLib/String.md) headerName  ;

**Returns**\
[Object](../../JSLib/Object.md) 


**Sample**

```javascript
var contentLength = response.getResponseHeaders("Content-Length");
```
### getStatusCode()

Gets the status code of the response, the list of the possible values is in HTTP_STATUS constants.

In case there was an exception executing the request, please ignore/do not use this value (it will be 0).
You can check that situation using response.getException().


**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var status = response.getStatusCode();// compare with HTTP_STATUS constants
```
### getStatusReasonPhrase()

Gets the status code's reason phrase. For example if a response contains status code 403 (Forbidden) it might be useful to know why.

For example a Jenkins API req. could answer with "403 No valid crumb was included in the request" which will let you know
that you simply have to reques a crumb and then put that in the request headers as "Jenkins-Crumb". But you could not know that from 403 status alone...


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var statusReasonPhrase = response.getStatusReasonPhrase();
```

