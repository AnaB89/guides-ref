#  Namespace

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](./String.md) | [prefix](Namespace.md#prefix)                   | Identifies the prefix of this namespace, if applicable..                                    |
| [String](./String.md) | [uri](Namespace.md#uri)                   | Identifies the namespace of this Namespace, if applicable..                                    |

## Properties Details

### prefix

Identifies the prefix of this namespace, if applicable.

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

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
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var xmlElement = <xhtml:p xmlns:xhtml="http://www.w3.org/1999/xhtml">Hello World!</xhtml:p>;
var namespace = xmlElement.namespace();
application.output("Prefix: " + namespace.prefix); //will output: 'xhtml'
application.output("URI: " + namespace.uri); //will output: 'http://www.w3.org/1999/xhtml'
```

