# Smart Document Editor

## Getting Started

Welcome to the **Smart Docs Editor** project wiki! The editor is a standard Web Component which can be added to your Servoy application. To get going, simply open the Servoy Package Manager (SPM) in your IDE and choose the Smart Document Editor package. The component will be installed and available to place on your form.

\* Please see the companion [**Smart Docs Utils API**](../../modules/home-7/smart-doc-editor-utils.md#contents) module for the best documentation and examples.

**Working with documents**

Like all the standard input controls, the editor can be bound to a _"Data Provider"_ in your project. This means that the document contents will be automatically rendered from, and updated to any persistent data source column or session variable. In short, loading and saving documents is easy!

***

## API reference

***

**Properties**

| Property                  | Type                                        | Summary                                                                                                                                                                                                                                                                                                                                                                |
| ------------------------- | ------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Attributes**            | Object                                      | Standard property for all components. HTML attributes which can be sent to the browser. Simple `name:value` entries                                                                                                                                                                                                                                                    |
| **dataProvider**          | DataProvider\<String>                       | Standard property for many components. Binds the contents of the editor to a Data Provider, with data type `String`                                                                                                                                                                                                                                                    |
| **editorStyleSheet**      | String                                      | Override the default styling of the editor with a Style Sheet reference.                                                                                                                                                                                                                                                                                               |
| **language**              | String                                      | The language code that defines which language the editor controls will display. Default is the locale language of the client.                                                                                                                                                                                                                                          |
| **mentionFeeds**          | Array<[MentionFeeds](home.md#mentionfeeds)> | Defines the mention tags that will be used by the editor.                                                                                                                                                                                                                                                                                                              |
| **overWriteTabForEditor** | Boolean                                     | Defines the `TAB` key action in the editor. Default is `true`, meaning the `TAB` key is written in the document.                                                                                                                                                                                                                                                       |
| **readOnly**              | Boolean                                     | Can be used to lock the editor form receiving input. Default is `false`.                                                                                                                                                                                                                                                                                               |
| **responsiveHeight**      | Number                                      | The minimum height of the component. Only applies for a responsive form.                                                                                                                                                                                                                                                                                               |
| **showInspector**         | Boolean                                     | This can be used to enable the component inspector in the browser. The user can more easily troubleshoot the component and view the generated markup real-time. Default is `true`.                                                                                                                                                                                     |
| **showToolbar**           | Boolean                                     | This setting can be used to toggle the visibility of the toolbar. Default is `true`.                                                                                                                                                                                                                                                                                   |
| **styleClass**            | String                                      | Standard property for all components. Enables additional style customization.                                                                                                                                                                                                                                                                                          |
| **toolbarItems**          | Array<[ToolbarItems](home.md#toolbaritems)> | The items that will be shown in the toolbar.                                                                                                                                                                                                                                                                                                                           |
| **viewType**              | Enum\<DOCUMENT\|WEB>                        | This setting changes how the document will be displayed in the editor. The default is `DOCUMENT`, which shows a standard page layout view. This is ideal for printable docs. One can switch to `WEB` to enable a pure web view, where the editor will take up the entire space of its container. This is ideal for in-app use cases, such as comment/activity streams. |
| **visible**               | Boolean                                     | Standard property for all components. Toggles the visibility of the component.                                                                                                                                                                                                                                                                                         |

***

**Event Summary**

| Name                             | Summary                                                                                                                                                                                                                                            |
| -------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [**onAction**](home.md#onaction) | Standard event for all components to indicate a default action.                                                                                                                                                                                    |
| **onDataChange**                 | Standard event for all input controls to indicate that the model has changed. In the case of the editor, this event is invoked when the document contents are changed via the editor. (Unlike other input controls, the user need not lose focus.) |
| **onError**                      | An event to indicate that an unexpected runtime error has happened in the component rendering. This should be used only for debugging purposes.                                                                                                    |
| **onFileUploaded**               | Indicates that a file has been uploaded through the component.                                                                                                                                                                                     |
| **onFocusGained**                | Standard event for all input controls to indicate that the component acquired focus.                                                                                                                                                               |
| **onFocusLost**                  | Standard event for all input controls to indicate that the component lost focus.                                                                                                                                                                   |
| **onReady**                      | Indicates that the component is fully rendered and ready for user input, runtime commands.                                                                                                                                                         |

**Event Details**

***

### **onAction**

Standard event for all components to indicate a default action. In the case of the editor, the event is invoked if it is clicked while in a `readOnly` state.

### **Methods**

### **Custom Types**

### **MentionFeeds**

### **ToolbarItems**
