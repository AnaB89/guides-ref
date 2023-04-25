#  excelxport

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../../JSLib/Boolean.md) | [exportEnabled](excelxport.md#exportEnabled)                   | Enable the export feature of this plugin..                                    |
| [Boolean](../../JSLib/Boolean.md) | [importEnabled](excelxport.md#importEnabled)                   | Enable the import feature of this plugin..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Array](../../JSLib/Array.md) | [excelExport(foundSet, dataProviderIds)](excelxport.md#excelexport-foundset-dataproviderids)                   | Export to Excel data.                                    |
| [Array](../../JSLib/Array.md) | [excelExport(foundSet, dataProviderIds, templateXLS)](excelxport.md#excelexport-foundset-dataproviderids-templatexls)                   | Export to Excel data.                                    |
| [Array](../../JSLib/Array.md) | [excelExport(foundSet, dataProviderIds, templateXLS, sheetName)](excelxport.md#excelexport-foundset-dataproviderids-templatexls-sheetname)                   | Export to Excel data.                                    |
| [Array](../../JSLib/Array.md) | [excelExport(foundSet, dataProviderIds, templateXLS, sheetName, outputColumnNames, startRow)](excelxport.md#excelexport-foundset-dataproviderids-templatexls-sheetname-outputcolumnnames-startrow)                   | Export to Excel data.                                    |
| [Array](../../JSLib/Array.md) | [excelExport(foundSet, dataProviderIds, templateXLS, sheetName, startRow, startColumn)](excelxport.md#excelexport-foundset-dataproviderids-templatexls-sheetname-startrow-startcolumn)                   | Export to Excel data.                                    |
| [Array](../../JSLib/Array.md) | [excelExport(foundSet, dataProviderIds, templateXLS, sheetName)](excelxport.md#excelexport-foundset-dataproviderids-templatexls-sheetname)                   | Export to Excel data.                                    |
| [Array](../../JSLib/Array.md) | [excelExport(foundSet, dataProviderIds, templateXLS, sheetName, outputColumnNames, startRow)](excelxport.md#excelexport-foundset-dataproviderids-templatexls-sheetname-outputcolumnnames-startrow)                   | Export to Excel data.                                    |
| [Array](../../JSLib/Array.md) | [excelExport(foundSet, dataProviderIds, templateXLS, sheetName, outputColumnNames, startRow, startColumn)](excelxport.md#excelexport-foundset-dataproviderids-templatexls-sheetname-outputcolumnnames-startrow-startcolumn)                   | Export to Excel data.                                    |

## Properties Details

### exportEnabled

Enable the export feature of this plugin.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
plugins.excelxport.exportEnabled = true;
var isEnabled = plugins.excelxport.exportEnabled;
```
### importEnabled

Enable the import feature of this plugin.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
plugins.excelxport.importEnabled = true;
var isEnabled = plugins.excelxport.importEnabled;
```

## Methods Details

### excelExport(foundSet, dataProviderIds)

Export to Excel data

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundSet the foundset on which to export\
[Array](../../JSLib/Array.md) dataProviderIds the ids of the dataproviders

**Returns**\
[Array](../../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//export in new byte array
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name']);
//export by adding to templateXLS in default (new) 'Servoy Data' worksheet
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS);
//export by adding to templateXLS, in 'mySheet' worksheet, starting at default(1/1) row/column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet');
//export by adding to templateXLS, in 'mySheet' worksheet, with column names 'ID' and 'Name' starting at default(1/1) row/column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet', ['ID', 'Name']);
//export by adding to templateXLS, in 'mySheet' worksheet, starting at 3rd row and 5th column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet',3,5);
* //export by adding to templateXLS, in 'mySheet' worksheet, with column names 'ID' and 'Name', starting at 3rd row and 5th column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet', ['ID', 'Name'], 3, 5);
```
### excelExport(foundSet, dataProviderIds, templateXLS)

Export to Excel data

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundSet the foundset on which to export\
[Array](../../JSLib/Array.md) dataProviderIds the ids of the dataproviders\
[Array](../../JSLib/Array.md) templateXLS the xls template to export in

**Returns**\
[Array](../../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//export in new byte array
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name']);
//export by adding to templateXLS in default (new) 'Servoy Data' worksheet
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS);
//export by adding to templateXLS, in 'mySheet' worksheet, starting at default(1/1) row/column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet');
//export by adding to templateXLS, in 'mySheet' worksheet, with column names 'ID' and 'Name' starting at default(1/1) row/column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet', ['ID', 'Name']);
//export by adding to templateXLS, in 'mySheet' worksheet, starting at 3rd row and 5th column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet',3,5);
* //export by adding to templateXLS, in 'mySheet' worksheet, with column names 'ID' and 'Name', starting at 3rd row and 5th column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet', ['ID', 'Name'], 3, 5);
```
### excelExport(foundSet, dataProviderIds, templateXLS, sheetName)

Export to Excel data

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundSet the foundset on which to export\
[Array](../../JSLib/Array.md) dataProviderIds the ids of the dataproviders\
[Array](../../JSLib/Array.md) templateXLS the xls template to export in\
[String](../../JSLib/String.md) sheetName the name of the worksheet

**Returns**\
[Array](../../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//export in new byte array
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name']);
//export by adding to templateXLS in default (new) 'Servoy Data' worksheet
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS);
//export by adding to templateXLS, in 'mySheet' worksheet, starting at default(1/1) row/column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet');
//export by adding to templateXLS, in 'mySheet' worksheet, with column names 'ID' and 'Name' starting at default(1/1) row/column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet', ['ID', 'Name']);
//export by adding to templateXLS, in 'mySheet' worksheet, starting at 3rd row and 5th column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet',3,5);
* //export by adding to templateXLS, in 'mySheet' worksheet, with column names 'ID' and 'Name', starting at 3rd row and 5th column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet', ['ID', 'Name'], 3, 5);
```
### excelExport(foundSet, dataProviderIds, templateXLS, sheetName, outputColumnNames, startRow)

Export to Excel data

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundSet the foundset on which to export\
[Array](../../JSLib/Array.md) dataProviderIds the ids of the dataproviders\
[Array](../../JSLib/Array.md) templateXLS the xls template to export in\
[String](../../JSLib/String.md) sheetName the name of the worksheet\
[Object](../../JSLib/Object.md) outputColumnNames is used to set the column headers independently from the dataprovider names\
[Number](../../JSLib/Number.md) startRow row in the foundset at which to start the export

**Returns**\
[Array](../../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//export in new byte array
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name']);
//export by adding to templateXLS in default (new) 'Servoy Data' worksheet
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS);
//export by adding to templateXLS, in 'mySheet' worksheet, starting at default(1/1) row/column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet');
//export by adding to templateXLS, in 'mySheet' worksheet, with column names 'ID' and 'Name' starting at default(1/1) row/column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet', ['ID', 'Name']);
//export by adding to templateXLS, in 'mySheet' worksheet, starting at 3rd row and 5th column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet',3,5);
* //export by adding to templateXLS, in 'mySheet' worksheet, with column names 'ID' and 'Name', starting at 3rd row and 5th column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet', ['ID', 'Name'], 3, 5);
```
### excelExport(foundSet, dataProviderIds, templateXLS, sheetName, startRow, startColumn)

Export to Excel data

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundSet the foundset on which to export\
[Array](../../JSLib/Array.md) dataProviderIds the ids of the dataproviders\
[Array](../../JSLib/Array.md) templateXLS the xls template to export in\
[String](../../JSLib/String.md) sheetName the name of the worksheet\
[Number](../../JSLib/Number.md) startRow row in the foundset at which to start the export\
[Number](../../JSLib/Number.md) startColumn column in the foundset at which to start the export

**Returns**\
[Array](../../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//export in new byte array
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name']);
//export by adding to templateXLS in default (new) 'Servoy Data' worksheet
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS);
//export by adding to templateXLS, in 'mySheet' worksheet, starting at default(1/1) row/column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet');
//export by adding to templateXLS, in 'mySheet' worksheet, with column names 'ID' and 'Name' starting at default(1/1) row/column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet', ['ID', 'Name']);
//export by adding to templateXLS, in 'mySheet' worksheet, starting at 3rd row and 5th column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet',3,5);
* //export by adding to templateXLS, in 'mySheet' worksheet, with column names 'ID' and 'Name', starting at 3rd row and 5th column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet', ['ID', 'Name'], 3, 5);
```
### excelExport(foundSet, dataProviderIds, templateXLS, sheetName)

Export to Excel data

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundSet the foundset on which to export\
[Array](../../JSLib/Array.md) dataProviderIds the ids of the dataproviders\
[Array](../../JSLib/Array.md) templateXLS the xls template to export in\
[String](../../JSLib/String.md) sheetName the name of the worksheet

**Returns**\
[Array](../../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//export in new byte array
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name']);
//export by adding to templateXLS in default (new) 'Servoy Data' worksheet
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS);
//export by adding to templateXLS, in 'mySheet' worksheet, starting at default(1/1) row/column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet');
//export by adding to templateXLS, in 'mySheet' worksheet, with column names 'ID' and 'Name' starting at default(1/1) row/column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet', ['ID', 'Name']);
//export by adding to templateXLS, in 'mySheet' worksheet, starting at 3rd row and 5th column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet',3,5);
* //export by adding to templateXLS, in 'mySheet' worksheet, with column names 'ID' and 'Name', starting at 3rd row and 5th column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet', ['ID', 'Name'], 3, 5);
```
### excelExport(foundSet, dataProviderIds, templateXLS, sheetName, outputColumnNames, startRow)

Export to Excel data

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundSet the foundset on which to export\
[Array](../../JSLib/Array.md) dataProviderIds the ids of the dataproviders\
[Array](../../JSLib/Array.md) templateXLS the xls template to export in\
[String](../../JSLib/String.md) sheetName the name of the worksheet\
[Array](../../JSLib/Array.md) outputColumnNames is used to set the column headers independently from the dataprovider names\
[Number](../../JSLib/Number.md) startRow row in the foundset at which to start the export

**Returns**\
[Array](../../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//export in new byte array
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name']);
//export by adding to templateXLS in default (new) 'Servoy Data' worksheet
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS);
//export by adding to templateXLS, in 'mySheet' worksheet, starting at default(1/1) row/column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet');
//export by adding to templateXLS, in 'mySheet' worksheet, with column names 'ID' and 'Name' starting at default(1/1) row/column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet', ['ID', 'Name']);
//export by adding to templateXLS, in 'mySheet' worksheet, starting at 3rd row and 5th column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet',3,5);
* //export by adding to templateXLS, in 'mySheet' worksheet, with column names 'ID' and 'Name', starting at 3rd row and 5th column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet', ['ID', 'Name'], 3, 5);
```
### excelExport(foundSet, dataProviderIds, templateXLS, sheetName, outputColumnNames, startRow, startColumn)

Export to Excel data

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundSet the foundset on which to export\
[Array](../../JSLib/Array.md) dataProviderIds the ids of the dataproviders\
[Array](../../JSLib/Array.md) templateXLS the xls template to export in\
[String](../../JSLib/String.md) sheetName the name of the worksheet\
[Array](../../JSLib/Array.md) outputColumnNames is used to set the column headers independently from the dataprovider names\
[Number](../../JSLib/Number.md) startRow row in the foundset at which to start the export\
[Number](../../JSLib/Number.md) startColumn column in the foundset at which to start the export

**Returns**\
[Array](../../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//export in new byte array
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name']);
//export by adding to templateXLS in default (new) 'Servoy Data' worksheet
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS);
//export by adding to templateXLS, in 'mySheet' worksheet, starting at default(1/1) row/column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet');
//export by adding to templateXLS, in 'mySheet' worksheet, with column names 'ID' and 'Name' starting at default(1/1) row/column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet', ['ID', 'Name']);
//export by adding to templateXLS, in 'mySheet' worksheet, starting at 3rd row and 5th column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet',3,5);
* //export by adding to templateXLS, in 'mySheet' worksheet, with column names 'ID' and 'Name', starting at 3rd row and 5th column
var bytes = plugins.excelxport.excelExport(forms.form1.foundset, ['id','name'],templateXLS, 'mySheet', ['ID', 'Name'], 3, 5);
```

