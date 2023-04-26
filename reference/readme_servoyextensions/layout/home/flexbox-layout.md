# Flexbox Layout

The flexbox layout divides the available height in 3 vertical sections, **header**, **content** and **footer**. The **header** and the **footer** section will grow in height depending on their content while the **content** section will take all the remaining height and show a scrollbar if the content doesn't fit.

**IMPORTANT!** The Flexbox layout is using the CSS3 Flexbox layout model. Now days the Flexbox model is largely supported from modern browsers (see [supported browsers](https://caniuse.com/#feat=flexbox)). However there are few known issues with IE and Safari (open the [Known issues](https://caniuse.com/#feat=flexbox) tab).

### Getting Started

You can drop Servoy any Servoy Web Components and nest other 12Grid containers into the **header**, **footer** and **content** section.

You may decide to leave empty the **header** or **footer** section, not necessarely you need to use these section; however you may use at least one of these 2 sections; otherwise you may not use this container at all since there is no benefit on using only the **content** section.

**IMPORTANT!** The parent container of the flexbox layout MUST have a known height, the flexbox layout is not useful at all if the height of it's top container is 'auto' (which is an unknown value). In case the parent container of the flexbox layout is the Servoy form itself, add a CSS styleClass to the form which will let the form use 100% of the available height.\
**IMPORTANT!** if the form is nested within another form via a tab/tabless panel, the panel MUST have a known height as well, so that the inner form can use 100% of the panel height.

![Flexbobx Layout IMG](../../../../extensions/layout/12grid/images/2017-10-19\_1044.png)

![Flexbox Layout Outline](../../../../extensions/layout/12grid/images/2017-10-19\_1029.png)

### Flexbox Layout and Table Components

When a Servoy Table Component from the [Bootstrap components](https://github.com/Servoy/bootstrapcomponents) package or from the [Servoy Extra](../../ui-components/grids/table.md) package or from the Servoy NG Grids package is placed within the content section of the flexbox layout as direct child, the table height will use 100% of the available height if the _responsiveHeight_ property is set to 0.

**NOTE** for the Table component from the Servoy Extra package the property _responsiveDynamicHeight_, should be set to _false_ if you wish to use all the available height of the content section; if the _responsiveDynamicHeight_ is set to _true_ the Table will have a max-height equal to the design _responsiveHeight_ property of the Table; the max-height may be smaller than the available height resulting in unused space.

If instead you prefer to use the design height of the Table component, wrap the Table component within a different 12Grid container. However letting the table use a different height than the available height in the content section may result in bad UX for the User since may result in double vertical scrollbars.

### Nesting Flexbox Layout

You can nest multiple FlexLayout within the **content** section to sub-divide the available height of the content section.

![FlexBox Layout Nested IMG](../../../../extensions/layout/12grid/images/2017-10-19\_1821.png)

![FlexBox Layout Nested Outline](../../../../extensions/layout/12grid/images/2017-10-19\_1823.png)

In the sample above the available height of the first flexbox layout content is divided in 2 blocks of 50% height using the custom styleClass _half-size_.

```
.half-size {
	height: 50%;
}
```

### Flexbox Layout and tab/tablesspanel

If you include a tab or tabless panel into the **content** section and you would like to let the panel use all the available height of the content section add a CSS styleClass to the tab or tabless panel component to let the panel use 100% of the height.
