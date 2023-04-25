# Word

The office365Word service enables the [Javascript API for a Word](https://dev.office.com/reference/add-ins/javascript-api-for-office?product=word) Office document.

## Word API

| Method                                     | Params                                                                              | Return  | Description                                                                                                                                                                   |
| ------------------------------------------ | ----------------------------------------------------------------------------------- | ------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| isOfficeEnabled                            |                                                                                     | Boolean | Returns true if Office API are correctly enabled.                                                                                                                             |
| getDownloadUrl                             |                                                                                     | String  | Returns the url to download the document.                                                                                                                                     |
| getDocumentUrl                             |                                                                                     | String  | Returns the url to the online document.                                                                                                                                       |
| getSelectedData                            | [coercionType](Word.md#coerciontype):String, onError:Function                       | Object  | Returns the selected data. The coercionType should match the selected data; if the selectedData is a table coercionType should be 'matrix' coercionType is 'text' by default. |
| [setSelectedData](Word.md#setselecteddata) | text:String, [coercionType](Word.md#coerciontype):String, onError:Function          | Boolean | Set data into the current selection.                                                                                                                                          |
| selectBody                                 | [selectionMode](Word.md#selectionmode):String, onError:Function                     | Boolean | Set selection in the body. Default selectionMode 'select'.                                                                                                                    |
| getBodyText                                | loadOptions:Object, onError:Function                                                | String  | Returns the body of the document as a text.                                                                                                                                   |
| getBodyOoxml                               | onError:Function                                                                    | String  | Returns the body of the document as a Ooxml.                                                                                                                                  |
| getBodyHtml                                | onError:Function                                                                    | String  | Returns the body of the document as HTML.                                                                                                                                     |
| insertTextToBody                           | text:String, [insertLocation](Word.md#insertlocation):String, onError:Function      | Boolean | Inserts text at the given location. Default insertLocation 'end'.                                                                                                             |
| insertHtmlToBody                           | htmlText:String, [insertLocation](Word.md#insertlocation):String, onError:Function  | Boolean | Inserts text at the given location. Default insertLocation 'end'.                                                                                                             |
| insertOoxmlToBody                          | ooxmlText:String, [insertLocation](Word.md#insertlocation):String, onError:Function | Boolean | Inserts the ooxml at the given location. Default insertLocation 'end'.                                                                                                        |

### setSelectedData

**Params**

| Type     | Name         | Description                                              | Required                  |
| -------- | ------------ | -------------------------------------------------------- | ------------------------- |
| String   | text         | the id of the menu item.                                 | Required                  |
| String   | coercionType | The coercionType of the data inserted into the document. | Optional, Default 'text'. |
| Function | onError      | The onError handler invoked in case of error.            | Optional.                 |

**Returns** Boolean

Set data into the current selection.

Example

```
// write plain text into the document
plugins.office365Word.setSelectedData("Hello Word", scopes.office365.COERCION_TYPE.TEXT, onError);


// write a JSDataSet as a matrix into the document
var query = "select productname, unitsinstock from products"
var ds = databaseManager.getDataSetByQuery("example_data", query, [], -1);
var matrix = [];
for (var i = 1; i <= ds.getMaxRowIndex(); i++) {
	matrix.push(ds.getRowAsArray(i));
}
plugins.office365Word.setSelectedData(matrix, scopes.office365.COERCION_TYPE.MATRIX, onError);

function onError(error) {
    application.output(error);
}
```

## Enumerations

#### selectionMode

| Value  | Description                         |
| ------ | ----------------------------------- |
| end    | Go at the end of the content.       |
| select | Select the whole the content.       |
| start  | Go at the beginning of the content. |

#### insertLocation

| Value   | Description              |
| ------- | ------------------------ |
| end     | Insert at the end.       |
| replace | Replace the content.     |
| start   | Insert at the beginning. |

#### coercionType

| Value  | Description                                                                                                                                      |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| html   | Return or set data as HTML.                                                                                                                      |
| image  | Data is returned or set as an image stream.                                                                                                      |
| matrix | Return or set data as tabular data with no headers. Data is returned or set as an array of arrays containing one-dimensional runs of characters. |
| table  | Return or set data as tabular data with optional headers. Data is returned or set as an array of arrays with optional headers.                   |
| ooxml  | Return or set data as Office Open XML.                                                                                                           |
| text   | Return or set data as text (string).Data is returned or set as a one-dimensional run of characters.                                              |
