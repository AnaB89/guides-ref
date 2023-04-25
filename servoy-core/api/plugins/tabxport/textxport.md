#  textxport


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [TabExporter](../../TabExporter.md) | [createExporter(foundSet, separator, exportHeader)](textxport.md#createexporter-foundset-separator-exportheader)                   | Create exporter for easier export set up..                                    |
| [String](../../JSLib/String.md) | [textExport(foundSet, dataProviderIds)](textxport.md#textexport-foundset-dataproviderids)                   | Export to text 'separated value' data (*..                                    |
| [String](../../JSLib/String.md) | [textExport(foundSet, dataProviderIds, separator)](textxport.md#textexport-foundset-dataproviderids-separator)                   | Export to text 'separated value' data (*..                                    |
| [String](../../JSLib/String.md) | [textExport(foundSet, dataProviderIds, separator, exportHeader)](textxport.md#textexport-foundset-dataproviderids-separator-exportheader)                   | Export to text 'separated value' data (*..                                    |

## Properties Details


## Methods Details

### createExporter(foundSet, separator, exportHeader)

Create exporter for easier export set up. Can either use this method (for more complex exports) or textExport(...) API

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundSet the foundset to export with\
[String](../../JSLib/String.md) separator the separator of the data\
[Boolean](../../JSLib/Boolean.md) exportHeader export a header

**Returns**\
[TabExporter](../../TabExporter.md) exporter object


**Sample**

```javascript
//export with ';' separator and no header
var exporter = plugins.textxport.createExporter(forms.form1.foundset,';',false);
```
### textExport(foundSet, dataProviderIds)

Export to text 'separated value' data (*.tab/*.csv)

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundSet the foundset to export with\
[Array](../../JSLib/Array.md) dataProviderIds the ids of the dataproviders

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
//export with default separator(tab) and no header
var dataToBeWritten = plugins.textxport.textExport(forms.form1.foundset,['id','name']);
```
### textExport(foundSet, dataProviderIds, separator)

Export to text 'separated value' data (*.tab/*.csv)

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundSet the foundset to export with\
[Array](../../JSLib/Array.md) dataProviderIds the ids of the dataproviders\
[String](../../JSLib/String.md) separator the separator of the data

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
//export with ';' separator and no header
var dataToBeWritten = plugins.textxport.textExport(forms.form1.foundset,['id','name'],';');
```
### textExport(foundSet, dataProviderIds, separator, exportHeader)

Export to text 'separated value' data (*.tab/*.csv)

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundSet the foundset to export with\
[Array](../../JSLib/Array.md) dataProviderIds the ids of the dataproviders\
[String](../../JSLib/String.md) separator the separator of the data\
[Boolean](../../JSLib/Boolean.md) exportHeader true for exporting with the table header, false for not

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
//export with ';' separator and header
var dataToBeWritten = plugins.textxport.textExport(forms.form1.foundset,['id','name'],';',true);
```

