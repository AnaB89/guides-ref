#  openid

## **Return Types**
[JSAuthenticateRequest](./JSAuthenticateRequest.md),[JSAuthenticateResult](./JSAuthenticateResult.md),
## **Supported Clients**

    WebClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSAuthenticateRequest](./JSAuthenticateRequest.md) | [createAuthenticateRequest(identifier, callback)](openid.md#createauthenticaterequest-identifier-callback)                   | Redirect to openID provider to login, callback method will receive answer..                                    |

## Methods Details

### createAuthenticateRequest(identifier, callback)

Redirect to openID provider to login, callback method will receive answer.

**Parameters**\
[String](../../JSLib/String.md) identifier  ;\
[Function](../../JSLib/Function.md) callback  ;

**Returns**\
[JSAuthenticateRequest](./JSAuthenticateRequest.md) 

**Supported Clients**\
WebClient

**Sample**

```javascript
var authenticateRequest = plugins.openid.createAuthenticateRequest('https://www.google.com/accounts/o8/id',openIDLoginCallback);
authenticateRequest.addAttributeRequest('email','http://axschema.org/contact/email',true);
//see http://www.axschema.org/types/ for more attributes, not all are supported by all providers!
authenticateRequest.execute();

//sample
//function openIDLoginCallback(identifier,authenticateResult)
//{
//	var ok = false;
//	if (identifier)
//	{
//		var id = identifier.substring(identifier.lastIndexOf('=')+1)
//		application.output('id:'+id)
//		var email = authenticateResult.getAttributeValue('email')
//		application.output('email:'+email)
//		ok = security.login(email, id, ['Administrators'])
//	}
//	if (!ok)
//	{
//		application.output('Login failed')
//	}
//}
```

