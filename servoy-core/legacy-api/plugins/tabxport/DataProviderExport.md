#  DataProviderExport

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [DataProviderExport](../../DataProviderExport.md) | [setFormat(format)](DataProviderExport.md#setformat-format)                   | Set format for dataprovider value..                                    |
| [DataProviderExport](../../DataProviderExport.md) | [setHeaderText(headerText)](DataProviderExport.md#setheadertext-headertext)                   | Set header text for dataprovider value..                                    |
| [DataProviderExport](../../DataProviderExport.md) | [setValueList(valuelistName)](DataProviderExport.md#setvaluelist-valuelistname)                   | Set valuelist to resolve display value for dataprovider..                                    |

## Methods Details

### setFormat(format)

Set format for dataprovider value.

**Parameters**\
[String](../../JSLib/String.md) format the dataprovider format

**Returns**\
[DataProviderExport](../../DataProviderExport.md) dataprovider export object

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var exporter = plugins.textxport.createExporter(forms.form1.foundset,';',false);
exporter.addDataProvider('mydate').setFormat('yyyy/dd/MM');
var content = exporter.textExport();
```
### setHeaderText(headerText)

Set header text for dataprovider value. If no header text is set and exportHeader is true dataprovider will be used as header text.

**Parameters**\
[String](../../JSLib/String.md) headerText the header text

**Returns**\
[DataProviderExport](../../DataProviderExport.md) dataprovider export object

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var exporter = plugins.textxport.createExporter(forms.form1.foundset,';',true);
exporter.addDataProvider('orderid').setHeaderText('Order ID');
var content = exporter.textExport();
```
### setValueList(valuelistName)

Set valuelist to resolve display value for dataprovider.

**Parameters**\
[String](../../JSLib/String.md) valuelistName the valuelist name

**Returns**\
[DataProviderExport](../../DataProviderExport.md) dataprovider export object

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var exporter = plugins.textxport.createExporter(forms.form1.foundset,';',true);
exporter.addDataProvider('item_id').setValueList('myvaluelist');
var content = exporter.textExport();
```

