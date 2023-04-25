#  Cookie


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../../JSLib/String.md) | [getDomain()](Cookie.md#getdomain)                   | Returns the cookie domain..                                    |
| [String](../../JSLib/String.md) | [getName()](Cookie.md#getname)                   | Returns the cookie name..                                    |
| [String](../../JSLib/String.md) | [getPath()](Cookie.md#getpath)                   | Returns the cookie path..                                    |
| [Boolean](../../JSLib/Boolean.md) | [getSecure()](Cookie.md#getsecure)                   | Returns the cookie secure attribute..                                    |
| [String](../../JSLib/String.md) | [getValue()](Cookie.md#getvalue)                   | Returns the cookie value..                                    |

## Methods Details

### getDomain()

Returns the cookie domain.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var cookie = client.getCookie('cookieName')
var domain = cookie.getDomain();
```
### getName()

Returns the cookie name.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var cookie = client.getCookie('cookieName')
var name = cookie.getName();
```
### getPath()

Returns the cookie path.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var cookie = client.getCookie('cookieName')
var path = cookie.getPath();
```
### getSecure()

Returns the cookie secure attribute.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var cookie = client.getCookie('cookieName')
var path = cookie.getSecure();
```
### getValue()

Returns the cookie value.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var cookie = client.getCookie('cookieName')
var value = cookie.getValue();
```

