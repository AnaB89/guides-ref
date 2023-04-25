#  JSDataSet

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [rowIndex](JSDataSet.md#rowIndex)                   | Get or set the record index of the dataset..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../JSLib/Boolean.md) | [addColumn(name)](JSDataSet.md#addcolumn-name)                   | adds a column with the specified name to the dataset..                                    |
| [Boolean](../JSLib/Boolean.md) | [addColumn(name, index)](JSDataSet.md#addcolumn-name-index)                   | adds a column with the specified name to the dataset..                                    |
| [Boolean](../JSLib/Boolean.md) | [addColumn(name, index, type)](JSDataSet.md#addcolumn-name-index-type)                   | adds a column with the specified name to the dataset..                                    |
|void | [addHTMLProperty(row, col, name, value)](JSDataSet.md#addhtmlproperty-row-col-name-value)                   | Add an HTML property to an HTML tag produced in getAsHTML()..                                    |
|void | [addRow(index, array)](JSDataSet.md#addrow-index-array)                   | Add a row to the dataset..                                    |
|void | [addRow(array)](JSDataSet.md#addrow-array)                   | Add a row to the dataset..                                    |
| [String](../JSLib/String.md) | [createDataSource(name)](JSDataSet.md#createdatasource-name)                   | Create a datasource from the data set with specified name and using specified types..                                    |
| [String](../JSLib/String.md) | [createDataSource(name, types)](JSDataSet.md#createdatasource-name-types)                   | Create a datasource from the data set with specified name and using specified types..                                    |
| [String](../JSLib/String.md) | [createDataSource(name, types, pkNames)](JSDataSet.md#createdatasource-name-types-pknames)                   | Create a datasource from the data set with specified name and using specified types..                                    |
| [String](../JSLib/String.md) | [getAsHTML()](JSDataSet.md#getashtml)                   | Get the dataset as an html table, do not escape values or spaces, no multi_line_markup, do not add indentation, add column names..                                    |
| [String](../JSLib/String.md) | [getAsHTML(escape_values)](JSDataSet.md#getashtml-escape_values)                   | Get the dataset as an html table, do not escape spaces, no multi_line_markup, do not add indentation, add column names..                                    |
| [String](../JSLib/String.md) | [getAsHTML(escape_values, escape_spaces)](JSDataSet.md#getashtml-escape_values-escape_spaces)                   | Get the dataset as an html table, no multi_line_markup, do not add indentation, add column names..                                    |
| [String](../JSLib/String.md) | [getAsHTML(escape_values, escape_spaces, multi_line_markup)](JSDataSet.md#getashtml-escape_values-escape_spaces-multi_line_markup)                   | Get the dataset as an html table, do not add indentation, add column names..                                    |
| [String](../JSLib/String.md) | [getAsHTML(escape_values, escape_spaces, multi_line_markup, pretty_indent)](JSDataSet.md#getashtml-escape_values-escape_spaces-multi_line_markup-pretty_indent)                   | Get the dataset as an html table, add column names..                                    |
| [String](../JSLib/String.md) | [getAsHTML(escape_values, escape_spaces, multi_line_markup, pretty_indent, add_column_names)](JSDataSet.md#getashtml-escape_values-escape_spaces-multi_line_markup-pretty_indent-add_column_names)                   | Get the dataset as an html table..                                    |
| [String](../JSLib/String.md) | [getAsText(column_separator, row_separator, value_delimiter, add_column_names)](JSDataSet.md#getastext-column_separator-row_separator-value_delimiter-add_column_names)                   | Get the dataset as formatted text..                                    |
| [Array](../JSLib/Array.md) | [getColumnAsArray(index)](JSDataSet.md#getcolumnasarray-index)                   | Get the column data of a dataset as an Array..                                    |
| [String](../JSLib/String.md) | [getColumnName(index)](JSDataSet.md#getcolumnname-index)                   | Get a column name based on index..                                    |
| [Array](../JSLib/Array.md) | [getColumnNames()](JSDataSet.md#getcolumnnames)                   | Get the column names of a dataset..                                    |
| [Number](../JSLib/Number.md) | [getColumnType(index)](JSDataSet.md#getcolumntype-index)                   | Get a column type based on index..                                    |
| [Exception](../Exception.md) | [getException()](JSDataSet.md#getexception)                   | Get the database exception if an error occurred..                                    |
| [Number](../JSLib/Number.md) | [getMaxColumnIndex()](JSDataSet.md#getmaxcolumnindex)                   | Get the number of columns in the dataset..                                    |
| [Number](../JSLib/Number.md) | [getMaxRowIndex()](JSDataSet.md#getmaxrowindex)                   | Get the number of rows in the dataset..                                    |
| [Array](../JSLib/Array.md) | [getRowAsArray(index)](JSDataSet.md#getrowasarray-index)                   | Get the row data of a dataset as an Array..                                    |
| [Object](../JSLib/Object.md) | [getValue(row, col)](JSDataSet.md#getvalue-row-col)                   | Get the value specified by row and column position from the dataset..                                    |
| [Boolean](../JSLib/Boolean.md) | [hadMoreData()](JSDataSet.md#hadmoredata)                   | Return true if there is more data in the resultset then specified by maxReturnedRows at query time..                                    |
| [Boolean](../JSLib/Boolean.md) | [removeColumn(index)](JSDataSet.md#removecolumn-index)                   | Remove a column by index from the dataset..                                    |
|void | [removeRow(row)](JSDataSet.md#removerow-row)                   | Remove a row from the dataset..                                    |
|void | [setColumnName(index, columnName)](JSDataSet.md#setcolumnname-index-columnname)                   | Set a column name based on index..                                    |
|void | [setValue(row, col, obj)](JSDataSet.md#setvalue-row-col-obj)                   | Set the value specified by row and column position from the dataset..                                    |
|void | [sort(col, sort_direction)](JSDataSet.md#sort-col-sort_direction)                   | Sort the dataset on the given column (1-based) in ascending or descending..                                    |
|void | [sort(comparator)](JSDataSet.md#sort-comparator)                   | Sort the dataset using the function as comparator..                                    |

## Properties Details

### rowIndex

Get or set the record index of the dataset.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
//to set the rowIndex:
dataset.rowIndex = 1 //sets the rowIndex to the first row (dataset is 1-based)
//to retrieve the rowIndex of the currently selected row
var currRow = dataset.rowIndex
```

## Methods Details

### addColumn(name)

adds a column with the specified name to the dataset.

**Parameters**\
[String](../JSLib/String.md) name column name.

**Returns**\
[Boolean](../JSLib/Boolean.md) true if succeeded, else false.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
var success = dataset.addColumn('columnName',1);
```
### addColumn(name, index)

adds a column with the specified name to the dataset.

**Parameters**\
[String](../JSLib/String.md) name column name.\
[Number](../JSLib/Number.md) index column index number between 1 and getMaxColumnIndex().

**Returns**\
[Boolean](../JSLib/Boolean.md) true if succeeded, else false.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
var success = dataset.addColumn('columnName',1);
```
### addColumn(name, index, type)

adds a column with the specified name to the dataset.

**Parameters**\
[String](../JSLib/String.md) name column name.\
[Number](../JSLib/Number.md) index column index number between 1 and getMaxColumnIndex().\
[Number](../JSLib/Number.md) type the type of column, see JSColumn constants.

**Returns**\
[Boolean](../JSLib/Boolean.md) true if succeeded, else false.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
var success = dataset.addColumn('columnName',1);
```
### addHTMLProperty(row, col, name, value)

Add an HTML property to an HTML tag produced in getAsHTML().

For row and col parameters use:
1 = applies to the container
0 = applies to all
>0 = applies to specific cell

**Parameters**\
[Number](../JSLib/Number.md) row row number\
[Number](../JSLib/Number.md) col column number\
[String](../JSLib/String.md) name String property name\
[String](../JSLib/String.md) value String property value

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//adds a container property (to TABLE tag)
dataset.addHTMLProperty(-1,-1,'cellspacing','3');
dataset.addHTMLProperty(-1,-1,'style','border-collapse:collapse;'); //to have a single line border

//adds a row property to all rows (to TR tag)
dataset.addHTMLProperty(0,0,'class','text');

//adds a row property to second row (to TR tag)
dataset.addHTMLProperty(2,0,'class','text');

//adds a column property to all 3rd columns (to TD tag)
dataset.addHTMLProperty(0,3,'class','redcolumn') ;

//adds a specific cell property (to TD tag)
dataset.addHTMLProperty(2,4,'color','blue');

scopes.globals.html_field = '<html>'+dataset.getAsHTML()+'</html>';
```
### addRow(index, array)

Add a row to the dataset.

**Parameters**\
[Number](../JSLib/Number.md) index index to add row (1-based)\
[Array](../JSLib/Array.md) array row data

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
dataset.addRow(new Array(1,2,3,4,5,6,7,7)); //adds a row with 8 columns
dataset.addRow(2, new Array(1,2,3,4,5,6,7,7)); //adds a row with 8 columns at row 2
```
### addRow(array)

Add a row to the dataset. The row will be added as the last row.

**Parameters**\
[Array](../JSLib/Array.md) array row data

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
dataset.addRow(new Array(1,2,3,4,5,6,7,7)); //adds a row with 8 columns
dataset.addRow(2, new Array(1,2,3,4,5,6,7,7)); //adds a row with 8 columns at row 2
```
### createDataSource(name)

Create a datasource from the data set with specified name and using specified types.
The types are inferred from the data if possible.

A temporary datasource cannot be removed because once created there may always be forms or relations that refer to it.
When the client exits, all datasources used by that client are removed automatically.

Most resources used by the datasource can be released by deleting all records:
  dataset.removeRow(-1) or databaseManager.getFoundSet(datasource).deleteAllRecords()

**Parameters**\
[String](../JSLib/String.md) name datasource name

**Returns**\
[String](../JSLib/String.md) String uri reference to the created datasource.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
ds.addColumn('my_id'); // note: use regular javascript identifiers so they can be used in scripting
ds.addColumn('my_label');
var uri = ds.createDataSource('mydata', [JSColumn.INTEGER, JSColumn.TEXT]);
var jsform = solutionModel.newForm(fname, uri, null, true, 300, 300);

var query = 'select customerid, address, city, country  from customers';
var ds2 = databaseManager.getDataSetByQuery('example_data', query, null, 999);
var uri2 = ds2.createDataSource('mydata2'); // types are inferred from query result
```
### createDataSource(name, types)

Create a datasource from the data set with specified name and using specified types.

A temporary datasource cannot be removed because once created there may always be forms or relations that refer to it.
When the client exits, all datasources used by that client are removed automatically.

Most resources used by the datasource can be released by deleting all records:
  dataset.removeRow(-1) or databaseManager.getFoundSet(datasource).deleteAllRecords()

A datasource can be reused if the data has the same signature (column names and types).
A new createDataSource() call will clear the datasource contents from a previous call and insert the current data.

**Parameters**\
[String](../JSLib/String.md) name datasource name\
[Object](../JSLib/Object.md) types array of types as defined in JSColumn

**Returns**\
[String](../JSLib/String.md) String uri reference to the created datasource.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
ds.addColumn('my_id'); // note: use regular javascript identifiers so they can be used in scripting
ds.addColumn('my_label');
var uri = ds.createDataSource('mydata', [JSColumn.INTEGER, JSColumn.TEXT]);
var jsform = solutionModel.newForm(fname, uri, null, true, 300, 300);

var query = 'select customerid, address, city, country  from customers';
var ds2 = databaseManager.getDataSetByQuery('example_data', query, null, 999);
var uri2 = ds2.createDataSource('mydata2'); // types are inferred from query result
```
### createDataSource(name, types, pkNames)

Create a datasource from the data set with specified name and using specified types.

A temporary datasource cannot be removed because once created there may always be forms or relations that refer to it.
When the client exits, all datasources used by that client are removed automatically.

Most resources used by the datasource can be released by deleting all records:
  dataset.removeRow(-1) or databaseManager.getFoundSet(datasource).deleteAllRecords()

**Parameters**\
[String](../JSLib/String.md) name datasource name\
[Object](../JSLib/Object.md) types array of types as defined in JSColumn, when null types are inferred from the query result\
[Array](../JSLib/Array.md) pkNames array of pk names, when null a hidden pk-column will be added

**Returns**\
[String](../JSLib/String.md) String uri reference to the created datasource.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
ds.addColumn('my_id'); // note: use regular javascript identifiers so they can be used in scripting
ds.addColumn('my_label');
var uri = ds.createDataSource('mydata', [JSColumn.INTEGER, JSColumn.TEXT], ['my_id']);
var jsform = solutionModel.newForm(fname, uri, null, true, 300, 300);

var query = 'select customerid, address, city, country  from customers';
var ds2 = databaseManager.getDataSetByQuery('example_data', query, null, 999);
var uri2 = ds2.createDataSource('mydata2', null, ['customerid']); // types are inferred from query result, use customerid as pk
```
### getAsHTML()

Get the dataset as an html table, do not escape values or spaces, no multi_line_markup, do not add indentation, add column names.


**Returns**\
[String](../JSLib/String.md) String html.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//gets a dataset based on a query
//useful to limit the number of rows
var maxReturnedRows = 10;
var query = 'select c1,c2,c3 from test_table where start_date = ?';

//to access data by name, do not use '.' or special characters in names or aliases
var args = new Array();
args[0] = order_date //or new Date();
var dataset = databaseManager.getDataSetByQuery(databaseManager.getDataSourceServerName(controller.getDataSource()),query,args,maxReturnedRows);

// gets a dataset with escape values; escape spaces (lines will not wrap); no multi-line markup; with pretty indentation; shows column names
var htmlTable = dataset.getAsHTML(true, true, false, true, true);

//assigns the dataset to a field and sets the display type to HTML_AREA
//assuming the html_field is a global text variable
scopes.globals.html_field = '<html>'+dataset.getAsHTML()+'</html>';

//Note: To display an HTML_AREA field as an HTML page, add HTML tags at the beginning '<html>' and at the end '</html>'.
```
### getAsHTML(escape_values)

Get the dataset as an html table, do not escape spaces, no multi_line_markup, do not add indentation, add column names.

**Parameters**\
[Boolean](../JSLib/Boolean.md) escape_values if true, replaces illegal HTML characters with corresponding valid escape sequences.

**Returns**\
[String](../JSLib/String.md) String html.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//gets a dataset based on a query
//useful to limit the number of rows
var maxReturnedRows = 10;
var query = 'select c1,c2,c3 from test_table where start_date = ?';

//to access data by name, do not use '.' or special characters in names or aliases
var args = new Array();
args[0] = order_date //or new Date();
var dataset = databaseManager.getDataSetByQuery(databaseManager.getDataSourceServerName(controller.getDataSource()),query,args,maxReturnedRows);

// gets a dataset with escape values; escape spaces (lines will not wrap); no multi-line markup; with pretty indentation; shows column names
var htmlTable = dataset.getAsHTML(true, true, false, true, true);

//assigns the dataset to a field and sets the display type to HTML_AREA
//assuming the html_field is a global text variable
scopes.globals.html_field = '<html>'+dataset.getAsHTML()+'</html>';

//Note: To display an HTML_AREA field as an HTML page, add HTML tags at the beginning '<html>' and at the end '</html>'.
```
### getAsHTML(escape_values, escape_spaces)

Get the dataset as an html table, no multi_line_markup, do not add indentation, add column names.

**Parameters**\
[Boolean](../JSLib/Boolean.md) escape_values if true, replaces illegal HTML characters with corresponding valid escape sequences.\
[Boolean](../JSLib/Boolean.md) escape_spaces if true, replaces text spaces with non-breaking space tags ( ) and tabs by four non-breaking space tags.

**Returns**\
[String](../JSLib/String.md) String html.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//gets a dataset based on a query
//useful to limit the number of rows
var maxReturnedRows = 10;
var query = 'select c1,c2,c3 from test_table where start_date = ?';

//to access data by name, do not use '.' or special characters in names or aliases
var args = new Array();
args[0] = order_date //or new Date();
var dataset = databaseManager.getDataSetByQuery(databaseManager.getDataSourceServerName(controller.getDataSource()),query,args,maxReturnedRows);

// gets a dataset with escape values; escape spaces (lines will not wrap); no multi-line markup; with pretty indentation; shows column names
var htmlTable = dataset.getAsHTML(true, true, false, true, true);

//assigns the dataset to a field and sets the display type to HTML_AREA
//assuming the html_field is a global text variable
scopes.globals.html_field = '<html>'+dataset.getAsHTML()+'</html>';

//Note: To display an HTML_AREA field as an HTML page, add HTML tags at the beginning '<html>' and at the end '</html>'.
```
### getAsHTML(escape_values, escape_spaces, multi_line_markup)

Get the dataset as an html table, do not add indentation, add column names.

**Parameters**\
[Boolean](../JSLib/Boolean.md) escape_values if true, replaces illegal HTML characters with corresponding valid escape sequences.\
[Boolean](../JSLib/Boolean.md) escape_spaces if true, replaces text spaces with non-breaking space tags ( ) and tabs by four non-breaking space tags.\
[Boolean](../JSLib/Boolean.md) multi_line_markup if true, multiLineMarkup will enforce new lines that are in the text; single new lines will be replaced by <br>, multiple new lines will be replaced by <p>

**Returns**\
[String](../JSLib/String.md) String html.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//gets a dataset based on a query
//useful to limit the number of rows
var maxReturnedRows = 10;
var query = 'select c1,c2,c3 from test_table where start_date = ?';

//to access data by name, do not use '.' or special characters in names or aliases
var args = new Array();
args[0] = order_date //or new Date();
var dataset = databaseManager.getDataSetByQuery(databaseManager.getDataSourceServerName(controller.getDataSource()),query,args,maxReturnedRows);

// gets a dataset with escape values; escape spaces (lines will not wrap); no multi-line markup; with pretty indentation; shows column names
var htmlTable = dataset.getAsHTML(true, true, false, true, true);

//assigns the dataset to a field and sets the display type to HTML_AREA
//assuming the html_field is a global text variable
scopes.globals.html_field = '<html>'+dataset.getAsHTML()+'</html>';

//Note: To display an HTML_AREA field as an HTML page, add HTML tags at the beginning '<html>' and at the end '</html>'.
```
### getAsHTML(escape_values, escape_spaces, multi_line_markup, pretty_indent)

Get the dataset as an html table, add column names.

**Parameters**\
[Boolean](../JSLib/Boolean.md) escape_values if true, replaces illegal HTML characters with corresponding valid escape sequences.\
[Boolean](../JSLib/Boolean.md) escape_spaces if true, replaces text spaces with non-breaking space tags ( ) and tabs by four non-breaking space tags.\
[Boolean](../JSLib/Boolean.md) multi_line_markup if true, multiLineMarkup will enforce new lines that are in the text; single new lines will be replaced by <br>, multiple new lines will be replaced by <p>\
[Boolean](../JSLib/Boolean.md) pretty_indent if true, adds indentation for more readable HTML code.

**Returns**\
[String](../JSLib/String.md) String html.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//gets a dataset based on a query
//useful to limit the number of rows
var maxReturnedRows = 10;
var query = 'select c1,c2,c3 from test_table where start_date = ?';

//to access data by name, do not use '.' or special characters in names or aliases
var args = new Array();
args[0] = order_date //or new Date();
var dataset = databaseManager.getDataSetByQuery(databaseManager.getDataSourceServerName(controller.getDataSource()),query,args,maxReturnedRows);

// gets a dataset with escape values; escape spaces (lines will not wrap); no multi-line markup; with pretty indentation; shows column names
var htmlTable = dataset.getAsHTML(true, true, false, true, true);

//assigns the dataset to a field and sets the display type to HTML_AREA
//assuming the html_field is a global text variable
scopes.globals.html_field = '<html>'+dataset.getAsHTML()+'</html>';

//Note: To display an HTML_AREA field as an HTML page, add HTML tags at the beginning '<html>' and at the end '</html>'.
```
### getAsHTML(escape_values, escape_spaces, multi_line_markup, pretty_indent, add_column_names)

Get the dataset as an html table.

**Parameters**\
[Boolean](../JSLib/Boolean.md) escape_values if true, replaces illegal HTML characters with corresponding valid escape sequences.\
[Boolean](../JSLib/Boolean.md) escape_spaces if true, replaces text spaces with non-breaking space tags ( ) and tabs by four non-breaking space tags.\
[Boolean](../JSLib/Boolean.md) multi_line_markup if true, multiLineMarkup will enforce new lines that are in the text; single new lines will be replaced by <br>, multiple new lines will be replaced by <p>\
[Boolean](../JSLib/Boolean.md) pretty_indent if true, adds indentation for more readable HTML code.\
[Boolean](../JSLib/Boolean.md) add_column_names if false, column headers will not be added to the table.

**Returns**\
[String](../JSLib/String.md) String html.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//gets a dataset based on a query
//useful to limit the number of rows
var maxReturnedRows = 10;
var query = 'select c1,c2,c3 from test_table where start_date = ?';

//to access data by name, do not use '.' or special characters in names or aliases
var args = new Array();
args[0] = order_date //or new Date();
var dataset = databaseManager.getDataSetByQuery(databaseManager.getDataSourceServerName(controller.getDataSource()),query,args,maxReturnedRows);

// gets a dataset with escape values; escape spaces (lines will not wrap); no multi-line markup; with pretty indentation; shows column names
var htmlTable = dataset.getAsHTML(true, true, false, true, true);

//assigns the dataset to a field and sets the display type to HTML_AREA
//assuming the html_field is a global text variable
scopes.globals.html_field = '<html>'+dataset.getAsHTML()+'</html>';

//Note: To display an HTML_AREA field as an HTML page, add HTML tags at the beginning '<html>' and at the end '</html>'.
```
### getAsText(column_separator, row_separator, value_delimiter, add_column_names)

Get the dataset as formatted text.

**Parameters**\
[String](../JSLib/String.md) column_separator any specified column separator; examples: tab '\t'; comma ','; semicolon ';'; space ' ' .\
[String](../JSLib/String.md) row_separator the specified row separator; examples: new line '\n'.\
[String](../JSLib/String.md) value_delimiter the specified value delimiter; null means empty string; example: double quote '"'.\
[Boolean](../JSLib/Boolean.md) add_column_names if true column names will be added as a first row.

**Returns**\
[String](../JSLib/String.md) String formatted text.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
//you can create csv or tab delimited results
var csv = dataset.getAsText(',','\n','"',true)
var tab = dataset.getAsText('\t','\n','"',true)
```
### getColumnAsArray(index)

Get the column data of a dataset as an Array.

**Parameters**\
[Number](../JSLib/Number.md) index index of column (1-based).

**Returns**\
[Array](../JSLib/Array.md) Object array of data.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
var dataArray = dataset.getColumnAsArray(1); //puts the contents from the first column of the dataset into an array
//once you have it as an array you can loop through it or feed it to a custom valuelist for example
```
### getColumnName(index)

Get a column name based on index.

**Parameters**\
[Number](../JSLib/Number.md) index index of column (1-based).

**Returns**\
[String](../JSLib/String.md) String column name.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
var firstColumName = dataset.getColumnName(1) //retrieves the first columnname into the variable firstColumName
//using a loop you can get all columnames in an array:
var query = 'select * from customers';
var dataset = databaseManager.getDataSetByQuery(databaseManager.getDataSourceServerName(controller.getDataSource()), query, null, 100);
var colArray = new Array()
for (var i = 1; i <= dataset.getMaxColumnIndex(); i++)
{
	colArray[i-1] = dataset.getColumnName(i)
	//note the -1, because an array is zero based and dataset is 1 based.
}
```
### getColumnNames()

Get the column names of a dataset.


**Returns**\
[Array](../JSLib/Array.md) String[] column names

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var query = 'select * from customers';
var dataset = databaseManager.getDataSetByQuery(databaseManager.getDataSourceServerName(controller.getDataSource()), query, null, 100);
var columnNames = dataset.getColumnNames();
```
### getColumnType(index)

Get a column type based on index.

**Parameters**\
[Number](../JSLib/Number.md) index index of column (1-based).

**Returns**\
[Number](../JSLib/Number.md) Number the column type (JSColumn constant)

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
var firstColumnType = dataset.getColumnType(1) //retrieves the first column's type into the variable firstColumnType
if (firstColumnType == JSColumn.NUMBER) { }
```
### getException()

Get the database exception if an error occurred.


**Returns**\
[Exception](../Exception.md) ServoyException exception or null when not available.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
var dbException = dataset.getException();
```
### getMaxColumnIndex()

Get the number of columns in the dataset.


**Returns**\
[Number](../JSLib/Number.md) int number of columns.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
for (var i = 1; i <= dataset.getMaxColumnIndex(); i++)
{
	colArray[i-1] = dataset.getColumnName(i)
	//have to subtract 1, because an array is zero based and a dataset is 1 based.
}
```
### getMaxRowIndex()

Get the number of rows in the dataset.


**Returns**\
[Number](../JSLib/Number.md) int number of rows.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
var totalRows = dataset.getMaxRowIndex();
```
### getRowAsArray(index)

Get the row data of a dataset as an Array.

**Parameters**\
[Number](../JSLib/Number.md) index index of row (1-based).

**Returns**\
[Array](../JSLib/Array.md) Object array of data.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
var dataArray = dataset.getRowAsArray(1); //puts the contents from the first row of the dataset into an array
//once you have it as an array you can loop through it
```
### getValue(row, col)

Get the value specified by row and column position from the dataset.

**Parameters**\
[Number](../JSLib/Number.md) row row number, 1-based\
[Number](../JSLib/Number.md) col column number, 1-based

**Returns**\
[Object](../JSLib/Object.md) Object value

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
var dataAtRow2Col1 = dataset.getValue(2, 1);
```
### hadMoreData()

Return true if there is more data in the resultset then specified by maxReturnedRows at query time.


**Returns**\
[Boolean](../JSLib/Boolean.md) boolean more data available

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var ds = databaseManager.getDataSetByQuery('example_data', 'select order_id from orders', null, 10000)
if (ds.hadMoreData())
{
	// handle large result
}
```
### removeColumn(index)

Remove a column by index from the dataset.

**Parameters**\
[Number](../JSLib/Number.md) index index of column to remove (1-based)

**Returns**\
[Boolean](../JSLib/Boolean.md) true if succeeded, else false.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
var success = dataset.removeColumn(1); // removes first column
```
### removeRow(row)

Remove a row from the dataset.

**Parameters**\
[Number](../JSLib/Number.md) row row index to remove, -1 for all rows

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
dataset.removeRow(1); //removes the first row
dataset.removeRow(-1); //removes all rows
```
### setColumnName(index, columnName)

Set a column name based on index.

**Parameters**\
[Number](../JSLib/Number.md) index index of column (1-based).\
[String](../JSLib/String.md) columnName new column name.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var query = 'select customerid, customername from customers';
var dataset = databaseManager.getDataSetByQuery(databaseManager.getDataSourceServerName(controller.getDataSource()), query, null, -1);
dataset.setColumnName(2, 'name_of_customer') // change the column name for second column.
```
### setValue(row, col, obj)

Set the value specified by row and column position from the dataset.
Use row = -1, to set columnnames.

**Parameters**\
[Number](../JSLib/Number.md) row row number, 1-based\
[Number](../JSLib/Number.md) col column number, 1-based\
[Object](../JSLib/Object.md) obj the value to be stored at the given row and column.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//assuming the variable dataset contains a dataset
dataset.setValue(2, 1,'data');
```
### sort(col, sort_direction)

Sort the dataset on the given column (1-based) in ascending or descending.

**Parameters**\
[Number](../JSLib/Number.md) col column number, 1-based\
[Boolean](../JSLib/Boolean.md) sort_direction ascending (true) or descending (false)

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// sort using column number
//assuming the variable dataset contains a dataset
dataset.sort(1, false)
```
### sort(comparator)

Sort the dataset using the function as comparator.
The comparator function is called to compare two rows, that are passed as arguments, and
it will return -1/0/1 if the first row is less/equal/greater then the second row.

NOTE: starting with 7.2 release, when called on datasource(foundset) dataset, this function doesn't save the data anymore

**Parameters**\
[Function](../JSLib/Function.md) comparator comparator function

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//sort using comparator
dataset.sort(mySortFunction);

function mySortFunction(r1, r2)
{
	var o = 0;
	if(r1[0] < r2[0])
	{
		o = -1;
	}
	else if(r1[0] > r2[0])
	{
		o = 1;
	}
	return o;
}
```

