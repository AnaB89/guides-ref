#  QName

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](./String.md) | [localName](QName.md#localName)                   | Identifies the local name of the QName..                                    |
| [String](./String.md) | [uri](QName.md#uri)                   | Identifies the namespace of the QName, if applicable..                                    |

## Properties Details

### localName

Identifies the local name of the QName.

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var Qnamevar = new QName('http://www.w3.org/1999/xhtml', 'author');
application.output(Qnamevar.localName);
application.output(Qnamevar.uri);
```
### uri

Identifies the namespace of the QName, if applicable.

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var Qnamevar = new QName('http://www.w3.org/1999/xhtml', 'author');
application.output(Qnamevar.localName);
application.output(Qnamevar.uri);
```

