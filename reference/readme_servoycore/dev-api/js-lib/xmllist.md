# XMLList

## Methods Summary

| Type                  | Name                                                                               | Summary                                                                                                                                |
| --------------------- | ---------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| [XMLList](xmllist.md) | [attribute(attributeName)](xmllist.md#attribute-attributename)                     | It calls the method attribute of each object in this XMLList and returns the results in order in an XMLList..                          |
| [XMLList](xmllist.md) | [attributes()](xmllist.md#attributes)                                              | Calls the method attributes of each object in this XMLList and returns an XMLList with the results in order..                          |
| [XMLList](xmllist.md) | [child(propertyName)](xmllist.md#child-propertyname)                               | Calls the method child of each XML object in this XMLList object to return an XMLList with the matching children in order..            |
| [XMLList](xmllist.md) | [children()](xmllist.md#children)                                                  | Returns an XMLList with the children of all XML objects in this XMLList..                                                              |
| [XMLList](xmllist.md) | [comments()](xmllist.md#comments)                                                  | Returns an XMLList with all the comment child nodes of XML objects in this XMLList in order..                                          |
| [Boolean](boolean.md) | [contains(value)](xmllist.md#contains-value)                                       | Returns true if there is (at least) one XML object in the list that compares equal to the value.                                       |
| [XMLList](xmllist.md) | [copy()](xmllist.md#copy)                                                          | Returns a deep copy of the XMLList it is called on..                                                                                   |
| [XMLList](xmllist.md) | [descendants()](xmllist.md#descendants)                                            | Returns an XMLList with all of the matching descendants of all XML objects..                                                           |
| [XMLList](xmllist.md) | [descendants(name)](xmllist.md#descendants-name)                                   | Returns an XMLList with all of the matching descendants of all XML objects..                                                           |
| [XMLList](xmllist.md) | [elements(name)](xmllist.md#elements-name)                                         | Returns an XMLList with the matching element children of all XML objects in this XMLList..                                             |
| [Boolean](boolean.md) | [hasComplexContent()](xmllist.md#hascomplexcontent)                                | Returns true if the XMLList contains exactly one XML object which has complex content or if the XMLList contains several XML objects.. |
| [Boolean](boolean.md) | [hasOwnProperty(propertyName)](xmllist.md#hasownproperty-propertyname)             | Returns true if the XMLList object has a property of that name and false otherwise..                                                   |
| [Boolean](boolean.md) | [hasSimpleContent()](xmllist.md#hassimplecontent)                                  | Returns true if the XMLList is empty or contains exactly one XML object which has simple content or contains no elements at all..      |
| [Number](number.md)   | [length()](xmllist.md#length)                                                      | Returns the number of XML objects this XMLList contains..                                                                              |
| [XMLList](xmllist.md) | [normalize()](xmllist.md#normalize)                                                | Returns the XMLList object it is called on after joining adjacent text nodes and removing empty text nodes..                           |
| [XML](xml.md)         | [parent()](xmllist.md#parent)                                                      | Returns the common parent of all XML objects in this XMLList if all those objects have the same parent..                               |
| [XMLList](xmllist.md) | [processingInstructions()](xmllist.md#processinginstructions)                      | Returns an XMLList with all the matching processing instruction child nodes of all XML objects in this XMLList..                       |
| [XMLList](xmllist.md) | [processingInstructions(name)](xmllist.md#processinginstructions-name)             | Returns an XMLList with all the matching processing instruction child nodes of all XML objects in this XMLList..                       |
| [Boolean](boolean.md) | [propertyIsEnumerable(propertyName)](xmllist.md#propertyisenumerable-propertyname) | Returns true if the property name converted to a number is greater than or equal to 0 and less than the length of this XMLList..       |
| [XMLList](xmllist.md) | [text()](xmllist.md#text)                                                          | Returns an XMLList containing all the text child nodes of all the XML objects contained in this XMLList..                              |
| [String](string.md)   | [toString()](xmllist.md#tostring)                                                  | Returns a string representation of the XMLList.                                                                                        |
| [String](string.md)   | [toXMLString()](xmllist.md#toxmlstring)                                            | Returns the concatenation of toXMLString called on each XML object..                                                                   |
| [XMLList](xmllist.md) | [valueOf()](xmllist.md#valueof)                                                    | Simply returns the XMLList object it is called on..                                                                                    |

## Methods Details

### attribute(attributeName)

It calls the method attribute of each object in this XMLList and returns the results in order in an XMLList.

**Parameters**\
[String](string.md) attributeName ;

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xmlList.attribute(attributeName)
```

### attributes()

Calls the method attributes of each object in this XMLList and returns an XMLList with the results in order.

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xmlList.attributes()
```

### child(propertyName)

Calls the method child of each XML object in this XMLList object to return an XMLList with the matching children in order.

**Parameters**\
[String](string.md) propertyName ;

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xmlList.child(propertyName)
```

### children()

Returns an XMLList with the children of all XML objects in this XMLList.

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xmlList.children()
```

### comments()

Returns an XMLList with all the comment child nodes of XML objects in this XMLList in order.

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xmlList.comments()
```

### contains(value)

Returns true if there is (at least) one XML object in the list that compares equal to the value

**Parameters**\
[Object](object.md) value ;

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
xmlList.contains(value)
```

### copy()

Returns a deep copy of the XMLList it is called on.

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xmlList.copy()
```

### descendants()

Returns an XMLList with all of the matching descendants of all XML objects.

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xmlList.descendants([name])
```

### descendants(name)

Returns an XMLList with all of the matching descendants of all XML objects.

**Parameters**\
[String](string.md) name ;

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xmlList.descendants([name])
```

### elements(name)

Returns an XMLList with the matching element children of all XML objects in this XMLList.

**Parameters**\
[String](string.md) name ;

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xmlList.elements([name])
```

### hasComplexContent()

Returns true if the XMLList contains exactly one XML object which has complex content or if the XMLList contains several XML objects.

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
xmlList.hasComplexContent()
```

### hasOwnProperty(propertyName)

Returns true if the XMLList object has a property of that name and false otherwise.

**Parameters**\
[String](string.md) propertyName ;

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
xmlList.hasOwnProperty(propertyName)
```

### hasSimpleContent()

Returns true if the XMLList is empty or contains exactly one XML object which has simple content or contains no elements at all.

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
xmlList.hasSimpleContent()
```

### length()

Returns the number of XML objects this XMLList contains.

**Returns**\
[Number](number.md)

**Sample**

```javascript
xmlList.length()
```

### normalize()

Returns the XMLList object it is called on after joining adjacent text nodes and removing empty text nodes.

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xmlList.normalize()
```

### parent()

Returns the common parent of all XML objects in this XMLList if all those objects have the same parent.

**Returns**\
[XML](xml.md)

**Sample**

```javascript
xmlList.parent()
```

### processingInstructions()

Returns an XMLList with all the matching processing instruction child nodes of all XML objects in this XMLList.

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xmlList.processingInstructions([name])
```

### processingInstructions(name)

Returns an XMLList with all the matching processing instruction child nodes of all XML objects in this XMLList.

**Parameters**\
[String](string.md) name ;

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xmlList.processingInstructions([name])
```

### propertyIsEnumerable(propertyName)

Returns true if the property name converted to a number is greater than or equal to 0 and less than the length of this XMLList.

**Parameters**\
[String](string.md) propertyName ;

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
xmlList.propertyIsEnumerable(propertyName)
```

### text()

Returns an XMLList containing all the text child nodes of all the XML objects contained in this XMLList.

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xmlList.text()
```

### toString()

Returns a string representation of the XMLList

**Returns**\
[String](string.md)

**Sample**

```javascript
xmlList.toString()
```

### toXMLString()

Returns the concatenation of toXMLString called on each XML object. The result for each XML object is put on a separate line if XML.prettyPrinting is true.

**Returns**\
[String](string.md)

**Sample**

```javascript
xmlList.toXMLString()
```

### valueOf()

Simply returns the XMLList object it is called on.

**Returns**\
[XMLList](xmllist.md)

**Sample**

```javascript
xmlList.valueOf()
```
