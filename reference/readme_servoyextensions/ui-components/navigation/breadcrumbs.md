# Breadcrumbs

The Breadcrumbs components wraps the standard [Bootstrap breadcrumbs](http://getbootstrap.com/components/#breadcrumbs) used to display navigational hierarchy in a simple NG client component. Here is how the component looks like

![Breadcrumbs](../../../../extensions/ui-components/navigation/breadcrumbs/images/image\_01.png)

## Table of contents

* [Breadcrumbs properties](breadcrumbs.md#breadcrumbs-properties)
* [Crumb type](breadcrumbs.md#crumb-type)
* [Breadcrumbs events](breadcrumbs.md#breadcrumbs-events)
* [Breadcrumbs API](breadcrumbs.md#breadcrumbs-api)

## Breadcrumbs properties

The component has the following properties:

| Property              | Type                                   | Default | Description                                                                |
| --------------------- | -------------------------------------- | ------- | -------------------------------------------------------------------------- |
| autoRemoveWhenClicked | Boolean                                | true    | When true, all crumbs to the one that was clicked will be removed on click |
| breadcrumbs           | [crumb\[\]](breadcrumbs.md#crumb-type) | null    | An array of all crumbs                                                     |
| styleClass            | String                                 | null    | Additional style class(es) of the component                                |
| crumbStyleClass       | String                                 | null    | The style class used for crumbs                                            |
| lastCrumbStyleClass   | String                                 | null    | The style class used for the last crumb                                    |
| visible               | Boolean                                | true    | The visible property of the component, default true.                       |

### Crumb type

Crumb is a component specific javascript type with the following properties:

| Property    | Type   | Default | Description                                     |
| ----------- | ------ | ------- | ----------------------------------------------- |
| crumbId     | String | null    | An Id used to identify the crumb                |
| displayName | String | null    | The name of the crumb as shown in the component |

## Breadcrumbs events

| Event          | Params                                                                | Return | Description                   |
| -------------- | --------------------------------------------------------------------- | ------ | ----------------------------- |
| onCrumbClicked | event:JSEvent, crumb:[crumb](breadcrumbs.md#crumb-type), index:Number |        | Fired when a crumb is clicked |

## Breadcrumbs API

| Method                                                | Params                                        | Return | Description                                            |
| ----------------------------------------------------- | --------------------------------------------- | ------ | ------------------------------------------------------ |
| [addCrumb](breadcrumbs.md#addcrumb)                   | crumb:[crumb](breadcrumbs.md#crumb-type)      |        | Adds the given crumb to the end of the list of crumbs. |
| [removeLastCrumb](breadcrumbs.md#removelastcrumb)     |                                               |        | Removes the last crumb from the component.             |
| [setCrumbs](breadcrumbs.md#setcrumbs)                 | crumbs:[crumb\[\]](breadcrumbs.md#crumb-type) |        | Sets all crumbs of the component.                      |
| [removeCrumbsAfter](breadcrumbs.md#removecrumbsafter) | index:Number                                  |        | Removes all crumbs after the given index.              |

### addCrumb

Adds a [crumb](breadcrumbs.md#crumb-type) at the end

**Params**

| Type                               | Name  | Description                                   | Required |
| ---------------------------------- | ----- | --------------------------------------------- | -------- |
| [crumb](breadcrumbs.md#crumb-type) | crumb | The [crumb](breadcrumbs.md#crumb-type) to add | Required |

**Returns** void

### removeLastCrumb

Removes the last crumb

**Params** none

**Returns** void

### setCrumbs

Sets all crumbs

**Params**

| Type                                   | Name   | Description                                    | Required |
| -------------------------------------- | ------ | ---------------------------------------------- | -------- |
| [crumb\[\]](breadcrumbs.md#crumb-type) | crumbs | The [crumbs](breadcrumbs.md#crumb-type) to set | Required |

**Returns** void

### removeCrumbsAfter

Removes all crumbs after the given index

**Params**

| Type   | Name  | Description                                  | Required |
| ------ | ----- | -------------------------------------------- | -------- |
| Number | index | The index after which all crumbs are removed | Required |

**Returns** void
