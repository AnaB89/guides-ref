#  textxport

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../../JSLib/Boolean.md) | [exportEnabled](textxport.md#exportEnabled)                   | Enable the export feature of this plugin..                                    |
| [Boolean](../../JSLib/Boolean.md) | [importEnabled](textxport.md#importEnabled)                   | Enable the import feature of this plugin..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [TabExporter](../../TabExporter.md) | [createExporter(foundSet, separator, exportHeader)](textxport.md#createexporter-foundset-separator-exportheader)                   | Create exporter for easier export set up..                                    |
| [String](../../JSLib/String.md) | [textExport(foundSet, dataProviderIds)](textxport.md#textexport-foundset-dataproviderids)                   | Export to text 'separated value' data (*..                                    |
| [String](../../JSLib/String.md) | [textExport(foundSet, dataProviderIds, separator)](textxport.md#textexport-foundset-dataproviderids-separator)                   | Export to text 'separated value' data (*..                                    |
| [String](../../JSLib/String.md) | [textExport(foundSet, dataProviderIds, separator, exportHeader)](textxport.md#textexport-foundset-dataproviderids-separator-exportheader)                   | Export to text 'separated value' data (*..                                    |

## Properties Details

### exportEnabled

Enable the export feature of this plugin.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient

**Sample**

```javascript
plugins.textxport.exportEnabled = true;
var isEnabled = plugins.textxport.exportEnabled;
```
### importEnabled

Enable the import feature of this plugin.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient

**Sample**

```javascript
plugins.textxport.importEnabled = true;
var isEnabled = plugins.textxport.importEnabled;
```

## Methods Details

### createExporter(foundSet, separator, exportHeader)

Create exporter for easier export set up. Can either use this method (for more complex exports) or textExport(...) API

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) foundSet the foundset to export with\
[String](../../JSLib/String.md) separator the separator of the data\
[Boolean](../../JSLib/Boolean.md) exportHeader export a header

**Returns**\
[TabExporter](../../TabExporter.md) exporter object

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
SmartClient,WebClient,NGClient

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

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//export with ';' separator and header
var dataToBeWritten = plugins.textxport.textExport(forms.form1.foundset,['id','name'],';',true);
```

