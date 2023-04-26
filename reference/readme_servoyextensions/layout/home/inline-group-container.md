# Inline Group Container

The Inline Group Container allow you to use at best the available width dividing the available width in 3 horizontal section, **left**, **right** and **content**; the left and the right section will use all and only the necessary width depending on their content (if any); the **content** section instead will use all the remaining width.

![Inline Group Container IMG](../../../../extensions/layout/12grid/images/2017-10-19\_1853.png)

### Getting Started

You can drop Servoy any Servoy Web Components and nest other 12Grid containers into the **left**, **right** and **content** section.

You may decide to leave empty the **right** or **left** section, not necessarely you need to use these section; however you may use at least one of these 2 sections; otherwise you may not use this container at all since there is no benefit on using only the **content** section.

**IMPORTANT!** The parent container of the inline group container MUST have a known width, the inline group container is not useful at all if the width of it's top container is 'auto' (which is an unknown value).

![Inline Group Container Outline](../../../../extensions/layout/12grid/images/2017-10-19\_1852.png)

### Fixed Left/Right Section Size

You may force the **left** and or **right** section to a fixed width by setting the respectively the **data-leftsize** and **data-rightsize** attribute of the inline group container to one of the pre-defined values _xs_, _sm_, _md_, _lg_.

Setting a fixed size to a section is particoularly useful when you want to align multiple label and fields using multiple inline group containers.

![Fixed Section width IMG](../../../../extensions/layout/12grid/images/2017-10-19\_1921.png)

![Fixed Section width Outline](../../../../extensions/layout/12grid/images/2017-10-19\_1922.png)

You can override the default sizes of the pre-defined values by adding the following CSS rules to the CSS styleSheet of your Solution.

```
 /* Inline Group Sizes */
.inline-group[data-leftsize="xs"] > .inline-group-left,
.inline-group[data-rightsize="xs"] > .inline-group-right {
 	width: 40px;
}
 
.inline-group[data-leftsize="sm"] > .inline-group-left,
.inline-group[data-rightsize="sm"] > .inline-group-right {
 	width: 80px;
}
 
.inline-group[data-leftsize="md"] > .inline-group-left,
.inline-group[data-rightsize="md"] > .inline-group-right {
 	width: 120px;
}
 
.inline-group[data-leftsize="lg"] > .inline-group-left,
.inline-group[data-rightsize="lg"] > .inline-group-right {
 	width: 160px;
}
```

You can of course decide also to add your own CSS class to set a specific width to the section instead of using the pre-defined sizes.

### Responsive Section

You can enable a responsive behavior for the **left** section using the attribute **data-responsive** of the inline-group-container. You can select a breakpoint value (sm, md, lg) for which the left section will move into a new line when the screen size is smaller thane the breakpoint value; see the [Bootstrap CSS Media Query](https://getbootstrap.com/docs/3.0/css/#grid-media-queries) for the breakpoint values.

![Responsive Section IMG](../../../../extensions/layout/12grid/images/2017-10-19\_1903.png)

![Responsive Section Outline](../../../../extensions/layout/12grid/images/2017-10-19\_1901.png)

### Nesting Inline Group Containers

You can nest multiple inline group container within the content section to sub-divide the available width of the content section.
