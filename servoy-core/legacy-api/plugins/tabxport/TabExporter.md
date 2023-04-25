#  TabExporter

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [DataProviderExport](../../DataProviderExport.md) | [addDataProvider(dataprovider)](TabExporter.md#adddataprovider-dataprovider)                   | Add a dataprovider from specified foundset to export..                                    |
| [String](../../JSLib/String.md) | [textExport()](TabExporter.md#textexport)                   | Export to text 'separated value' data (*..                                    |

## Methods Details

### addDataProvider(dataprovider)

Add a dataprovider from specified foundset to export.

**Parameters**\
[String](../../JSLib/String.md) dataprovider The dataprovider string to add as a column to export

**Returns**\
[DataProviderExport](../../DataProviderExport.md) dataprovider export object

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var exporter = plugins.textxport.createExporter(forms.form1.foundset,';',true);
exporter.addDataProvider('orderid').setHeaderText('Order ID');
exporter.addDataProvider('item_id').setValueList('myvaluelist');
exporter.addDataProvider('mydate').setFormat('yyyy/dd/MM');
var content = exporter.textExport();
```
### textExport()

Export to text 'separated value' data (*.tab/*.csv), based on values set on exporter


**Returns**\
[String](../../JSLib/String.md) exported text

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var exporter = plugins.textxport.createExporter(forms.form1.foundset,';',true);
exporter.addDataProvider('orderid').setHeaderText('Order ID');
exporter.addDataProvider('item_id').setValueList('myvaluelist');
exporter.addDataProvider('mydate').setFormat('yyyy/dd/MM');
var content = exporter.textExport();
```

