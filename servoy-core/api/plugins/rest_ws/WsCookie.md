#  WsCookie


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../../JSLib/String.md) | [comment](WsCookie.md#comment)                   | Cookie comment..                                    |
| [String](../../JSLib/String.md) | [domain](WsCookie.md#domain)                   | Cookie domain..                                    |
| [Boolean](../../JSLib/Boolean.md) | [httpOnly](WsCookie.md#httpOnly)                   | Cookie httpOnly flag..                                    |
| [Number](../../JSLib/Number.md) | [maxAge](WsCookie.md#maxAge)                   | Cookie maxAge..                                    |
| [String](../../JSLib/String.md) | [name](WsCookie.md#name)                   | Cookie name..                                    |
| [String](../../JSLib/String.md) | [path](WsCookie.md#path)                   | Cookie path..                                    |
| [Boolean](../../JSLib/Boolean.md) | [secure](WsCookie.md#secure)                   | Cookie secure flag..                                    |
| [String](../../JSLib/String.md) | [value](WsCookie.md#value)                   | Cookie value..                                    |
| [Number](../../JSLib/Number.md) | [version](WsCookie.md#version)                   | Cookie version..                                    |

## Properties Details

### comment

Cookie comment.
Specifies a comment that describes a cookie's purpose.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var cookie = plugins.rest_ws.createCookie('chocolate', 'chip');
cookie.comment = 'yummy';
```
### domain

Cookie domain.
Specifies the domain within which this cookie should be presented.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var cookie = plugins.rest_ws.createCookie('chocolate', 'chip');
cookie.domain = 'example.com';
```
### httpOnly

Cookie httpOnly flag.
Marks or unmarks this Cookie as HttpOnly

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var cookie = plugins.rest_ws.createCookie('chocolate', 'chip');
cookie.httpOnly = true;
```
### maxAge

Cookie maxAge.
Sets the maximum age in seconds for this Cookie.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var cookie = plugins.rest_ws.createCookie('chocolate', 'chip');
cookie.maxAge = 3600;
```
### name

Cookie name.

The cookie name allows only a sequence of non-special, non-white space characters, see
the cookie spec https://tools.ietf.org/html/rfc2965

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var cookie = plugins.rest_ws.createCookie('chocolate', 'chip');
cookie.name = 'doublechocolate';
```
### path

Cookie path.
Specifies a path for the cookie to which the client should return the cookie.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var cookie = plugins.rest_ws.createCookie('chocolate', 'chip');
cookie.path = '/subfolder';
```
### secure

Cookie secure flag.
Indicates to the browser whether the cookie should only be sent using a secure protocol, such as HTTPS or SSL.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var cookie = plugins.rest_ws.createCookie('chocolate', 'chip');
cookie.secure = true;
```
### value

Cookie value.

The cookie value allows only a sequence of non-special, non-white space characters, see
the cookie spec https://tools.ietf.org/html/rfc2965

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var cookie = plugins.rest_ws.createCookie('chocolate', 'chip');
cookie.value = 'mint';
```
### version

Cookie version.
Sets the version of the cookie protocol that this Cookie complies with.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var cookie = plugins.rest_ws.createCookie('chocolate', 'chip');
cookie.version = 1;
```

