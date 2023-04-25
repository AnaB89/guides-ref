#  jwt

## **Supported Clients**

    WebClient
    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Algorithm](../../Algorithm.md) | [ES256(publicKey)](jwt.md#es256-publickey)                   | Builder to create a new Algorithm instance using SHA256withECDSA..                                    |
| [Algorithm](../../Algorithm.md) | [ES256(publicKey, privateKey)](jwt.md#es256-publickey-privatekey)                   | Builder to create a new Algorithm instance using SHA256withECDSA..                                    |
| [Algorithm](../../Algorithm.md) | [ES256(publicKey)](jwt.md#es256-publickey)                   | Builder to create a new Algorithm instance using SHA256withECDSA..                                    |
| [Algorithm](../../Algorithm.md) | [ES256(publicKey, privateKey)](jwt.md#es256-publickey-privatekey)                   | Builder to create a new Algorithm instance using SHA256withECDSA..                                    |
| [Algorithm](../../Algorithm.md) | [ES384(publicKey)](jwt.md#es384-publickey)                   | Builder to create a new Algorithm instance using SHA384withECDSA..                                    |
| [Algorithm](../../Algorithm.md) | [ES384(publicKey, privateKey)](jwt.md#es384-publickey-privatekey)                   | Builder to create a new Algorithm instance using SHA384withECDSA..                                    |
| [Algorithm](../../Algorithm.md) | [ES384(publicKey)](jwt.md#es384-publickey)                   | Builder to create a new Algorithm instance using SHA384withECDSA..                                    |
| [Algorithm](../../Algorithm.md) | [ES384(publicKey, privateKey)](jwt.md#es384-publickey-privatekey)                   | Builder to create a new Algorithm instance using SHA384withECDSA..                                    |
| [Algorithm](../../Algorithm.md) | [ES512(publicKey)](jwt.md#es512-publickey)                   | Builder to create a new Algorithm instance using SHA512withECDSA..                                    |
| [Algorithm](../../Algorithm.md) | [ES512(publicKey, privateKey)](jwt.md#es512-publickey-privatekey)                   | Builder to create a new Algorithm instance using SHA512withECDSA..                                    |
| [Algorithm](../../Algorithm.md) | [ES512(publicKey)](jwt.md#es512-publickey)                   | Builder to create a new Algorithm instance using SHA512withECDSA..                                    |
| [Algorithm](../../Algorithm.md) | [ES512(publicKey, privateKey)](jwt.md#es512-publickey-privatekey)                   | Builder to create a new Algorithm instance using SHA512withECDSA..                                    |
| [Algorithm](../../Algorithm.md) | [HS256()](jwt.md#hs256)                   | Create a new Algorithm instance using HmacSHA256..                                    |
| [Algorithm](../../Algorithm.md) | [HS256(password)](jwt.md#hs256-password)                   | Create a new HmacSHA256 Algorithm using the specified password..                                    |
| [Algorithm](../../Algorithm.md) | [HS384()](jwt.md#hs384)                   | Create a new Algorithm instance using HmacSHA384..                                    |
| [Algorithm](../../Algorithm.md) | [HS384(password)](jwt.md#hs384-password)                   | Create a new HmacSHA384 Algorithm using the specified password..                                    |
| [Algorithm](../../Algorithm.md) | [HS512()](jwt.md#hs512)                   | Create a new Algorithm instance using HmacSHA512..                                    |
| [Algorithm](../../Algorithm.md) | [HS512(password)](jwt.md#hs512-password)                   | Create a new Algorithm instance using HmacSHA512..                                    |
| [Algorithm](../../Algorithm.md) | [JWK(url)](jwt.md#jwk-url)                   | Builder to create an algorithm instance based on a Json Web Key Set (JWKS) url..                                    |
| [Algorithm](../../Algorithm.md) | [RSA256(publicKey)](jwt.md#rsa256-publickey)                   | Builder to create a new Algorithm instance using SHA256withRSA..                                    |
| [Algorithm](../../Algorithm.md) | [RSA256(publicKey, privateKey)](jwt.md#rsa256-publickey-privatekey)                   | Builder to create a new Algorithm instance using SHA256withRSA..                                    |
| [Algorithm](../../Algorithm.md) | [RSA256(publicKey)](jwt.md#rsa256-publickey)                   | Builder to create a new Algorithm instance using SHA256withRSA..                                    |
| [Algorithm](../../Algorithm.md) | [RSA256(publicKey, privateKey)](jwt.md#rsa256-publickey-privatekey)                   | Builder to create a new Algorithm instance using SHA256withRSA..                                    |
| [Algorithm](../../Algorithm.md) | [RSA384(publicKey)](jwt.md#rsa384-publickey)                   | Builder to create a new Algorithm instance using SHA384withRSA..                                    |
| [Algorithm](../../Algorithm.md) | [RSA384(publicKey, privateKey)](jwt.md#rsa384-publickey-privatekey)                   | Builder to create a new Algorithm instance using SHA384withRSA..                                    |
| [Algorithm](../../Algorithm.md) | [RSA384(publicKey)](jwt.md#rsa384-publickey)                   | Builder to create a new Algorithm instance using SHA384withRSA..                                    |
| [Algorithm](../../Algorithm.md) | [RSA384(publicKey, privateKey)](jwt.md#rsa384-publickey-privatekey)                   | Builder to create a new Algorithm instance using SHA384withRSA..                                    |
| [Algorithm](../../Algorithm.md) | [RSA512(publicKey)](jwt.md#rsa512-publickey)                   | Builder to create a new Algorithm instance using SHA512withRSA..                                    |
| [Algorithm](../../Algorithm.md) | [RSA512(publicKey, privateKey)](jwt.md#rsa512-publickey-privatekey)                   | Builder to create a new Algorithm instance using SHA512withRSA..                                    |
| [Algorithm](../../Algorithm.md) | [RSA512(publicKey)](jwt.md#rsa512-publickey)                   | Builder to create a new Algorithm instance using SHA512withRSA..                                    |
| [Algorithm](../../Algorithm.md) | [RSA512(publicKey, privateKey)](jwt.md#rsa512-publickey-privatekey)                   | Builder to create a new Algorithm instance using SHA512withRSA..                                    |
| [Builder](../../Builder.md) | [builder()](jwt.md#builder)                   | Returns a JSON Web Token token builder..                                    |
| [String](../../JSLib/String.md) | [create(payload)](jwt.md#create-payload)                   | Create a JSON Web Token for the given payload that is signed with the (shared) secret key 'jwt..                                    |
| [String](../../JSLib/String.md) | [create(payload, expiresAt)](jwt.md#create-payload-expiresat)                   | Create a JSON Web Token for the given payload that is signed with the HS256 algorithm and the (shared) secret key 'jwt..                                    |
| [Object](../../JSLib/Object.md) | [verify(token)](jwt.md#verify-token)                   | Verify a JSON Web Token with the HS256 algorithm and the (shared) secret key 'jwt..                                    |
| [Object](../../JSLib/Object.md) | [verify(token, algorithm)](jwt.md#verify-token-algorithm)                   | Verify a JSON Web Token with a specific algorithm..                                    |

## Methods Details

### ES256(publicKey)

Builder to create a new Algorithm instance using SHA256withECDSA. Tokens specify this as "ES256".

**Parameters**\
[Array](../../JSLib/Array.md) publicKey a byte array representing the publicKey (mostly used to verify tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm builder used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### ES256(publicKey, privateKey)

Builder to create a new Algorithm instance using SHA256withECDSA. Tokens specify this as "ES256".

**Parameters**\
[Array](../../JSLib/Array.md) publicKey a byte array representing the publicKey (mostly used to verify tokens)\
[Array](../../JSLib/Array.md) privateKey a byte array representing the privateKey (mostly used to create tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### ES256(publicKey)

Builder to create a new Algorithm instance using SHA256withECDSA. Tokens specify this as "ES256".

**Parameters**\
[String](../../JSLib/String.md) publicKey a String representing the publicKey (mostly used to verify tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm builder used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
plugins.jwt.ES256('MFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEEV....')
     .kid('2X9R4H....')
```
### ES256(publicKey, privateKey)

Builder to create a new Algorithm instance using SHA256withECDSA. Tokens specify this as "ES256".

**Parameters**\
[String](../../JSLib/String.md) publicKey a String representing the publicKey (mostly used to verify tokens)\
[String](../../JSLib/String.md) privateKey a String representing the privateKey (mostly used to create tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
plugins.jwt.ES256.publicKey('MFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEEV....', 'MIGHAgEAMBMGByqGSM49AgEGCCqGSM49AwEHBG0wa...')
     .kid('2X9R4H....')
```
### ES384(publicKey)

Builder to create a new Algorithm instance using SHA384withECDSA. Tokens specify this as "ES384".

**Parameters**\
[Array](../../JSLib/Array.md) publicKey a byte array representing the publicKey (mostly used to verify tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm builder used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### ES384(publicKey, privateKey)

Builder to create a new Algorithm instance using SHA384withECDSA. Tokens specify this as "ES384".

**Parameters**\
[Array](../../JSLib/Array.md) publicKey a byte array representing the publicKey (mostly used to verify tokens)\
[Array](../../JSLib/Array.md) privateKey a byte array representing the privateKey (mostly used to create tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### ES384(publicKey)

Builder to create a new Algorithm instance using SHA384withECDSA. Tokens specify this as "ES384".

**Parameters**\
[String](../../JSLib/String.md) publicKey a String representing the publicKey (mostly used to verify tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm builder used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
plugins.jwt.ES384('MFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEEV....')
     .kid('2X9R4H....')
```
### ES384(publicKey, privateKey)

Builder to create a new Algorithm instance using SHA384withECDSA. Tokens specify this as "ES384".

**Parameters**\
[String](../../JSLib/String.md) publicKey a String representing the publicKey (mostly used to verify tokens)\
[String](../../JSLib/String.md) privateKey a String representing the privateKey (mostly used to create tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
plugins.jwt.ES384.publicKey('MFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEEV....', 'MIGHAgEAMBMGByqGSM49AgEGCCqGSM49AwEHBG0wa...')
     .kid('2X9R4H....')
```
### ES512(publicKey)

Builder to create a new Algorithm instance using SHA512withECDSA. Tokens specify this as "ES512".

**Parameters**\
[Array](../../JSLib/Array.md) publicKey a byte array representing the publicKey (mostly used to verify tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm builder used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### ES512(publicKey, privateKey)

Builder to create a new Algorithm instance using SHA512withECDSA. Tokens specify this as "ES512".

**Parameters**\
[Array](../../JSLib/Array.md) publicKey a byte array representing the publicKey (mostly used to verify tokens)\
[Array](../../JSLib/Array.md) privateKey a byte array representing the privateKey (mostly used to create tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### ES512(publicKey)

Builder to create a new Algorithm instance using SHA512withECDSA. Tokens specify this as "ES512".

**Parameters**\
[String](../../JSLib/String.md) publicKey a String representing the publicKey

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm builder used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
plugins.jwt.ES512('MFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEEV....')
     .kid('2X9R4H....')
```
### ES512(publicKey, privateKey)

Builder to create a new Algorithm instance using SHA512withECDSA. Tokens specify this as "ES512".

**Parameters**\
[String](../../JSLib/String.md) publicKey a String representing the publicKey (mostly used to verify tokens)\
[String](../../JSLib/String.md) privateKey a String representing the privateKey (mostly used to create tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
plugins.jwt.ES512.publicKey('MFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEEV....', 'MIGHAgEAMBMGByqGSM49AgEGCCqGSM49AwEHBG0wa...')
     .kid('2X9R4H....')
```
### HS256()

Create a new Algorithm instance using HmacSHA256. Tokens specify this as "HS256".
The password used to configure the algorithm is the (shared) secret key 'jwt.secret.password' that has to be configured on the admin page for this plugin.


**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
WebClient,NGClient

**Sample**

```javascript
plugins.jwt.HS256()
```
### HS256(password)

Create a new HmacSHA256 Algorithm using the specified password. Tokens specify this as "HS256".

**Parameters**\
[String](../../JSLib/String.md) password the secret used to encrypt and decrypt the tokens

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### HS384()

Create a new Algorithm instance using HmacSHA384. Tokens specify this as "HS384".
The password used to configure the algorithm is the (shared) secret key 'jwt.secret.password' that has to be configured on the admin page for this plugin.


**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
WebClient,NGClient

**Sample**

```javascript
plugins.jwt.HS384()
```
### HS384(password)

Create a new HmacSHA384 Algorithm using the specified password. Tokens specify this as "HS384".

**Parameters**\
[String](../../JSLib/String.md) password the secret used to encrypt and decrypt the tokens

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
plugins.jwt.HS384('your secret password.....')
```
### HS512()

Create a new Algorithm instance using HmacSHA512. Tokens specify this as "HS512".
The password used to configure the algorithm is the (shared) secret key 'jwt.secret.password' that has to be configured on the admin page for this plugin.


**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
WebClient,NGClient

**Sample**

```javascript
plugins.jwt.HS512.secret()
```
### HS512(password)

Create a new Algorithm instance using HmacSHA512. Tokens specify this as "HS512".

**Parameters**\
[String](../../JSLib/String.md) password the secret used to encrypt and decrypt the tokens

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
plugins.jwt.HS512.secret('your secret password.....')
```
### JWK(url)

Builder to create an algorithm instance based on a Json Web Key Set (JWKS) url.
Please note that the returned algorithm can only be used to verify tokens.

**Parameters**\
[String](../../JSLib/String.md) url the jwks url

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm which can only be used to VERIFY Json Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var alg = plugins.jwt.JWK('https://....')
        var verified = plugins.jwt.verify(token, alg)
```
### RSA256(publicKey)

Builder to create a new Algorithm instance using SHA256withRSA. Tokens specify this as "RS256".

**Parameters**\
[Array](../../JSLib/Array.md) publicKey a byte array representing the publicKey (mostly used to verify tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify Json Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### RSA256(publicKey, privateKey)

Builder to create a new Algorithm instance using SHA256withRSA. Tokens specify this as "RS256".

**Parameters**\
[Array](../../JSLib/Array.md) publicKey a byte array representing the publicKey (mostly used to verify tokens)\
[Array](../../JSLib/Array.md) privateKey a byte array representing the privateKey (mostly used to create tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify Json Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### RSA256(publicKey)

Builder to create a new Algorithm instance using SHA256withRSA. Tokens specify this as "RS256".

**Parameters**\
[String](../../JSLib/String.md) publicKey a String representing the publicKey (mostly used to verify tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify Json Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
plugins.jwt.RSA256('MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAnzyis...')
     .kid('2X9R4H....')
```
### RSA256(publicKey, privateKey)

Builder to create a new Algorithm instance using SHA256withRSA. Tokens specify this as "RS256".

**Parameters**\
[String](../../JSLib/String.md) publicKey a String representing the publicKey (mostly used to verify tokens)\
[String](../../JSLib/String.md) privateKey a String representing the privateKey (mostly used to create tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify Json Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
plugins.jwt.RSA256('MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAnzyis...', 'MIIEogIBAAKCAQEAnzyis1ZjfNB0bBgKFMSvvkTtwlvB...')
     .kid('2X9R4H....')
```
### RSA384(publicKey)

Builder to create a new Algorithm instance using SHA384withRSA. Tokens specify this as "RS384".

**Parameters**\
[Array](../../JSLib/Array.md) publicKey a byte array representing the publicKey (mostly used to verify tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### RSA384(publicKey, privateKey)

Builder to create a new Algorithm instance using SHA384withRSA. Tokens specify this as "RS384".

**Parameters**\
[Array](../../JSLib/Array.md) publicKey a byte array representing the publicKey (mostly used to verify tokens)\
[Array](../../JSLib/Array.md) privateKey a byte array representing the privateKey (mostly used to create tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### RSA384(publicKey)

Builder to create a new Algorithm instance using SHA384withRSA. Tokens specify this as "RS384".

**Parameters**\
[String](../../JSLib/String.md) publicKey a String representing the publicKey (mostly used to verify tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
plugins.jwt.RSA384('MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAnzyis...')
     .kid('2X9R4H....')
```
### RSA384(publicKey, privateKey)

Builder to create a new Algorithm instance using SHA384withRSA. Tokens specify this as "RS384".

**Parameters**\
[String](../../JSLib/String.md) publicKey a String representing the publicKey (mostly used to verify tokens)\
[String](../../JSLib/String.md) privateKey a String representing the privateKey (mostly used to create tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
plugins.jwt.RSA384.publicKey('MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAnzyis...', 'MIIEogIBAAKCAQEAnzyis1ZjfNB0bBgKFMSvvkTtwlvB...')
     .kid('2X9R4H....')
```
### RSA512(publicKey)

Builder to create a new Algorithm instance using SHA512withRSA. Tokens specify this as "RS512".

**Parameters**\
[Array](../../JSLib/Array.md) publicKey a byte array representing the publicKey (mostly used to verify tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### RSA512(publicKey, privateKey)

Builder to create a new Algorithm instance using SHA512withRSA. Tokens specify this as "RS512".

**Parameters**\
[Array](../../JSLib/Array.md) publicKey a byte array representing the publicKey (mostly used to verify tokens)\
[Array](../../JSLib/Array.md) privateKey a byte array representing the privateKey (mostly used to create tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### RSA512(publicKey)

Builder to create a new Algorithm instance using SHA512withRSA. Tokens specify this as "RS512".

**Parameters**\
[String](../../JSLib/String.md) publicKey a String representing the publicKey (mostly used to verify tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
plugins.jwt.RSA512('MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAnzyis...')
     .kid('2X9R4H....')
```
### RSA512(publicKey, privateKey)

Builder to create a new Algorithm instance using SHA512withRSA. Tokens specify this as "RS512".

**Parameters**\
[String](../../JSLib/String.md) publicKey a String representing the publicKey (mostly used to verify tokens)\
[String](../../JSLib/String.md) privateKey a String representing the privateKey (mostly used to create tokens)

**Returns**\
[Algorithm](../../Algorithm.md) an algorithm used to sign or verify JSON Web Tokens.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
plugins.jwt.RSA512('MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAnzyis...','MIIEogIBAAKCAQEAnzyis1ZjfNB0bBgKFMSvvkTtwlvB...')
     .kid('2X9R4H....')
```
### builder()

Returns a JSON Web Token token builder.


**Returns**\
[Builder](../../Builder.md) an object which creates a jwt token.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var algorithm = plugins.jwt.ES256(publicKey, privateKey);

		   var token = plugins.jwt.builder()
                    .payload({'some': 'data', 'somemore': 'data2'})
                    .sign(algorithm);
		   if (token != null) {
		       //success
		       application.output(token);
		   }
        else {
            application.output('Could not create a token.');
        }

        var verified = plugins.jwt.verify(token, algorithm);
        if (verified != null) {
             //success
		       application.output(verified);
        }
        else {
            application.output('The token is not valid.');
        }
```
### create(payload)

Create a JSON Web Token for the given payload that is signed with the (shared) secret key 'jwt.secret.password'.
The 'jwt.secret.password' plugin property has to be configured on the admin page.
The payload can be for example a user:username of the current user, so that with this token if it verifies with the same secret key you can assume it is the same user that wants to login.
This is a shorthand method of the #builder() method with a HS256 algorithm.

**Parameters**\
[Object](../../JSLib/Object.md) payload a json containing the data,
		e.g. {'some': 'data', 'somemore': 'data2'}

**Returns**\
[String](../../JSLib/String.md) a string representing the encrypted data
		or null if the token cannot be generated

**Supported Clients**\
WebClient,NGClient

**Sample**

```javascript

```
### create(payload, expiresAt)

Create a JSON Web Token for the given payload that is signed with the HS256 algorithm and the (shared) secret key 'jwt.secret.password'.
The 'jwt.secret.password' plugin property has to be configured on the admin page.
The payload can be for example a user:username of the current user, so that with this token if it verifies with the same secret key you can assume it is the same user that wants to login.
The expiresAt makes sure this token is only valid until that date.
This is a shorthand method of the #builder() method with a HS256 algorithm.

**Parameters**\
[Object](../../JSLib/Object.md) payload a json containing the data,
		e.g. {'some': 'data', 'somemore': 'data2'}\
[Date](../../JSLib/Date.md) expiresAt the date when the created token expires,
		after the expired date the token won't be verified

**Returns**\
[String](../../JSLib/String.md) a string representing the encrypted data
		or null if the token cannot be generated

**Supported Clients**\
WebClient,NGClient

**Sample**

```javascript

```
### verify(token)

Verify a JSON Web Token with the HS256 algorithm and the (shared) secret key 'jwt.secret.password'.
The 'jwt.secret.password' plugin property has to be configured on the admin page.
This will only verify and return the payload that was given if the token was created with the HS256 algorithm and the 'jwt.secret.password'.
Will also return null if the token passed its expire date.

**Parameters**\
[String](../../JSLib/String.md) token a JSON Web Token

**Returns**\
[Object](../../JSLib/Object.md) the payload or null if the token can't be verified

**Supported Clients**\
WebClient,NGClient

**Sample**

```javascript

```
### verify(token, algorithm)

Verify a JSON Web Token with a specific algorithm.
The token could be external or created with the #builder() method.

This will only verify and return the payload that was given if the token could be verified with the provided algorithm.
Will also return null if the token passed its expire date.

**Parameters**\
[String](../../JSLib/String.md) token a JSON Web Token\
[Algorithm](../../Algorithm.md) algorithm an algorithm used to verify the signature

**Returns**\
[Object](../../JSLib/Object.md) the payload or null if the token can't be verified

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```

