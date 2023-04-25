# Image label

A basic component for displaying an image from media library in html img tag. This component also supports svg images but doesn't support text.

NOTE: For svg images, we are seeing some issues with files which start with xml tag instead of svg. As soon as xl tag is removed the images display fine.

## Table of contents

* [Image label properties](Image-Label.md#image-label-properties)
* [Image label events](Image-Label.md#image-label-events)

## Image label properties

The component has the following properties:

| Property   | Type       | Default | Description                                                      |
| ---------- | ---------- | ------- | ---------------------------------------------------------------- |
| enabled    | enabled    | true    | When false image has disabled appearance and actions do not work |
| media      | media      | null    | The media image to display                                       |
| styleClass | styleclass | null    | Additional style class(es) of the component                      |
| tabSeq     | tabseq     | null    | Tab sequence number                                              |
| visible    | visible    | true    | When false component is not visible                              |

## Image label events

| Event                | Params        | Return | Description                          |
| -------------------- | ------------- | ------ | ------------------------------------ |
| onActionMethodID     | event:JSEvent |        | Fired when you click the image       |
| onRightClickMethodID | event:JSEvent |        | Fired when you right click the image |
