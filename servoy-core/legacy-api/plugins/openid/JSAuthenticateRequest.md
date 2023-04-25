#  JSAuthenticateRequest

## **Supported Clients**

    SmartClient
    WebClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [addAttributeRequest(alias, schemaURI, required)](JSAuthenticateRequest.md#addattributerequest-alias-schemauri-required)                   | Add attribute request.                                    |
|void | [execute()](JSAuthenticateRequest.md#execute)                   | .                                    |

## Methods Details

### addAttributeRequest(alias, schemaURI, required)

Add attribute request

**Parameters**\
[String](../../JSLib/String.md) alias  ;\
[String](../../JSLib/String.md) schemaURI  ;\
[Boolean](../../JSLib/Boolean.md) required  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
authenticateRequest.addAttributeRequest('email','http://axschema.org/contact/email',true);
```
### execute()




**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

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

