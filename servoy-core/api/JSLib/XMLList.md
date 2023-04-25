#  XMLList


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [XMLList](./XMLList.md) | [attribute(attributeName)](XMLList.md#attribute-attributename)                   | It calls the method attribute of each object in this XMLList and returns the results in order  in an XMLList..                                    |
| [XMLList](./XMLList.md) | [attributes()](XMLList.md#attributes)                   | Calls the method attributes of each object in this XMLList and returns an XMLList with  the results in order..                                    |
| [XMLList](./XMLList.md) | [child(propertyName)](XMLList.md#child-propertyname)                   | Calls the method child of each XML object in this XMLList object to return an XMLList  with the matching children in order..                                    |
| [XMLList](./XMLList.md) | [children()](XMLList.md#children)                   | Returns an XMLList with the children of all XML objects in this XMLList..                                    |
| [XMLList](./XMLList.md) | [comments()](XMLList.md#comments)                   | Returns an XMLList with all the comment child nodes of XML objects in this XMLList in order..                                    |
| [Boolean](./Boolean.md) | [contains(value)](XMLList.md#contains-value)                   | Returns true if there is (at least) one XML object in the list that compares equal to the value.                                    |
| [XMLList](./XMLList.md) | [copy()](XMLList.md#copy)                   | Returns a deep copy of the XMLList it is called on..                                    |
| [XMLList](./XMLList.md) | [descendants()](XMLList.md#descendants)                   | Returns an XMLList with all of the matching descendants of all XML objects..                                    |
| [XMLList](./XMLList.md) | [descendants(name)](XMLList.md#descendants-name)                   | Returns an XMLList with all of the matching descendants of all XML objects..                                    |
| [XMLList](./XMLList.md) | [elements(name)](XMLList.md#elements-name)                   | Returns an XMLList with the matching element children of all XML objects in this XMLList..                                    |
| [Boolean](./Boolean.md) | [hasComplexContent()](XMLList.md#hascomplexcontent)                   | Returns true if the XMLList contains exactly one XML object which has complex content or if  the XMLList contains several XML objects..                                    |
| [Boolean](./Boolean.md) | [hasOwnProperty(propertyName)](XMLList.md#hasownproperty-propertyname)                   | Returns true if the XMLList object has a property of that name and false otherwise..                                    |
| [Boolean](./Boolean.md) | [hasSimpleContent()](XMLList.md#hassimplecontent)                   | Returns true if the XMLList is empty or contains exactly one XML object which has simple  content or contains no elements at all..                                    |
| [Number](./Number.md) | [length()](XMLList.md#length)                   | Returns the number of XML objects this XMLList contains..                                    |
| [XMLList](./XMLList.md) | [normalize()](XMLList.md#normalize)                   | Returns the XMLList object it is called on after joining adjacent text nodes  and removing empty text nodes..                                    |
| [XML](./XML.md) | [parent()](XMLList.md#parent)                   | Returns the common parent of all XML objects in this XMLList if all those objects  have the same parent..                                    |
| [XMLList](./XMLList.md) | [processingInstructions()](XMLList.md#processinginstructions)                   | Returns an XMLList with all the matching processing instruction child nodes of all  XML objects in this XMLList..                                    |
| [XMLList](./XMLList.md) | [processingInstructions(name)](XMLList.md#processinginstructions-name)                   | Returns an XMLList with all the matching processing instruction child nodes of all  XML objects in this XMLList..                                    |
| [Boolean](./Boolean.md) | [propertyIsEnumerable(propertyName)](XMLList.md#propertyisenumerable-propertyname)                   | Returns true if the property name converted to a number is greater than or equal to  0 and less than the length of this XMLList..                                    |
| [XMLList](./XMLList.md) | [text()](XMLList.md#text)                   | Returns an XMLList containing all the text child nodes of all the XML objects contained in this XMLList..                                    |
| [String](./String.md) | [toString()](XMLList.md#tostring)                   | Returns a string representation of the XMLList.                                    |
| [String](./String.md) | [toXMLString()](XMLList.md#toxmlstring)                   | Returns the concatenation of toXMLString called on each XML object..                                    |
| [XMLList](./XMLList.md) | [valueOf()](XMLList.md#valueof)                   | Simply returns the XMLList object it is called on..                                    |

## Methods Details

### attribute(attributeName)

It calls the method attribute of each object in this XMLList and returns the results in order 
in an XMLList.

**Parameters**\
[String](./String.md) attributeName  ;

**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xmlList.attribute(attributeName)
```
### attributes()

Calls the method attributes of each object in this XMLList and returns an XMLList with 
the results in order.


**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xmlList.attributes()
```
### child(propertyName)

Calls the method child of each XML object in this XMLList object to return an XMLList 
with the matching children in order.

**Parameters**\
[String](./String.md) propertyName  ;

**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xmlList.child(propertyName)
```
### children()

Returns an XMLList with the children of all XML objects in this XMLList.


**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xmlList.children()
```
### comments()

Returns an XMLList with all the comment child nodes of XML objects in this XMLList in order.


**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xmlList.comments()
```
### contains(value)

Returns true if there is (at least) one XML object in the list that compares equal to the value

**Parameters**\
[Object](./Object.md) value  ;

**Returns**\
[Boolean](./Boolean.md) 


**Sample**

```javascript
xmlList.contains(value)
```
### copy()

Returns a deep copy of the XMLList it is called on.


**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xmlList.copy()
```
### descendants()

Returns an XMLList with all of the matching descendants of all XML objects.


**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xmlList.descendants([name])
```
### descendants(name)

Returns an XMLList with all of the matching descendants of all XML objects.

**Parameters**\
[String](./String.md) name  ;

**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xmlList.descendants([name])
```
### elements(name)

Returns an XMLList with the matching element children of all XML objects in this XMLList.

**Parameters**\
[String](./String.md) name  ;

**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xmlList.elements([name])
```
### hasComplexContent()

Returns true if the XMLList contains exactly one XML object which has complex content or if 
the XMLList contains several XML objects.


**Returns**\
[Boolean](./Boolean.md) 


**Sample**

```javascript
xmlList.hasComplexContent()
```
### hasOwnProperty(propertyName)

Returns true if the XMLList object has a property of that name and false otherwise.

**Parameters**\
[String](./String.md) propertyName  ;

**Returns**\
[Boolean](./Boolean.md) 


**Sample**

```javascript
xmlList.hasOwnProperty(propertyName)
```
### hasSimpleContent()

Returns true if the XMLList is empty or contains exactly one XML object which has simple 
content or contains no elements at all.


**Returns**\
[Boolean](./Boolean.md) 


**Sample**

```javascript
xmlList.hasSimpleContent()
```
### length()

Returns the number of XML objects this XMLList contains.


**Returns**\
[Number](./Number.md) 


**Sample**

```javascript
xmlList.length()
```
### normalize()

Returns the XMLList object it is called on after joining adjacent text nodes 
and removing empty text nodes.


**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xmlList.normalize()
```
### parent()

Returns the common parent of all XML objects in this XMLList if all those objects 
have the same parent.


**Returns**\
[XML](./XML.md) 


**Sample**

```javascript
xmlList.parent()
```
### processingInstructions()

Returns an XMLList with all the matching processing instruction child nodes of all 
XML objects in this XMLList.


**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xmlList.processingInstructions([name])
```
### processingInstructions(name)

Returns an XMLList with all the matching processing instruction child nodes of all 
XML objects in this XMLList.

**Parameters**\
[String](./String.md) name  ;

**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xmlList.processingInstructions([name])
```
### propertyIsEnumerable(propertyName)

Returns true if the property name converted to a number is greater than or equal to 
0 and less than the length of this XMLList.

**Parameters**\
[String](./String.md) propertyName  ;

**Returns**\
[Boolean](./Boolean.md) 


**Sample**

```javascript
xmlList.propertyIsEnumerable(propertyName)
```
### text()

Returns an XMLList containing all the text child nodes of all the XML objects contained in this XMLList.


**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xmlList.text()
```
### toString()

Returns a string representation of the XMLList


**Returns**\
[String](./String.md) 


**Sample**

```javascript
xmlList.toString()
```
### toXMLString()

Returns the concatenation of toXMLString called on each XML object. The result for each XML 
object is put on a separate line if XML.prettyPrinting is true.


**Returns**\
[String](./String.md) 


**Sample**

```javascript
xmlList.toXMLString()
```
### valueOf()

Simply returns the XMLList object it is called on.


**Returns**\
[XMLList](./XMLList.md) 


**Sample**

```javascript
xmlList.valueOf()
```

