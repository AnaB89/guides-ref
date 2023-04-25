#  XmlNode

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Array](../../JSLib/Array.md) | [getAttributeNames()](XmlNode.md#getattributenames)                   | Return all the attribute names of the current node..                                    |
| [String](../../JSLib/String.md) | [getAttributeValue(attributeName)](XmlNode.md#getattributevalue-attributename)                   | Return the value of the named attribute..                                    |
| [Array](../../JSLib/Array.md) | [getChildNodes()](XmlNode.md#getchildnodes)                   | Return the child nodes of the current node..                                    |
| [String](../../JSLib/String.md) | [getName()](XmlNode.md#getname)                   | Return the name of the XML node element..                                    |
| [String](../../JSLib/String.md) | [getTextValue()](XmlNode.md#gettextvalue)                   | Return the text-value of the XML node element..                                    |
| [String](../../JSLib/String.md) | [getType()](XmlNode.md#gettype)                   | Return the type of the XML node element..                                    |

## Methods Details

### getAttributeNames()

Return all the attribute names of the current node.


**Returns**\
[Array](../../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
nodes = plugins.XmlReader.readXmlDocumentFromString("<root attr1='value1' attr2='value2'/>")
rootNode = nodes[0];
attributes = rootNode.getAttributeNames();
application.output(attributes[0])
application.output(attributes[1])
val1 = rootNode.getAttributeValue('attr1');
application.output(val1)
```
### getAttributeValue(attributeName)

Return the value of the named attribute.

**Parameters**\
[String](../../JSLib/String.md) attributeName  ;

**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
nodes = plugins.XmlReader.readXmlDocumentFromString("<root attr1='value1' attr2='value2'/>")
rootNode = nodes[0];
attributes = rootNode.getAttributeNames();
application.output(attributes[0])
application.output(attributes[1])
val1 = rootNode.getAttributeValue('attr1');
application.output(val1)
```
### getChildNodes()

Return the child nodes of the current node.


**Returns**\
[Array](../../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
nodes = plugins.XmlReader.readXmlDocumentFromString('<father><child1>John</child1><child2>Mary</child2></father>');
application.output(nodes[0].getName())
application.output(nodes[0].getTextValue())
application.output(nodes[0].getType())
childs = nodes[0].getChildNodes()
application.output(childs[0].getName())
application.output(childs[0].getTextValue())
application.output(childs[0].getType())
subChilds = childs[0].getChildNodes()
application.output(subChilds[0].getName())
application.output(subChilds[0].getTextValue())
application.output(subChilds[0].getType())
```
### getName()

Return the name of the XML node element.


**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
nodes = plugins.XmlReader.readXmlDocumentFromString('<father><child1>John</child1><child2>Mary</child2></father>');
application.output(nodes[0].getName())
application.output(nodes[0].getTextValue())
application.output(nodes[0].getType())
childs = nodes[0].getChildNodes()
application.output(childs[0].getName())
application.output(childs[0].getTextValue())
application.output(childs[0].getType())
subChilds = childs[0].getChildNodes()
application.output(subChilds[0].getName())
application.output(subChilds[0].getTextValue())
application.output(subChilds[0].getType())
```
### getTextValue()

Return the text-value of the XML node element.


**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
nodes = plugins.XmlReader.readXmlDocumentFromString('<father><child1>John</child1><child2>Mary</child2></father>');
application.output(nodes[0].getName())
application.output(nodes[0].getTextValue())
application.output(nodes[0].getType())
childs = nodes[0].getChildNodes()
application.output(childs[0].getName())
application.output(childs[0].getTextValue())
application.output(childs[0].getType())
subChilds = childs[0].getChildNodes()
application.output(subChilds[0].getName())
application.output(subChilds[0].getTextValue())
application.output(subChilds[0].getType())
```
### getType()

Return the type of the XML node element.


**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
nodes = plugins.XmlReader.readXmlDocumentFromString('<father><child1>John</child1><child2>Mary</child2></father>');
application.output(nodes[0].getName())
application.output(nodes[0].getTextValue())
application.output(nodes[0].getType())
childs = nodes[0].getChildNodes()
application.output(childs[0].getName())
application.output(childs[0].getTextValue())
application.output(childs[0].getType())
subChilds = childs[0].getChildNodes()
application.output(subChilds[0].getName())
application.output(subChilds[0].getTextValue())
application.output(subChilds[0].getType())
```

