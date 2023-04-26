# Split Pane

## Table of contents

* [Split Pane properties](split-pane.md#split-pane-properties)
* [Split Pane events](split-pane.md#split-pane-events)
* [Split Pane API](split-pane.md#split-pane-api)

## Split Pane properties

The component has the following properties:

| Property         | Type    | Default | Description                                                                                                    |
| ---------------- | ------- | ------- | -------------------------------------------------------------------------------------------------------------- |
| divLocation      | Number  | -1      | Divider location, -1 or .5 = middle, lower then .5 = close to left/top, higher then .5 = close to right/bottom |
| divSize          | Number  | 5       | Divider size in pixels                                                                                         |
| enabled          | Boolean | true    | Whether the component is enabled or not                                                                        |
| pane1MinSize     | Number  | 30      | Min size of first panel in pixels                                                                              |
| pane2MinSize     | Number  | 30      | Min size of second panel in pixels                                                                             |
| resizeWeight     | Number  | 0       | Specifies how to distribute extra space when the size of the split pane changes                                |
| panes            | pane\[] |         | Panes of the split pane                                                                                        |
| styleClass       | String  |         | Style class of this component                                                                                  |
| splitType        | Number  |         | Divider orientation, can be HORIZONTAL (0) or VERTICAL (1)                                                     |
| tabSeq           | Number  |         | Tab sequence index of the form                                                                                 |
| visible          | Boolean | true    | Whether the component is visible or not                                                                        |
| responsiveHeight | Number  | 300     | Height of this component                                                                                       |

## Split Pane events

The component allows to attach handlers for the following events:

| Event    | Parameters                          | Return | Description                          |
| -------- | ----------------------------------- | ------ | ------------------------------------ |
| onChange | previousIndex:Number, event:JSEvent |        | Fired after divider location changed |

## Split Pane API

The component offers the following API methods:

| Method              | Parameters          | Return  | Description                                                                                                                                                                                       |
| ------------------- | ------------------- | ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| getDividerLocation  |                     | Number  | Gets the divider location in pixels                                                                                                                                                               |
| getDividerSize      |                     | Number  | Gets the divider size in pixels                                                                                                                                                                   |
| getLeftForm         |                     | Form    | Returns the left form of the split pane                                                                                                                                                           |
| getLeftFormMinSize  |                     | Number  | Gets left form minimum size in pixels                                                                                                                                                             |
| getResizeWeight     |                     | Number  | Gets the resize weight, which specifies how to distribute extra space when the size of the split pane changes                                                                                     |
| getRightForm        |                     | Form    | Returns the right form of the split pane                                                                                                                                                          |
| getRightFormMinSize |                     | Number  | Gets right form minimum size in pixels                                                                                                                                                            |
| setDividerLocation  | location:Number     |         | Sets divider location. If location is less then 1 then the location will be considered at (location \* 100) percent of the split pane from left, otherwise it will represent the pixels from left |
| setDividerSize      | size:Number         |         | Sets divider size in pixels                                                                                                                                                                       |
| setLeftForm         | form:Form           | Boolean | Set a relationless or related form as left panel                                                                                                                                                  |
| setLeftFormMinSize  | minSize:Number      |         | Sets left form minimum size in pixels                                                                                                                                                             |
| setResizeWeight     | resizeWeight:Number |         | Sets the resize weight, which specifies how to distribute extra space when the size of the split pane changes                                                                                     |
| setRightForm        | form:Form           | Boolean | Set a relationless or related form as right panel                                                                                                                                                 |
| setRightFormMinSize | minSize:Number      |         | Sets right form minimum size in pixels                                                                                                                                                            |

### Pane type

Pane is a custom type of the split pane component holding properties of a single pane of the panel:

| Property      | Type     | Default | Description                                |
| ------------- | -------- | ------- | ------------------------------------------ |
| containedForm | form     |         | The form shown in the pane                 |
| relationName  | relation |         | Optional relation for the form to be shown |
