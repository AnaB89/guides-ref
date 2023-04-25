#  JSAuthenticateResult

## **Supported Clients**

    SmartClient
    WebClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../../JSLib/String.md) | [getAttributeValue(alias)](JSAuthenticateResult.md#getattributevalue-alias)                   | Get attribute value.                                    |
| [Array](../../JSLib/Array.md) | [getAttributeValues(alias)](JSAuthenticateResult.md#getattributevalues-alias)                   | Get an array of attribute values.                                    |

## Methods Details

### getAttributeValue(alias)

Get attribute value

**Parameters**\
[String](../../JSLib/String.md) alias  ;

**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
var email = authenticateResult.getAttributeValue('email')
```
### getAttributeValues(alias)

Get an array of attribute values

**Parameters**\
[String](../../JSLib/String.md) alias  ;

**Returns**\
[Array](../../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
var namesArray = authenticateResult.getAttributeValues('names')
for (var i = 0; i < namesArray.length; i++) { 
	application.output(namesArray[i]); 
}
```

