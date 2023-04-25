#  Builder

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Builder](../../Builder.md) | [header(key, value)](Builder.md#header-key-value)                   | Adds a header to the JWT token..                                    |
| [Builder](../../Builder.md) | [payload(payload)](Builder.md#payload-payload)                   | Adds the payload (claims) to the web token..                                    |
| [String](../../JSLib/String.md) | [sign(alg)](Builder.md#sign-alg)                   | Sign the token with the given algorithm..                                    |
| [Builder](../../Builder.md) | [withClaim(key, value)](Builder.md#withclaim-key-value)                   | Adds data to the payload, which contains the claims..                                    |
| [Builder](../../Builder.md) | [withExpires(expire)](Builder.md#withexpires-expire)                   | Add a specific Expires At ("exp") claim to the Payload..                                    |

## Methods Details

### header(key, value)

Adds a header to the JWT token.

**Parameters**\
[String](../../JSLib/String.md) key a string representing the header name\
[String](../../JSLib/String.md) value can be a string

**Returns**\
[Builder](../../Builder.md) the jwt builder for method chaining

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### payload(payload)

Adds the payload (claims) to the web token.

**Parameters**\
[Object](../../JSLib/Object.md) payload a json containing the data,
		e.g. {'some': 'data', 'somemore': 'data2'}

**Returns**\
[Builder](../../Builder.md) the jwt builder for method chaining

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### sign(alg)

Sign the token with the given algorithm.
The 'alg' claim is automatically added to the token header.

**Parameters**\
[Algorithm](../../Algorithm.md) alg the algorithm used to sign the token.

**Returns**\
[String](../../JSLib/String.md) a string representing the constructed JSON Web Token.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### withClaim(key, value)

Adds data to the payload, which contains the claims.
Claims are statements about an entity (typically, the user) and additional data.

**Parameters**\
[String](../../JSLib/String.md) key a string representing the claim name (e.g. 'iss' which stands for issuer; 'email', 'name', etc.)\
[Object](../../JSLib/Object.md) value can be a string, a boolean, a date, a number or an array

**Returns**\
[Builder](../../Builder.md) the jwt builder for method chaining

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### withExpires(expire)

Add a specific Expires At ("exp") claim to the Payload.

**Parameters**\
[Date](../../JSLib/Date.md) expire a date representing the expiration time of the token

**Returns**\
[Builder](../../Builder.md) the jwt builder for method chaining

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```

