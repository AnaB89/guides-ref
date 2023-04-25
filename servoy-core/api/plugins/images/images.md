#  images

## **Return Types**
[JSImage](./JSImage.md),

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSImage](./JSImage.md) | [getImage(object)](images.md#getimage-object)                   | Get a javascript image/resource object for the given file/bytearray/bean/applet/form_element..                                    |

## Methods Details

### getImage(object)

Get a javascript image/resource object for the given file/bytearray/bean/applet/form_element.

**Parameters**\
[Object](../../JSLib/Object.md) object file/byte_array/bean/applet/form_element

**Returns**\
[JSImage](./JSImage.md) 


**Sample**

```javascript
var image = plugins.images.getImage(byteArray);
var height = image.getHeight();
var contentType = image.getContentType();
var scaled_image = image.resize(30, 30);

var snapshot_image = plugins.images.getImage(forms.companyReports.elements.employeesChartBean);
var tempFile = plugins.file.createTempFile('bean_snapshot','.jpg')
plugins.file.writeFile(tempFile, snapshot_image.getData())
application.setStatusText('Wrote file: '+tempFile)
```

