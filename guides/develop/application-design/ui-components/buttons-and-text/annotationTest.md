---
description: Guide for using buttons in your applications
---

# annotationTest

## Overview

This guide will show how to use buttons in your applications. See how easy it is to drag and drop buttons onto your forms and connect them to your business logic. Buttons can be modified, styled and even changed at runtime.

## Get Started

In the [Form Editor](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/servoy-core/page-3/object-editors/form-editor), drag the Button component from the Pallet onto the form.

<figure><img src="../../../../images/exampleButton - Add Button (1).gif" alt=""><figcaption><p>Add Button</p></figcaption></figure>

{% hint style="info" %}
If the component does not appear in the pallet, it means you do not have the Bootstrap Components package installed. Click "Get more components" at the top of the pallet to open the [Servoy Package Manager](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/servoy-core/page-3/package-manager) and install it.
{% endhint %}

## Modifying a Button at Design-Time

Buttons, like all components, have properties which can be modified at design-time[^desgin-time] to set the appearance and behavior of the component. Select the button in the [Form Editor](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/servoy-core/page-3/object-editors/form-editor) to see a list of properties in the [Component Properties Editor](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/servoy-core/page-3/object-editors/component-properties-editor). Below are some common properties and how to set them at design-time.

{% hint style="info" %}
See the reference docs for [Button](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/extensions/ui-components/buttons-and-text/button) for a complete list of its [properties](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/extensions/ui-components/buttons-and-text/button#button-properties).
{% endhint %}

### Setting the Text

The text displayed on a button can be modified by setting its [`text`](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/extensions/ui-components/buttons-and-text/button#text) property. Most often, this will just be plain text, such as "Submit" or "Cancel". In this case, just enter the value into the editor or directly on the component by double-clicking it. For more options open the [Text Property Editor](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/servoy-core/page-3/object-editors/text-property-editor).

### Setting a Tooltip message

Buttons, like many components, can display tooltip messages when a user hovers their cursor. Most often, this will just be plain text that describes what will happen on-click. In this case, just enter the value into the editor. For more options open the [Text Property Editor](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/servoy-core/page-3/object-editors/text-property-editor).

<figure><img src="../../../../images/exampleButton - tooltipText.gif" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Remember that text can also be dynamic, data-driven[^2] or localized[^3]. For more options, you can open edit the text property in the [Text Property Editor](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/servoy-core/page-3/object-editors/text-property-editor).
{% endhint %}

### Setting an Image / Font-Icon

Many times, a button will be decorated with an image or font icon. To add an image to your button, edit the [`imageStyleClass`](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/extensions/ui-components/buttons-and-text/button#imagestyleclass) property and choose the image style class of the font icon you wish to use. For example, enter a value of `fa fa-user-plus` to get a nice "Add User" icon.

<figure><img src="../../../../images/exampleButton - imageStyleClass.PNG" alt=""><figcaption></figcaption></figure>

For more information, please see the [Font Icon](../../styling-and-themes/font-icons.md) section of the giude on [Styling and Themes](../../styling-and-themes/).

### Styling

Like all components, a Button has a button can be styled using themes, variants and raw CSS. To apply any available style class, simply enter one or more space-delimited values for the `styleClass` property.

<img src="../../../../images/image.png" alt="" data-size="original">For example, `styleClass="btn btn-default btn-primary"`

#### Button Variants

If you are using Variants[^4], then you can easily drag and drop variations of your button onto your form.

<figure><img src="../../../../images/exampleButton - Variant.gif" alt=""><figcaption><p>Button Variant being dropped on a form</p></figcaption></figure>

## Handling Events

Like most components, Buttons have events, which allow you to execute some logic when something happens in the UI. Of course, the most common event for a button is the `onAction` event, which is triggered when the button is clicked or the user hits the `Enter` key while the button has focus.

To Handle the event, double-click the value for the `onAction` property in the [Properties Editor](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/servoy-core/page-3/object-editors/component-properties-editor). You will see the [Method Selection Wizard](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/servoy-core/page-3/object-editors/method-selection-wizard). You'll have the option select an existing Method or create a new Method. The method will be called when the button's `onAction` event is fired and the [Event](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/servoy-core/dev-api/application/jsevent) object will be passed to it.

<figure><img src="../../../../images/exampleButton - onAction (1).gif" alt=""><figcaption><p>Create a method t handle the onAction event</p></figcaption></figure>

```javascript
/**
 * @param {JSEvent} event
 *
 * @properties={typeid:24,uuid:"A74C281C-00AA-46AA-BB38-500C937F2D1A"}
 */
function onAction(event) {
	// Enter custom code
}
```

{% hint style="info" %}
See the [Button reference](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/extensions/ui-components/buttons-and-text/button) for comprehensive list of [all events](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/extensions/ui-components/buttons-and-text/button#events-summary)
{% endhint %}

## Modifying a Button at Runtime

Buttons, like many components, can be modified at runtime through code. Below are a few examples of controlling a Button from code.

### Enabling / Disabling a button

You can easily change the `enabled` state of a Button at runtime.

```javascript
function disableButton(){
	elements.myButton.enabled = false;
}
```

### Hiding/Showing a Button

You can easily change the `visible` state of a Button at runtime.

```javascript
function hideButton(){
	elements.myButton.visible = false;
}
```

## Calling Button API Methods

Like most components, a Button has API methods which can be called from code. Below is an example of common API calls.

### Give Keyboard Focus

You can easily give keyboard focus to a button using the [`requestFocus`](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/extensions/ui-components/buttons-and-text/button#requestfocus) method.

```javascript
function focusButton(){
	elements.myButton.requestFocus();
}
```

{% hint style="info" %}
See the [Button Reference Docs](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/extensions/ui-components/buttons-and-text/button) for a complete list of programmable [properties](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/extensions/ui-components/buttons-and-text/button#properties-summary) and [methods](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/extensions/ui-components/buttons-and-text/button#methods-summary).
{% endhint %}

## Related Articles

The following articles are recommended for additional reading:

* [Button Reference Documentation](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/extensions/ui-components/buttons-and-text/button)
* [Styling and Themes](../../styling-and-themes/)
* [Scripting the UI](../../../programming-guide/scripting-the-ui/)

1. Anywhere you show text, it can be translated and localized to the users language. For more information, read our guide on [Multi-Language Support](../../../multi-language-support.md)

[^desgin-time]: design-time annotation test

[^2]: Anywhere text is displayed, it can be substituted and merged with the data in context. For more information read about the [Text Property Editor](http://localhost:5000/s/QDXZ8sPLqo1Z0IswdI3w/servoy-core/page-3/object-editors/text-property-editor)

[^3]: Anywhere you show text, it can be translated and localized to the users language. For more information, read our guide on [Multi-Language Support](../../../multi-language-support.md)

[^4]: [Variants](../../styling-and-themes/component-variants.md) are pre-styled variations of components. You can create variants using theme properties and CSS and they will be available to quickly add to your forms. For more information, see the guid on [Styling and Themes](../../styling-and-themes/).
