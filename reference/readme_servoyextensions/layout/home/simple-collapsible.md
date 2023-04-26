# Simple Collapsible

The Simple Collapsible container allow to toggle the visibility of it's content in a Servoy Responsive Form. It has a toggle section and a content section; the toggle section is always visible and toggles the visibility of the content section when the user clicks on it.

![Simple Collapsible IMG](../../../../extensions/layout/12grid/images/2017-10-13\_1555.png)

**Note**: layout containers are not stateful, therefore the Simple Collapsible it will always return to it's design state when the user navigates away from the form or the browser is refreshed.

### Getting Started

You can drop Servoy Web Components and nest other 12Grid containers into both toggle and content section.

The Simple Collapsible uses attributes of it's inner _div_ containers to achieve the collapsible behavior. To obtain the collapsible behavior the "data-target" attribute of the "**simple-collapsible-toggle**" must target the correspondant "**simple-collapsible-content**" via CSS selector.

![Simple Collapsible Outline](../../../../extensions/layout/12grid/images/2017-10-13\_1551.png)

Is reccomanded to edit the default value and set an unique "**id**" attribute in the "**simple-collapsible-conten**t"; adjust accordingly the "**data-target**" of the "**simple-collapsible-toggle**".

### Change default toggle to collapsed

The collapsible container is expanded by default; you can modify the classes of it's sections to change the default state to collapsed.

![Collapsed](../../../../extensions/layout/12grid/images/2017-10-13\_1711.png)

Remove the class "**in**" from the "_simple-collapsible-content_" class property to collapse the content by default and add the class "**collapsed**" in the "_simple-collapsible-toggle_" class property.

![Collapsed Simple Container](../../../../extensions/layout/12grid/images/2017-10-13\_1722.png)

### Customize the toggle icon.

You can decide to remove the icon in the toggle section and place any component of your choice to be used as icon.

You can also change the default icon in the styleSheet of your solution using CSS3.

```
.simple-collapsible-toggle > .simple-collapsible-icon {
	font-family: "Glyphicons Halflings";
	display: inline-block;
}
.simple-collapsible-toggle > .simple-collapsible-icon:before {
	content: "\e113"; /* GlyphIcon chevron down when expanded */
}
.simple-collapsible-toggle.collapsed > .simple-collapsible-icon:before {
	content: "\e114"; /* GlyphIcon chevron up when collapsed */
}
```
