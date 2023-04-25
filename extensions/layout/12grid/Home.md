# Boostrap 12grid layout

Welcome to the 12grid wiki!

This is the bootstrap 12 grid layout package for making responsive forms. It is meant to work with the bootstrap components package or any other compatible component packages. You can build a responsive layout for your form using this combination or components and layouts. 12grid is based on bootstrap grid system, see https://getbootstrap.com/docs/5.0/layout/grid/ for more details.

## [Collapsible Container](Collapsible-Container.md)

![Collapsible Container IMG](images/2017-10-13\_1802.png)

## [Simple Collapsible](Simple-Collapsible.md)

![Simple Collapsible IMG](images/2017-10-13\_1555.png)

## [Center Container](Center-Container.md)

![Centered Container IMG](images/2017-10-13\_1814.png)

## [Inline Group Container](Inline-Group-Container.md)

![Inline Group Container IMG](images/2017-10-19\_1853.png)

## [Flexbox Layout](Flexbox-Layout.md)

![Flexbobx Layout IMG](images/2017-10-19\_1044.png)

## Nesting responsive forms

In responsive layouts, when you nest multiple forms using tab panels or other types of container-components it may happen that a tab/child form that has in it directly "row" layout containers (so no root layout "container" or layout "container-fluid") shows unwanted scroll-bars. That happens because bootstrap requires that all 'row' divs must either be put in a 'container', a 'container-fluid' or in a 'column', while in the case of a tabpanel for example the parent DOM Element is just some intermediate div. Because 'row' has negative margins of -15px and parent intermediate div might not have padding of 15px, the scrollbars can appear (if that div has overflow: auto). For example:

\| container\
\|    row\
\|      column\
\|         div style="overflow: auto" // the intermediate div of container-component\
\|           row // results in a scrollbar because of margin -15px\
\|             columns

The problem does not appear when a 'row' is inside a 'column', a 'container' or a 'container fluid' - because those have a padding of 15px defined. However, bootstrap doesn't allow nesting of containers in it's layout docs - so adding a container layout as root of child/contained form is not an option. But as the tabpanel might want to contain absolute forms as well (for example), that intermediate div cannot always set a 15px padding - as that might not be necessary... So we just need to change the margins of such rows as in the rule below (that is included already in "standard\_ngclient.css"):

```
div:not(.container):not(.container-fluid):not([class^="col-xs-"]):not([class^="col-sm-"]):not([class^="col-md-"]):not([class^="col-lg-"])
 > .row {
    margin-right: 0;
    margin-left: 0;
}
```
