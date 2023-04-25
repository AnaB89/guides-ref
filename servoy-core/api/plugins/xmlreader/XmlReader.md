#  XmlReader

## **Return Types**
[XmlNode](./XmlNode.md),

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Array](../../JSLib/Array.md) | [readXmlDocumentFromFile(argument)](XmlReader.md#readxmldocumentfromfile-argument)                   | Reads an XML document from a file..                                    |
| [Array](../../JSLib/Array.md) | [readXmlDocumentFromString(argument)](XmlReader.md#readxmldocumentfromstring-argument)                   | Reads an XML document from a string..                                    |

## Methods Details

### readXmlDocumentFromFile(argument)

Reads an XML document from a file.

**Parameters**\
[Object](../../JSLib/Object.md) argument  ;

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
// specifies a reference to a file containing valid XML
var xmlNodes = plugins.XmlReader.readXmlDocumentFromFile('c:/test.xml');
var childNodes = xmlNodes[0].getChildNodes();
// shows a dialog to open an xml file, then reads the file
var xmlFile = plugins.file.showFileOpenDialog(1);
var xmlNodes = plugins.XmlReader.readXmlDocumentFromFile(xmlFile);
var childNodes = xmlNodes[0].getChildNodes();
```
### readXmlDocumentFromString(argument)

Reads an XML document from a string.

**Parameters**\
[String](../../JSLib/String.md) argument  ;

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
var xmlString = '<books><book price="44.95">' +
'<title>Core Java 1.5</title>' +
'<author>Piet Klerksen</author>' +
'<nrPages>1487</nrPages>' +
'</book>' +
'<book price="59.95">' +
'<title>Developing with Servoy</title>' +
'<author>Cheryl Owens and others</author><nrPages>492</nrPages></book></books>';
var xmlNodes = plugins.XmlReader.readXmlDocumentFromString(xmlString);
```

