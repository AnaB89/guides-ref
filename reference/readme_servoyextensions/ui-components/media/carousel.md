# Carousel

The Carousel component offers a simple carousel to show several images in a slide show

![Carousel](https://github.com/Servoy/bootstrapextracomponents/wiki/carousel/images/image\_01.png)

## Table of contents

* [Carousel properties](carousel.md#carousel-properties)
* [Slide type](carousel.md#slide-type)
* [cssProperty type](carousel.md#cssproperty-type)
* [Carousel events](carousel.md#carousel-events)
* [Carousel API](carousel.md#carousel-api)

## Carousel properties

The component has the following properties:

| Property       | Type                                            | Default | Description                                                                                                                                                                                                                                                                          |
| -------------- | ----------------------------------------------- | ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| cycleInterval  | Number                                          | 5000    | Number of milliseconds between transitions; when <= 0, slides will not auto-cylce                                                                                                                                                                                                    |
| imageCss       | [cssProperty\[\]](carousel.md#cssproperty-type) | null    | css properties for the images; if set, the imageOptions property is ignored                                                                                                                                                                                                          |
| imageOptions   | String                                          | Reduce  | Attempts to size images of different sizes to either "Reduce" (images are only reduced when larger), "Reduce/Enlarge" (images are resized to fit the component), "Scale to fit" (images are proportionally resized to fit the component) and "Crop" (images are cut off when larger) |
| lazyLoading    | Boolean                                         | true    | When true, images are only loaded when needed                                                                                                                                                                                                                                        |
| noPause        | Boolean                                         | false   | When true, the animation does not stop when the mouse is over the component                                                                                                                                                                                                          |
| noTransition   | Boolean                                         | false   | Whether to disable the transition animation between slides                                                                                                                                                                                                                           |
| slides         | [slide\[\]](carousel.md#slide-type)             | null    | Array of slides to show                                                                                                                                                                                                                                                              |
| slidesFoundset | JSFoundSet                                      | null    | Foundset to load images from; the "image" dataprovider provides the image, the "caption" dataprovider provides the caption text shown                                                                                                                                                |
| styleClass     | Boolean                                         | true    | Additional style classe(s) of the component                                                                                                                                                                                                                                          |
| visible        | Boolean                                         | true    | The visible property of the component, default true.                                                                                                                                                                                                                                 |

### Slide type

Slide is a component specific javascript type with the following properties:

| Property | Type   | Default | Description                    |
| -------- | ------ | ------- | ------------------------------ |
| imageUrl | String | null    | The url to load the image from |
| caption  | String | null    | The caption text of the image  |

### cssProperty type

cssProperty is a component specific javascript type with the following properties:

| Property      | Type   | Default | Description                                        |
| ------------- | ------ | ------- | -------------------------------------------------- |
| propertyName  | String | null    | The name of the css property to set (e.g. 'width') |
| propertyValue | String | null    | The value of the property (e.g. '100%')            |

## Carousel events

The carousel currently has no events

## Carousel API

| Method                                           | Params                                     | Return | Description                                               |
| ------------------------------------------------ | ------------------------------------------ | ------ | --------------------------------------------------------- |
| [addSlide](carousel.md#addslide)                 | slideToAdd:[slide](carousel.md#slide-type) |        | Adds the given slide at the end of the list of slides.    |
| [removeSlide](carousel.md#removeslide)           | index:Number                               |        | Removes the slide at the given index (0 based).           |
| [getSelectedIndex](carousel.md#getselectedindex) |                                            | Number | Gets the index of the currently selected slide (0 based). |
| [setSelectedIndex](carousel.md#setselectedindex) | index:Number                               |        | Animates to the slide with the given index (0 based).     |
| [setSlides](carousel.md#setslides)               | slides:[slide\[\]](carousel.md#slide-type) |        | Sets all slides to be shown.                              |

### addSlide

Adds a [slide](carousel.md#slide-type) at the end of the list of slides

**Params**

| Type                            | Name  | Description                                | Required |
| ------------------------------- | ----- | ------------------------------------------ | -------- |
| [slide](carousel.md#slide-type) | slide | The [slide](carousel.md#slide-type) to add | Required |

**Returns** void

### removeSlide

Removes the slide at the given index (0 based)

**Params**

| Type   | Name  | Description                          | Required |
| ------ | ----- | ------------------------------------ | -------- |
| Number | index | The index at which to remove a slide | Required |

**Returns** void

### getSelectedIndex

Gets the index of the currently selected slide (0 based)

**Params** none

**Returns** Number slideIndex

### setSelectedIndex

Animates to the slide with the given index (0 based).

**Params**

| Type   | Name  | Description                      | Required |
| ------ | ----- | -------------------------------- | -------- |
| Number | index | The index of the slide to select | Required |

**Returns** void

### setSlides

Sets all slides to be shown in the carousel.

**Params**

| Type                                | Name   | Description       | Required |
| ----------------------------------- | ------ | ----------------- | -------- |
| [slide\[\]](carousel.md#slide-type) | slides | The slides to set | Required |

**Returns** void
