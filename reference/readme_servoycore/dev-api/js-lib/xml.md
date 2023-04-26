# XML

## Property Summary

| Type                  | Name                                                                | Summary                                                                                                               |
| --------------------- | ------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| [Boolean](boolean.md) | [ignoreComments](xml.md#ignoreComments)                             | If set to true, then comments in the XML are ignored when constructing new XML objects..                              |
| [Boolean](boolean.md) | [ignoreProcessingInstructions](xml.md#ignoreProcessingInstructions) | If set to true, then processing instructions are ignored when constructing new XML objects..                          |
| [Boolean](boolean.md) | [ignoreWhitespace](xml.md#ignoreWhitespace)                         | If set to true, then whitespace in the XML is ignored when constructing new XML objects..                             |
| [Boolean](boolean.md) | [prettyIndent](xml.md#prettyIndent)                                 | The amount of positions used when indenting child nodes are relative to their parent if prettyPrinting is enabled..   |
| [Boolean](boolean.md) | [prettyPrinting](xml.md#prettyPrinting)                             | If set to true, then toString() and toXMLString() methods will normalize the output to achieve a uniform appearance.. |

## Methods Summary

| Type                      | Name                                                                                                                | Summary                                                                                                                                                           |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [XML](xml.md)             | [addNamespace(namespaceToAdd)](xml.md#addnamespace-namespacetoadd)                                                  | Takes one argument which can be a string with a namespace URI or a Namespace object and adds the argument to the in scope namespaces of this XML object..         |
| [XML](xml.md)             | [appendChild(childToAppend)](xml.md#appendchild-childtoappend)                                                      | Appends a new child at the end of this XML object's properties, the changed XML object is then returned..                                                         |
| [XMLList](xmllist.md)     | [attribute(attributeName)](xml.md#attribute-attributename)                                                          | Takes a single argument with the attribute name and returns an XMLList with attributes matching the argument..                                                    |
| [XMLList](xmllist.md)     | [attributes()](xml.md#attributes)                                                                                   | Returns an XMLList with the attributes of this XML object which are in no namespace..                                                                             |
| [XMLList](xmllist.md)     | [child(propertyName)](xml.md#child-propertyname)                                                                    | Returns an XMLList with children matching the property name..                                                                                                     |
| [Number](number.md)       | [childIndex()](xml.md#childindex)                                                                                   | If the XML object has no parent then the special number NaN is returned, otherwise the ordinal position the object has in the context of its parent is returned.. |
| [XMLList](xmllist.md)     | [children()](xml.md#children)                                                                                       | Returns an XMLList with the child nodes of this XML object..                                                                                                      |
| [XMLList](xmllist.md)     | [comments()](xml.md#comments)                                                                                       | Returns an XMLList with the comment nodes which are children of this XML object..                                                                                 |
| [Boolean](boolean.md)     | [contains(value)](xml.md#contains-value)                                                                            | Calling xmlObject..                                                                                                                                               |
| [XML](xml.md)             | [copy()](xml.md#copy)                                                                                               | Returns a deep copy of the XML object it is called on where the internal parent property is set to null.                                                          |
| [Object](object.md)       | [defaultSettings()](xml.md#defaultsettings)                                                                         | Returns an object containing the default XML settings..                                                                                                           |
| [XMLList](xmllist.md)     | [descendants()](xml.md#descendants)                                                                                 | Returns an XMLList with the descendants matching the passed name argument or with all descendants if no argument is passed..                                      |
| [XMLList](xmllist.md)     | [descendants(name)](xml.md#descendants-name)                                                                        | Returns an XMLList with the descendants matching the passed name argument or with all descendants if no argument is passed..                                      |
| [XMLList](xmllist.md)     | [elements()](xml.md#elements)                                                                                       | Takes one optional argument, the name of elements you are looking for, and returns an XMLList with all matching child elements..                                  |
| [XMLList](xmllist.md)     | [elements(name)](xml.md#elements-name)                                                                              | Takes one optional argument, the name of elements you are looking for, and returns an XMLList with all matching child elements..                                  |
| [Boolean](boolean.md)     | [hasComplexContent()](xml.md#hascomplexcontent)                                                                     | Returns false for XML objects of node kind 'text', 'attribute', 'comment', and 'processing-instruction'..                                                         |
| [Boolean](boolean.md)     | [hasOwnProperty(propertyName)](xml.md#hasownproperty-propertyname)                                                  | Returns true if the XML object the method is called on has a property of that name..                                                                              |
| [Boolean](boolean.md)     | [hasSimpleContent()](xml.md#hassimplecontent)                                                                       | Returns true for XML objects of node kind text or attribute..                                                                                                     |
| [Array](array.md)         | [inScopeNamespaces()](xml.md#inscopenamespaces)                                                                     | Returns an array of Namespace objects representing the namespace that are in scope for this XML object..                                                          |
| [XML](xml.md)             | [insertChildAfter(childToInserAfter, childToInsert)](xml.md#insertchildafter-childtoinserafter-childtoinsert)       | Takes two arguments, an existing child to insert after and the new child to be inserted..                                                                         |
| [XML](xml.md)             | [insertChildBefore(childToInsertBefore, childToInsert)](xml.md#insertchildbefore-childtoinsertbefore-childtoinsert) | Takes two arguments, an existing child to insert before and the new child to be inserted..                                                                        |
| [Number](number.md)       | [length()](xml.md#length)                                                                                           | This always returns 1..                                                                                                                                           |
| [String](string.md)       | [localName()](xml.md#localname)                                                                                     | returns the local name part if the XML object has a name..                                                                                                        |
| [QName](qname.md)         | [name()](xml.md#name)                                                                                               | Returns the qualified name (a QName object) of the XML object it is called.                                                                                       |
| [Namespace](namespace.md) | [namespace()](xml.md#namespace)                                                                                     | If no argument is passed to the method then it returns the namespace associated with the qualified name of this XML object..                                      |
| [Namespace](namespace.md) | [namespace(prefix)](xml.md#namespace-prefix)                                                                        | If no argument is passed to the method then it returns the namespace associated with the qualified name of this XML object..                                      |
| [Array](array.md)         | [namespaceDeclarations()](xml.md#namespacedeclarations)                                                             | Returns an array with the namespace declarations associated with the XML object it is called on..                                                                 |
| [String](string.md)       | [nodeKind()](xml.md#nodekind)                                                                                       | Returns a string denoting the kind of node this XML object represents..                                                                                           |
| [XML](xml.md)             | [normalize()](xml.md#normalize)                                                                                     | Returns this XML object after normalizing all text content..                                                                                                      |
| [XML](xml.md)             | [parent()](xml.md#parent)                                                                                           | Returns the parent XML object of this XML object or null if there is no parent..                                                                                  |
| [XML](xml.md)             | [prependChild(childToPrepend)](xml.md#prependchild-childtoprepend)                                                  | Iinserts the given value as the first child of the XML object and returns the XML object..                                                                        |
| [XMLList](xmllist.md)     | [processingInstructions()](xml.md#processinginstructions)                                                           | If no argument is passed in then the method returns an XMLList with all the children of the XML object which are processing instructions..                        |
| [XMLList](xmllist.md)     | [processingInstructions(name)](xml.md#processinginstructions-name)                                                  | If no argument is passed in then the method returns an XMLList with all the children of the XML object which are processing instructions..                        |
| [Boolean](boolean.md)     | [propertyIsEnumerable(propertyName)](xml.md#propertyisenumerable-propertyname)                                      | Returns true if the property name is '0' and false otherwise..                                                                                                    |
| [XML](xml.md)             | [removeNamespace(namespace)](xml.md#removenamespace-namespace)                                                      | Removes the namespace from the in scope namespaces of this XML object if the namespace is not used for the qualified name of the object or its attributes..       |
| [XML](xml.md)             | [replace(propertyName, replacementValue)](xml.md#replace-propertyname-replacementvalue)                             | Takes two arguments, the property name of the property / properties to be replaced, and the value to replace the properties..                                     |
| [XML](xml.md)             | [setChildren(value)](xml.md#setchildren-value)                                                                      | Replaces all children of the XML object with this value..                                                                                                         |
| void                      | [setLocalName(name)](xml.md#setlocalname-name)                                                                      | Changes the local name of this XML object to the name passed in..                                                                                                 |
| void                      | [setName(name)](xml.md#setname-name)                                                                                | Replaces the name of this XML object with the name passed in..                                                                                                    |
| void                      | [setNamespace(namespace)](xml.md#setnamespace-namespace)                                                            | Changes the namespace associated with the name of this XML object to the new namespace..                                                                          |
| void                      | [setSettings()](xml.md#setsettings)                                                                                 | Allows the global XML settings to be adjusted or restored to their default values..                                                                               |
| void                      | [setSettings(settings)](xml.md#setsettings-settings)                                                                | Allows the global XML settings to be adjusted or restored to their default values..                                                                               |
| [Object](object.md)       | [settings()](xml.md#settings)                                                                                       | Returns an object containing the global XML settings..                                                                                                            |
| [XMLList](xmllist.md)     | [text()](xml.md#text)                                                                                               | Returns an XMLList with all the children of this XML object that represent text nodes..                                                                           |
| [String](string.md)       | [toString()](xml.md#tostring)                                                                                       | Returns a convenient string value of this XML object..                                                                                                            |
| [String](string.md)       | [toXMLString()](xml.md#toxmlstring)                                                                                 | Returns a string with the serialized XML markup for this XML object..                                                                                             |
| [XML](xml.md)             | [valueOf()](xml.md#valueof)                                                                                         | The method simply returns the XML object it is called on..                                                                                                        |

## Properties Details

### ignoreComments

If set to true, then comments in the XML are ignored when constructing new XML objects.

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
var element = <foo><!-- my comment --><bar/></foo>;
application.output(element.comments().length());
application.output(element.toXMLString());

XML.ignoreComments = false;

element = <foo><!-- my comment --><bar/></foo>;
application.output(element.comments().length());
application.output(element.toXMLString());
```

### ignoreProcessingInstructions

If set to true, then processing instructions are ignored when constructing new XML objects.

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
XML.ignoreProcessingInstructions=false;
var xmlElement = <publishing><?process author="yes"?><author type="leadership">John C. Maxwell</author></publishing>;
application.output(" Element = "+ xmlElement.toXMLString());
```

### ignoreWhitespace

If set to true, then whitespace in the XML is ignored when constructing new XML objects.

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
XML.ignoreWhitespace = false;
 var xmlElement =
 <publishing>
 	<author>John C. Maxwell</author>
 </publishing>;
 application.output(xmlElement.toString());
```

### prettyIndent

The amount of positions used when indenting child nodes are relative to their parent if prettyPrinting is enabled.

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
var xmlElement = <publishing><author>Tom DeMarco</author><author>Roger S. Pressman</author></publishing>;
application.output(xmlElement.toXMLString());
XML.prettyPrinting = true;
XML.prettyIndent = 4;
xmlElement = <publishing><author>Tom DeMarco</author><author>Roger S. Pressman</author></publishing>;
application.output(xmlElement.toXMLString());
```

### prettyPrinting

If set to true, then toString() and toXMLString() methods will normalize the output to achieve a uniform appearance.

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
var xmlElement = <publishing><author>Tom DeMarco</author><author>Roger S. Pressman</author></publishing>;
application.output(xmlElement.toXMLString());
XML.prettyPrinting = true;
XML.prettyIndent = 4;
xmlElement = <publishing><author>Tom DeMarco</author><author>Roger S. Pressman</author></publishing>;
application.output(xmlElement.toXMLString());
```

## Methods Details

### addNamespace(namespaceToAdd)

Takes one argument which can be a string with a namespace URI or a Namespace object and adds the argument to the in scope namespaces of this XML object.

**Parameters**\
[String](string.md) namespaceToAdd ;

**Returns**\
[XML](xml.md)

**Sample**

```javascript
xml.addNamespace(namespaceToAdd)
```

### appendChild(childToAppend)

Appends a new child at the end of this XML object's properties, the changed XML object is then returned.

**Parameters**\
[XML](xml.md) childToAppend ;

**Returns**\
[XML](xml.md)

**Sample**

```javascript
xml.appendChild(childToAppend)
```

### attribute(attributeName)

Takes a single argument with the attribute name and returns an XMLList with attributes matching the argument.

**Parameters**\
[String](string.md) attributeName ;

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xml.attribute(attributeName)
```

### attributes()

Returns an XMLList with the attributes of this XML object which are in no namespace.

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xml.attributes()
```

### child(propertyName)

Returns an XMLList with children matching the property name.

**Parameters**\
[String](string.md) propertyName ;

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xml.child(childPropertyName)
```

### childIndex()

If the XML object has no parent then the special number NaN is returned, otherwise the ordinal position the object has in the context of its parent is returned.

**Returns**\
[Number](number.md)

**Sample**

```javascript
xml.childIndex()
```

### children()

Returns an XMLList with the child nodes of this XML object.

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xml.children()
```

### comments()

Returns an XMLList with the comment nodes which are children of this XML object.

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xml.comments()
```

### contains(value)

Calling xmlObject.contains(value) yields the same result as the equality comparison xmlObject == value

**Parameters**\
[Object](object.md) value ;

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
xml.contains(value)
```

### copy()

Returns a deep copy of the XML object it is called on where the internal parent property is set to null

**Returns**\
[XML](xml.md)

**Sample**

```javascript
xml.copy()
```

### defaultSettings()

Returns an object containing the default XML settings.

**Returns**\
[Object](object.md)

**Sample**

```javascript
xml.defaultSettings()
```

### descendants()

Returns an XMLList with the descendants matching the passed name argument or with all descendants if no argument is passed.

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xml.descendants([name])
```

### descendants(name)

Returns an XMLList with the descendants matching the passed name argument or with all descendants if no argument is passed.

**Parameters**\
[String](string.md) name ;

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xml.descendants([name])
```

### elements()

Takes one optional argument, the name of elements you are looking for, and returns an XMLList with all matching child elements.

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xml.elements([name])
```

### elements(name)

Takes one optional argument, the name of elements you are looking for, and returns an XMLList with all matching child elements.

**Parameters**\
[String](string.md) name ;

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xml.elements([name])
```

### hasComplexContent()

Returns false for XML objects of node kind 'text', 'attribute', 'comment', and 'processing-instruction'. For objects of kind 'element' it checks whether the element has at least one child element.

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
xml.hasComplexContent()
```

### hasOwnProperty(propertyName)

Returns true if the XML object the method is called on has a property of that name.

**Parameters**\
[String](string.md) propertyName ;

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
xml.hasOwnProperty(propertyName)
```

### hasSimpleContent()

Returns true for XML objects of node kind text or attribute. For XML objects of node kind element it returns true if the element has no child elements and false otherwise. For other node kinds (comment, processing instruction) the method always returns false.

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
xml.hasSimpleContent()
```

### inScopeNamespaces()

Returns an array of Namespace objects representing the namespace that are in scope for this XML object.

**Returns**\
[Array](array.md)

**Sample**

```javascript
xml.inScopeNamespaces()
```

### insertChildAfter(childToInserAfter, childToInsert)

Takes two arguments, an existing child to insert after and the new child to be inserted. If the first argument is null then the second argument is inserted as the first child of this XML.

**Parameters**\
[XML](xml.md) childToInserAfter ;\
[XML](xml.md) childToInsert ;

**Returns**\
[XML](xml.md)

**Sample**

```javascript
xml.insertChildAfter(childToInsertAfter, childToInsert)
```

### insertChildBefore(childToInsertBefore, childToInsert)

Takes two arguments, an existing child to insert before and the new child to be inserted. If the first argument is null then the child is inserted as the last child.

**Parameters**\
[XML](xml.md) childToInsertBefore ;\
[XML](xml.md) childToInsert ;

**Returns**\
[XML](xml.md)

**Sample**

```javascript
xml.insertChildBefore(childToInsertBefore, childToInsert)
```

### length()

This always returns 1. This is done to blur the distinction between an XML object and an XMLList containing exactly one value.

**Returns**\
[Number](number.md)

**Sample**

```javascript
xml.length()
```

### localName()

returns the local name part if the XML object has a name.

**Returns**\
[String](string.md)

**Sample**

```javascript
xml.localName()
```

### name()

Returns the qualified name (a QName object) of the XML object it is called

**Returns**\
[QName](qname.md)

**Sample**

```javascript
xml.name()
```

### namespace()

If no argument is passed to the method then it returns the namespace associated with the qualified name of this XML object. If a prefix is passed to the method then it looks for a matching namespace in the in scope namespace of this XML object and returns it when found, otherwise undefined is returned.

**Returns**\
[Namespace](namespace.md)

**Sample**

```javascript
xml.namespace([prefix])
```

### namespace(prefix)

If no argument is passed to the method then it returns the namespace associated with the qualified name of this XML object. If a prefix is passed to the method then it looks for a matching namespace in the in scope namespace of this XML object and returns it when found, otherwise undefined is returned.

**Parameters**\
[String](string.md) prefix ;

**Returns**\
[Namespace](namespace.md)

**Sample**

```javascript
xml.namespace([prefix])
```

### namespaceDeclarations()

Returns an array with the namespace declarations associated with the XML object it is called on.

**Returns**\
[Array](array.md)

**Sample**

```javascript
xml.namespaceDeclarations()
```

### nodeKind()

Returns a string denoting the kind of node this XML object represents. Possible values: 'element', 'attribute', 'text', 'comment', 'processing-instruction'.

**Returns**\
[String](string.md)

**Sample**

```javascript
xml.nodeKind()
```

### normalize()

Returns this XML object after normalizing all text content.

**Returns**\
[XML](xml.md)

**Sample**

```javascript
xml.normalize()
```

### parent()

Returns the parent XML object of this XML object or null if there is no parent.

**Returns**\
[XML](xml.md)

**Sample**

```javascript
xml.parent()
```

### prependChild(childToPrepend)

Iinserts the given value as the first child of the XML object and returns the XML object.

**Parameters**\
[XML](xml.md) childToPrepend ;

**Returns**\
[XML](xml.md)

**Sample**

```javascript
xml.prependChild(childToPrepend)
```

### processingInstructions()

If no argument is passed in then the method returns an XMLList with all the children of the XML object which are processing instructions. If an argument is passed in then the method returns an XMLList with all children of the XML object which are processing instructions where the name matches the argument.

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xml.processingInstructions([name])
```

### processingInstructions(name)

If no argument is passed in then the method returns an XMLList with all the children of the XML object which are processing instructions. If an argument is passed in then the method returns an XMLList with all children of the XML object which are processing instructions where the name matches the argument.

**Parameters**\
[String](string.md) name ;

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xml.processingInstructions([name])
```

### propertyIsEnumerable(propertyName)

Returns true if the property name is '0' and false otherwise.

**Parameters**\
[String](string.md) propertyName ;

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
xml.propertyIsEnumerable(propertyName)
```

### removeNamespace(namespace)

Removes the namespace from the in scope namespaces of this XML object if the namespace is not used for the qualified name of the object or its attributes.

**Parameters**\
[Namespace](namespace.md) namespace ;

**Returns**\
[XML](xml.md)

**Sample**

```javascript
xml.removeNamespace(namespace)
```

### replace(propertyName, replacementValue)

Takes two arguments, the property name of the property / properties to be replaced, and the value to replace the properties.

**Parameters**\
[String](string.md) propertyName ;\
[XML](xml.md) replacementValue ;

**Returns**\
[XML](xml.md)

**Sample**

```javascript
xml.replace(propertyName, replacementValue)
```

### setChildren(value)

Replaces all children of the XML object with this value. The method returns the XML object it is called on.

**Parameters**\
[Object](object.md) value ;

**Returns**\
[XML](xml.md)

**Sample**

```javascript
xml.setChildren(value)
```

### setLocalName(name)

Changes the local name of this XML object to the name passed in.

**Parameters**\
[String](string.md) name ;

**Returns**\
void

**Sample**

```javascript
xml.setLocalName(name)
```

### setName(name)

Replaces the name of this XML object with the name passed in.

**Parameters**\
[String](string.md) name ;

**Returns**\
void

**Sample**

```javascript
xml.setName(name)
```

### setNamespace(namespace)

Changes the namespace associated with the name of this XML object to the new namespace.

**Parameters**\
[Namespace](namespace.md) namespace ;

**Returns**\
void

**Sample**

```javascript
xml.setNamespace(namespace)
```

### setSettings()

Allows the global XML settings to be adjusted or restored to their default values.

**Returns**\
void

**Sample**

```javascript
xml.setSettings(settings)
```

### setSettings(settings)

Allows the global XML settings to be adjusted or restored to their default values.

**Parameters**\
[Object](object.md) settings The new settings that should be applied globally to the XML object.

**Returns**\
void

**Sample**

```javascript
xml.setSettings(settings)
```

### settings()

Returns an object containing the global XML settings.

**Returns**\
[Object](object.md)

**Sample**

```javascript
xml.settings()
```

### text()

Returns an XMLList with all the children of this XML object that represent text nodes.

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xml.text()
```

### toString()

Returns a convenient string value of this XML object.

**Returns**\
[String](string.md)

**Sample**

```javascript
xml.toString()
```

### toXMLString()

Returns a string with the serialized XML markup for this XML object. XML.prettyPrinting and XML.prettyIndent settings affect the returned string.

**Returns**\
[String](string.md)

**Sample**

```javascript
xml.toXMLString()
```

### valueOf()

The method simply returns the XML object it is called on.

**Returns**\
[XML](xml.md)

**Sample**

```javascript
xml.valueOf()
```
