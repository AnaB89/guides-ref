# Namespace

## Property Summary

| Type                | Name                          | Summary                                                     |
| ------------------- | ----------------------------- | ----------------------------------------------------------- |
| [String](string.md) | [prefix](namespace.md#prefix) | Identifies the prefix of this namespace, if applicable..    |
| [String](string.md) | [uri](namespace.md#uri)       | Identifies the namespace of this Namespace, if applicable.. |

## Properties Details

### prefix

Identifies the prefix of this namespace, if applicable.

**Returns**\
[String](string.md)

**Sample**

```javascript
var xmlElement = <xhtml:p xmlns:xhtml="http://www.w3.org/1999/xhtml">Hello World!</xhtml:p>;
var namespace = xmlElement.namespace();
application.output("Prefix: " + namespace.prefix); //will output: 'xhtml'
application.output("URI: " + namespace.uri); //will output: 'http://www.w3.org/1999/xhtml'
```

### uri

Identifies the namespace of this Namespace, if applicable.

**Returns**\
[String](string.md)

**Sample**

```javascript
var xmlElement = <xhtml:p xmlns:xhtml="http://www.w3.org/1999/xhtml">Hello World!</xhtml:p>;
var namespace = xmlElement.namespace();
application.output("Prefix: " + namespace.prefix); //will output: 'xhtml'
application.output("URI: " + namespace.uri); //will output: 'http://www.w3.org/1999/xhtml'
```
