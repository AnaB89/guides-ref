#  MEDIAOPTION

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [CROP](MEDIAOPTION.md#CROP)                   | Constant used when setting the media option for components which display images..                                    |
| [Number](../JSLib/Number.md) | [ENLARGE](MEDIAOPTION.md#ENLARGE)                   | Constant used when setting the media option for components which display images..                                    |
| [Number](../JSLib/Number.md) | [KEEPASPECT](MEDIAOPTION.md#KEEPASPECT)                   | Constant used when setting the media option for components which display images..                                    |
| [Number](../JSLib/Number.md) | [REDUCE](MEDIAOPTION.md#REDUCE)                   | Constant used when setting the media option for components which display images..                                    |

## Constants Details

### CROP

Constant used when setting the media option for components which display images.
Makes the image be displayed at its original size. If the component is smaller
than the image, then only a part of the image will show up.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var bigBytes = plugins.file.readFile('d:/big.jpg');
var bigImage = solutionModel.newMedia('big.jpg', bigBytes);
var smallBytes = plugins.file.readFile('d:/small.jpg');
var smallImage = solutionModel.newMedia('small.jpg', smallBytes);
var smallLabelWithBigImageCrop = form.newLabel('', 130, 10, 50, 50);
smallLabelWithBigImageCrop.imageMedia = bigImage;
smallLabelWithBigImageCrop.background = 'yellow';	
smallLabelWithBigImageCrop.mediaOptions = SM_MEDIAOPTION.CROP;
var bigLabelWithSmallImageCrop = form.newLabel('', 10, 290, 200, 100);
bigLabelWithSmallImageCrop.imageMedia = smallImage;
bigLabelWithSmallImageCrop.background = 'yellow';
bigLabelWithSmallImageCrop.mediaOptions = SM_MEDIAOPTION.CROP; // This does not do any cropping actually if the label is larger than the image.
```
### ENLARGE

Constant used when setting the media option for components which display images.
Makes the image be scaled up to fit the size of the component, if the component is
larger than the image. Can be used in combination with KEEPASPECT in order to preserve
the aspect ratio of the image.

It can also be used in combination with REDUCE, to cover all possibilities when
the size of the component is not known upfront.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var smallBytes = plugins.file.readFile('d:/small.jpg');
var smallImage = solutionModel.newMedia('small.jpg', smallBytes);
var bigLabelWithSmallImageEnlargeKeepAspect = form.newLabel('', 10, 70, 200, 100);
bigLabelWithSmallImageEnlargeKeepAspect.imageMedia = smallImage;
bigLabelWithSmallImageEnlargeKeepAspect.background = 'yellow';
bigLabelWithSmallImageEnlargeKeepAspect.mediaOptions = SM_MEDIAOPTION.ENLARGE | SM_MEDIAOPTION.KEEPASPECT;
var bigLabelWithSmallImageEnlargeNoAspect = form.newLabel('', 10, 180, 200, 100);
bigLabelWithSmallImageEnlargeNoAspect.imageMedia = smallImage;
bigLabelWithSmallImageEnlargeNoAspect.background = 'yellow';
bigLabelWithSmallImageEnlargeNoAspect.mediaOptions = SM_MEDIAOPTION.ENLARGE;
```
### KEEPASPECT

Constant used when setting the media option for components which display images.
Can be used in combination with REDUCE and/or ENLARGE, to maintain the aspect
ratio of the image while it is scaled down or up.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var bigBytes = plugins.file.readFile('d:/big.jpg');
var bigImage = solutionModel.newMedia('big.jpg', bigBytes);
var smallBytes = plugins.file.readFile('d:/small.jpg');
var smallImage = solutionModel.newMedia('small.jpg', smallBytes);
var smallLabelWithBigImageReduceKeepAspect = form.newLabel('', 10, 10, 50, 50);
smallLabelWithBigImageReduceKeepAspect.imageMedia = bigImage;
smallLabelWithBigImageReduceKeepAspect.background = 'yellow';	
smallLabelWithBigImageReduceKeepAspect.mediaOptions = SM_MEDIAOPTION.REDUCE | SM_MEDIAOPTION.KEEPASPECT;
var bigLabelWithSmallImageEnlargeKeepAspect = form.newLabel('', 10, 70, 200, 100);
bigLabelWithSmallImageEnlargeKeepAspect.imageMedia = smallImage;
bigLabelWithSmallImageEnlargeKeepAspect.background = 'yellow';
bigLabelWithSmallImageEnlargeKeepAspect.mediaOptions = SM_MEDIAOPTION.ENLARGE | SM_MEDIAOPTION.KEEPASPECT;
```
### REDUCE

Constant used when setting the media option for components which display images.
Makes the image be scaled down to fit the size of the component, if the component
is smaller than the image. It can be used in combination with KEEPASPECT in order
to preserve the aspect ratio of the image.

It can also be used in combination with ENLARGE, to cover all possibilities when
the size of the component is not known upfront.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var bigBytes = plugins.file.readFile('d:/big.jpg');
var bigImage = solutionModel.newMedia('big.jpg', bigBytes);
var smallLabelWithBigImageReduceKeepAspect = form.newLabel('', 10, 10, 50, 50);
smallLabelWithBigImageReduceKeepAspect.imageMedia = bigImage;
smallLabelWithBigImageReduceKeepAspect.background = 'yellow';	
smallLabelWithBigImageReduceKeepAspect.mediaOptions = SM_MEDIAOPTION.REDUCE | SM_MEDIAOPTION.KEEPASPECT;
var smallLabelWithBigImageReduceNoAspect = form.newLabel('', 70, 10, 50, 50);
smallLabelWithBigImageReduceNoAspect.imageMedia = bigImage;
smallLabelWithBigImageReduceNoAspect.background = 'yellow';	
smallLabelWithBigImageReduceNoAspect.mediaOptions = SM_MEDIAOPTION.REDUCE;
```

