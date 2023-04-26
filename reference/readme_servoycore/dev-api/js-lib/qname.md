# QName

## Property Summary

| Type                | Name                            | Summary                                                |
| ------------------- | ------------------------------- | ------------------------------------------------------ |
| [String](string.md) | [localName](qname.md#localName) | Identifies the local name of the QName..               |
| [String](string.md) | [uri](qname.md#uri)             | Identifies the namespace of the QName, if applicable.. |

## Properties Details

### localName

Identifies the local name of the QName.

**Returns**\
[String](string.md)

**Sample**

```javascript
var Qnamevar = new QName('http://www.w3.org/1999/xhtml', 'author');
application.output(Qnamevar.localName);
application.output(Qnamevar.uri);
```

### uri

Identifies the namespace of the QName, if applicable.

**Returns**\
[String](string.md)

**Sample**

```javascript
var Qnamevar = new QName('http://www.w3.org/1999/xhtml', 'author');
application.output(Qnamevar.localName);
application.output(Qnamevar.uri);
```
