# Collapsible Container

The Collapsible Container is a responsive container, to be used in a Servoy Responsive Form, which behaves as a toggle on small screen sizes. When the size of the screen is smaller than 992px it presents a toggle section on which the user can click to toggle the visibility of it's content. On medium and large screens instead it always display it's content and hide it's toggle section.

![Collapsible Container](https://content.screencast.com/users/paronne/folders/Jing/media/dac324f1-368c-4487-8f53-d5e00018cdce/2017-10-13\_1737.png)

**Note**: layout containers are not stateful, therefore the Collapsible Container it will always return to it's design state when the user navigates away from the form or the browser is refreshed.

### Getting Started

You can drop Servoy Web Components and nest other 12Grid containers into both toggle and container section.

The Collapsible Container uses attributes of it's inner _div_ containers to achieve the collapsible behavior. To obtain the collapsible behavior the "data-target" attribute of the "**collapsible-toggle**" must target the correspondant "**collapsible-container**" via CSS selector.

![Collapsible Container Outline](../../../../extensions/layout/12grid/images/2017-10-13\_1754.png)

Is reccomanded to edit the default value and set an unique "**id**" attribute in the "**collapsible-container**"; adjust accordingly the "**data-target**" of the "**collapsible-toggle**".

### Change default toggle to expanded

The collapsible container is collaped by default on small screens; you can modify the classes of it's sections to change the default state to be expanded.

![Expanded](../../../../extensions/layout/12grid/images/2017-10-13\_1802.png)

Add the class "**in**" to the div having the "_collapsible-container_" class property to expand the content by default and remove the class "**collapsed**" from the div having "_collapsible-toggle_" class property.

![Expanded Collapsible Container Outline](../../../../extensions/layout/12grid/images/2017-10-13\_1801.png)

### Customize the toggle icon.

You can decide to remove the icon in the toggle section and place any component of your choice to be used as icon.
