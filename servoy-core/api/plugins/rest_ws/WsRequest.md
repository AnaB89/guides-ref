#  WsRequest


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../../JSLib/String.md) | [characterEncoding](WsRequest.md#characterEncoding)                   | Returns the name of the character encoding used in the body of this request..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](../../JSLib/Number.md) | [getContentLength()](WsRequest.md#getcontentlength)                   | Returns the length, in bytes, of the request body and made available by the input stream, or -1 if the length is not known..                                    |
| [String](../../JSLib/String.md) | [getContentType()](WsRequest.md#getcontenttype)                   | Returns the MIME type of the body of the request, or <code>null</code> if the type is not known..                                    |
| [Array](../../JSLib/Array.md) | [getContents()](WsRequest.md#getcontents)                   | Get raw the contents of the request..                                    |
| [String](../../JSLib/String.md) | [getContextPath()](WsRequest.md#getcontextpath)                   | Returns the portion of the request URI that indicates the context of the request..                                    |
| [Array](../../JSLib/Array.md) | [getCookies()](WsRequest.md#getcookies)                   | Returns an array containing all of the <code>Cookie</code> objects the client sent with this request..                                    |
| [Number](../../JSLib/Number.md) | [getDateHeader(name)](WsRequest.md#getdateheader-name)                   | Returns the value of the specified request header as a <code>long</code> value that represents a <code>Date</code> object..                                    |
| [String](../../JSLib/String.md) | [getHeader(name)](WsRequest.md#getheader-name)                   | Returns the value of the specified request header as a String..                                    |
| [Array](../../JSLib/Array.md) | [getHeaderNames()](WsRequest.md#getheadernames)                   | Returns an enumeration of all the header names this request contains..                                    |
| [Array](../../JSLib/Array.md) | [getHeaders(name)](WsRequest.md#getheaders-name)                   | Returns all the values of the specified request header as an array of <code>String</code> objects..                                    |
| [Number](../../JSLib/Number.md) | [getIntHeader(name)](WsRequest.md#getintheader-name)                   | Returns the value of the specified request header as an <code>int</code>..                                    |
| [String](../../JSLib/String.md) | [getLocalAddr()](WsRequest.md#getlocaladdr)                   | Returns the Internet Protocol (IP) address of the interface on which the request  was received..                                    |
| [String](../../JSLib/String.md) | [getLocalName()](WsRequest.md#getlocalname)                   | Returns the host name of the Internet Protocol (IP) interface on which the request was received..                                    |
| [Number](../../JSLib/Number.md) | [getLocalPort()](WsRequest.md#getlocalport)                   | Returns the Internet Protocol (IP) port number of the interface on which the request was received..                                    |
| [String](../../JSLib/String.md) | [getLocaleLanguageTag()](WsRequest.md#getlocalelanguagetag)                   | Returns the preferred <code>Locale</code> that the client will accept content in, based on the Accept-Language header..                                    |
| [Array](../../JSLib/Array.md) | [getLocalesLanguageTags()](WsRequest.md#getlocaleslanguagetags)                   | Returns an array of <code>Locale</code> objects indicating, in decreasing order starting with the preferred locale, the locales that are acceptable to the client based on the Accept-Language header..                                    |
| [String](../../JSLib/String.md) | [getMethod()](WsRequest.md#getmethod)                   | Returns the name of the HTTP method with which this request was made, for example, GET, POST, or PUT..                                    |
| [String](../../JSLib/String.md) | [getParameter(name)](WsRequest.md#getparameter-name)                   | Returns the value of a request parameter as a <code>String</code>, or <code>null</code> if the parameter does not exist..                                    |
| [Object](../../JSLib/Object.md) | [getParameterMap()](WsRequest.md#getparametermap)                   | Returns an object of the parameters of this request..                                    |
| [Array](../../JSLib/Array.md) | [getParameterNames()](WsRequest.md#getparameternames)                   | Returns an array of <code>String</code> objects containing the names of the parameters contained in this request..                                    |
| [Array](../../JSLib/Array.md) | [getParameterValues(name)](WsRequest.md#getparametervalues-name)                   | Returns an array of <code>String</code> objects containing all of the values the given request parameter has, or <code>null</code> if the parameter does not exist..                                    |
| [String](../../JSLib/String.md) | [getPathInfo()](WsRequest.md#getpathinfo)                   | Returns any extra path information associated with the URL the client sent when it made this request..                                    |
| [String](../../JSLib/String.md) | [getPathTranslated()](WsRequest.md#getpathtranslated)                   | Returns any extra path information after the servlet name but before the query string, and translates it to a real path..                                    |
| [String](../../JSLib/String.md) | [getProtocol()](WsRequest.md#getprotocol)                   | Returns the name and version of the protocol the request uses in the form <i>protocol/majorVersion..                                    |
| [String](../../JSLib/String.md) | [getQueryString()](WsRequest.md#getquerystring)                   | Returns the query string that is contained in the request URL after the path..                                    |
| [String](../../JSLib/String.md) | [getRealPath(path)](WsRequest.md#getrealpath-path)                   | Gets the <i>real</i> path corresponding to the given <i>virtual</i> path..                                    |
| [String](../../JSLib/String.md) | [getRemoteAddr()](WsRequest.md#getremoteaddr)                   | Returns the Internet Protocol (IP) address of the client or last proxy that sent the request..                                    |
| [String](../../JSLib/String.md) | [getRemoteHost()](WsRequest.md#getremotehost)                   | Returns the fully qualified name of the client or the last proxy that sent the request..                                    |
| [Number](../../JSLib/Number.md) | [getRemotePort()](WsRequest.md#getremoteport)                   | Returns the Internet Protocol (IP) source port of the client or last proxy that sent the request..                                    |
| [String](../../JSLib/String.md) | [getRequestURI()](WsRequest.md#getrequesturi)                   | Returns the part of this request's URL from the protocol name up to the query string in the first line of the HTTP request..                                    |
| [String](../../JSLib/String.md) | [getRequestURL()](WsRequest.md#getrequesturl)                   | Reconstructs the URL the client used to make the request..                                    |
| [String](../../JSLib/String.md) | [getScheme()](WsRequest.md#getscheme)                   | Returns the name of the scheme used to make this request, for example, <code>http</code>, <code>https</code>, or <code>ftp</code>..                                    |
| [String](../../JSLib/String.md) | [getServerName()](WsRequest.md#getservername)                   | Returns the host name of the server to which the request was sent..                                    |
| [Number](../../JSLib/Number.md) | [getServerPort()](WsRequest.md#getserverport)                   | Returns the port number to which the request was sent..                                    |
| [String](../../JSLib/String.md) | [getServletPath()](WsRequest.md#getservletpath)                   | Returns the part of this request's URL that calls the servlet..                                    |
| [Boolean](../../JSLib/Boolean.md) | [isSecure()](WsRequest.md#issecure)                   | Returns a boolean indicating whether this request was made using a secure channel, such as HTTPS..                                    |

## Properties Details

### characterEncoding

Returns the name of the character encoding used in the body of this
request. This method returns <code>null</code> if the request
does not specify a character encoding

**Returns**\
[String](../../JSLib/String.md) a <code>String</code> containing the name of the character
encoding, or <code>null</code> if the request does not specify a
character encoding


**Sample**

```javascript

```

## Methods Details

### getContentLength()

Returns the length, in bytes, of the request body and made available by
the input stream, or -1 if the length is not known. For HTTP servlets,
same as the value of the CGI variable CONTENT_LENGTH.


**Returns**\
[Number](../../JSLib/Number.md) a long containing the length of the request body or -1L if
the length is not known


**Sample**

```javascript

```
### getContentType()

Returns the MIME type of the body of the request, or
<code>null</code> if the type is not known. For HTTP servlets,
same as the value of the CGI variable CONTENT_TYPE.


**Returns**\
[String](../../JSLib/String.md) a <code>String</code> containing the name of the MIME type
of the request, or null if the type is not known


**Sample**

```javascript

```
### getContents()

Get raw the contents of the request.

In case of multipart request, all uploaded items are listed separately.
In case of a request with a single body, the contents array consists of one item, the body.

This method returns an empty array if the request has no contents.


**Returns**\
[Array](../../JSLib/Array.md) an array of WsContents objects.


**Sample**

```javascript
var request = plugins.rest_ws.getRequest();
var contents = request.getContents();
```
### getContextPath()

Returns the portion of the request URI that indicates the context
of the request. The context path always comes first in a request
URI. The path starts with a "/" character but does not end with a "/"
character. For servlets in the default (root) context, this method
returns "". The container does not decode this string.

<p>It is possible that a servlet container may match a context by
more than one context path. In such cases this method will return the
actual context path used by the request and it may differ from the
path returned by the
javax.servlet.ServletContext#getContextPath() method.
The context path returned by
javax.servlet.ServletContext#getContextPath()
should be considered as the prime or preferred context path of the
application.


**Returns**\
[String](../../JSLib/String.md) a <code>String</code> specifying the
			portion of the request URI that indicates the context
			of the request


**Sample**

```javascript

```
### getCookies()

Returns an array containing all of the <code>Cookie</code>
objects the client sent with this request.
This method returns an empty array if no cookies were sent.


**Returns**\
[Array](../../JSLib/Array.md) an array of all the <code>Cookies</code>
			included with this request


**Sample**

```javascript

```
### getDateHeader(name)

Returns the value of the specified request header
as a <code>long</code> value that represents a
<code>Date</code> object. Use this method with
headers that contain dates, such as
<code>If-Modified-Since</code>.

<p>The date is returned as
the number of milliseconds since January 1, 1970 GMT.
The header name is case insensitive.

<p>If the request did not have a header of the
specified name, this method returns -1. If the header
can't be converted to a date, the method throws
an <code>IllegalArgumentException</code>.

**Parameters**\
[String](../../JSLib/String.md) name a <code>String</code> specifying the
				name of the header

**Returns**\
[Number](../../JSLib/Number.md) a <code>long</code> value
				representing the date specified
				in the header expressed as
				the number of milliseconds
				since January 1, 1970 GMT,
				or -1 if the named header
				was not included with the
				request


**Sample**

```javascript

```
### getHeader(name)

Returns the value of the specified request header as a String.
If the request did not include a header of the specified name, this method returns null.
If there are multiple headers with the same name, this method returns the first head in the request.
The header name is case insensitive. You can use this method with any request header.

**Parameters**\
[String](../../JSLib/String.md) name The name of the header to get

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var request = plugins.rest_ws.getRequest();
var header = request.getHeader('');
```
### getHeaderNames()

Returns an enumeration of all the header names
this request contains. If the request has no
headers, this method returns an empty enumeration.

<p>Some servlet containers do not allow
servlets to access headers using this method, in
which case this method returns <code>null</code>


**Returns**\
[Array](../../JSLib/Array.md) an enumeration of all the
				header names sent with this
				request; if the request has
				no headers, an empty enumeration;
				if the servlet container does not
				allow servlets to use this method,
				<code>null</code>


**Sample**

```javascript

```
### getHeaders(name)

Returns all the values of the specified request header
as an array of <code>String</code> objects.

<p>Some headers, such as <code>Accept-Language</code> can be sent
by clients as several headers each with a different value rather than
sending the header as a comma separated list.

<p>If the request did not include any headers
of the specified name, this method returns an empty
array.
The header name is case insensitive. You can use
this method with any request header.

**Parameters**\
[String](../../JSLib/String.md) name a <code>String</code> specifying the
				header name

**Returns**\
[Array](../../JSLib/Array.md) an array containing
                 	the values of the requested header. If
                 	the request does not have any headers of
                 	that name return an empty
                 	enumeration. If
                 	the container does not allow access to
                 	header information, return null


**Sample**

```javascript

```
### getIntHeader(name)

Returns the value of the specified request header
as an <code>int</code>. If the request does not have a header
of the specified name, this method returns -1. If the
header cannot be converted to an integer, this method
throws a <code>NumberFormatException</code>.

<p>The header name is case insensitive.

**Parameters**\
[String](../../JSLib/String.md) name a <code>String</code> specifying the name
				of a request header

**Returns**\
[Number](../../JSLib/Number.md) an integer expressing the value
				of the request header or -1
				if the request doesn't have a
				header of this name


**Sample**

```javascript

```
### getLocalAddr()

Returns the Internet Protocol (IP) address of the interface on
which the request  was received.


**Returns**\
[String](../../JSLib/String.md) a <code>String</code> containing the
IP address on which the request was received.


**Sample**

```javascript

```
### getLocalName()

Returns the host name of the Internet Protocol (IP) interface on
which the request was received.


**Returns**\
[String](../../JSLib/String.md) a <code>String</code> containing the host
        name of the IP on which the request was received.


**Sample**

```javascript

```
### getLocalPort()

Returns the Internet Protocol (IP) port number of the interface
on which the request was received.


**Returns**\
[Number](../../JSLib/Number.md) an integer specifying the port number


**Sample**

```javascript

```
### getLocaleLanguageTag()

Returns the preferred <code>Locale</code> that the client will
accept content in, based on the Accept-Language header.
If the client request doesn't provide an Accept-Language header,
this method returns the default locale for the server.

Returns a well-formed IETF BCP 47 language tag representing
this locale.


**Returns**\
[String](../../JSLib/String.md) the preferred <code>Locale</code> for the client


**Sample**

```javascript

```
### getLocalesLanguageTags()

Returns an array of <code>Locale</code> objects
indicating, in decreasing order starting with the preferred locale, the
locales that are acceptable to the client based on the Accept-Language
header.
If the client request doesn't provide an Accept-Language header,
this method returns an array containing one
<code>Locale</code>, the default locale for the server.

Returns well-formed IETF BCP 47 language tags representing
the locales.


**Returns**\
[Array](../../JSLib/Array.md) an array of preferred
<code>Locale</code> objects for the client


**Sample**

```javascript

```
### getMethod()

Returns the name of the HTTP method with which this
request was made, for example, GET, POST, or PUT.
Same as the value of the CGI variable REQUEST_METHOD.


**Returns**\
[String](../../JSLib/String.md) a <code>String</code>
				specifying the name
				of the method with which
				this request was made


**Sample**

```javascript

```
### getParameter(name)

Returns the value of a request parameter as a <code>String</code>,
or <code>null</code> if the parameter does not exist. Request parameters
are extra information sent with the request.  For HTTP servlets,
parameters are contained in the query string or posted form data.

<p>You should only use this method when you are sure the
parameter has only one value. If the parameter might have
more than one value, use #getParameterValues(String).

<p>If you use this method with a multivalued
parameter, the value returned is equal to the first value
in the array returned by <code>getParameterValues</code>.

<p>If the parameter data was sent in the request body, such as occurs
with an HTTP POST request, then reading the body directly via 
#getInputStream or #getReader can interfere
with the execution of this method.

**Parameters**\
[String](../../JSLib/String.md) name a <code>String</code> specifying the name of the parameter

**Returns**\
[String](../../JSLib/String.md) a <code>String</code> representing the single value of
the parameter


**Sample**

```javascript

```
### getParameterMap()

Returns an object of the parameters of this request.

<p>Request parameters are extra information sent with the request.
For HTTP servlets, parameters are contained in the query string or
posted form data.


**Returns**\
[Object](../../JSLib/Object.md) an object containing parameter names as
keys and parameter values as map values. The keys in the parameter
map are of type String. The values in the parameter map are of type
String array.


**Sample**

```javascript

```
### getParameterNames()

Returns an array of <code>String</code>
objects containing the names of the parameters contained
in this request. If the request has
no parameters, the method returns an empty array.


**Returns**\
[Array](../../JSLib/Array.md) an array of <code>String</code>
objects, each <code>String</code> containing the name of
a request parameter; or an empty array
if the request has no parameters


**Sample**

```javascript

```
### getParameterValues(name)

Returns an array of <code>String</code> objects containing
all of the values the given request parameter has, or
<code>null</code> if the parameter does not exist.

<p>If the parameter has a single value, the array has a length
of 1.

**Parameters**\
[String](../../JSLib/String.md) name a <code>String</code> containing the name of
the parameter whose value is requested

**Returns**\
[Array](../../JSLib/Array.md) an array of <code>String</code> objects
containing the parameter's values


**Sample**

```javascript

```
### getPathInfo()

Returns any extra path information associated with
the URL the client sent when it made this request.
The extra path information follows the servlet path
but precedes the query string and will start with
a "/" character.

<p>This method returns <code>null</code> if there
was no extra path information.

<p>Same as the value of the CGI variable PATH_INFO.


**Returns**\
[String](../../JSLib/String.md) a <code>String</code>, decoded by the
			web container, specifying
			extra path information that comes
			after the servlet path but before
			the query string in the request URL;
			or <code>null</code> if the URL does not have
			any extra path information


**Sample**

```javascript

```
### getPathTranslated()

Returns any extra path information after the servlet name
but before the query string, and translates it to a real
path. Same as the value of the CGI variable PATH_TRANSLATED.

<p>If the URL does not have any extra path information,
this method returns <code>null</code> or the servlet container
cannot translate the virtual path to a real path for any reason
(such as when the web application is executed from an archive).

The web container does not decode this string.


**Returns**\
[String](../../JSLib/String.md) a <code>String</code> specifying the
			real path, or <code>null</code> if
			the URL does not have any extra path
			information


**Sample**

```javascript

```
### getProtocol()

Returns the name and version of the protocol the request uses
in the form <i>protocol/majorVersion.minorVersion</i>, for
example, HTTP/1.1. For HTTP servlets, the value
returned is the same as the value of the CGI variable
<code>SERVER_PROTOCOL</code>.


**Returns**\
[String](../../JSLib/String.md) a <code>String</code> containing the protocol
name and version number


**Sample**

```javascript

```
### getQueryString()

Returns the query string that is contained in the request
URL after the path. This method returns <code>null</code>
if the URL does not have a query string. Same as the value
of the CGI variable QUERY_STRING.


**Returns**\
[String](../../JSLib/String.md) a <code>String</code> containing the query
			string or <code>null</code> if the URL
			contains no query string. The value is not
			decoded by the container.


**Sample**

```javascript

```
### getRealPath(path)

Gets the <i>real</i> path corresponding to the given
<i>virtual</i> path.

**Parameters**\
[String](../../JSLib/String.md) path the <i>virtual</i> path to be translated to a
<i>real</i> path

**Returns**\
[String](../../JSLib/String.md) the <i>real</i> path, or <tt>null</tt> if the
translation cannot be performed


**Sample**

```javascript

```
### getRemoteAddr()

Returns the Internet Protocol (IP) address of the client
or last proxy that sent the request.
For HTTP servlets, same as the value of the
CGI variable <code>REMOTE_ADDR</code>.


**Returns**\
[String](../../JSLib/String.md) a <code>String</code> containing the
IP address of the client that sent the request


**Sample**

```javascript

```
### getRemoteHost()

Returns the fully qualified name of the client
or the last proxy that sent the request.
If the engine cannot or chooses not to resolve the hostname
(to improve performance), this method returns the dotted-string form of
the IP address. For HTTP servlets, same as the value of the CGI variable
<code>REMOTE_HOST</code>.


**Returns**\
[String](../../JSLib/String.md) a <code>String</code> containing the fully
qualified name of the client


**Sample**

```javascript

```
### getRemotePort()

Returns the Internet Protocol (IP) source port of the client
or last proxy that sent the request.


**Returns**\
[Number](../../JSLib/Number.md) an integer specifying the port number


**Sample**

```javascript

```
### getRequestURI()

Returns the part of this request's URL from the protocol
name up to the query string in the first line of the HTTP request.
The web container does not decode this String.
For example:

<table summary="Examples of Returned Values">
<tr align=left><th>First line of HTTP request      </th>
<th>     Returned Value</th>
<tr><td>POST /some/path.html HTTP/1.1<td><td>/some/path.html
<tr><td>GET http://foo.bar/a.html HTTP/1.0
<td><td>/a.html
<tr><td>HEAD /xyz?a=b HTTP/1.1<td><td>/xyz
</table>


**Returns**\
[String](../../JSLib/String.md) a <code>String</code> containing
			the part of the URL from the
			protocol name up to the query string


**Sample**

```javascript

```
### getRequestURL()

Reconstructs the URL the client used to make the request.
The returned URL contains a protocol, server name, port
number, and server path, but it does not include query
string parameters.

<p>If this request has been forwarded using
javax.servlet.RequestDispatcher#forward(ServletRequest,ServletResponse), the server path in the
reconstructed URL must reflect the path used to obtain the
RequestDispatcher, and not the server path specified by the client.

<p>This method is useful for creating redirect messages
and for reporting errors.


**Returns**\
[String](../../JSLib/String.md) a <code>StringBuffer</code> object containing
			the reconstructed URL


**Sample**

```javascript

```
### getScheme()

Returns the name of the scheme used to make this request,
for example,
<code>http</code>, <code>https</code>, or <code>ftp</code>.
Different schemes have different rules for constructing URLs,
as noted in RFC 1738.


**Returns**\
[String](../../JSLib/String.md) a <code>String</code> containing the name
of the scheme used to make this request


**Sample**

```javascript

```
### getServerName()

Returns the host name of the server to which the request was sent.
It is the value of the part before ":" in the <code>Host</code>
header value, if any, or the resolved server name, or the server IP
address.


**Returns**\
[String](../../JSLib/String.md) a <code>String</code> containing the name of the server


**Sample**

```javascript

```
### getServerPort()

Returns the port number to which the request was sent.
It is the value of the part after ":" in the <code>Host</code>
header value, if any, or the server port where the client connection
was accepted on.


**Returns**\
[Number](../../JSLib/Number.md) an integer specifying the port number


**Sample**

```javascript

```
### getServletPath()

Returns the part of this request's URL that calls
the servlet. This path starts with a "/" character
and includes either the servlet name or a path to
the servlet, but does not include any extra path
information or a query string. Same as the value of
the CGI variable SCRIPT_NAME.

<p>This method will return an empty string ("") if the
servlet used to process this request was matched using
the "/*" pattern.


**Returns**\
[String](../../JSLib/String.md) a <code>String</code> containing
			the name or path of the servlet being
			called, as specified in the request URL,
			decoded, or an empty string if the servlet
			used to process the request is matched
			using the "/*" pattern.


**Sample**

```javascript

```
### isSecure()

Returns a boolean indicating whether this request was made using a
secure channel, such as HTTPS.


**Returns**\
[Boolean](../../JSLib/Boolean.md) a boolean indicating if the request was made using a
secure channel


**Sample**

```javascript

```

