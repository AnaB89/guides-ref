#  JSImage

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSImage](./JSImage.md) | [flip(type)](JSImage.md#flip-type)                   | Flips the image verticaly (type param=0) or horizontaly (type param=1)..                                    |
| [String](../../JSLib/String.md) | [getContentType()](JSImage.md#getcontenttype)                   | Gets the contenttype (image/jpeg) of this image..                                    |
| [Array](../../JSLib/Array.md) | [getData()](JSImage.md#getdata)                   | Gets the bytes of this image, so that they can be saved to disk or stored the database..                                    |
| [Number](../../JSLib/Number.md) | [getHeight()](JSImage.md#getheight)                   | Gets the height of this image..                                    |
| [String](../../JSLib/String.md) | [getMetaDataDescription(property)](JSImage.md#getmetadatadescription-property)                   | Gets the description of a metadata property from the image..                                    |
| [Object](../../JSLib/Object.md) | [getMetaDataObject(property)](JSImage.md#getmetadataobject-property)                   | Gets the real object of a metadata property from the image..                                    |
| [Array](../../JSLib/Array.md) | [getMetaDataProperties()](JSImage.md#getmetadataproperties)                   | Gets the available metadata properties from the image..                                    |
| [Number](../../JSLib/Number.md) | [getWidth()](JSImage.md#getwidth)                   | Gets the width of this image..                                    |
| [JSImage](./JSImage.md) | [resize(width, height)](JSImage.md#resize-width-height)                   | Resizes the image to the width/height given, keeping aspect ratio..                                    |
| [JSImage](./JSImage.md) | [rotate(degrees)](JSImage.md#rotate-degrees)                   | Rotates the image the number of degrees that is given..                                    |

## Methods Details

### flip(type)

Flips the image verticaly (type param=0) or horizontaly (type param=1). A new JSImage is returned.

**Parameters**\
[Number](../../JSLib/Number.md) type  ;

**Returns**\
[JSImage](./JSImage.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var image = plugins.images.getImage(byteArray_or_file_or_filename);//loads the image
image = image.flip(0);//flip vertically
var bytes = image.getData();//gets the image bytes
plugins.file.writeFile('filename',bytes);//saves the image bytes
```
### getContentType()

Gets the contenttype (image/jpeg) of this image.


**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var image = plugins.images.getImage(byteArray_or_file);
var width = image.getWidth();
var height = image.getHeight();
var contentType = image.getContentType();
```
### getData()

Gets the bytes of this image, so that they can be saved to disk or stored the database.


**Returns**\
[Array](../../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var image = plugins.images.getImage(byteArray_or_file_or_filename);//loads the image
image = image.resize(200,200);//resizes it to 200,200
var bytes = image.getData();//gets the image bytes
plugins.file.writeFile('filename',bytes);//saves the image bytes
```
### getHeight()

Gets the height of this image.


**Returns**\
[Number](../../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var image = plugins.images.getImage(byteArray_or_file);
var width = image.getWidth();
var height = image.getHeight();
var contentType = image.getContentType();
```
### getMetaDataDescription(property)

Gets the description of a metadata property from the image. Currently only jpg is supported.

**Parameters**\
[String](../../JSLib/String.md) property  ;

**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var image = plugins.images.getImage(byteArray_or_file_or_filename);//loads the image
// get the available metadata properties from the image, currently only jpg is supported
var propertiesArray = image.getMetaDataProperties();
for(var i=0;i<propertiesArray.length;i++)
{
	var property = propertiesArray[i]
	application.output("property: " + property);
	application.output("description (string): " + image.getMetaDataDescription(property))
	application.output("real object: " + image.getMetaDataObject(property))
}
// Thumbnail data is stored under property 'Exif - Thumbnail Data', extract that and set it in a dataprovider
thumbnail = image.getMetaDataObject("Exif - Thumbnail Data"); // gets thumbnail data from the image
```
### getMetaDataObject(property)

Gets the real object of a metadata property from the image. Currently only jpg is supported.

**Parameters**\
[String](../../JSLib/String.md) property  ;

**Returns**\
[Object](../../JSLib/Object.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var image = plugins.images.getImage(byteArray_or_file_or_filename);//loads the image
// get the available metadata properties from the image, currently only jpg is supported
var propertiesArray = image.getMetaDataProperties();
for(var i=0;i<propertiesArray.length;i++)
{
	var property = propertiesArray[i]
	application.output("property: " + property);
	application.output("description (string): " + image.getMetaDataDescription(property))
	application.output("real object: " + image.getMetaDataObject(property))
}
// Thumbnail data is stored under property 'Exif - Thumbnail Data', extract that and set it in a dataprovider
thumbnail = image.getMetaDataObject("Exif - Thumbnail Data"); // gets thumbnail data from the image
```
### getMetaDataProperties()

Gets the available metadata properties from the image. Currently only jpg is supported.


**Returns**\
[Array](../../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var image = plugins.images.getImage(byteArray_or_file_or_filename);//loads the image
// get the available metadata properties from the image, currently only jpg is supported
var propertiesArray = image.getMetaDataProperties();
for(var i=0;i<propertiesArray.length;i++)
{
	var property = propertiesArray[i]
	application.output("property: " + property);
	application.output("description (string): " + image.getMetaDataDescription(property))
	application.output("real object: " + image.getMetaDataObject(property))
}
// Thumbnail data is stored under property 'Exif - Thumbnail Data', extract that and set it in a dataprovider
thumbnail = image.getMetaDataObject("Exif - Thumbnail Data"); // gets thumbnail data from the image
```
### getWidth()

Gets the width of this image.


**Returns**\
[Number](../../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var image = plugins.images.getImage(byteArray_or_file);
var width = image.getWidth();
var height = image.getHeight();
var contentType = image.getContentType();
```
### resize(width, height)

Resizes the image to the width/height given, keeping aspect ratio. A new JSImage is returned.

**Parameters**\
[Number](../../JSLib/Number.md) width  ;\
[Number](../../JSLib/Number.md) height  ;

**Returns**\
[JSImage](./JSImage.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var image = plugins.images.getImage(byteArray_or_file_or_filename);//loads the image
image = image.resize(200,200);//resizes it to 200,200
var bytes = image.getData();//gets the image bytes
plugins.file.writeFile('filename',bytes);//saves the image bytes
```
### rotate(degrees)

Rotates the image the number of degrees that is given. A new JSImage is returned.

**Parameters**\
[Number](../../JSLib/Number.md) degrees  ;

**Returns**\
[JSImage](./JSImage.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var image = plugins.images.getImage(byteArray_or_file_or_filename);//loads the image
image = image.rotate(90);//rotate the image 90 degrees
var bytes = image.getData();//gets the image bytes
plugins.file.writeFile('filename',bytes);//saves the image bytes
```

