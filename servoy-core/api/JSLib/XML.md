#  XML


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](./Boolean.md) | [ignoreComments](XML.md#ignoreComments)                   | If set to true, then comments in the XML are ignored when constructing new XML objects..                                    |
| [Boolean](./Boolean.md) | [ignoreProcessingInstructions](XML.md#ignoreProcessingInstructions)                   | If set to true, then processing instructions are ignored when constructing new XML objects..                                    |
| [Boolean](./Boolean.md) | [ignoreWhitespace](XML.md#ignoreWhitespace)                   | If set to true, then whitespace in the XML is ignored when constructing new XML objects..                                    |
| [Boolean](./Boolean.md) | [prettyIndent](XML.md#prettyIndent)                   | The amount of positions used when indenting child nodes are relative to their parent if prettyPrinting is enabled..                                    |
| [Boolean](./Boolean.md) | [prettyPrinting](XML.md#prettyPrinting)                   | If set to true, then toString() and toXMLString() methods will normalize the output to achieve a uniform appearance..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [XML](./XML.md) | [addNamespace(namespaceToAdd)](XML.md#addnamespace-namespacetoadd)                   | Takes one argument which can be a string with a namespace URI or a Namespace object and adds the  argument to the in scope namespaces of this XML object..                                    |
| [XML](./XML.md) | [appendChild(childToAppend)](XML.md#appendchild-childtoappend)                   | Appends a new child at the end of this XML object's properties, the changed XML object is then returned..                                    |
| [XMLList](./XMLList.md) | [attribute(attributeName)](XML.md#attribute-attributename)                   | Takes a single argument with the attribute name and returns an XMLList with attributes  matching the argument..                                    |
| [XMLList](./XMLList.md) | [attributes()](XML.md#attributes)                   | Returns an XMLList with the attributes of this XML object which are in no namespace..                                    |
| [XMLList](./XMLList.md) | [child(propertyName)](XML.md#child-propertyname)                   | Returns an XMLList with children matching the property name..                                    |
| [Number](./Number.md) | [childIndex()](XML.md#childindex)                   | If the XML object has no parent then the special number NaN is returned, otherwise the ordinal  position the object has in the context of its parent is returned..                                    |
| [XMLList](./XMLList.md) | [children()](XML.md#children)                   | Returns an XMLList with the child nodes of this XML object..                                    |
| [XMLList](./XMLList.md) | [comments()](XML.md#comments)                   | Returns an XMLList with the comment nodes which are children of this XML object..                                    |
| [Boolean](./Boolean.md) | [contains(value)](XML.md#contains-value)                   | Calling xmlObject..                                    |
| [XML](./XML.md) | [copy()](XML.md#copy)                   | Returns a deep copy of the XML object it is called on where the internal parent property is set to null.                                    |
| [Object](./Object.md) | [defaultSettings()](XML.md#defaultsettings)                   | Returns an object containing the default XML settings..                                    |
| [XMLList](./XMLList.md) | [descendants()](XML.md#descendants)                   | Returns an XMLList with the descendants matching the passed name argument or with all descendants  if no argument is passed..                                    |
| [XMLList](./XMLList.md) | [descendants(name)](XML.md#descendants-name)                   | Returns an XMLList with the descendants matching the passed name argument or with all descendants  if no argument is passed..                                    |
| [XMLList](./XMLList.md) | [elements()](XML.md#elements)                   | Takes one optional argument, the name of elements you are looking for, and returns an XMLList with  all matching child elements..                                    |
| [XMLList](./XMLList.md) | [elements(name)](XML.md#elements-name)                   | Takes one optional argument, the name of elements you are looking for, and returns an XMLList with  all matching child elements..                                    |
| [Boolean](./Boolean.md) | [hasComplexContent()](XML.md#hascomplexcontent)                   | Returns false for XML objects of node kind 'text', 'attribute', 'comment', and 'processing-instruction'..                                    |
| [Boolean](./Boolean.md) | [hasOwnProperty(propertyName)](XML.md#hasownproperty-propertyname)                   | Returns true if the XML object the method is called on has a property of that name..                                    |
| [Boolean](./Boolean.md) | [hasSimpleContent()](XML.md#hassimplecontent)                   | Returns true for XML objects of node kind text or attribute..                                    |
| [Array](./Array.md) | [inScopeNamespaces()](XML.md#inscopenamespaces)                   | Returns an array of Namespace objects representing the namespace that are in scope for this XML object..                                    |
| [XML](./XML.md) | [insertChildAfter(childToInserAfter, childToInsert)](XML.md#insertchildafter-childtoinserafter-childtoinsert)                   | Takes two arguments, an existing child to insert after and the new child to be inserted..                                    |
| [XML](./XML.md) | [insertChildBefore(childToInsertBefore, childToInsert)](XML.md#insertchildbefore-childtoinsertbefore-childtoinsert)                   | Takes two arguments, an existing child to insert before and the new child to be inserted..                                    |
| [Number](./Number.md) | [length()](XML.md#length)                   | This always returns 1..                                    |
| [String](./String.md) | [localName()](XML.md#localname)                   | returns the local name part if the XML object has a name..                                    |
| [QName](./QName.md) | [name()](XML.md#name)                   | Returns the qualified name (a QName object) of the XML object it is called.                                    |
| [Namespace](./Namespace.md) | [namespace()](XML.md#namespace)                   | If no argument is passed to the method then it returns the namespace associated with the qualified  name of this XML object..                                    |
| [Namespace](./Namespace.md) | [namespace(prefix)](XML.md#namespace-prefix)                   | If no argument is passed to the method then it returns the namespace associated with the qualified  name of this XML object..                                    |
| [Array](./Array.md) | [namespaceDeclarations()](XML.md#namespacedeclarations)                   | Returns an array with the namespace declarations associated with the XML object it is called on..                                    |
| [String](./String.md) | [nodeKind()](XML.md#nodekind)                   | Returns a string denoting the kind of node this XML object represents..                                    |
| [XML](./XML.md) | [normalize()](XML.md#normalize)                   | Returns this XML object after normalizing all text content..                                    |
| [XML](./XML.md) | [parent()](XML.md#parent)                   | Returns the parent XML object of this XML object or null if there is no parent..                                    |
| [XML](./XML.md) | [prependChild(childToPrepend)](XML.md#prependchild-childtoprepend)                   | Iinserts the given value as the first child of the XML object and returns the XML object..                                    |
| [XMLList](./XMLList.md) | [processingInstructions()](XML.md#processinginstructions)                   | If no argument is passed in then the method returns an XMLList with all the children of the XML  object which are processing instructions..                                    |
| [XMLList](./XMLList.md) | [processingInstructions(name)](XML.md#processinginstructions-name)                   | If no argument is passed in then the method returns an XMLList with all the children of the XML  object which are processing instructions..                                    |
| [Boolean](./Boolean.md) | [propertyIsEnumerable(propertyName)](XML.md#propertyisenumerable-propertyname)                   | Returns true if the property name is '0' and false otherwise..                                    |
| [XML](./XML.md) | [removeNamespace(namespace)](XML.md#removenamespace-namespace)                   | Removes the namespace from the in scope namespaces of this XML object if the namespace  is not used for the qualified name of the object or its attributes..                                    |
| [XML](./XML.md) | [replace(propertyName, replacementValue)](XML.md#replace-propertyname-replacementvalue)                   | Takes two arguments, the property name of the property / properties to be replaced, and the  value to replace the properties..                                    |
| [XML](./XML.md) | [setChildren(value)](XML.md#setchildren-value)                   | Replaces all children of the XML object with this value..                                    |
|void | [setLocalName(name)](XML.md#setlocalname-name)                   | Changes the local name of this XML object to the name passed in..                                    |
|void | [setName(name)](XML.md#setname-name)                   | Replaces the name of this XML object with the name passed in..                                    |
|void | [setNamespace(namespace)](XML.md#setnamespace-namespace)                   | Changes the namespace associated with the name of this XML object to the new namespace..                                    |
|void | [setSettings()](XML.md#setsettings)                   | Allows the global XML settings to be adjusted or restored to their default values..                                    |
|void | [setSettings(settings)](XML.md#setsettings-settings)                   | Allows the global XML settings to be adjusted or restored to their default values..                                    |
| [Object](./Object.md) | [settings()](XML.md#settings)                   | Returns an object containing the global XML settings..                                    |
| [XMLList](./XMLList.md) | [text()](XML.md#text)                   | Returns an XMLList with all the children of this XML object that represent text nodes..                                    |
| [String](./String.md) | [toString()](XML.md#tostring)                   | Returns a convenient string value of this XML object..                                    |
| [String](./String.md) | [toXMLString()](XML.md#toxmlstring)                   | Returns a string with the serialized XML markup for this XML object..                                    |
| [XML](./XML.md) | [valueOf()](XML.md#valueof)                   | The method simply returns the XML object it is called on..                                    |

## Properties Details

### ignoreComments

If set to true, then comments in the XML are ignored when constructing new XML objects.

**Returns**\
[Boolean](./Boolean.md) 


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
[Boolean](./Boolean.md) 


**Sample**

```javascript
XML.ignoreProcessingInstructions=false;
var xmlElement = <publishing><?process author="yes"?><author type="leadership">John C. Maxwell</author></publishing>;
application.output(" Element = "+ xmlElement.toXMLString());
```
### ignoreWhitespace

If set to true, then whitespace in the XML is ignored when constructing new XML objects.

**Returns**\
[Boolean](./Boolean.md) 


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

The amount of positions used when indenting child nodes are relative to their parent
if prettyPrinting is enabled.

**Returns**\
[Boolean](./Boolean.md) 


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

If set to true, then toString() and toXMLString() methods will normalize the output
to achieve a uniform appearance.

**Returns**\
[Boolean](./Boolean.md) 


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

Takes one argument which can be a string with a namespace URI or a Namespace object and adds the 
argument to the in scope namespaces of this XML object.

**Parameters**\
[String](./String.md) namespaceToAdd  ;

**Returns**\
[XML](./XML.md) 


**Sample**

```javascript
xml.addNamespace(namespaceToAdd)
```
### appendChild(childToAppend)

Appends a new child at the end of this XML object's properties, the changed XML object is then returned.

**Parameters**\
[XML](./XML.md) childToAppend  ;

**Returns**\
[XML](./XML.md) 


**Sample**

```javascript
xml.appendChild(childToAppend)
```
### attribute(attributeName)

Takes a single argument with the attribute name and returns an XMLList with attributes 
matching the argument.

**Parameters**\
[String](./String.md) attributeName  ;

**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xml.attribute(attributeName)
```
### attributes()

Returns an XMLList with the attributes of this XML object which are in no namespace.


**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xml.attributes()
```
### child(propertyName)

Returns an XMLList with children matching the property name.

**Parameters**\
[String](./String.md) propertyName  ;

**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xml.child(childPropertyName)
```
### childIndex()

If the XML object has no parent then the special number NaN is returned, otherwise the ordinal 
position the object has in the context of its parent is returned.


**Returns**\
[Number](./Number.md) 


**Sample**

```javascript
xml.childIndex()
```
### children()

Returns an XMLList with the child nodes of this XML object.


**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xml.children()
```
### comments()

Returns an XMLList with the comment nodes which are children of this XML object.


**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xml.comments()
```
### contains(value)

Calling xmlObject.contains(value) yields the same result as the equality comparison xmlObject == value

**Parameters**\
[Object](./Object.md) value  ;

**Returns**\
[Boolean](./Boolean.md) 


**Sample**

```javascript
xml.contains(value)
```
### copy()

Returns a deep copy of the XML object it is called on where the internal parent property is set to null


**Returns**\
[XML](./XML.md) 


**Sample**

```javascript
xml.copy()
```
### defaultSettings()

Returns an object containing the default XML settings.


**Returns**\
[Object](./Object.md) 


**Sample**

```javascript
xml.defaultSettings()
```
### descendants()

Returns an XMLList with the descendants matching the passed name argument or with all descendants 
if no argument is passed.


**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xml.descendants([name])
```
### descendants(name)

Returns an XMLList with the descendants matching the passed name argument or with all descendants 
if no argument is passed.

**Parameters**\
[String](./String.md) name  ;

**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xml.descendants([name])
```
### elements()

Takes one optional argument, the name of elements you are looking for, and returns an XMLList with 
all matching child elements.


**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xml.elements([name])
```
### elements(name)

Takes one optional argument, the name of elements you are looking for, and returns an XMLList with 
all matching child elements.

**Parameters**\
[String](./String.md) name  ;

**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xml.elements([name])
```
### hasComplexContent()

Returns false for XML objects of node kind 'text', 'attribute', 'comment', and 'processing-instruction'.
For objects of kind 'element' it checks whether the element has at least one child element.


**Returns**\
[Boolean](./Boolean.md) 


**Sample**

```javascript
xml.hasComplexContent()
```
### hasOwnProperty(propertyName)

Returns true if the XML object the method is called on has a property of that name.

**Parameters**\
[String](./String.md) propertyName  ;

**Returns**\
[Boolean](./Boolean.md) 


**Sample**

```javascript
xml.hasOwnProperty(propertyName)
```
### hasSimpleContent()

Returns true for XML objects of node kind text or attribute. For XML objects of node kind 
element it returns true if the element has no child elements and false otherwise.
For other node kinds (comment, processing instruction) the method always returns false.


**Returns**\
[Boolean](./Boolean.md) 


**Sample**

```javascript
xml.hasSimpleContent()
```
### inScopeNamespaces()

Returns an array of Namespace objects representing the namespace that are in scope for this XML object.


**Returns**\
[Array](./Array.md) 


**Sample**

```javascript
xml.inScopeNamespaces()
```
### insertChildAfter(childToInserAfter, childToInsert)

Takes two arguments, an existing child to insert after and the new child to be inserted.
If the first argument is null then the second argument is inserted as the first child of this XML.

**Parameters**\
[XML](./XML.md) childToInserAfter  ;\
[XML](./XML.md) childToInsert  ;

**Returns**\
[XML](./XML.md) 


**Sample**

```javascript
xml.insertChildAfter(childToInsertAfter, childToInsert)
```
### insertChildBefore(childToInsertBefore, childToInsert)

Takes two arguments, an existing child to insert before and the new child to be inserted.
If the first argument is null then the child is inserted as the last child.

**Parameters**\
[XML](./XML.md) childToInsertBefore  ;\
[XML](./XML.md) childToInsert  ;

**Returns**\
[XML](./XML.md) 


**Sample**

```javascript
xml.insertChildBefore(childToInsertBefore, childToInsert)
```
### length()

This always returns 1. This is done to blur the distinction between an XML object and an XMLList 
containing exactly one value.


**Returns**\
[Number](./Number.md) 


**Sample**

```javascript
xml.length()
```
### localName()

returns the local name part if the XML object has a name.


**Returns**\
[String](./String.md) 


**Sample**

```javascript
xml.localName()
```
### name()

Returns the qualified name (a QName object) of the XML object it is called


**Returns**\
[QName](./QName.md) 


**Sample**

```javascript
xml.name()
```
### namespace()

If no argument is passed to the method then it returns the namespace associated with the qualified 
name of this XML object. If a prefix is passed to the method then it looks for a matching namespace 
in the in scope namespace of this XML object and returns it when found, otherwise undefined is returned.


**Returns**\
[Namespace](./Namespace.md) 


**Sample**

```javascript
xml.namespace([prefix])
```
### namespace(prefix)

If no argument is passed to the method then it returns the namespace associated with the qualified 
name of this XML object. If a prefix is passed to the method then it looks for a matching namespace 
in the in scope namespace of this XML object and returns it when found, otherwise undefined is returned.

**Parameters**\
[String](./String.md) prefix  ;

**Returns**\
[Namespace](./Namespace.md) 


**Sample**

```javascript
xml.namespace([prefix])
```
### namespaceDeclarations()

Returns an array with the namespace declarations associated with the XML object it is called on.


**Returns**\
[Array](./Array.md) 


**Sample**

```javascript
xml.namespaceDeclarations()
```
### nodeKind()

Returns a string denoting the kind of node this XML object represents. Possible values: 'element', 
'attribute', 'text', 'comment', 'processing-instruction'.


**Returns**\
[String](./String.md) 


**Sample**

```javascript
xml.nodeKind()
```
### normalize()

Returns this XML object after normalizing all text content.


**Returns**\
[XML](./XML.md) 


**Sample**

```javascript
xml.normalize()
```
### parent()

Returns the parent XML object of this XML object or null if there is no parent.


**Returns**\
[XML](./XML.md) 


**Sample**

```javascript
xml.parent()
```
### prependChild(childToPrepend)

Iinserts the given value as the first child of the XML object and returns the XML object.

**Parameters**\
[XML](./XML.md) childToPrepend  ;

**Returns**\
[XML](./XML.md) 


**Sample**

```javascript
xml.prependChild(childToPrepend)
```
### processingInstructions()

If no argument is passed in then the method returns an XMLList with all the children of the XML 
object which are processing instructions. If an argument is passed in then the method returns an 
XMLList with all children of the XML object which are processing instructions where the name 
matches the argument.


**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xml.processingInstructions([name])
```
### processingInstructions(name)

If no argument is passed in then the method returns an XMLList with all the children of the XML 
object which are processing instructions. If an argument is passed in then the method returns an 
XMLList with all children of the XML object which are processing instructions where the name 
matches the argument.

**Parameters**\
[String](./String.md) name  ;

**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xml.processingInstructions([name])
```
### propertyIsEnumerable(propertyName)

Returns true if the property name is '0' and false otherwise.

**Parameters**\
[String](./String.md) propertyName  ;

**Returns**\
[Boolean](./Boolean.md) 


**Sample**

```javascript
xml.propertyIsEnumerable(propertyName)
```
### removeNamespace(namespace)

Removes the namespace from the in scope namespaces of this XML object if the namespace 
is not used for the qualified name of the object or its attributes.

**Parameters**\
[Namespace](./Namespace.md) namespace  ;

**Returns**\
[XML](./XML.md) 


**Sample**

```javascript
xml.removeNamespace(namespace)
```
### replace(propertyName, replacementValue)

Takes two arguments, the property name of the property / properties to be replaced, and the 
value to replace the properties.

**Parameters**\
[String](./String.md) propertyName  ;\
[XML](./XML.md) replacementValue  ;

**Returns**\
[XML](./XML.md) 


**Sample**

```javascript
xml.replace(propertyName, replacementValue)
```
### setChildren(value)

Replaces all children of the XML object with this value. The method returns the XML object it 
is called on.

**Parameters**\
[Object](./Object.md) value  ;

**Returns**\
[XML](./XML.md) 


**Sample**

```javascript
xml.setChildren(value)
```
### setLocalName(name)

Changes the local name of this XML object to the name passed in.

**Parameters**\
[String](./String.md) name  ;

**Returns**\
void 


**Sample**

```javascript
xml.setLocalName(name)
```
### setName(name)

Replaces the name of this XML object with the name passed in.

**Parameters**\
[String](./String.md) name  ;

**Returns**\
void 


**Sample**

```javascript
xml.setName(name)
```
### setNamespace(namespace)

Changes the namespace associated with the name of this XML object to the new namespace.

**Parameters**\
[Namespace](./Namespace.md) namespace  ;

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
[Object](./Object.md) settings The new settings that should be applied globally to the XML object.

**Returns**\
void 


**Sample**

```javascript
xml.setSettings(settings)
```
### settings()

Returns an object containing the global XML settings.


**Returns**\
[Object](./Object.md) 


**Sample**

```javascript
xml.settings()
```
### text()

Returns an XMLList with all the children of this XML object that represent text nodes.


**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xml.text()
```
### toString()

Returns a convenient string value of this XML object.


**Returns**\
[String](./String.md) 


**Sample**

```javascript
xml.toString()
```
### toXMLString()

Returns a string with the serialized XML markup for this XML object. XML.prettyPrinting 
and XML.prettyIndent settings affect the returned string.


**Returns**\
[String](./String.md) 


**Sample**

```javascript
xml.toXMLString()
```
### valueOf()

The method simply returns the XML object it is called on.


**Returns**\
[XML](./XML.md) 


**Sample**

```javascript
xml.valueOf()
```

