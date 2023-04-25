#  JSForm


## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [String](../JSLib/String.md) | [EMPTY_FOUNDSET](JSForm.md#EMPTY_FOUNDSET)                   | Constant used for form namedFoundset property..                                    |
| [Number](../JSLib/Number.md) | [LIST_VIEW](JSForm.md#LIST_VIEW)                   | The constants to set or get the view property of a JSForm..                                    |
| [Number](../JSLib/Number.md) | [LOCKED_LIST_VIEW](JSForm.md#LOCKED_LIST_VIEW)                   | The constants to set or get the view property of a JSForm..                                    |
| [Number](../JSLib/Number.md) | [LOCKED_RECORD_VIEW](JSForm.md#LOCKED_RECORD_VIEW)                   | The constants to set or get the view property of a JSForm..                                    |
| [Number](../JSLib/Number.md) | [LOCKED_TABLE_VIEW](JSForm.md#LOCKED_TABLE_VIEW)                   | The constants to set or get the view property of a JSForm..                                    |
| [Number](../JSLib/Number.md) | [RECORD_VIEW](JSForm.md#RECORD_VIEW)                   | The constants to set or get the view property of a JSForm..                                    |
| [Number](../JSLib/Number.md) | [SELECTION_MODE_DEFAULT](JSForm.md#SELECTION_MODE_DEFAULT)                   | Constant used for form selectionMode property..                                    |
| [Number](../JSLib/Number.md) | [SELECTION_MODE_MULTI](JSForm.md#SELECTION_MODE_MULTI)                   | Constant used for form selectionMode property..                                    |
| [Number](../JSLib/Number.md) | [SELECTION_MODE_SINGLE](JSForm.md#SELECTION_MODE_SINGLE)                   | Constant used for form selectionMode property..                                    |
| [String](../JSLib/String.md) | [SEPARATE_FOUNDSET](JSForm.md#SEPARATE_FOUNDSET)                   | Constant used for form namedFoundset property..                                    |

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [borderType](JSForm.md#borderType)                   | The type, color and style of border of the component..                                    |
| [String](../JSLib/String.md) | [dataSource](JSForm.md#dataSource)                   | The names of the database server and table that this form is linked to..                                    |
| [Number](../JSLib/Number.md) | [encapsulation](JSForm.md#encapsulation)                   | Get or set the encapsulation level for the form..                                    |
| [JSForm](./JSForm.md) | [extendsForm](JSForm.md#extendsForm)                   | A JSForm instance representing the super form of this form, if this form has a super form..                                    |
| [String](../JSLib/String.md) | [initialSort](JSForm.md#initialSort)                   | The default sort order only when the form loads..                                    |
| [String](../JSLib/String.md) | [name](JSForm.md#name)                   | The name of the form..                                    |
| [String](../JSLib/String.md) | [namedFoundSet](JSForm.md#namedFoundSet)                   | Property that tells the form to use a named foundset instead of the default foundset..                                    |
| [Object](../JSLib/Object.md) | [navigator](JSForm.md#navigator)                   | The navigator (previously named "controller") that is used to control/navigate to the form..                                    |
| [Boolean](../JSLib/Boolean.md) | [ngReadOnlyMode](JSForm.md#ngReadOnlyMode)                   | Get or set the ngReadonlyMode for the form..                                    |
| [JSMethod](./JSMethod.md) | [onBeforeHide](JSForm.md#onBeforeHide)                   | This method is triggered when the form wants to hide; this will be called before onHide, and should be used to return if this form can be hidden or not..                                    |
| [JSMethod](./JSMethod.md) | [onDeleteAllRecordsCmd](JSForm.md#onDeleteAllRecordsCmd)                   | The method that overrides the Servoy menu item Select > Delete All..                                    |
| [JSMethod](./JSMethod.md) | [onDeleteRecordCmd](JSForm.md#onDeleteRecordCmd)                   | The method that overrides the Servoy menu item Select > Delete Record (or keyboard shortcut)..                                    |
| [JSMethod](./JSMethod.md) | [onDuplicateRecordCmd](JSForm.md#onDuplicateRecordCmd)                   | The method that overrides the Servoy menu item Select > Duplicate Record (or keyboard shortcut)..                                    |
| [JSMethod](./JSMethod.md) | [onElementDataChange](JSForm.md#onElementDataChange)                   | Method that is executed when the data in one of the form's component is successfully changed and the onDataChange callback from the component does not exist or exists and returned true.                                    |
| [JSMethod](./JSMethod.md) | [onElementFocusGained](JSForm.md#onElementFocusGained)                   | The method that is triggered when focus is gained by a component inside the form..                                    |
| [JSMethod](./JSMethod.md) | [onElementFocusLost](JSForm.md#onElementFocusLost)                   | The method that gets triggered when focus is lost by a component inside the form..                                    |
| [JSMethod](./JSMethod.md) | [onFindCmd](JSForm.md#onFindCmd)                   | The method that overrides the Servoy menu item Select > Find (or keyboard shortcut) in Data (ready) mode..                                    |
| [JSMethod](./JSMethod.md) | [onHide](JSForm.md#onHide)                   | This method is triggered when the form gets hidden..                                    |
| [JSMethod](./JSMethod.md) | [onInvertRecordsCmd](JSForm.md#onInvertRecordsCmd)                   | The method that overrides the Servoy menu item Select > Invert Records..                                    |
| [JSMethod](./JSMethod.md) | [onLoad](JSForm.md#onLoad)                   | The method that is triggered when a form is loaded/reloaded from the repository; used to alter elements, set globals, hide toolbars, etc; onShow method can also be assigned..                                    |
| [JSMethod](./JSMethod.md) | [onNewRecordCmd](JSForm.md#onNewRecordCmd)                   | The method that overrides the Servoy menu item Select > New Record (or keyboard shortcut)..                                    |
| [JSMethod](./JSMethod.md) | [onNextRecordCmd](JSForm.md#onNextRecordCmd)                   | The method that overrides the Servoy menu item Select > Next Record..                                    |
| [JSMethod](./JSMethod.md) | [onOmitRecordCmd](JSForm.md#onOmitRecordCmd)                   | The method that overrides the Servoy menu item Select > Omit Record..                                    |
| [JSMethod](./JSMethod.md) | [onPreviousRecordCmd](JSForm.md#onPreviousRecordCmd)                   | The method that overrides the Servoy menu item Select > Previous Record..                                    |
| [JSMethod](./JSMethod.md) | [onRecordEditStart](JSForm.md#onRecordEditStart)                   | The method that is triggered when a user clicks into a column on the form..                                    |
| [JSMethod](./JSMethod.md) | [onRecordEditStop](JSForm.md#onRecordEditStop)                   | The method that is triggered when a record is being saved..                                    |
| [JSMethod](./JSMethod.md) | [onRecordSelection](JSForm.md#onRecordSelection)                   | The method that is triggered each time a record is selected..                                    |
| [JSMethod](./JSMethod.md) | [onResize](JSForm.md#onResize)                   | The method that gets triggered when resize occurs..                                    |
| [JSMethod](./JSMethod.md) | [onSearchCmd](JSForm.md#onSearchCmd)                   | The method that overrides the Servoy menu item Select > Search (or keyboard shortcut) in Find mode..                                    |
| [JSMethod](./JSMethod.md) | [onShow](JSForm.md#onShow)                   | The method that is triggered EVERY TIME the form is displayed; an argument must be passed to the method if this is the first time the form is displayed..                                    |
| [JSMethod](./JSMethod.md) | [onShowAllRecordsCmd](JSForm.md#onShowAllRecordsCmd)                   | The method that overrides the Servoy menu item Select > Show All (or keyboard shortcut)..                                    |
| [JSMethod](./JSMethod.md) | [onShowOmittedRecordsCmd](JSForm.md#onShowOmittedRecordsCmd)                   | The method that overrides the Servoy menu item Select > Show Omitted Records..                                    |
| [JSMethod](./JSMethod.md) | [onSortCmd](JSForm.md#onSortCmd)                   | The method that overrides the Servoy menu item Select > Sort..                                    |
| [JSMethod](./JSMethod.md) | [onUnLoad](JSForm.md#onUnLoad)                   | The method that is triggered when a form is unloaded from the repository..                                    |
| [Boolean](../JSLib/Boolean.md) | [responsiveLayout](JSForm.md#responsiveLayout)                   | Returns true if this form is in responsive mode.                                    |
| [Number](../JSLib/Number.md) | [scrollbars](JSForm.md#scrollbars)                   | Scrollbar options for the vertical and horizontal scrollbars..                                    |
| [Number](../JSLib/Number.md) | [selectionMode](JSForm.md#selectionMode)                   | Returns the value of the form's selectionMode property..                                    |
| [String](../JSLib/String.md) | [serverName](JSForm.md#serverName)                   | Get the server name used by this form..                                    |
| [Boolean](../JSLib/Boolean.md) | [showInMenu](JSForm.md#showInMenu)                   | When set, the form is displayed under the Window menu..                                    |
| [String](../JSLib/String.md) | [styleClass](JSForm.md#styleClass)                   | The Cascading Style Sheet (CSS) class name applied to the form..                                    |
| [String](../JSLib/String.md) | [tableName](JSForm.md#tableName)                   | The [name of the table/SQL view]..                                    |
| [String](../JSLib/String.md) | [titleText](JSForm.md#titleText)                   | The text that displays in the title bar of the form window..                                    |
| [Boolean](../JSLib/Boolean.md) | [transparent](JSForm.md#transparent)                   | When set, the form is transparent..                                    |
| [Boolean](../JSLib/Boolean.md) | [useCssPosition](JSForm.md#useCssPosition)                   | Get or set the positioning (either use anchoring or use css position) for the form..                                    |
| [Number](../JSLib/Number.md) | [view](JSForm.md#view)                   | The default form view mode..                                    |
| [Number](../JSLib/Number.md) | [width](JSForm.md#width)                   | The width of the form in pixels..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSLayoutContainer](./JSLayoutContainer.md) | [findLayoutContainer(name)](JSForm.md#findlayoutcontainer-name)                   | Returns a JSLayoutContainer that has the given name throughout the whole form hierarchy..                                    |
| [JSComponent](./JSComponent.md) | [findWebComponent(name)](JSForm.md#findwebcomponent-name)                   | Returns a JSWebComponent that has the given name through the whole hierarchy of JSLayoutContainers.                                    |
| [JSComponent](./JSComponent.md) | [getBean(name)](JSForm.md#getbean-name)                   | Returns a JSBean that has the given name..                                    |
| [Array](../JSLib/Array.md) | [getBeans()](JSForm.md#getbeans)                   | Returns all JSBeans of this form..                                    |
| [Array](../JSLib/Array.md) | [getBeans(returnInheritedElements)](JSForm.md#getbeans-returninheritedelements)                   | Returns all JSBeans of this form..                                    |
| [JSPart](./JSPart.md) | [getBodyPart()](JSForm.md#getbodypart)                   | Retrieves the Body part of the form..                                    |
| [JSComponent](./JSComponent.md) | [getButton(name)](JSForm.md#getbutton-name)                   | Returns a JSButton that has the given name..                                    |
| [Array](../JSLib/Array.md) | [getButtons()](JSForm.md#getbuttons)                   | Returns all JSButtons of this form, including the ones without a name..                                    |
| [Array](../JSLib/Array.md) | [getButtons(returnInheritedElements)](JSForm.md#getbuttons-returninheritedelements)                   | Returns all JSButtons of this form, including the ones without a name..                                    |
| [String](../JSLib/String.md) | [getComment()](JSForm.md#getcomment)                   | Returns the comment of this container..                                    |
| [JSComponent](./JSComponent.md) | [getComponent(name)](JSForm.md#getcomponent-name)                   | Returns a JSComponent that has the given name; if found it will be a JSField, JSLabel, JSButton, JSPortal, JSBean, JSWebComponent or JSTabPanel..                                    |
| [Array](../JSLib/Array.md) | [getComponents()](JSForm.md#getcomponents)                   | Returns a array of all the JSComponents that a form has; they are of type JSField,JSLabel,JSButton,JSPortal,JSBean, JSWebComponents or JSTabPanel..                                    |
| [Array](../JSLib/Array.md) | [getComponents(returnInheritedElements)](JSForm.md#getcomponents-returninheritedelements)                   | Returns a array of all the JSComponents that a form has; they are of type JSField,JSLabel,JSButton,JSPortal,JSBean, JSWebComponent or JSTabPanel..                                    |
| [Object](../JSLib/Object.md) | [getDesignTimeProperty(key)](JSForm.md#getdesigntimeproperty-key)                   | Get a design-time property of a form..                                    |
| [Array](../JSLib/Array.md) | [getDesignTimePropertyNames()](JSForm.md#getdesigntimepropertynames)                   | Get the design-time properties of a form..                                    |
| [JSField](./JSField.md) | [getField(name)](JSForm.md#getfield-name)                   | The field with the specified name..                                    |
| [Array](../JSLib/Array.md) | [getFields()](JSForm.md#getfields)                   | Returns all JSField objects of this form, including the ones without a name..                                    |
| [Array](../JSLib/Array.md) | [getFields(returnInheritedElements)](JSForm.md#getfields-returninheritedelements)                   | Returns all JSField objects of this form, including the ones without a name..                                    |
| [JSPart](./JSPart.md) | [getFooterPart()](JSForm.md#getfooterpart)                   | Retrieves the Footer part of the form..                                    |
| [JSPart](./JSPart.md) | [getHeaderPart()](JSForm.md#getheaderpart)                   | Retrieves the Header part of the form..                                    |
| [JSComponent](./JSComponent.md) | [getLabel(name)](JSForm.md#getlabel-name)                   | Returns a JSLabel that has the given name..                                    |
| [Array](../JSLib/Array.md) | [getLabels()](JSForm.md#getlabels)                   | Returns all JSLabels of this form (not including its super form), including the ones without a name..                                    |
| [Array](../JSLib/Array.md) | [getLabels(returnInheritedElements)](JSForm.md#getlabels-returninheritedelements)                   | Returns all JSLabels of this form (optionally including it super forms labels), including the ones without a name..                                    |
| [JSLayoutContainer](./JSLayoutContainer.md) | [getLayoutContainer(name)](JSForm.md#getlayoutcontainer-name)                   | Returns a JSLayoutContainer that has the given name of this container..                                    |
| [Array](../JSLib/Array.md) | [getLayoutContainers()](JSForm.md#getlayoutcontainers)                   | Returns all JSLayoutContainers objects of this container..                                    |
| [Array](../JSLib/Array.md) | [getLayoutContainers(returnInheritedElements)](JSForm.md#getlayoutcontainers-returninheritedelements)                   | Returns all JSLayoutContainers objects of this container.                                    |
| [JSPart](./JSPart.md) | [getLeadingGrandSummaryPart()](JSForm.md#getleadinggrandsummarypart)                   | Retrieves the Leading Grand Summary part of the form..                                    |
| [Array](../JSLib/Array.md) | [getLeadingSubSummaryParts()](JSForm.md#getleadingsubsummaryparts)                   | Gets an array of the Leading Subsummary parts of the form, ordered by their height from top == 0 to bottom..                                    |
| [JSMethod](./JSMethod.md) | [getMethod(name)](JSForm.md#getmethod-name)                   | Gets an existing form method for the given name..                                    |
| [Array](../JSLib/Array.md) | [getMethods()](JSForm.md#getmethods)                   | Returns all existing form methods for this form..                                    |
| [Array](../JSLib/Array.md) | [getMethods(returnInheritedElements)](JSForm.md#getmethods-returninheritedelements)                   | Returns all existing form methods for this form..                                    |
| [JSPart](./JSPart.md) | [getPart(type)](JSForm.md#getpart-type)                   | Gets a part of the form from the given type (see JSPart constants)..                                    |
| [JSPart](./JSPart.md) | [getPart(type, height)](JSForm.md#getpart-type-height)                   | Gets a part of the form from the given type (see JSPart constants)..                                    |
| [Number](../JSLib/Number.md) | [getPartYOffset(type)](JSForm.md#getpartyoffset-type)                   | Returns the Y offset of a given part (see JSPart) of the form..                                    |
| [Number](../JSLib/Number.md) | [getPartYOffset(type, height)](JSForm.md#getpartyoffset-type-height)                   | Returns the Y offset of a given part (see JSPart) of the form..                                    |
| [Array](../JSLib/Array.md) | [getParts()](JSForm.md#getparts)                   | Gets all the parts from the form (not including the parts of the parent form), ordered by there height (lowerbound) property, from top == 0 to bottom..                                    |
| [Array](../JSLib/Array.md) | [getParts(returnInheritedElements)](JSForm.md#getparts-returninheritedelements)                   | Gets all the parts from the form (optionally also from the parent form), ordered by there height (lowerbound) property, from top == 0 to bottom..                                    |
| [JSComponent](./JSComponent.md) | [getPortal(name)](JSForm.md#getportal-name)                   | Returns a JSPortal that has the given name..                                    |
| [Array](../JSLib/Array.md) | [getPortals()](JSForm.md#getportals)                   | Returns all JSPortal objects of this form (not including the ones from the parent form), including the ones without a name..                                    |
| [Array](../JSLib/Array.md) | [getPortals(returnInheritedElements)](JSForm.md#getportals-returninheritedelements)                   | Returns all JSPortal objects of this form (optionally also the ones from the parent form), including the ones without a name..                                    |
| [JSComponent](./JSComponent.md) | [getTabPanel(name)](JSForm.md#gettabpanel-name)                   | Returns a JSTabPanel that has the given name..                                    |
| [Array](../JSLib/Array.md) | [getTabPanels()](JSForm.md#gettabpanels)                   | Returns all JSTabPanels of this form (not including the ones from the parent form), including the ones without a name..                                    |
| [Array](../JSLib/Array.md) | [getTabPanels(returnInheritedElements)](JSForm.md#gettabpanels-returninheritedelements)                   | Returns all JSTabPanels of this form (optionally the ones from the parent form), including the ones without a name..                                    |
| [JSPart](./JSPart.md) | [getTitleFooterPart()](JSForm.md#gettitlefooterpart)                   | Retrieves the Title Footer part of the form..                                    |
| [JSPart](./JSPart.md) | [getTitleHeaderPart()](JSForm.md#gettitleheaderpart)                   | Retrieves the Title Header part of the form..                                    |
| [JSPart](./JSPart.md) | [getTrailingGrandSummaryPart()](JSForm.md#gettrailinggrandsummarypart)                   | Retrieves the Trailing Grand Summary part of the form..                                    |
| [Array](../JSLib/Array.md) | [getTrailingSubSummaryParts()](JSForm.md#gettrailingsubsummaryparts)                   | Gets an array of the Trailing Subsummary parts of the form, ordered by their height from top == 0 to bottom..                                    |
| [UUID](../Application/UUID.md) | [getUUID()](JSForm.md#getuuid)                   | Returns the UUID of this form..                                    |
| [JSVariable](./JSVariable.md) | [getVariable(name)](JSForm.md#getvariable-name)                   | Gets an existing form variable for the given name..                                    |
| [Array](../JSLib/Array.md) | [getVariables()](JSForm.md#getvariables)                   | An array consisting of all form variables for this form..                                    |
| [Array](../JSLib/Array.md) | [getVariables(returnInheritedElements)](JSForm.md#getvariables-returninheritedelements)                   | An array consisting of all form variables for this form..                                    |
| [JSComponent](./JSComponent.md) | [getWebComponent(name)](JSForm.md#getwebcomponent-name)                   | Returns a JSWebComponent that has the given name that is a child of this layout container..                                    |
| [Array](../JSLib/Array.md) | [getWebComponents()](JSForm.md#getwebcomponents)                   | Returns all JSWebComponents of this form/container..                                    |
| [Array](../JSLib/Array.md) | [getWebComponents(returnInheritedElements)](JSForm.md#getwebcomponents-returninheritedelements)                   | Returns all JSWebComponents of this form/container..                                    |
| [JSComponent](./JSComponent.md) | [newBean(name, className, x, y, width, height)](JSForm.md#newbean-name-classname-x-y-width-height)                   | Creates a new JSBean object on the form - including the name of the JSBean object; the classname the JSBean object is based on, the "x" and "y" position of the JSBean object in pixels, as well as the width and height of the JSBean object in pixels..                                    |
| [JSComponent](./JSComponent.md) | [newButton(txt, x, y, width, height, action)](JSForm.md#newbutton-txt-x-y-width-height-action)                   | Creates a new button on the form with the given text, place, size and JSMethod as the onAction event triggered action..                                    |
| [JSComponent](./JSComponent.md) | [newButton(txt, action)](JSForm.md#newbutton-txt-action)                   | Creates a new button on the form with the given text and JSMethod as the onAction event triggered action..                                    |
| [JSField](./JSField.md) | [newCalendar(dataprovider)](JSForm.md#newcalendar-dataprovider)                   | Creates a new JSField object on the form with the displayType of CALENDAR - including the dataprovider/JSVariable of the JSField object..                                    |
| [JSField](./JSField.md) | [newCalendar(dataprovider, x, y, width, height)](JSForm.md#newcalendar-dataprovider-x-y-width-height)                   | Creates a new JSField object on the form with the displayType of CALENDAR - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels..                                    |
| [JSField](./JSField.md) | [newCheck(dataprovider)](JSForm.md#newcheck-dataprovider)                   | Creates a new JSField object on the form with the displayType of CHECK (checkbox) - including the dataprovider/JSVariable of the JSField object..                                    |
| [JSField](./JSField.md) | [newCheck(dataprovider, x, y, width, height)](JSForm.md#newcheck-dataprovider-x-y-width-height)                   | Creates a new JSField object on the form with the displayType of CHECK (checkbox) - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels..                                    |
| [JSField](./JSField.md) | [newComboBox(dataprovider)](JSForm.md#newcombobox-dataprovider)                   | Creates a new JSField object on the form with the displayType of COMBOBOX - including the dataprovider/JSVariable of the JSField object..                                    |
| [JSField](./JSField.md) | [newComboBox(dataprovider, x, y, width, height)](JSForm.md#newcombobox-dataprovider-x-y-width-height)                   | Creates a new JSField object on the form with the displayType of COMBOBOX - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels..                                    |
| [JSField](./JSField.md) | [newField(dataprovider, type)](JSForm.md#newfield-dataprovider-type)                   | Creates a new JSField object on the form - including the dataprovider/JSVariable of the JSField object..                                    |
| [JSField](./JSField.md) | [newField(dataprovider, type, x, y, width, height)](JSForm.md#newfield-dataprovider-type-x-y-width-height)                   | Creates a new JSField object on the form - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels..                                    |
| [JSPart](./JSPart.md) | [newFooterPart(height)](JSForm.md#newfooterpart-height)                   | Creates a new Footer part on the form..                                    |
| [JSPart](./JSPart.md) | [newHeaderPart(height)](JSForm.md#newheaderpart-height)                   | Creates a new Header part on the form..                                    |
| [JSField](./JSField.md) | [newHtmlArea(dataprovider)](JSForm.md#newhtmlarea-dataprovider)                   | Creates a new JSField object on the form with the displayType of HTML_AREA - including the dataprovider/JSVariable of the JSField object..                                    |
| [JSField](./JSField.md) | [newHtmlArea(dataprovider, x, y, width, height)](JSForm.md#newhtmlarea-dataprovider-x-y-width-height)                   | Creates a new JSField object on the form with the displayType of HTML_AREA - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels..                                    |
| [JSField](./JSField.md) | [newImageMedia(dataprovider)](JSForm.md#newimagemedia-dataprovider)                   | Creates a new JSField object on the form with the displayType of IMAGE_MEDIA - including the dataprovider/JSVariable of the JSField object..                                    |
| [JSField](./JSField.md) | [newImageMedia(dataprovider, x, y, width, height)](JSForm.md#newimagemedia-dataprovider-x-y-width-height)                   | Creates a new JSField object on the form with the displayType of IMAGE_MEDIA - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels..                                    |
| [JSComponent](./JSComponent.md) | [newLabel(txt)](JSForm.md#newlabel-txt)                   | Creates a new JSLabel object on the form - including the text of the label..                                    |
| [JSComponent](./JSComponent.md) | [newLabel(txt, x, y, width, height)](JSForm.md#newlabel-txt-x-y-width-height)                   | Creates a new JSLabel object on the form - including the text of the label, the "x" and "y" position of the label object in pixels, the width and height of the label object in pixels..                                    |
| [JSComponent](./JSComponent.md) | [newLabel(txt, x, y, width, height, action)](JSForm.md#newlabel-txt-x-y-width-height-action)                   | Creates a new JSLabel object on the form - including the text of the label, the "x" and "y" position of the label object in pixels, the width and height of the label object in pixels and a JSMethod action such as the method for an onAction event..                                    |
| [JSLayoutContainer](./JSLayoutContainer.md) | [newLayoutContainer()](JSForm.md#newlayoutcontainer)                   | Create a new layout container as the last child of its parent container..                                    |
| [JSLayoutContainer](./JSLayoutContainer.md) | [newLayoutContainer(position)](JSForm.md#newlayoutcontainer-position)                   | Create a new layout container..                                    |
| [JSLayoutContainer](./JSLayoutContainer.md) | [newLayoutContainer(position, spec)](JSForm.md#newlayoutcontainer-position-spec)                   | Create a new layout container..                                    |
| [JSLayoutContainer](./JSLayoutContainer.md) | [newLayoutContainer(spec)](JSForm.md#newlayoutcontainer-spec)                   | Create a new layout container as the last child in its parent container..                                    |
| [JSPart](./JSPart.md) | [newLeadingGrandSummaryPart(height)](JSForm.md#newleadinggrandsummarypart-height)                   | Creates a new Leading Grand Summary part on the form..                                    |
| [JSPart](./JSPart.md) | [newLeadingSubSummaryPart(height)](JSForm.md#newleadingsubsummarypart-height)                   | Creates a new Leading Subsummary part on the form..                                    |
| [JSField](./JSField.md) | [newListBox(dataprovider)](JSForm.md#newlistbox-dataprovider)                   | Creates a new JSField object on the form with the displayType of LISTBOX - including the dataprovider/JSVariable of the JSField object..                                    |
| [JSField](./JSField.md) | [newListBox(dataprovider, x, y, width, height)](JSForm.md#newlistbox-dataprovider-x-y-width-height)                   | Creates a new JSField object on the form with the displayType of LISTBOX - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels..                                    |
| [JSMethod](./JSMethod.md) | [newMethod(code)](JSForm.md#newmethod-code)                   | Creates a new form JSMethod - based on the specified code..                                    |
| [JSField](./JSField.md) | [newMultiSelectListBox(dataprovider)](JSForm.md#newmultiselectlistbox-dataprovider)                   | Creates a new JSField object on the form with the displayType of MULTISELECT_LISTBOX - including the dataprovider/JSVariable of the JSField object..                                    |
| [JSField](./JSField.md) | [newMultiSelectListBox(dataprovider, x, y, width, height)](JSForm.md#newmultiselectlistbox-dataprovider-x-y-width-height)                   | Creates a new JSField object on the form with the displayType of MULTISELECT_LISTBOX - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels..                                    |
| [JSPart](./JSPart.md) | [newPart(type, height)](JSForm.md#newpart-type-height)                   | Creates a new part on the form..                                    |
| [JSField](./JSField.md) | [newPassword(dataprovider)](JSForm.md#newpassword-dataprovider)                   | Creates a new JSField object on the form with the displayType of PASSWORD - including the dataprovider/JSVariable of the JSField object..                                    |
| [JSField](./JSField.md) | [newPassword(dataprovider, x, y, width, height)](JSForm.md#newpassword-dataprovider-x-y-width-height)                   | Creates a new JSField object on the form with the displayType of PASSWORD - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels..                                    |
| [JSComponent](./JSComponent.md) | [newPortal(name, relation)](JSForm.md#newportal-name-relation)                   | Creates a new JSPortal object on the form - including the name of the JSPortal object and the relation the JSPortal object is based on..                                    |
| [JSComponent](./JSComponent.md) | [newPortal(name, relation, x, y, width, height)](JSForm.md#newportal-name-relation-x-y-width-height)                   | Creates a new JSPortal object on the form - including the name of the JSPortal object; the relation the JSPortal object is based on, the "x" and "y" position of the JSPortal object in pixels, as well as the width and height of the JSPortal object in pixels..                                    |
| [JSField](./JSField.md) | [newRadios(dataprovider)](JSForm.md#newradios-dataprovider)                   | Creates a new JSField object on the form with the displayType of RADIOS (radio buttons) - including the dataprovider/JSVariable of the JSField object..                                    |
| [JSField](./JSField.md) | [newRadios(dataprovider, x, y, width, height)](JSForm.md#newradios-dataprovider-x-y-width-height)                   | Creates a new JSField object on the form with the displayType of RADIOS (radio buttons) - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels..                                    |
| [JSField](./JSField.md) | [newRtfArea(dataprovider, x, y, width, height)](JSForm.md#newrtfarea-dataprovider-x-y-width-height)                   | Creates a new JSField object on the form with the displayType of RTF_AREA (enables more than one line of text to be displayed in a field) - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels..                                    |
| [JSField](./JSField.md) | [newSpinner(dataprovider)](JSForm.md#newspinner-dataprovider)                   | Creates a new JSField object on the form with the displayType of SPINNER - including the dataprovider/JSVariable of the JSField object..                                    |
| [JSField](./JSField.md) | [newSpinner(dataprovider, x, y, width, height)](JSForm.md#newspinner-dataprovider-x-y-width-height)                   | Creates a new JSField object on the form with the displayType of SPINNER - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels..                                    |
| [JSComponent](./JSComponent.md) | [newTabPanel(name)](JSForm.md#newtabpanel-name)                   | Creates a new JSTabPanel object on the form - including the name of the JSTabPanel object..                                    |
| [JSComponent](./JSComponent.md) | [newTabPanel(name, x, y, width, height)](JSForm.md#newtabpanel-name-x-y-width-height)                   | Creates a new JSTabPanel object on the form - including the name of the JSTabPanel object, the "x" and "y" position of the JSTabPanel object in pixels, as well as the width and height of the JSTabPanel object in pixels..                                    |
| [JSField](./JSField.md) | [newTextArea(dataprovider)](JSForm.md#newtextarea-dataprovider)                   | Creates a new JSField object on the form with the displayType of TEXT_AREA - including the dataprovider/JSVariable of the JSField object..                                    |
| [JSField](./JSField.md) | [newTextArea(dataprovider, x, y, width, height)](JSForm.md#newtextarea-dataprovider-x-y-width-height)                   | Creates a new JSField object on the form with the displayType of TEXT_AREA - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels..                                    |
| [JSField](./JSField.md) | [newTextField(dataprovider)](JSForm.md#newtextfield-dataprovider)                   | Creates a new JSField object on the form with the displayType of TEXT_FIELD - including the dataprovider/JSVariable of the JSField object..                                    |
| [JSField](./JSField.md) | [newTextField(dataprovider, x, y, width, height)](JSForm.md#newtextfield-dataprovider-x-y-width-height)                   | Creates a new JSField object on the form with the displayType of TEXT_FIELD - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels..                                    |
| [JSPart](./JSPart.md) | [newTitleFooterPart(height)](JSForm.md#newtitlefooterpart-height)                   | Creates a new Title Footer part on the form..                                    |
| [JSPart](./JSPart.md) | [newTitleHeaderPart(height)](JSForm.md#newtitleheaderpart-height)                   | Creates a new Title Header part on the form..                                    |
| [JSPart](./JSPart.md) | [newTrailingGrandSummaryPart(height)](JSForm.md#newtrailinggrandsummarypart-height)                   | Creates a new Trailing Grand Summary part on the form..                                    |
| [JSPart](./JSPart.md) | [newTrailingSubSummaryPart(height)](JSForm.md#newtrailingsubsummarypart-height)                   | Creates a new Trailing Subsummary part on the form..                                    |
| [JSField](./JSField.md) | [newTypeAhead(dataprovider)](JSForm.md#newtypeahead-dataprovider)                   | Creates a new JSField object on the form with the displayType of TYPE_AHEAD - including the dataprovider/JSVariable of the JSField object..                                    |
| [JSField](./JSField.md) | [newTypeAhead(dataprovider, x, y, width, height)](JSForm.md#newtypeahead-dataprovider-x-y-width-height)                   | Creates a new JSField object on the form with the displayType of TYPE_AHEAD - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels..                                    |
| [JSVariable](./JSVariable.md) | [newVariable(name, type)](JSForm.md#newvariable-name-type)                   | Creates a new form JSVariable - based on the name of the variable object and the number type, uses the SolutionModel JSVariable constants..                                    |
| [JSVariable](./JSVariable.md) | [newVariable(name, type, defaultValue)](JSForm.md#newvariable-name-type-defaultvalue)                   | Creates a new form JSVariable - based on the name of the variable object , the  type  and it's default value , uses the SolutionModel JSVariable constants..                                    |
| [JSComponent](./JSComponent.md) | [newWebComponent(type)](JSForm.md#newwebcomponent-type)                   | Creates a new JSWebComponent (spec based component) object on the RESPONSIVE form..                                    |
| [JSComponent](./JSComponent.md) | [newWebComponent(type, position)](JSForm.md#newwebcomponent-type-position)                   | Creates a new JSWebComponent (spec based component) object on the RESPONSIVE form..                                    |
| [JSComponent](./JSComponent.md) | [newWebComponent(name, type)](JSForm.md#newwebcomponent-name-type)                   | Creates a new JSWebComponent (spec based component) object on a form..                                    |
| [JSComponent](./JSComponent.md) | [newWebComponent(name, type, position)](JSForm.md#newwebcomponent-name-type-position)                   | Creates a new JSWebComponent (spec based component) object on the RESPONSIVE form..                                    |
| [JSComponent](./JSComponent.md) | [newWebComponent(name, type, x, y, width, height)](JSForm.md#newwebcomponent-name-type-x-y-width-height)                   | Creates a new JSWebComponent (spec based component) object on the form..                                    |
| [Object](../JSLib/Object.md) | [putDesignTimeProperty(key, value)](JSForm.md#putdesigntimeproperty-key-value)                   | Set a design-time property of a form..                                    |
| [Boolean](../JSLib/Boolean.md) | [removeBean(name)](JSForm.md#removebean-name)                   | Removes a JSBean that has the specified name..                                    |
| [Boolean](../JSLib/Boolean.md) | [removeButton(name)](JSForm.md#removebutton-name)                   | Removes a JSButton that has the specified name..                                    |
| [Boolean](../JSLib/Boolean.md) | [removeComponent(name)](JSForm.md#removecomponent-name)                   | Removes a component (JSLabel, JSButton, JSField, JSPortal, JSBean, JSTabpanel, JSWebComponent) that has the given name..                                    |
| [Object](../JSLib/Object.md) | [removeDesignTimeProperty(key)](JSForm.md#removedesigntimeproperty-key)                   | Clear a design-time property of a form..                                    |
| [Boolean](../JSLib/Boolean.md) | [removeField(name)](JSForm.md#removefield-name)                   | Removes a JSField that has the given name..                                    |
| [Boolean](../JSLib/Boolean.md) | [removeLabel(name)](JSForm.md#removelabel-name)                   | Removes a JSLabel that has the given name..                                    |
| [Boolean](../JSLib/Boolean.md) | [removeMethod(name)](JSForm.md#removemethod-name)                   | Removes a  form JSMethod - based on the specified code..                                    |
| [Boolean](../JSLib/Boolean.md) | [removePart(type)](JSForm.md#removepart-type)                   | Removes a JSPart of the given type..                                    |
| [Boolean](../JSLib/Boolean.md) | [removePart(type, height)](JSForm.md#removepart-type-height)                   | Removes a JSPart of the given type..                                    |
| [Boolean](../JSLib/Boolean.md) | [removePortal(name)](JSForm.md#removeportal-name)                   | Removes a JSPortal that has the given name..                                    |
| [Boolean](../JSLib/Boolean.md) | [removeTabPanel(name)](JSForm.md#removetabpanel-name)                   | Removes a JSTabPanel that has the given name..                                    |
| [Boolean](../JSLib/Boolean.md) | [removeVariable(name)](JSForm.md#removevariable-name)                   | Removes a form JSVariable - based on the name of the variable object..                                    |
| [Boolean](../JSLib/Boolean.md) | [removeWebComponent(name)](JSForm.md#removewebcomponent-name)                   | Removes a JSWebComponent that has the specified name..                                    |

## Constants Details

### EMPTY_FOUNDSET

Constant used for form namedFoundset property. The form that uses empty namedFoundset will initially have an empty (cleared) foundset.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
// form with empty foundset
var frmEmpty = solutionModel.newForm('products_empty', 'example_data', 'products', null, true, 640, 480);
frmEmpty.newLabel("Empty FoundSet",10,10,200,20);
frmEmpty.newField('categoryid',JSField.TEXT_FIELD,10,40,200,20);
frmEmpty.newField('productname',JSField.TEXT_FIELD,10,70,200,20);
frmEmpty.namedFoundSet = JSForm.EMPTY_FOUNDSET;
```
### LIST_VIEW

The constants to set or get the view property of a JSForm. 
They are as follows: JSForm.LIST_VIEW, JSForm.LOCKED_LIST_VIEW, JSForm.LOCKED_RECORD_VIEW, JSForm.LOCKED_TABLE_VIEW, JSForm.RECORD_VIEW.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var myListViewForm = solutionModel.newForm('newForm1', myDatasource, myStyleName, false, 800, 600);
myListViewForm.view = JSForm.LIST_VIEW;

var myLockedListViewForm = solutionModel.newForm('newForm2', myDatasource, myStyleName, false, 800, 600);	
myLockedListViewForm.view = JSForm.LOCKED_LIST_VIEW;

var myLockedRecordViewForm = solutionModel.newForm('newForm3', myDatasource, myStyleName, false, 800, 600);
myLockedRecordViewForm.view = JSForm.LOCKED_RECORD_VIEW;

var myLockedTableViewForm = solutionModel.newForm('newForm4', myDatasource, myStyleName, false, 800, 600);
myLockedTableViewForm.view = JSForm.LOCKED_TABLE_VIEW;

var myRecordViewForm = solutionModel.newForm('newForm5', myDatasource, myStyleName, false, 800, 600);
myRecordViewForm.view = JSForm.RECORD_VIEW;
```
### LOCKED_LIST_VIEW

The constants to set or get the view property of a JSForm. 
They are as follows: JSForm.LIST_VIEW, JSForm.LOCKED_LIST_VIEW, JSForm.LOCKED_RECORD_VIEW, JSForm.LOCKED_TABLE_VIEW, JSForm.RECORD_VIEW.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var myListViewForm = solutionModel.newForm('newForm1', myDatasource, myStyleName, false, 800, 600);
myListViewForm.view = JSForm.LIST_VIEW;

var myLockedListViewForm = solutionModel.newForm('newForm2', myDatasource, myStyleName, false, 800, 600);	
myLockedListViewForm.view = JSForm.LOCKED_LIST_VIEW;

var myLockedRecordViewForm = solutionModel.newForm('newForm3', myDatasource, myStyleName, false, 800, 600);
myLockedRecordViewForm.view = JSForm.LOCKED_RECORD_VIEW;

var myLockedTableViewForm = solutionModel.newForm('newForm4', myDatasource, myStyleName, false, 800, 600);
myLockedTableViewForm.view = JSForm.LOCKED_TABLE_VIEW;

var myRecordViewForm = solutionModel.newForm('newForm5', myDatasource, myStyleName, false, 800, 600);
myRecordViewForm.view = JSForm.RECORD_VIEW;
```
### LOCKED_RECORD_VIEW

The constants to set or get the view property of a JSForm. 
They are as follows: JSForm.LIST_VIEW, JSForm.LOCKED_LIST_VIEW, JSForm.LOCKED_RECORD_VIEW, JSForm.LOCKED_TABLE_VIEW, JSForm.RECORD_VIEW.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var myListViewForm = solutionModel.newForm('newForm1', myDatasource, myStyleName, false, 800, 600);
myListViewForm.view = JSForm.LIST_VIEW;

var myLockedListViewForm = solutionModel.newForm('newForm2', myDatasource, myStyleName, false, 800, 600);	
myLockedListViewForm.view = JSForm.LOCKED_LIST_VIEW;

var myLockedRecordViewForm = solutionModel.newForm('newForm3', myDatasource, myStyleName, false, 800, 600);
myLockedRecordViewForm.view = JSForm.LOCKED_RECORD_VIEW;

var myLockedTableViewForm = solutionModel.newForm('newForm4', myDatasource, myStyleName, false, 800, 600);
myLockedTableViewForm.view = JSForm.LOCKED_TABLE_VIEW;

var myRecordViewForm = solutionModel.newForm('newForm5', myDatasource, myStyleName, false, 800, 600);
myRecordViewForm.view = JSForm.RECORD_VIEW;
```
### LOCKED_TABLE_VIEW

The constants to set or get the view property of a JSForm. 
They are as follows: JSForm.LIST_VIEW, JSForm.LOCKED_LIST_VIEW, JSForm.LOCKED_RECORD_VIEW, JSForm.LOCKED_TABLE_VIEW, JSForm.RECORD_VIEW.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var myListViewForm = solutionModel.newForm('newForm1', myDatasource, myStyleName, false, 800, 600);
myListViewForm.view = JSForm.LIST_VIEW;

var myLockedListViewForm = solutionModel.newForm('newForm2', myDatasource, myStyleName, false, 800, 600);	
myLockedListViewForm.view = JSForm.LOCKED_LIST_VIEW;

var myLockedRecordViewForm = solutionModel.newForm('newForm3', myDatasource, myStyleName, false, 800, 600);
myLockedRecordViewForm.view = JSForm.LOCKED_RECORD_VIEW;

var myLockedTableViewForm = solutionModel.newForm('newForm4', myDatasource, myStyleName, false, 800, 600);
myLockedTableViewForm.view = JSForm.LOCKED_TABLE_VIEW;

var myRecordViewForm = solutionModel.newForm('newForm5', myDatasource, myStyleName, false, 800, 600);
myRecordViewForm.view = JSForm.RECORD_VIEW;
```
### RECORD_VIEW

The constants to set or get the view property of a JSForm. 
They are as follows: JSForm.LIST_VIEW, JSForm.LOCKED_LIST_VIEW, JSForm.LOCKED_RECORD_VIEW, JSForm.LOCKED_TABLE_VIEW, JSForm.RECORD_VIEW.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var myListViewForm = solutionModel.newForm('newForm1', myDatasource, myStyleName, false, 800, 600);
myListViewForm.view = JSForm.LIST_VIEW;

var myLockedListViewForm = solutionModel.newForm('newForm2', myDatasource, myStyleName, false, 800, 600);	
myLockedListViewForm.view = JSForm.LOCKED_LIST_VIEW;

var myLockedRecordViewForm = solutionModel.newForm('newForm3', myDatasource, myStyleName, false, 800, 600);
myLockedRecordViewForm.view = JSForm.LOCKED_RECORD_VIEW;

var myLockedTableViewForm = solutionModel.newForm('newForm4', myDatasource, myStyleName, false, 800, 600);
myLockedTableViewForm.view = JSForm.LOCKED_TABLE_VIEW;

var myRecordViewForm = solutionModel.newForm('newForm5', myDatasource, myStyleName, false, 800, 600);
myRecordViewForm.view = JSForm.RECORD_VIEW;
```
### SELECTION_MODE_DEFAULT

Constant used for form selectionMode property. It means that the foundset's multiSelect property is used.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var myForm = solutionModel.getForm('my_form_name');
myForm.selectionMode = JSForm.SELECTION_MODE_DEFAULT;
```
### SELECTION_MODE_MULTI

Constant used for form selectionMode property. It means that the form will force multiSelect to true on the foundset it uses.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var myForm = solutionModel.getForm('my_form_name');
myForm.selectionMode = JSForm.SELECTION_MODE_MULTI;
```
### SELECTION_MODE_SINGLE

Constant used for form selectionMode property. It means that the form will force multiSelect to false on the foundset it uses.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var myForm = solutionModel.getForm('my_form_name');
myForm.selectionMode = JSForm.SELECTION_MODE_SINGLE;
```
### SEPARATE_FOUNDSET

Constant used for form namedFoundset property. The form that uses a separate namedFoundset will initially have an separate (not shared with other forms) foundset.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
// form with separate foundset
var frmSeparate = solutionModel.newForm('products_separate', 'example_data', 'products', null, true, 640, 480);
frmSeparate.newLabel("Separate FoundSet",10,10,200,20);
frmSeparate.newField('categoryid',JSField.TEXT_FIELD,10,40,200,20);
frmSeparate.newField('productname',JSField.TEXT_FIELD,10,70,200,20);
frmSeparate.namedFoundSet = JSForm.SEPARATE_FOUNDSET;
forms['products_separate'].controller.find();
forms['products_separate'].categoryid = '=2';
forms['products_separate'].controller.search();
```

## Properties Details

### borderType

The type, color and style of border of the component.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
//HINT: To know exactly the notation of this property set it in the designer and then read it once out through the solution model.
var field = form.newField('my_table_text', JSField.TEXT_FIELD, 10, 10, 100, 20);
field.borderType = solutionModel.createLineBorder(1,'#ff0000');
```
### dataSource

The names of the database server and table that this form is linked to.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var myForm = solutionModel.newForm('newForm', 'db:/a_server/a_table', 'aStyleName', false, 800, 600)
myForm.dataSource = 'db:/anotherServerName/anotherTableName'
```
### encapsulation

Get or set the encapsulation level for the form.

Encapsulation is one of constants JSForm.DEFAULT_ENCAPSULATION, JSForm.PRIVATE_ENCAPSULATION, JSForm.MODULE_PRIVATE_ENCAPSULATION,
JSForm.HIDE_DATAPROVIDERS_ENCAPSULATION, JSForm.HIDE_FOUNDSET_ENCAPSULATION, JSForm.HIDE_CONTROLLER_ENCAPSULATION or JSForm.HIDE_ELEMENTS_ENCAPSULATION

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var myForm = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
myForm.encapsulation = JSForm.HIDE_CONTROLLER_ENCAPSULATION;
```
### extendsForm

A JSForm instance representing the super form of this form, if this form has a super form.

**Returns**\
[JSForm](./JSForm.md) 


**Sample**

```javascript
var subForm = solutionModel.newForm('childForm',myDatasource,null,true,800,600);
var superForm = solutionModel.newForm('childForm',myDatasource,null,true,800,600);
subForm.extendsForm = superForm;
```
### initialSort

The default sort order only when the form loads.
This is applied each time an internal SQL query is being executed (find, find-all, open form); and is only executed when no other manual sort has been performed on the foundset.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var form = solutionModel.newForm('myForm',myDatasource,null,true,800,600);
form.initialSort = "column1 desc, column2 asc, column3 asc";
```
### name

The name of the form.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var form = solutionModel.newForm('myForm',myDatasource,null,true,800,600);
var formName = form.name;
application.output(formName);
```
### namedFoundSet

Property that tells the form to use a named foundset instead of the default foundset.
When JSForm.SEPARATE_FOUNDSET is specified the form will always create a copy of assigned foundset and therefore become separated from other foundsets.
When JSForm.EMPTY_FOUNDSET, the form will have an initially empty foundset.

The namedFoundset can be based on a global relation; in this case namedFoundset is the relation's name.
You can also set the namedFoundset to a JSRelation object directly.
It will tell this form to initially load a global relation based foundset.
The global relation's foreign datasource must match the form's datasource.
Do not use relations named "empty" or "separate" to avoid confusions.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
// form with separate foundset
var frmSeparate = solutionModel.newForm('products_separate', 'db:/example_data/products', null, true, 640, 480);
frmSeparate.newLabel("Separate FoundSet",10,10,200,20);
frmSeparate.newField('categoryid',JSField.TEXT_FIELD,10,40,200,20);
frmSeparate.newField('productname',JSField.TEXT_FIELD,10,70,200,20);
frmSeparate.namedFoundSet = JSForm.SEPARATE_FOUNDSET;
forms['products_separate'].controller.find();
forms['products_separate'].categoryid = '=2';
forms['products_separate'].controller.search();

// form with empty foundset
var frmEmpty = solutionModel.newForm('products_empty', 'db:/example_data/products', null, true, 640, 480);
frmEmpty.newLabel("Empty FoundSet",10,10,200,20);
frmEmpty.newField('categoryid',JSField.TEXT_FIELD,10,40,200,20);
frmEmpty.newField('productname',JSField.TEXT_FIELD,10,70,200,20);
frmEmpty.namedFoundSet = JSForm.EMPTY_FOUNDSET;

// form with an initial foundset based on a global relation
var frmGlobalRel = solutionModel.newForm("categories_related", solutionModel.getForm("categories"));
frmGlobalRel.namedFoundSet = "g2_to_category_name";

// form with an initial foundset based on a global relation
var frmGlobalRel = solutionModel.newForm("categories_related", solutionModel.getForm("categories"));
frmGlobalRel.namedFoundSet = solutionModel.getRelation("g1_to_categories");
```
### navigator

The navigator (previously named "controller")
that is used to control/navigate to the form. The navigator is shown at
the left or at the right side of the form, depending on the page orientation.

The following options are available:
-none- - no navigator is assigned.
DEFAULT - the Servoy default navigator is assigned.
IGNORE - the navigator last assigned to a previous form.
Custom - a custom navigator based on a selected form.

**Returns**\
[Object](../JSLib/Object.md) 


**Sample**

```javascript
var aForm = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
// you can also use SM_DEFAULTS.INGORE to just reuse the navigator that is already set, or SM_DEFAULTS.DEFAULT to have the default servoy navigator.
// here we assign an other new form as the navigator.
var aNavigator = solutionModel.newForm('navForm', myDatasource, null, false, 800, 600);
// set the navigators navigator to NONE
aNavigator.navigator = SM_DEFAULTS.NONE; // Hide the navigator on the form.
myListViewForm.navigator = aNavigator;
application.output(myListViewForm.navigator.name);
```
### ngReadOnlyMode

Get or set the ngReadonlyMode for the form. This flag is a performance optimization for tableview/listview to show labels instead of editable fields.

**Returns**\
[Boolean](../JSLib/Boolean.md) 


**Sample**

```javascript
var myForm = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
myForm.ngReadOnlyMode = true;
```
### onBeforeHide

This method is triggered when the form wants to hide; this will be called before onHide, and should be used to return if this form can be hidden or not.
Before the form is really going to hide, this form and all the forms that this form is also showing in its ui hierarchy must allow the hide (return true in onBeforeHide - if present).
For example, when using onBeforeHide with showFormInDialog, the form will not close by clicking the dialog close box (X) if the main form in the dialog or any
of the other visible forms in tabpanels/containers are nested in the main are returning false.

If the hide operation is allowed for all the forms that are in the affected visible hierarchy, then the onHide handler/method will get called on them as well afterwards.

So this handler (on each form) can be used to validate input in the main form and/or any nested visible forms - that are getting ready to hide.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onShow = form.newMethod('function onShow(firstShow, event) { application.output("onShow intercepted on " + event.getFormName() + ". first show? " + firstShow); return false; }');
form.onHide = form.newMethod('function onHide(event) { application.output("Hide called but this should not block, use onbefore hdie for that" + event.getFormName());}');
form.onBeforeHide = form.newMethod('function onHide(event) { application.output("onBeforeHide blocked on " + event.getFormName()); return false; }');
```
### onDeleteAllRecordsCmd

The method that overrides the Servoy menu item Select > Delete All.
This property is automatically set to "DEFAULT" (no override) when the form is created.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onNewRecordCmd = form.newMethod('function onNewRecordCmd(event) { application.output("onNewRecordCmd intercepted on " + event.getFormName()); }');
form.onDuplicateRecordCmd = form.newMethod('function onDuplicateRecordCmd(event) { application.output("onDuplicateRecordCmd intercepted on " + event.getFormName()); }');
form.onDeleteRecordCmd = form.newMethod('function onDeleteRecordCmd(event) { application.output("onDeleteRecordCmd intercepted on " + event.getFormName()); }');
form.onDeleteAllRecordsCmd = form.newMethod('function onDeleteAllRecordsCmd(event) { application.output("onDeleteAllRecordsCmd intercepted on " + event.getFormName()); }');
```
### onDeleteRecordCmd

The method that overrides the Servoy menu item Select > Delete Record (or keyboard shortcut).
This property is automatically set to "DEFAULT" (no override) when the form is created.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onNewRecordCmd = form.newMethod('function onNewRecordCmd(event) { application.output("onNewRecordCmd intercepted on " + event.getFormName()); }');
form.onDuplicateRecordCmd = form.newMethod('function onDuplicateRecordCmd(event) { application.output("onDuplicateRecordCmd intercepted on " + event.getFormName()); }');
form.onDeleteRecordCmd = form.newMethod('function onDeleteRecordCmd(event) { application.output("onDeleteRecordCmd intercepted on " + event.getFormName()); }');
form.onDeleteAllRecordsCmd = form.newMethod('function onDeleteAllRecordsCmd(event) { application.output("onDeleteAllRecordsCmd intercepted on " + event.getFormName()); }');
```
### onDuplicateRecordCmd

The method that overrides the Servoy menu item Select > Duplicate Record (or keyboard shortcut).
This property is automatically set to "DEFAULT" (no override) when the form is created.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onNewRecordCmd = form.newMethod('function onNewRecordCmd(event) { application.output("onNewRecordCmd intercepted on " + event.getFormName()); }');
form.onDuplicateRecordCmd = form.newMethod('function onDuplicateRecordCmd(event) { application.output("onDuplicateRecordCmd intercepted on " + event.getFormName()); }');
form.onDeleteRecordCmd = form.newMethod('function onDeleteRecordCmd(event) { application.output("onDeleteRecordCmd intercepted on " + event.getFormName()); }');
form.onDeleteAllRecordsCmd = form.newMethod('function onDeleteAllRecordsCmd(event) { application.output("onDeleteAllRecordsCmd intercepted on " + event.getFormName()); }');
```
### onElementDataChange

Method that is executed when the data in one of the form's component is successfully changed and
the onDataChange callback from the component does not exist or exists and returned true

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onElementDataChange = form.newMethod('function onElementDataChange(oldValue, newValue, event) { application.output("Data changed from " + oldValue + " to " + newValue + " at " + event.getTimestamp()); }');
```
### onElementFocusGained

The method that is triggered when focus is gained by a component inside the form.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onElementFocusGained = form.newMethod('function onElementFocusGained(event) { application.output("onElementFocusGained intercepted from " + event.getSource()); }');
form.onElementFocusLost = form.newMethod('function onElementFocusLost(event) { application.output("onElementFocusLost intercepted from " + event.getSource()); }');
```
### onElementFocusLost

The method that gets triggered when focus is lost by a component inside the form.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onElementFocusGained = form.newMethod('function onElementFocusGained(event) { application.output("onElementFocusGained intercepted from " + event.getSource()); }');
form.onElementFocusLost = form.newMethod('function onElementFocusLost(event) { application.output("onElementFocusLost intercepted from " + event.getSource()); }');
```
### onFindCmd

The method that overrides the Servoy menu item Select > Find (or keyboard shortcut) in Data (ready) mode.
This property is automatically set to "DEFAULT" (no override) when the form is created.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onFindCmd = form.newMethod('function onFindCmd(event) { application.output("onFindCmd intercepted on " + event.getFormName()); }');
form.onSearchCmd = form.newMethod('function onSearchCmd(event) { application.output("onSearchCmd intercepted on " + event.getFormName()); }');
form.onShowAllRecordsCmd = form.newMethod('function onShowAllRecordsCmd(event) { application.output("onShowAllRecordsCmd intercepted on " + event.getFormName()); }');
```
### onHide

This method is triggered when the form gets hidden.

Return value is DEPRECATED: false return value should no longer be used. In the past, if the onHide method returned false, the form hide could be prevented from happening
in some cases (for example, when using onHide with showFormInDialog, the form will not close by clicking the dialog close box (X)). But that lead to
unexpected situations when the form being hidden had visible nested children it it (tab panels, splits etc.) because only the current form would
decide if hide could be denied, and all other forms, even if they returned false in their on-hide, would not be able to block the hide if this form allowed it.
So those nested forms might think that they are still visible even though they are not.

Please use the new onBeforeHide method/handler instead if you want to prevent forms from hiding.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onShow = form.newMethod('function onShow(firstShow, event) { application.output("onShow intercepted on " + event.getFormName() + ". first show? " + firstShow); return false; }');
form.onHide = form.newMethod('function onHide(event) { application.output("Hide called but this should not block, use onbefore hdie for that" + event.getFormName());}');
form.onBeforeHide = form.newMethod('function onHide(event) { application.output("onBeforeHide blocked on " + event.getFormName()); return false; }');
```
### onInvertRecordsCmd

The method that overrides the Servoy menu item Select > Invert Records.
This property is automatically set to "DEFAULT" (no override) when the form is created.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onOmitRecordCmd = form.newMethod('function onOmitRecordCmd(event) { application.output("onOmitRecordCmd intercepted on " + event.getFormName()); }');
form.onShowOmittedRecordsCmd = form.newMethod('function onShowOmittedRecordsCmd(event) { application.output("onShowOmittedRecordsCmd intercepted on " + event.getFormName()); }');
form.onInvertRecordsCmd = form.newMethod('function onInvertRecordsCmd(event) { application.output("onInvertRecordsCmd intercepted on " + event.getFormName()); }');
```
### onLoad

The method that is triggered when a form is loaded/reloaded from the repository; used to alter elements, set globals, hide toolbars,
etc; onShow method can also be assigned.
NOTE: onShow should be used to access current foundset dataproviders; onLoad cannot be used because the foundset data is not loaded until after the form is loaded.
Also calls to loadRecords() should be done in the onShow method and not in the onLoad method
If you call loadRecords() in the onShow method, you may want to set the namedFoundSet property of the form to 'empty' to prevent the first default form query.
NOTE: the onLoad event bubbles down, meaning that the onLoad is first fired on the parent then on a tab in a tabpanel (and in tab of that tab panels if you are 3 deep)

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onLoad = form.newMethod('function onLoad(event) { application.output("onLoad intercepted on " + event.getFormName()); }');
form.onUnLoad = form.newMethod('function onUnLoad(event) { application.output("onUnLoad intercepted on " + event.getFormName()); }');
```
### onNewRecordCmd

The method that overrides the Servoy menu item Select > New Record (or keyboard shortcut).
This property is automatically set to "DEFAULT" (no override) when the form is created.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onNewRecordCmd = form.newMethod('function onNewRecordCmd(event) { application.output("onNewRecordCmd intercepted on " + event.getFormName()); }');
form.onDuplicateRecordCmd = form.newMethod('function onDuplicateRecordCmd(event) { application.output("onDuplicateRecordCmd intercepted on " + event.getFormName()); }');
form.onDeleteRecordCmd = form.newMethod('function onDeleteRecordCmd(event) { application.output("onDeleteRecordCmd intercepted on " + event.getFormName()); }');
form.onDeleteAllRecordsCmd = form.newMethod('function onDeleteAllRecordsCmd(event) { application.output("onDeleteAllRecordsCmd intercepted on " + event.getFormName()); }');
```
### onNextRecordCmd

The method that overrides the Servoy menu item Select > Next Record.
This property is automatically set to "DEFAULT" (no override) when the form is created.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onPreviousRecordCmd = form.newMethod('function onPreviousRecordCmd(event) { application.output("onPreviousRecordCmd intercepted on " + event.getFormName()); }');
form.onNextRecordCmd = form.newMethod('function onNextRecordCmd(event) { application.output("onNextRecordCmd intercepted on " + event.getFormName()); }');
```
### onOmitRecordCmd

The method that overrides the Servoy menu item Select > Omit Record.
This property is automatically set to "DEFAULT" (no override) when the form is created.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onOmitRecordCmd = form.newMethod('function onOmitRecordCmd(event) { application.output("onOmitRecordCmd intercepted on " + event.getFormName()); }');
form.onShowOmittedRecordsCmd = form.newMethod('function onShowOmittedRecordsCmd(event) { application.output("onShowOmittedRecordsCmd intercepted on " + event.getFormName()); }');
form.onInvertRecordsCmd = form.newMethod('function onInvertRecordsCmd(event) { application.output("onInvertRecordsCmd intercepted on " + event.getFormName()); }');
```
### onPreviousRecordCmd

The method that overrides the Servoy menu item Select > Previous Record.
This property is automatically set to "DEFAULT" (no override) when the form is created.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onPreviousRecordCmd = form.newMethod('function onPreviousRecordCmd(event) { application.output("onPreviousRecordCmd intercepted on " + event.getFormName()); }');
form.onNextRecordCmd = form.newMethod('function onNextRecordCmd(event) { application.output("onNextRecordCmd intercepted on " + event.getFormName()); }');
```
### onRecordEditStart

The method that is triggered when a user clicks into a column on the form.
NOTE: There is a small "e" displayed in the lower left side of the Servoy Client screen in the status area at the bottom of the window when the record is being edited.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onRecordEditStart = form.newMethod('function onRecordEditStart(event) { application.output("onRecordEditStart intercepted on " + event.getFormName()); }');
form.onRecordEditStop = form.newMethod('function onRecordEditStop(record, event) { application.output("onRecordEditStop intercepted on " + event.getFormName() + ". record is: " + record); }');
form.onRecordSelection = form.newMethod('function onRecordSelection(event) { application.output("onRecordSelection intercepted on " + event.getFormName()); }');
```
### onRecordEditStop

The method that is triggered when a record is being saved.
A record is saved when a user clicks out of it (for example on an empty part of the layout or to another form).
When the method returns false (for example as part of a validation), the user cannot leave the record, for example in
a table view a user cannot move to another record when the callback returns false.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onRecordEditStart = form.newMethod('function onRecordEditStart(event) { application.output("onRecordEditStart intercepted on " + event.getFormName()); }');
form.onRecordEditStop = form.newMethod('function onRecordEditStop(record, event) { application.output("onRecordEditStop intercepted on " + event.getFormName() + ". record is: " + record); }');
form.onRecordSelection = form.newMethod('function onRecordSelection(event) { application.output("onRecordSelection intercepted on " + event.getFormName()); }');
```
### onRecordSelection

The method that is triggered each time a record is selected.
If a form is in List view or Special table view - when the user clicks on it.
In Record view - after the user navigates to another record using the slider or clicks up or down for next/previous record.
NOTE: Data and Servoy tag values are returned when the onRecordSelection method is executed.
NOTE: this will also fire if the selection goes to -1 because the foundset is cleared. So foundset.getSelectedRecord() can return null.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onRecordEditStart = form.newMethod('function onRecordEditStart(event) { application.output("onRecordEditStart intercepted on " + event.getFormName()); }');
form.onRecordEditStop = form.newMethod('function onRecordEditStop(record, event) { application.output("onRecordEditStop intercepted on " + event.getFormName() + ". record is: " + record); }');
form.onRecordSelection = form.newMethod('function onRecordSelection(event) { application.output("onRecordSelection intercepted on " + event.getFormName()); }');
```
### onResize

The method that gets triggered when resize occurs.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onResize = form.newMethod('function onResize(event) { application.output("onResize intercepted on " + event.getFormName()); }');
```
### onSearchCmd

The method that overrides the Servoy menu item Select > Search (or keyboard shortcut) in Find mode.
This property is automatically set to "DEFAULT" (no override) when the form is created.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onFindCmd = form.newMethod('function onFindCmd(event) { application.output("onFindCmd intercepted on " + event.getFormName()); }');
form.onSearchCmd = form.newMethod('function onSearchCmd(event) { application.output("onSearchCmd intercepted on " + event.getFormName()); }');
form.onShowAllRecordsCmd = form.newMethod('function onShowAllRecordsCmd(event) { application.output("onShowAllRecordsCmd intercepted on " + event.getFormName()); }');
```
### onShow

The method that is triggered EVERY TIME the form is displayed; an argument must be passed to the method if this is the first time the form is displayed.

NOTE: onShow can be used to access current foundset dataproviders; onLoad cannot be used because the foundset data is not loaded until after the form is loaded.

NOTE: the onShow event bubbles down, meaning that the onShow event of a form displayed in a tabPanel is fired after the onShow event of the parent.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onShow = form.newMethod('function onShow(firstShow, event) { application.output("onShow intercepted on " + event.getFormName() + ". first show? " + firstShow); return false; }');
form.onHide = form.newMethod('function onHide(event) { application.output("Hide called but this should not block, use onbefore hdie for that" + event.getFormName());}');
form.onBeforeHide = form.newMethod('function onHide(event) { application.output("onBeforeHide blocked on " + event.getFormName()); return false; }');
```
### onShowAllRecordsCmd

The method that overrides the Servoy menu item Select > Show All (or keyboard shortcut).
This property is automatically set to "DEFAULT" (no override) when the form is created.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onFindCmd = form.newMethod('function onFindCmd(event) { application.output("onFindCmd intercepted on " + event.getFormName()); }');
form.onSearchCmd = form.newMethod('function onSearchCmd(event) { application.output("onSearchCmd intercepted on " + event.getFormName()); }');
form.onShowAllRecordsCmd = form.newMethod('function onShowAllRecordsCmd(event) { application.output("onShowAllRecordsCmd intercepted on " + event.getFormName()); }');
```
### onShowOmittedRecordsCmd

The method that overrides the Servoy menu item Select > Show Omitted Records.
This property is automatically set to "DEFAULT" (no override) when the form is created.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onOmitRecordCmd = form.newMethod('function onOmitRecordCmd(event) { application.output("onOmitRecordCmd intercepted on " + event.getFormName()); }');
form.onShowOmittedRecordsCmd = form.newMethod('function onShowOmittedRecordsCmd(event) { application.output("onShowOmittedRecordsCmd intercepted on " + event.getFormName()); }');
form.onInvertRecordsCmd = form.newMethod('function onInvertRecordsCmd(event) { application.output("onInvertRecordsCmd intercepted on " + event.getFormName()); }');
```
### onSortCmd

The method that overrides the Servoy menu item Select > Sort.
This property is automatically set to "DEFAULT" (no override) when the form is created.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onSortCmd = form.newMethod('function onSortCmd(dataProviderID, asc, event) { application.output("onSortCmd intercepted on " + event.getFormName() + ". data provider: " + dataProviderID + ". asc: " + asc); }');
```
### onUnLoad

The method that is triggered when a form is unloaded from the repository.
NOTE: Forms can be prevented from being removed from memory by referencing the form object in a global variable or inside an array inside a global variable. Do take care using this technique.
Forms take up memory and if too many forms are in memory and cannot be unloaded, there is a possibility of running out of memory.

**Returns**\
[JSMethod](./JSMethod.md) 


**Sample**

```javascript
form.onLoad = form.newMethod('function onLoad(event) { application.output("onLoad intercepted on " + event.getFormName()); }');
form.onUnLoad = form.newMethod('function onUnLoad(event) { application.output("onUnLoad intercepted on " + event.getFormName()); }');
```
### responsiveLayout

Returns true if this form is in responsive mode

**Returns**\
[Boolean](../JSLib/Boolean.md) 


**Sample**

```javascript
var myForm = solutionModel.getForm('myform');
if (myForm.isResponsive()) {}
```
### scrollbars

Scrollbar options for the vertical and horizontal scrollbars. Each of the
vertical and horizontal scrollbars can be configured to display all the time,
to display only when needed or to never display.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var form = solutionModel.newForm('myForm',myDatasource,null,true,1000,600);
form.scrollbars = SM_SCROLLBAR.VERTICAL_SCROLLBAR_NEVER;
forms['newForm1'].controller.show();
```
### selectionMode

Returns the value of the form's selectionMode property.
Selection mode is applied when necessary to the foundset used by the form (through it's multiSelect property), even if the foundset changes.
If two or more forms with non-default and different selectionMode values share the same foundset, the visible one decides.
If two or more non-visible forms with non-default and different selectionMode values share the same foundset, one of them (always the same from a set of forms) decides.
If two or more visible forms with non-default and different selectionMode values share the same foundset, one of them (always the same from a set of forms) decides what the
foundset's selectionMode should be.

Can be one of SELECTION_MODE_DEFAULT, SELECTION_MODE_SINGLE or SELECTION_MODE_MULTI.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var myForm = solutionModel.getForm('my_form_name');
if (myForm.selectionMode == JSForm.SELECTION_MODE_MULTI) myForm.selectionMode = JSForm.SELECTION_MODE_DEFAULT;
```
### serverName

Get the server name used by this form.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var form = solutionModel.newForm('myForm',myDatasource,null,true,800,600);
form.serverName = 'anotherServerName';
var theServerName = form.serverName;
application.output(theServerName);
```
### showInMenu

When set, the form is displayed under the Window menu.
If it is not set, the form will be 'hidden'.
NOTE: This is only applicable for Servoy Client. Servoy Developer always shows all forms so that
developers have access to all forms within a solution during development.

**Returns**\
[Boolean](../JSLib/Boolean.md) 


**Sample**

```javascript
var aForm = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
var anotherForm= solutionModel.newForm('newForm2', myDatasource, null, true, 800, 600);
//using 'anotherForm' as navigator for aForm
anotherForm.showInMenu = false;
anotherForm.navigator = null;
aForm.navigator = anotherForm;
application.output(aForm.navigator.name);
```
### styleClass

The Cascading Style Sheet (CSS) class name applied to the form.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var aForm = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
if (aForm.styleClass == null)
	aForm.styleClass = someStyleClass;
else
	application.output("The Cascading Style Sheet (CSS) class name applied to this form is " + aForm.styleClass);
```
### tableName

The [name of the table/SQL view].[the name of the database server connection] the form is based on.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var aForm = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
aForm.tableName = 'anotherTableOfMine'
if (forms['newForm1'].controller.find())
{
	columnTextDataProvider = '=aSearchedValue'
	columnNumberDataProvider = '>10';
	forms['newForm1'].controller.search()
}
```
### titleText

The text that displays in the title bar of the form window.
NOTE: Data tags and Servoy tags can be used as part of the title text.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var myForm = solutionModel.newForm('newForm', 'db:/a_server/a_table', 'aStyleName', false, 800, 600)
forms['newForm'].controller.show();
if (myForm.titleText == null)
{
	myForm.titleText = "My new title text should be really cool!"
	forms['newForm'].controller.recreateUI();
}
else
	application.output("My text text is already cool");
```
### transparent

When set, the form is transparent.

**Returns**\
[Boolean](../JSLib/Boolean.md) 


**Sample**

```javascript
var form = solutionModel.newForm('myForm',myDatasource,null,true,1000,800);
if (form.transparent == false)
{
	var style = solutionModel.newStyle('myStyle','form { background-color: yellow; }');
	style.text = style.text + 'field { background-color: blue; }';
	form.styleName = 'myStyle';
}
var field = form.newField('columnTextDataProvider',JSField.TEXT_FIELD,100,100,100,50);
forms['myForm'].controller.show();
```
### useCssPosition

Get or set the positioning (either use anchoring or use css position) for the form.
This is only working for absolute layout forms in NGClient.

**Returns**\
[Boolean](../JSLib/Boolean.md) 


**Sample**

```javascript
var myForm = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
myForm.useCssPosition = true;
```
### view

The default form view mode.

The view can be changed using a method at runtime. The following views are available:
- Record view
- List view
- Record view (locked)
- List view (locked)
- Table View (locked)

NOTE: Only Table View (locked) uses asynchronized related data loading.
This feature defers all related foundset data loading to the background - enhancing
the visual display of a related foundset.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var myForm = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
myForm.view = JSForm.RECORD_VIEW;
forms['newForm1'].controller.show();
```
### width

The width of the form in pixels.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var myForm = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
forms['newForm1'].controller.show();
myForm.width = 120;
forms['newForm1'].controller.recreateUI();
```

## Methods Details

### findLayoutContainer(name)

Returns a JSLayoutContainer that has the given name throughout the whole form hierarchy.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the container

**Returns**\
[JSLayoutContainer](./JSLayoutContainer.md) a JSLayoutContainer object


**Sample**

```javascript
var container = myForm.findLayoutContainer("row1");
application.output(container.name);
```
### findWebComponent(name)

Returns a JSWebComponent that has the given name through the whole hierarchy of JSLayoutContainers

**Parameters**\
[String](../JSLib/String.md) name the specified name of the web component

**Returns**\
[JSComponent](./JSComponent.md) a JSWebComponent object


**Sample**

```javascript
var btn = myForm.findWebComponent("mycomponent");
application.output(mybean.typeName);
```
### getBean(name)

Returns a JSBean that has the given name.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the bean

**Returns**\
[JSComponent](./JSComponent.md) a JSBean object


**Sample**

```javascript
var btn = myForm.getBean("mybean");
application.output(mybean.className);
```
### getBeans()

Returns all JSBeans of this form.


**Returns**\
[Array](../JSLib/Array.md) the list of all JSBeans on this forms


**Sample**

```javascript
var beans = myForm.getBeans();
for (var b in beans)
{
	if (beans[b].name != null)
		application.output(beans[b].name);
}
```
### getBeans(returnInheritedElements)

Returns all JSBeans of this form.

**Parameters**\
[Boolean](../JSLib/Boolean.md) returnInheritedElements true to also return the elements from parent form

**Returns**\
[Array](../JSLib/Array.md) the list of all JSBeans on this forms


**Sample**

```javascript
var beans = myForm.getBeans();
for (var b in beans)
{
	if (beans[b].name != null)
		application.output(beans[b].name);
}
```
### getBodyPart()

Retrieves the Body part of the form.


**Returns**\
[JSPart](./JSPart.md) A JSPart instance corresponding to the Body part of the form.


**Sample**

```javascript
form.getBodyPart().background = 'blue';
```
### getButton(name)

Returns a JSButton that has the given name.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the button

**Returns**\
[JSComponent](./JSComponent.md) a JSButton object


**Sample**

```javascript
var btn = myForm.getButton("hello");
application.output(btn.text);
```
### getButtons()

Returns all JSButtons of this form, including the ones without a name.


**Returns**\
[Array](../JSLib/Array.md) the list of all JSButtons on this forms


**Sample**

```javascript
var buttons = myForm.getButtons();
for (var b in buttons)
{
	if (buttons[b].name != null)
		application.output(buttons[b].name);
	else
		application.output(buttons[b].text + " has no name ");
}
```
### getButtons(returnInheritedElements)

Returns all JSButtons of this form, including the ones without a name.

**Parameters**\
[Boolean](../JSLib/Boolean.md) returnInheritedElements true to also return the elements from parent form

**Returns**\
[Array](../JSLib/Array.md) the list of all JSButtons on this forms


**Sample**

```javascript
var buttons = myForm.getButtons();
for (var b in buttons)
{
	if (buttons[b].name != null)
		application.output(buttons[b].name);
	else
		application.output(buttons[b].text + " has no name ");
}
```
### getComment()

Returns the comment of this container.


**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var comment = solutionModel.getForm("my_form").getComment();
application.output(comment);
```
### getComponent(name)

Returns a JSComponent that has the given name; if found it will be a JSField, JSLabel, JSButton, JSPortal, JSBean, JSWebComponent or JSTabPanel.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the component

**Returns**\
[JSComponent](./JSComponent.md) a JSComponent object (might be a JSField, JSLabel, JSButton, JSPortal, JSBean, JSWebComponent or JSTabPanel)


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var cmp = frm.getComponent("componentName");
application.output("Component type and name: " + cmp);
```
### getComponents()

Returns a array of all the JSComponents that a form has; they are of type JSField,JSLabel,JSButton,JSPortal,JSBean, JSWebComponents or JSTabPanel.


**Returns**\
[Array](../JSLib/Array.md) an array of all the JSComponents on the form.


**Sample**

```javascript
var form = solutionModel.getForm("myForm");
var components = form.getComponents();
for (var i in components)
	application.output("Component type and name: " + components[i]);
```
### getComponents(returnInheritedElements)

Returns a array of all the JSComponents that a form has; they are of type JSField,JSLabel,JSButton,JSPortal,JSBean, JSWebComponent or JSTabPanel.

**Parameters**\
[Boolean](../JSLib/Boolean.md) returnInheritedElements true to also return the elements from the parent form

**Returns**\
[Array](../JSLib/Array.md) an array of all the JSComponents on the form.


**Sample**

```javascript
var form = solutionModel.getForm("myForm");
var components = form.getComponents();
for (var i in components)
	application.output("Component type and name: " + components[i]);
```
### getDesignTimeProperty(key)

Get a design-time property of a form.

**Parameters**\
[String](../JSLib/String.md) key the property name

**Returns**\
[Object](../JSLib/Object.md) 


**Sample**

```javascript
var frm = solutionModel.getForm('orders')
var prop = frm.getDesignTimeProperty('myprop')
```
### getDesignTimePropertyNames()

Get the design-time properties of a form.


**Returns**\
[Array](../JSLib/Array.md) 


**Sample**

```javascript
var frm = solutionModel.getForm('orders')
var propNames = frm.getDesignTimePropertyNames()
```
### getField(name)

The field with the specified name.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the field

**Returns**\
[JSField](./JSField.md) a JSField object


**Sample**

```javascript
var form = solutionModel.getForm("myForm");
var field = form.getField("myField");
application.output(field.dataProviderID);
```
### getFields()

Returns all JSField objects of this form, including the ones without a name.


**Returns**\
[Array](../JSLib/Array.md) all JSField objects of this form


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var fields = frm.getFields();
for (var f in fields)
{
	var fname = fields[f].name;
	if (fname != null)
		application.output(fname);
}
```
### getFields(returnInheritedElements)

Returns all JSField objects of this form, including the ones without a name.

**Parameters**\
[Boolean](../JSLib/Boolean.md) returnInheritedElements true to also return the elements from the parent form

**Returns**\
[Array](../JSLib/Array.md) all JSField objects of this form


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var fields = frm.getFields();
for (var f in fields)
{
	var fname = fields[f].name;
	if (fname != null)
		application.output(fname);
}
```
### getFooterPart()

Retrieves the Footer part of the form.


**Returns**\
[JSPart](./JSPart.md) A JSPart instance corresponding to the Footer part of the form.


**Sample**

```javascript
form.getFooterPart().background = 'magenta';
```
### getHeaderPart()

Retrieves the Header part of the form.


**Returns**\
[JSPart](./JSPart.md) A JSPart instance corresponding to the Header part of the form.


**Sample**

```javascript
form.getHeaderPart().background = 'orange';
```
### getLabel(name)

Returns a JSLabel that has the given name.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the label

**Returns**\
[JSComponent](./JSComponent.md) a JSLabel object (or null if the label with the specified name does not exist)


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var label = frm.getLabel("myLabel");
application.output(label.text);
```
### getLabels()

Returns all JSLabels of this form (not including its super form), including the ones without a name.


**Returns**\
[Array](../JSLib/Array.md) all JSLabels on this form


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var labels = frm.getLabels();
for (var i in labels)
{
	var lname = labels[i].name;
	if (lname != null)
		application.output(lname);
}
```
### getLabels(returnInheritedElements)

Returns all JSLabels of this form (optionally including it super forms labels), including the ones without a name.

**Parameters**\
[Boolean](../JSLib/Boolean.md) returnInheritedElements true to also return the elements from parent form

**Returns**\
[Array](../JSLib/Array.md) all JSLabels on this form


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var labels = frm.getLabels();
for (var i in labels)
{
	var lname = labels[i].name;
	if (lname != null)
		application.output(lname);
}
```
### getLayoutContainer(name)

Returns a JSLayoutContainer that has the given name of this container.
Use findLayoutContainer() method to find a JSLayoutContainter through the hierarchy

**Parameters**\
[String](../JSLib/String.md) name the specified name of the container

**Returns**\
[JSLayoutContainer](./JSLayoutContainer.md) a JSLayoutContainer object


**Sample**

```javascript
var container = myForm.getLayoutContainer("row1");
application.output(container.name);
```
### getLayoutContainers()

Returns all JSLayoutContainers objects of this container.
Does not return the inherited containers, use #getLayoutContainers(true) to get the inherited as well.


**Returns**\
[Array](../JSLib/Array.md) all JSLayoutContainers objects of this container


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var containers = frm.getLayoutContainers();
for (var c in containers)
{
		var fname = containers[c].name;
		application.output(fname);
}
```
### getLayoutContainers(returnInheritedElements)

Returns all JSLayoutContainers objects of this container

**Parameters**\
[Boolean](../JSLib/Boolean.md) returnInheritedElements true to also return the elements from parent form

**Returns**\
[Array](../JSLib/Array.md) all JSLayoutContainers objects of this container


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var containers = frm.getLayoutContainers();
for (var c in containers)
{
		var fname = containers[c].name;
		application.output(fname);
}
```
### getLeadingGrandSummaryPart()

Retrieves the Leading Grand Summary part of the form.


**Returns**\
[JSPart](./JSPart.md) A JSPart instance corresponding to the Leading Grand Summary part of the form.


**Sample**

```javascript
form.getLeadingGrandSummaryPart().background = 'yellow';
```
### getLeadingSubSummaryParts()

Gets an array of the Leading Subsummary parts of the form, ordered by their height from top == 0 to bottom.


**Returns**\
[Array](../JSLib/Array.md) An array of JSPart instances corresponding to the Leading Subsummary parts of the form.


**Sample**

```javascript
form.getLeadingSubSummaryParts()[0].background = 'green';
```
### getMethod(name)

Gets an existing form method for the given name.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the method

**Returns**\
[JSMethod](./JSMethod.md) a JSMethod object (or null if the method with the specified name does not exist)


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var method = frm.getMethod("myMethod");
application.output(method.code);
```
### getMethods()

Returns all existing form methods for this form.


**Returns**\
[Array](../JSLib/Array.md) all form methods for the form


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var methods = frm.getMethods();
for (var m in methods)
	application.output(methods[m].getName());
```
### getMethods(returnInheritedElements)

Returns all existing form methods for this form.

**Parameters**\
[Boolean](../JSLib/Boolean.md) returnInheritedElements true to also return the elements from the parent form

**Returns**\
[Array](../JSLib/Array.md) all form methods for the form


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var methods = frm.getMethods();
for (var m in methods)
	application.output(methods[m].getName());
```
### getPart(type)

Gets a part of the form from the given type (see JSPart constants).

**Parameters**\
[Number](../JSLib/Number.md) type The type of the part to retrieve.

**Returns**\
[JSPart](./JSPart.md) A JSPart instance representing the retrieved form part.


**Sample**

```javascript
form.getPart(JSPart.HEADER).background = 'red';
form.getPart(JSPart.LEADING_SUBSUMMARY, 160).background = 'red';
```
### getPart(type, height)

Gets a part of the form from the given type (see JSPart constants).
Use the height if you want to get a specific LEADING_SUBSUMMARY or TRAILING_SUBSUMMARY.

**Parameters**\
[Number](../JSLib/Number.md) type The type of the part to retrieve.\
[Number](../JSLib/Number.md) height The height of the part to retrieve. Use this parameter when retrieving one of multiple
	                      Leading/Trailing Subsummary parts.

**Returns**\
[JSPart](./JSPart.md) A JSPart instance representing the retrieved form part.


**Sample**

```javascript
form.getPart(JSPart.HEADER).background = 'red';
form.getPart(JSPart.LEADING_SUBSUMMARY, 160).background = 'red';
```
### getPartYOffset(type)

Returns the Y offset of a given part (see JSPart) of the form. This will include
all the super forms parts if this form extends a form.

**Parameters**\
[Number](../JSLib/Number.md) type The type of the part whose Y offset will be returned.

**Returns**\
[Number](../JSLib/Number.md) A number holding the Y offset of the specified form part.


**Sample**

```javascript
// get the subform
var form = solutionModel.getForm('SubForm');
// get the start offset of the body
var height = form.getPartYOffset(JSPart.BODY);
// place a new button based on the start offset.
form.newButton('mybutton',50,50+height,80,20,solutionModel.getGlobalMethod('globals', 'test'));
```
### getPartYOffset(type, height)

Returns the Y offset of a given part (see JSPart) of the form. This will include
all the super forms parts if this form extends a form. Use the height parameter for
targetting one of multiple subsummary parts.

**Parameters**\
[Number](../JSLib/Number.md) type The type of the part whose Y offset will be returned.\
[Number](../JSLib/Number.md) height The height of the part whose Y offset will be returned. This is used when
                       one of multiple Leading/Trailing Sumsummary parts is retrieved.

**Returns**\
[Number](../JSLib/Number.md) A number holding the Y offset of the specified form part.


**Sample**

```javascript
// get the subform
var form = solutionModel.getForm('SubForm');
// get the start offset of the body
var height = form.getPartYOffset(JSPart.BODY);
// place a new button based on the start offset.
form.newButton('mybutton',50,50+height,80,20,solutionModel.getGlobalMethod('globals', 'test'));
```
### getParts()

Gets all the parts from the form (not including the parts of the parent form), ordered by there height (lowerbound) property, from top == 0 to bottom.


**Returns**\
[Array](../JSLib/Array.md) An array of JSPart instances corresponding to the parts of the form.


**Sample**

```javascript
var allParts = form.getParts()
for (var i=0; i<allParts.length; i++) {
	if (allParts[i].getPartType() == JSPart.BODY)
		application.output('body Y offset: ' + allParts[i].getPartYOffset());
}
```
### getParts(returnInheritedElements)

Gets all the parts from the form (optionally also from the parent form), ordered by there height (lowerbound) property, from top == 0 to bottom.

**Parameters**\
[Boolean](../JSLib/Boolean.md) returnInheritedElements true to also return the parts from parent form

**Returns**\
[Array](../JSLib/Array.md) An array of JSPart instances corresponding to the parts of the form.


**Sample**

```javascript
var allParts = form.getParts()
for (var i=0; i<allParts.length; i++) {
	if (allParts[i].getPartType() == JSPart.BODY)
		application.output('body Y offset: ' + allParts[i].getPartYOffset());
}
```
### getPortal(name)

Returns a JSPortal that has the given name.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the portal

**Returns**\
[JSComponent](./JSComponent.md) a JSPortal object


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var portal = frm.getPortal("myPortal");
portal.initialSort = 'my_table_text desc';
```
### getPortals()

Returns all JSPortal objects of this form (not including the ones from the parent form), including the ones without a name.


**Returns**\
[Array](../JSLib/Array.md) an array of all JSPortal objects on this form


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var portals = frm.getPortals();
for (var i in portals)
{
	var p = portals[i];
	if (p.name != null)
		application.output(p.name);
	else
		application.output("unnamed portal detected");
}
```
### getPortals(returnInheritedElements)

Returns all JSPortal objects of this form (optionally also the ones from the parent form), including the ones without a name.

**Parameters**\
[Boolean](../JSLib/Boolean.md) returnInheritedElements true to also return the elements from parent form

**Returns**\
[Array](../JSLib/Array.md) an array of all JSPortal objects on this form


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var portals = frm.getPortals();
for (var i in portals)
{
	var p = portals[i];
	if (p.name != null)
		application.output(p.name);
	else
		application.output("unnamed portal detected");
}
```
### getTabPanel(name)

Returns a JSTabPanel that has the given name.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the tabpanel

**Returns**\
[JSComponent](./JSComponent.md) a JSTabPanel object


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var tabPanel = frm.getTabPanel("myTabPanel");
var tabs = tabPanel.getTabs();
for (var i=0; i<tabs.length; i++)
	application.output("Tab " + i + " has text " + tabs[i].text);
```
### getTabPanels()

Returns all JSTabPanels of this form (not including the ones from the parent form), including the ones without a name.


**Returns**\
[Array](../JSLib/Array.md) an array of all JSTabPanel objects on this form


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var tabPanels = frm.getTabPanels();
for (var i in tabPanels)
{
	var tp = tabPanels[i];
	if (tp.name != null)
		application.output("Tab " + tp.name + " has text " + tp.text);
	else
		application.output("Tab with text " + tp.text + " has no name");
}
```
### getTabPanels(returnInheritedElements)

Returns all JSTabPanels of this form (optionally the ones from the parent form), including the ones without a name.

**Parameters**\
[Boolean](../JSLib/Boolean.md) returnInheritedElements true to also return the elements from parent form

**Returns**\
[Array](../JSLib/Array.md) an array of all JSTabPanel objects on this form


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var tabPanels = frm.getTabPanels();
for (var i in tabPanels)
{
	var tp = tabPanels[i];
	if (tp.name != null)
		application.output("Tab " + tp.name + " has text " + tp.text);
	else
		application.output("Tab with text " + tp.text + " has no name");
}
```
### getTitleFooterPart()

Retrieves the Title Footer part of the form.


**Returns**\
[JSPart](./JSPart.md) A JSPart instance corresponding to the Title Footer part of the form.


**Sample**

```javascript
form.getTitleFooterPart().background = 'gray';
```
### getTitleHeaderPart()

Retrieves the Title Header part of the form.


**Returns**\
[JSPart](./JSPart.md) A JSPart instance corresponding to the Title Header part of the form.


**Sample**

```javascript
form.getTitleHeaderPart().background = 'red';
```
### getTrailingGrandSummaryPart()

Retrieves the Trailing Grand Summary part of the form.


**Returns**\
[JSPart](./JSPart.md) A JSPart instance corresponding to the Trailing Grand Summary part of the form.


**Sample**

```javascript
form.getTrailingGrandSummaryPart().background = 'yellow';
```
### getTrailingSubSummaryParts()

Gets an array of the Trailing Subsummary parts of the form, ordered by their height from top == 0 to bottom.


**Returns**\
[Array](../JSLib/Array.md) An array of JSPart instances corresponding to the Trailing Subsummary parts of the form.


**Sample**

```javascript
form.getTrailingSubSummaryParts()[0].background = 'green';
```
### getUUID()

Returns the UUID of this form.


**Returns**\
[UUID](../Application/UUID.md) 


**Sample**

```javascript
var form_UUID = myForm.getUUID();
application.output(form_UUID.toString());
```
### getVariable(name)

Gets an existing form variable for the given name.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the variable

**Returns**\
[JSVariable](./JSVariable.md) a JSVariable object


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
	var fvariable = frm.getVariable("myVarName");
	application.output(fvariable.name + " has the default value of " + fvariable.defaultValue);
```
### getVariables()

An array consisting of all form variables for this form.


**Returns**\
[Array](../JSLib/Array.md) an array of all variables on this form


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var variables = frm.getVariables();
for (var i in variables)
	application.output(variables[i].name);
```
### getVariables(returnInheritedElements)

An array consisting of all form variables for this form.

**Parameters**\
[Boolean](../JSLib/Boolean.md) returnInheritedElements true to also return the elements from the parent form

**Returns**\
[Array](../JSLib/Array.md) an array of all variables on this form


**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var variables = frm.getVariables();
for (var i in variables)
	application.output(variables[i].name);
```
### getWebComponent(name)

Returns a JSWebComponent that has the given name that is a child of this layout container.
Use findWebComponent() to find a webcomponent through the hierarchy

**Parameters**\
[String](../JSLib/String.md) name the specified name of the web component

**Returns**\
[JSComponent](./JSComponent.md) a JSWebComponent object


**Sample**

```javascript
var btn = myForm.getWebComponent("mycomponent");
application.output(mybean.typeName);
```
### getWebComponents()

Returns all JSWebComponents of this form/container.
If this method is called on a form, then it will return all web components on that form.
If the form is responsive, it will return the web components from all the containers.
It does not return the inherited components, use #getWebComponents(true) to get the inherited as well.


**Returns**\
[Array](../JSLib/Array.md) the list of all JSWebComponent on this forms


**Sample**

```javascript
var webComponents = myForm.getWebComponents();
for (var i in webComponents)
{
	if (webComponents[i].name != null)
		application.output(webComponents[i].name);
}
```
### getWebComponents(returnInheritedElements)

Returns all JSWebComponents of this form/container.
If this method is called on a form, then it will return all web components on that form.
If the form is responsive, it will return the web components from all the containers.

**Parameters**\
[Boolean](../JSLib/Boolean.md) returnInheritedElements true to also return the elements from parent form

**Returns**\
[Array](../JSLib/Array.md) the list of all JSWebComponents on this forms


**Sample**

```javascript
var webComponents = myForm.getWebComponents(false);
for (var i in webComponents)
{
	if (webComponents[i].name != null)
		application.output(webComponents[i].name);
}
```
### newBean(name, className, x, y, width, height)

Creates a new JSBean object on the form - including the name of the JSBean object; the classname the JSBean object is based on, the "x" and "y" position of the JSBean object in pixels, as well as the width and height of the JSBean object in pixels.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the JSBean object\
[String](../JSLib/String.md) className the class name of the JSBean object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSBean object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSBean object in pixels\
[Number](../JSLib/Number.md) width the width of the JSBean object in pixels\
[Number](../JSLib/Number.md) height the height of the JSBean object in pixels

**Returns**\
[JSComponent](./JSComponent.md) a JSBean object


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', 'db:/server1/table1', null, true, 800, 600);
var bean = form.newBean('bean','com.servoy.extensions.beans.dbtreeview.DBTreeView',200,200,300,300);
forms['newForm1'].controller.show();
```
### newButton(txt, x, y, width, height, action)

Creates a new button on the form with the given text, place, size and JSMethod as the onAction event triggered action.

**Parameters**\
[String](../JSLib/String.md) txt the text on the button\
[Number](../JSLib/Number.md) x the x coordinate of the button location on the form\
[Number](../JSLib/Number.md) y the y coordinate of the button location on the form\
[Number](../JSLib/Number.md) width the width of the button\
[Number](../JSLib/Number.md) height the height of the button\
[Object](../JSLib/Object.md) action the method assigned to handle an onAction event

**Returns**\
[JSComponent](./JSComponent.md) a new JSButton object


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
var method = form.newMethod('function onAction(event) { application.output("onAction intercepted on " + event.getFormName()); }');
var button = form.newButton('myButton', 10, 10, 100, 30, method);
application.output("The new button: " + button.name + " has the following onAction event handling method assigned " + button.onAction.getName());
```
### newButton(txt, action)

Creates a new button on the form with the given text and JSMethod as the onAction event triggered action. You must set location/dimension or css position afterwards

**Parameters**\
[String](../JSLib/String.md) txt the text on the button\
[Object](../JSLib/Object.md) action the method assigned to handle an onAction event

**Returns**\
[JSComponent](./JSComponent.md) a new JSButton object


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
form.useCssPosition = true
var method = form.newMethod('function onAction(event) { application.output("onAction intercepted on " + event.getFormName()); }');
var button = form.newButton('myButton', method);
button.cssPosition.l("10%").t("10%").w("80px").h("30px")
application.output("The new button: " + button.name + " has the following onAction event handling method assigned " + button.onAction.getName());
```
### newCalendar(dataprovider)

Creates a new JSField object on the form with the displayType of CALENDAR - including the dataprovider/JSVariable of the JSField object. You must set location/dimension or css position afterwards

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object

**Returns**\
[JSField](./JSField.md) a new JSField object on the form with the displayType of CALENDAR


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
form.useCssPosition = true
var calendar = form.newCalendar(myDataProvider);
calendar.cssPosition.l("10").t("10").w("20%").h("30px")
forms['newForm1'].controller.show();
```
### newCalendar(dataprovider, x, y, width, height)

Creates a new JSField object on the form with the displayType of CALENDAR - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels.

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSfield object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSField object in pixels\
[Number](../JSLib/Number.md) width the width of the JSField object in pixels\
[Number](../JSLib/Number.md) height the height of the JSField object in pixels

**Returns**\
[JSField](./JSField.md) a new JSField object on the form with the displayType of CALENDAR


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
var calendar = form.newCalendar(myDataProvider, 100, 100, 200, 200);
forms['newForm1'].controller.show();
```
### newCheck(dataprovider)

Creates a new JSField object on the form with the displayType of CHECK (checkbox) - including the dataprovider/JSVariable of the JSField object. You must set location/dimension or css position afterwards

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object

**Returns**\
[JSField](./JSField.md) a new JSField object on the form with the displayType of CHECK (checkbox)


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
form.useCssPosition = true
var check = form.newCheck(myDataProvider);
check.cssPosition.l("10").t("10").w("20%").h("30px")
forms['newForm1'].controller.show();
```
### newCheck(dataprovider, x, y, width, height)

Creates a new JSField object on the form with the displayType of CHECK (checkbox) - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels.

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSfield object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSField object in pixels\
[Number](../JSLib/Number.md) width the width of the JSField object in pixels\
[Number](../JSLib/Number.md) height the height of the JSField object in pixels

**Returns**\
[JSField](./JSField.md) a new JSField object on the form with the displayType of CHECK (checkbox)


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
var calendar = form.newCheck(myDataProvider, 100, 100, 200, 200);
forms['newForm1'].controller.show();
```
### newComboBox(dataprovider)

Creates a new JSField object on the form with the displayType of COMBOBOX - including the dataprovider/JSVariable of the JSField object. You must set location/dimension or css position afterwards

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object

**Returns**\
[JSField](./JSField.md) a new JSField object on the form with the displayType of COMBOBOX


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
form.useCssPosition = true
var combo = form.newComboBox(myDataProvider);
combo.cssPosition.l("10").t("10").w("20%").h("30px")
forms['newForm1'].controller.show();
```
### newComboBox(dataprovider, x, y, width, height)

Creates a new JSField object on the form with the displayType of COMBOBOX - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels.

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSfield object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSField object in pixels\
[Number](../JSLib/Number.md) width the width of the JSField object in pixels\
[Number](../JSLib/Number.md) height the height of the JSField object in pixels

**Returns**\
[JSField](./JSField.md) a new JSField object on the form with the displayType of COMBOBOX


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
var calendar = form.newComboBox(myDataProvider, 100, 100, 200, 200);
forms['newForm1'].controller.show();
```
### newField(dataprovider, type)

Creates a new JSField object on the form - including the dataprovider/JSVariable of the JSField object. You must set location/dimension or css position afterwards

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object\
[Number](../JSLib/Number.md) type the display type of the JSField object (see the Solution Model -> JSField node for display types)

**Returns**\
[JSField](./JSField.md) 


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
form.useCssPosition = true
var variable = form.newVariable('myVar', JSVariable.TEXT);
variable.defaultValue = "'This is a default value (with triple quotes)!'";
var field = form.newField(variable, JSField.TEXT_FIELD);
field.cssPosition.l("10").t("10").w("20%").h("30px")
forms['newForm1'].controller.show();
```
### newField(dataprovider, type, x, y, width, height)

Creates a new JSField object on the form - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels.

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object\
[Number](../JSLib/Number.md) type the display type of the JSField object (see the Solution Model -> JSField node for display types)\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSField object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSField object in pixels\
[Number](../JSLib/Number.md) width the width of the JSField object in pixels\
[Number](../JSLib/Number.md) height the height of the JSField object in pixels

**Returns**\
[JSField](./JSField.md) a new JSField object (of the specified display type)


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
var variable = form.newVariable('myVar', JSVariable.TEXT);
variable.defaultValue = "'This is a default value (with triple quotes)!'";
var field = form.newField(variable, JSField.TEXT_FIELD, 100, 100, 200, 200);
forms['newForm1'].controller.show();
```
### newFooterPart(height)

Creates a new Footer part on the form.

**Parameters**\
[Number](../JSLib/Number.md) height The height of the new part

**Returns**\
[JSPart](./JSPart.md) A JSFooter instance corresponding to the newly created Footer form part.


**Sample**

```javascript
var footer = form.newFooterPart(440);
```
### newHeaderPart(height)

Creates a new Header part on the form.

**Parameters**\
[Number](../JSLib/Number.md) height The height of the new part

**Returns**\
[JSPart](./JSPart.md) A JSPart instance corresponding to the newly created Header form part.


**Sample**

```javascript
var header = form.newHeaderPart(80);
```
### newHtmlArea(dataprovider)

Creates a new JSField object on the form with the displayType of HTML_AREA - including the dataprovider/JSVariable of the JSField object. You must set location/dimension or css position afterwards

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object

**Returns**\
[JSField](./JSField.md) a JSField object on the form with the displayType of HTML_AREA


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
form.useCssPosition = true
var textProvider = form.newVariable('myVar',JSVariable.TEXT);
textProvider.defaultValue = "'This is a triple quoted text!'";
var htmlArea = myListViewForm.newHtmlArea(textProvider);
htmlArea.cssPosition.l("10").t("10").w("20%").h("30px")
forms['newForm1'].controller.show();
```
### newHtmlArea(dataprovider, x, y, width, height)

Creates a new JSField object on the form with the displayType of HTML_AREA - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels.

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSfield object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSField object in pixels\
[Number](../JSLib/Number.md) width the width of the JSField object in pixels\
[Number](../JSLib/Number.md) height the height of the JSField object in pixels

**Returns**\
[JSField](./JSField.md) a JSField object on the form with the displayType of HTML_AREA


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
var textProvider = form.newVariable('myVar',JSVariable.TEXT);
textProvider.defaultValue = "'This is a triple quoted text!'";
var htmlArea = myListViewForm.newHtmlArea(textProvider,100,100,100,100);
forms['newForm1'].controller.show();
```
### newImageMedia(dataprovider)

Creates a new JSField object on the form with the displayType of IMAGE_MEDIA - including the dataprovider/JSVariable of the JSField object. You must set location/dimension or css position afterwards

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object

**Returns**\
[JSField](./JSField.md) a new JSField object on the form with the displayType of IMAGE_MEDIA


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
form.useCssPosition = true
var myMediaVar = form.newVariable("media", JSVariable.MEDIA);
var imageMedia = form.newImageMedia(myMediaVar)
imageMedia.cssPosition.l("10").t("10").w("20%").h("30px")
forms['newForm1'].controller.show();
```
### newImageMedia(dataprovider, x, y, width, height)

Creates a new JSField object on the form with the displayType of IMAGE_MEDIA - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels.

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSfield object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSField object in pixels\
[Number](../JSLib/Number.md) width the width of the JSField object in pixels\
[Number](../JSLib/Number.md) height the height of the JSField object in pixels

**Returns**\
[JSField](./JSField.md) a new JSField object on the form with the displayType of IMAGE_MEDIA


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
var myMediaVar = form.newVariable("media", JSVariable.MEDIA);
var imageMedia = form.newImageMedia(myMediaVar,100,100,200,200)
forms['newForm1'].controller.show();
```
### newLabel(txt)

Creates a new JSLabel object on the form - including the text of the label. You must set location/dimension or css position afterwards

**Parameters**\
[String](../JSLib/String.md) txt the specified text of the label object

**Returns**\
[JSComponent](./JSComponent.md) a JSLabel object


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
form.useCssPosition = true
var label = form.newLabel('The text on the label');
label.cssPosition.l("10%").t("10%").w("80px").h("30px")
forms['newForm1'].controller.show();
```
### newLabel(txt, x, y, width, height)

Creates a new JSLabel object on the form - including the text of the label, the "x" and "y" position of the label object in pixels, the width and height of the label object in pixels.

**Parameters**\
[String](../JSLib/String.md) txt the specified text of the label object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the label object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the label object in pixels\
[Number](../JSLib/Number.md) width the width of the label object in pixels\
[Number](../JSLib/Number.md) height the height of the label object in pixels

**Returns**\
[JSComponent](./JSComponent.md) a JSLabel object


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
var label = form.newLabel('The text on the label', 140, 140, 50, 20);
forms['newForm1'].controller.show();
```
### newLabel(txt, x, y, width, height, action)

Creates a new JSLabel object on the form - including the text of the label, the "x" and "y" position of the label object in pixels, the width and height of the label object in pixels and a JSMethod action such as the method for an onAction event.

**Parameters**\
[String](../JSLib/String.md) txt the specified text of the label object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the label object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the label object in pixels\
[Number](../JSLib/Number.md) width the width of the label object in pixels\
[Number](../JSLib/Number.md) height the height of the label object in pixels\
[Object](../JSLib/Object.md) action the event action JSMethod of the label object

**Returns**\
[JSComponent](./JSComponent.md) a JSLabel object


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
var label = form.newLabel('The text on the label', 140, 140, 50, 20);
forms['newForm1'].controller.show();
```
### newLayoutContainer()

Create a new layout container as the last child of its parent container.
This method can only be used in responsive forms.

If you want to use default values and so on from a layout package (like 12grid) or if you use the solution model
to create a form that is saved back into the workspace (servoyDeveloper.save(form)) then you have to set the
packageName and specName properties. So that it works later on in the designer.

If the packageName and specName are not provided, then:
   the packageName is the same as for the parent container
   the specName is the first allowed child defined in the specification of the parent container

If the specification of the parent container does not defined allowed children, then if it is not empty
   the packageName and the specName are copied from the first child layout container.


**Returns**\
[JSLayoutContainer](./JSLayoutContainer.md) the new layout container


**Sample**

```javascript
var container = form.newLayoutContainer();
container.packageName = "12grid";
container.specName = "row";
```
### newLayoutContainer(position)

Create a new layout container. The position is used to determine the generated order in html markup.
This method can only be used in responsive forms.

If you want to use default values and so on from a layout package (like 12grid) or if you use the solution model
to create a form that is saved back into the workspace (servoyDeveloper.save(form)) then you have to set the
packageName and specName properties. So that it works later on in the designer.

If the packageName and specName are not provided, then:
   the packageName is the same as for the parent container
   the specName is the first allowed child defined in the specification of the parent container

If the specification of the parent container does not defined allowed children, then if it is not empty
   the packageName and the specName are copied from the first child layout container.

**Parameters**\
[Number](../JSLib/Number.md) position the position of JSWebComponent object in its parent container

**Returns**\
[JSLayoutContainer](./JSLayoutContainer.md) the new layout container


**Sample**

```javascript
var container = form.newLayoutContainer(1);
container.packageName = "12grid";
container.specName = "row";
```
### newLayoutContainer(position, spec)

Create a new layout container. The position is used to determine the generated order in html markup.
This method can only be used in responsive forms.

**Parameters**\
[Number](../JSLib/Number.md) position the position of JSWebComponent object in its parent container\
[String](../JSLib/String.md) spec a string of the form 'packageName-layoutName', or 'layoutName'

**Returns**\
[JSLayoutContainer](./JSLayoutContainer.md) the new layout container


**Sample**

```javascript
var container = form.newLayoutContainer(1, "12grid-row");
container.newLayoutContainer(1, "column");
```
### newLayoutContainer(spec)

Create a new layout container as the last child in its parent container.
This method can only be used in responsive forms.

**Parameters**\
[String](../JSLib/String.md) spec a string of the form 'packageName-layoutName', or 'layoutName'

**Returns**\
[JSLayoutContainer](./JSLayoutContainer.md) the new layout container


**Sample**

```javascript
var container = form.newLayoutContainer(1, "12grid-row");
container.newLayoutContainer(1, "column");
```
### newLeadingGrandSummaryPart(height)

Creates a new Leading Grand Summary part on the form.

**Parameters**\
[Number](../JSLib/Number.md) height The height of the new part

**Returns**\
[JSPart](./JSPart.md) A JSPart instance corresponding to the newly created Leading Grand Summary form part.


**Sample**

```javascript
var leadingGrandSummary = form.newLeadingGrandSummaryPart(120);
```
### newLeadingSubSummaryPart(height)

Creates a new Leading Subsummary part on the form.

**Parameters**\
[Number](../JSLib/Number.md) height The height of the new part

**Returns**\
[JSPart](./JSPart.md) A JSPart instance corresponding to the newly created Leading Subsummary form part.


**Sample**

```javascript
var leadingSubsummary = form.newLeadingSubSummaryPart(160);
```
### newListBox(dataprovider)

Creates a new JSField object on the form with the displayType of LISTBOX - including the dataprovider/JSVariable of the JSField object. You must set location/dimension or css position afterwards

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object

**Returns**\
[JSField](./JSField.md) a new JSField object on the form with the displayType of LISTBOX


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', 'myServer', 'myTable', null, true, 800, 600);
form.useCssPosition = true
var list = form.newListBox(myDataProvider);
list.cssPosition.l("10").t("10").w("20%").h("30px")
forms['newForm1'].controller.show();
```
### newListBox(dataprovider, x, y, width, height)

Creates a new JSField object on the form with the displayType of LISTBOX - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels.

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSfield object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSField object in pixels\
[Number](../JSLib/Number.md) width the width of the JSField object in pixels\
[Number](../JSLib/Number.md) height the height of the JSField object in pixels

**Returns**\
[JSField](./JSField.md) a new JSField object on the form with the displayType of LISTBOX


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', 'myServer', 'myTable', null, true, 800, 600);
var list = form.newListBox(myDataProvider, 100, 100, 200, 200);
forms['newForm1'].controller.show();
```
### newMethod(code)

Creates a new form JSMethod - based on the specified code.

**Parameters**\
[String](../JSLib/String.md) code the specified code for the new method

**Returns**\
[JSMethod](./JSMethod.md) a new JSMethod object for this form


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
var method = form.newMethod('function aMethod(event){application.output("Hello world!");}');
var button = myListViewForm.newButton('Show message!',50,50,100,30,method);
forms['newForm1'].controller.show();
```
### newMultiSelectListBox(dataprovider)

Creates a new JSField object on the form with the displayType of MULTISELECT_LISTBOX - including the dataprovider/JSVariable of the JSField object. You must set location/dimension or css position afterwards

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object

**Returns**\
[JSField](./JSField.md) a new JSField object on the form with the displayType of MULTISELECT_LISTBOX


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', 'myServer', 'myTable', null, true, 800, 600);
form.useCssPosition = true
var list = form.newMultiSelectListBox(myDataProvider);
list.cssPosition.l("10").t("10").w("20%").h("30px")
forms['newForm1'].controller.show();
```
### newMultiSelectListBox(dataprovider, x, y, width, height)

Creates a new JSField object on the form with the displayType of MULTISELECT_LISTBOX - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels.

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSfield object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSField object in pixels\
[Number](../JSLib/Number.md) width the width of the JSField object in pixels\
[Number](../JSLib/Number.md) height the height of the JSField object in pixels

**Returns**\
[JSField](./JSField.md) a new JSField object on the form with the displayType of MULTISELECT_LISTBOX


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', 'myServer', 'myTable', null, true, 800, 600);
var calendar = form.newMultiSelectListBox(myDataProvider, 100, 100, 200, 200);
forms['newForm1'].controller.show();
```
### newPart(type, height)

Creates a new part on the form. The type of the new part (use one of the JSPart constants)
and its height must be specified.

**Parameters**\
[Number](../JSLib/Number.md) type The type of the new part.\
[Number](../JSLib/Number.md) height The height of the new part

**Returns**\
[JSPart](./JSPart.md) A JSPart instance corresponding to the newly created form part.


**Sample**

```javascript
var form = solutionModel.newForm('myForm', 'db:/example_data/my_table', null, false, 1200, 800);
var header = form.newPart(JSPart.HEADER, 100);
header.background = 'yellow';
var body = form.newPart(JSPart.BODY, 700);
body.background = 'green';
var footer = form.newPart(JSPart.FOOTER, 800);
footer.background = 'orange';
```
### newPassword(dataprovider)

Creates a new JSField object on the form with the displayType of PASSWORD - including the dataprovider/JSVariable of the JSField object. You must set location/dimension or css position afterwards

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object

**Returns**\
[JSField](./JSField.md) a new JSField object on the form with the displayType of PASSWORD


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
form.useCssPosition = true
var pass = form.newPassword(scopes.globals.aVariable);
pass.cssPosition.l("10").t("10").w("20%").h("30px")
forms['newForm1'].controller.show();
```
### newPassword(dataprovider, x, y, width, height)

Creates a new JSField object on the form with the displayType of PASSWORD - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels.

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSfield object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSField object in pixels\
[Number](../JSLib/Number.md) width the width of the JSField object in pixels\
[Number](../JSLib/Number.md) height the height of the JSField object in pixels

**Returns**\
[JSField](./JSField.md) a new JSField object on the form with the displayType of PASSWORD


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
var pass = form.newPassword(scopes.globals.aVariable, 100, 100, 70, 30);
forms['newForm1'].controller.show();
```
### newPortal(name, relation)

Creates a new JSPortal object on the form - including the name of the JSPortal object and the relation the JSPortal object is based on. You must set location/dimension or css position afterwards

**Parameters**\
[String](../JSLib/String.md) name the specified name of the JSPortal object\
[Object](../JSLib/Object.md) relation the relation of the JSPortal object

**Returns**\
[JSComponent](./JSComponent.md) a JSPortal object


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', 'db:/server1/table1', null, true, 800, 600);
form.useCssPosition = true
var relation = solutionModel.newRelation('parentToChild','db:/server1/table1','db:/server2/table2',JSRelation.INNER_JOIN);
relation.newRelationItem('another_parent_table_id', '=', 'another_child_table_parent_id');
var portal = form.newPortal('portal',relation);
portal.cssPosition.l("10%").t("10%").b("10%").r("10%")
portal.newField('someColumn',JSField.TEXT_FIELD,200,200,120);
forms['newForm1'].controller.show();
```
### newPortal(name, relation, x, y, width, height)

Creates a new JSPortal object on the form - including the name of the JSPortal object; the relation the JSPortal object is based on, the "x" and "y" position of the JSPortal object in pixels, as well as the width and height of the JSPortal object in pixels.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the JSPortal object\
[Object](../JSLib/Object.md) relation the relation of the JSPortal object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSPortal object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSPortal object in pixels\
[Number](../JSLib/Number.md) width the width of the JSPortal object in pixels\
[Number](../JSLib/Number.md) height the height of the JSPortal object in pixels

**Returns**\
[JSComponent](./JSComponent.md) a JSPortal object


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', 'db:/server1/table1', null, true, 800, 600);
var relation = solutionModel.newRelation('parentToChild','db:/server1/table1','db:/server2/table2',JSRelation.INNER_JOIN);
relation.newRelationItem('another_parent_table_id', '=', 'another_child_table_parent_id');
var portal = form.newPortal('portal',relation,200,200,300,300);
portal.newField('someColumn',JSField.TEXT_FIELD,200,200,120);
forms['newForm1'].controller.show();
```
### newRadios(dataprovider)

Creates a new JSField object on the form with the displayType of RADIOS (radio buttons) - including the dataprovider/JSVariable of the JSField object. You must set location/dimension or css position afterwards

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object

**Returns**\
[JSField](./JSField.md) a JSField object with the displayType of RADIOS (radio buttons)


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
form.useCssPosition = true
var vlist = solutionModel.newValueList('options',JSValueList.CUSTOM_VALUES);
vlist.customValues = "value1\nvalue2\nvalue3";
var radios = form.newRadios('columnDataProvider');
radios.cssPosition.l("10").t("10").w("20%").h("30px")
radios.valuelist = vlist;
```
### newRadios(dataprovider, x, y, width, height)

Creates a new JSField object on the form with the displayType of RADIOS (radio buttons) - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels.

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSfield object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSField object in pixels\
[Number](../JSLib/Number.md) width the width of the JSField object in pixels\
[Number](../JSLib/Number.md) height the height of the JSField object in pixels

**Returns**\
[JSField](./JSField.md) a JSField object with the displayType of RADIOS (radio buttons)


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
var vlist = solutionModel.newValueList('options',JSValueList.CUSTOM_VALUES);
vlist.customValues = "value1\nvalue2\nvalue3";
var radios = form.newRadios('columnDataProvider',100,100,200,200);
radios.valuelist = vlist;
```
### newRtfArea(dataprovider, x, y, width, height)

Creates a new JSField object on the form with the displayType of RTF_AREA (enables more than one line of text to be displayed in a field) - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels.

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSfield object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSField object in pixels\
[Number](../JSLib/Number.md) width the width of the JSField object in pixels\
[Number](../JSLib/Number.md) height the height of the JSField object in pixels

**Returns**\
[JSField](./JSField.md) a JSField object with the displayType of RTF_AREA


**Sample**

```javascript
var form = solutionModel.newForm('newForm1',myDatasource,null,true,800,600);
var rtf_area = form.newRtfArea('columnDataProvider',100,100,100,100);
forms['newForm1'].controller.show();
```
### newSpinner(dataprovider)

Creates a new JSField object on the form with the displayType of SPINNER - including the dataprovider/JSVariable of the JSField object. You must set location/dimension or css position afterwards

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object

**Returns**\
[JSField](./JSField.md) a new JSField object on the form with the displayType of SPINNER


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', 'myServer', 'myTable', null, true, 800, 600);
form.useCssPosition = true
var spinner = form.newSpinner(myDataProvider, 10, 460, 100, 20);
spinner.cssPosition.l("10").t("10").w("20%").h("30px")
forms['newForm1'].controller.show();
```
### newSpinner(dataprovider, x, y, width, height)

Creates a new JSField object on the form with the displayType of SPINNER - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels.

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSfield object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSField object in pixels\
[Number](../JSLib/Number.md) width the width of the JSField object in pixels\
[Number](../JSLib/Number.md) height the height of the JSField object in pixels

**Returns**\
[JSField](./JSField.md) a new JSField object on the form with the displayType of SPINNER


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', 'myServer', 'myTable', null, true, 800, 600);
var spinner = form.newSpinner(myDataProvider, 10, 460, 100, 20);
forms['newForm1'].controller.show();
```
### newTabPanel(name)

Creates a new JSTabPanel object on the form - including the name of the JSTabPanel object. You must set location/dimension or css position afterwards

**Parameters**\
[String](../JSLib/String.md) name the specified name of the JSTabPanel object

**Returns**\
[JSComponent](./JSComponent.md) a JSTabPanel object


**Sample**

```javascript
var form = solutionModel.newForm('parentForm','db:/server1/parent_table',null,false,640,480);
form.useCssPosition = true
var childOne = solutionModel.newForm('childOne','db:/server1/child_table',null,false,400,300);
childOne.newField('child_table_text', JSField.TEXT_FIELD,10,10,100,20);
var parentToChild = solutionModel.newRelation('parentToChild','db:/server1/parent_table','db:/server1/child_table',JSRelation.INNER_JOIN);
parentToChild.newRelationItem('parent_table_id','=','child_table_parent_id');
var childTwo = solutionModel.newForm('childTwo','db:/server1/my_table',null,false,400,300);
childTwo.newField('my_table_image', JSField.IMAGE_MEDIA,10,10,100,100);
var tabPanel = form.newTabPanel('tabs');
tabPanel.cssPosition.l("10%").t("10%").b("10%").r("10%")
tabPanel.newTab('tab1','Child One',childOne,parentToChild);
tabPanel.newTab('tab2','Child Two',childTwo);
forms['parentForm'].controller.show();
```
### newTabPanel(name, x, y, width, height)

Creates a new JSTabPanel object on the form - including the name of the JSTabPanel object, the "x" and "y" position of the JSTabPanel object in pixels, as well as the width and height of the JSTabPanel object in pixels.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the JSTabPanel object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSTabPanel object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSTabPanel object in pixels\
[Number](../JSLib/Number.md) width the width of the JSTabPanel object in pixels\
[Number](../JSLib/Number.md) height the height of the JSTabPanel object in pixels

**Returns**\
[JSComponent](./JSComponent.md) a JSTabPanel object


**Sample**

```javascript
var form = solutionModel.newForm('parentForm','db:/server1/parent_table',null,false,640,480);
var childOne = solutionModel.newForm('childOne','db:/server1/child_table',null,false,400,300);
childOne.newField('child_table_text', JSField.TEXT_FIELD,10,10,100,20);
var parentToChild = solutionModel.newRelation('parentToChild','db:/server1/parent_table','db:/server1/child_table',JSRelation.INNER_JOIN);
parentToChild.newRelationItem('parent_table_id','=','child_table_parent_id');
var childTwo = solutionModel.newForm('childTwo','db:/server1/my_table',null,false,400,300);
childTwo.newField('my_table_image', JSField.IMAGE_MEDIA,10,10,100,100);
var tabPanel = form.newTabPanel('tabs',10,10,620,460);
tabPanel.newTab('tab1','Child One',childOne,parentToChild);
tabPanel.newTab('tab2','Child Two',childTwo);
forms['parentForm'].controller.show();
```
### newTextArea(dataprovider)

Creates a new JSField object on the form with the displayType of TEXT_AREA - including the dataprovider/JSVariable of the JSField object. You must set location/dimension or css position afterwards

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object

**Returns**\
[JSField](./JSField.md) a JSField object with the displayType of TEXT_AREA


**Sample**

```javascript
var form = solutionModel.newForm('newForm1',myDatasource,null,true,800,600);
form.useCssPosition = true
var globalVar = solutionModel.newGlobalVariable('globals', 'myGlobal',JSVariable.TEXT);
globalVar.defaultValue = "'Type your text in here'";
var textArea = form.newTextArea(globalVar);
textArea.cssPosition.l("10").t("10").w("20%").h("30px")
forms['newForm1'].controller.show();
```
### newTextArea(dataprovider, x, y, width, height)

Creates a new JSField object on the form with the displayType of TEXT_AREA - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels.

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSTabPanel object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSTabPanel object in pixels\
[Number](../JSLib/Number.md) width the width of the JSTabPanel object in pixels\
[Number](../JSLib/Number.md) height the height of the JSTabPanel object in pixels

**Returns**\
[JSField](./JSField.md) a JSField object with the displayType of TEXT_AREA


**Sample**

```javascript
var form = solutionModel.newForm('newForm1',myDatasource,null,true,800,600);
var globalVar = solutionModel.newGlobalVariable('globals', 'myGlobal',JSVariable.TEXT);
globalVar.defaultValue = "'Type your text in here'";
var textArea = form.newTextArea(globalVar,100,100,300,150);
forms['newForm1'].controller.show();
```
### newTextField(dataprovider)

Creates a new JSField object on the form with the displayType of TEXT_FIELD - including the dataprovider/JSVariable of the JSField object. You must set location/dimension or css position afterwards

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object

**Returns**\
[JSField](./JSField.md) a JSField object with the displayType of TEXT_FIELD


**Sample**

```javascript
var form = solutionModel.newForm('newForm1',myDatasource,null,true,800,600);
form.useCssPosition = true
var x = solutionModel.newGlobalVariable('globals', 'myGlobal',JSVariable.TEXT);
x.defaultValue = "'Text from a global variable'"
var textField = form.newTextField(x);
textField.cssPosition.l("10").t("10").w("20%").h("30px")
forms['newForm1'].controller.show();
```
### newTextField(dataprovider, x, y, width, height)

Creates a new JSField object on the form with the displayType of TEXT_FIELD - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels.

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSfield object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSField object in pixels\
[Number](../JSLib/Number.md) width the width of the JSField object in pixels\
[Number](../JSLib/Number.md) height the height of the JSField object in pixels

**Returns**\
[JSField](./JSField.md) a JSField object with the displayType of TEXT_FIELD


**Sample**

```javascript
var form = solutionModel.newForm('newForm1',myDatasource,null,true,800,600);
//choose the dataprovider or jsvariable you want for the Text Field
var x = null;
//global jsvariable as the dataprovider
//x = solutionModel.newGlobalVariable('globals', 'myGlobal',JSVariable.TEXT);
//x.defaultValue = "'Text from a global variable'";
//or a form jsvariable as the dataprovider
//x = form.newVariable('myFormVar',JSVariable.TEXT);
//x.defaultValue = "'Text from a form variable'";
var textField = form.newTextField(x,100,100,200,50);
//or a column data provider as the dataprovider
//textField.dataProviderID = columnTextDataProvider;
forms['newForm1'].controller.show();
```
### newTitleFooterPart(height)

Creates a new Title Footer part on the form.

**Parameters**\
[Number](../JSLib/Number.md) height The height of the new part

**Returns**\
[JSPart](./JSPart.md) A JSPart instance corresponding to the newly created Title Footer form part.


**Sample**

```javascript
var titleFooter = form.newTitleFooterPart(500);
```
### newTitleHeaderPart(height)

Creates a new Title Header part on the form.

**Parameters**\
[Number](../JSLib/Number.md) height The height of the new part

**Returns**\
[JSPart](./JSPart.md) A JSPart instance corresponding to the newly created Title Header form part.


**Sample**

```javascript
var titleHeader = form.newTitleHeaderPart(40);
```
### newTrailingGrandSummaryPart(height)

Creates a new Trailing Grand Summary part on the form.

**Parameters**\
[Number](../JSLib/Number.md) height The height of the new part

**Returns**\
[JSPart](./JSPart.md) A JSPart instance corresponding to the newly created Trailing Grand Summary form part.


**Sample**

```javascript
var trailingGrandSummary = form.newTrailingGrandSummaryPart(400);
```
### newTrailingSubSummaryPart(height)

Creates a new Trailing Subsummary part on the form.

**Parameters**\
[Number](../JSLib/Number.md) height The height of the new part

**Returns**\
[JSPart](./JSPart.md) A JSPart instance corresponding to the newly created Trailing Subsummary form part.


**Sample**

```javascript
var trailingSubsummary = form.newTrailingSubSummaryPart(360);
```
### newTypeAhead(dataprovider)

Creates a new JSField object on the form with the displayType of TYPE_AHEAD - including the dataprovider/JSVariable of the JSField object. You must set location/dimension or css position afterwards

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object

**Returns**\
[JSField](./JSField.md) a JSField object with the displayType of TYPE_AHEAD


**Sample**

```javascript
var form = solutionModel.newForm('newForm1',myDatasource,null,true,800,600);
form.useCssPosition = true
var vlist = solutionModel.newValueList('options',JSValueList.CUSTOM_VALUES);
vlist.customValues = "value1\nvalue2\nvalue3";
var typeAhead = form.newTypeAhead(columnTextDataProvider);
typeAhead.cssPosition.l("10").t("10").w("20%").h("30px")
typeAhead.valuelist = vlist;
forms['newForm1'].controller.show();
```
### newTypeAhead(dataprovider, x, y, width, height)

Creates a new JSField object on the form with the displayType of TYPE_AHEAD - including the dataprovider/JSVariable of the JSField object, the "x" and "y" position of the JSField object in pixels, as well as the width and height of the JSField object in pixels.

**Parameters**\
[Object](../JSLib/Object.md) dataprovider the specified dataprovider name/JSVariable of the JSField object\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSfield object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSField object in pixels\
[Number](../JSLib/Number.md) width the width of the JSField object in pixels\
[Number](../JSLib/Number.md) height the height of the JSField object in pixels

**Returns**\
[JSField](./JSField.md) a JSField object with the displayType of TYPE_AHEAD


**Sample**

```javascript
var form = solutionModel.newForm('newForm1',myDatasource,null,true,800,600);
var vlist = solutionModel.newValueList('options',JSValueList.CUSTOM_VALUES);
vlist.customValues = "value1\nvalue2\nvalue3";
var typeAhead = form.newTypeAhead(columnTextDataProvider,100,100,300,200);
typeAhead.valuelist = vlist;
forms['newForm1'].controller.show();
```
### newVariable(name, type)

Creates a new form JSVariable - based on the name of the variable object and the number type, uses the SolutionModel JSVariable constants.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the variable\
[Number](../JSLib/Number.md) type the specified type of the variable (see Solution Model -> JSVariable node constants)

**Returns**\
[JSVariable](./JSVariable.md) a JSVariable object


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
var variable = form.newVariable('myVar', JSVariable.TEXT , "'This is a default value (with triple quotes)!'");
//or variable = form.newVariable('myVar', JSVariable.TEXT)
//variable.defaultValue = "'This is a default value (with triple quotes)!'" // setting the default value after the variable is created requires form recreation
//variable.defaultValue = "{a:'First letter',b:'Second letter'}"
var field = form.newField(variable, JSField.TEXT_FIELD, 100, 100, 200, 200);
forms['newForm1'].controller.show();
```
### newVariable(name, type, defaultValue)

Creates a new form JSVariable - based on the name of the variable object , the  type  and it's default value , uses the SolutionModel JSVariable constants.

This method does not require the form to be destroyed and recreated. Use this method if you want to change the form's model without destroying the runtime form</b>

**Parameters**\
[String](../JSLib/String.md) name the specified name of the variable\
[Number](../JSLib/Number.md) type the specified type of the variable (see Solution Model -> JSVariable node constants)\
[String](../JSLib/String.md) defaultValue the default value as a javascript expression string

**Returns**\
[JSVariable](./JSVariable.md) a JSVariable object


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', myDatasource, null, true, 800, 600);
var variable = form.newVariable('myVar', JSVariable.TEXT , "'This is a default value (with triple quotes)!'");
//or variable = form.newVariable('myVar', JSVariable.TEXT)
//variable.defaultValue = "'This is a default value (with triple quotes)!'" // setting the default value after the variable is created requires form recreation
//variable.defaultValue = "{a:'First letter',b:'Second letter'}"
var field = form.newField(variable, JSField.TEXT_FIELD, 100, 100, 200, 200);
forms['newForm1'].controller.show();
```
### newWebComponent(type)

Creates a new JSWebComponent (spec based component) object on the RESPONSIVE form.
Will receive a generated name. Will be added as last position in container.

**Parameters**\
[String](../JSLib/String.md) type the webcomponent name as it appears in the spec

**Returns**\
[JSComponent](./JSComponent.md) a JSWebComponent object


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', 'db:/server1/table1', null, true, 800, 600);
var container = myForm.getLayoutContainer("row1")
var bean = container.newWebComponent('mypackage-testcomponent');
```
### newWebComponent(type, position)

Creates a new JSWebComponent (spec based component) object on the RESPONSIVE form.
Will receive a generated name.

**Parameters**\
[String](../JSLib/String.md) type the webcomponent name as it appears in the spec\
[Number](../JSLib/Number.md) position the position of JSWebComponent object in its parent container

**Returns**\
[JSComponent](./JSComponent.md) a JSWebComponent object


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', 'db:/server1/table1', null, true, 800, 600);
var container = myForm.getLayoutContainer("row1")
var bean = container.newWebComponent('mypackage-testcomponent',1);
```
### newWebComponent(name, type)

Creates a new JSWebComponent (spec based component) object on a form. You must set location/dimension or css position afterwards

**Parameters**\
[String](../JSLib/String.md) name the specified name of the JSWebComponent object\
[String](../JSLib/String.md) type the webcomponent name as it appears in the spec

**Returns**\
[JSComponent](./JSComponent.md) a JSWebComponent object


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', 'db:/server1/table1', null, true, 800, 600);
form.useCssPosition = true
var webcomponent = form.newWebComponent('mywebcomponent','mypackage-testcomponent');
```
### newWebComponent(name, type, position)

Creates a new JSWebComponent (spec based component) object on the RESPONSIVE form.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the JSWebComponent object\
[String](../JSLib/String.md) type the webcomponent name as it appears in the spec\
[Number](../JSLib/Number.md) position the position of JSWebComponent object in its parent container

**Returns**\
[JSComponent](./JSComponent.md) a JSWebComponent object


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', 'db:/server1/table1', null, true, 800, 600);
var container = myForm.getLayoutContainer("row1")
var bean = container.newWebComponent('bean','mypackage-testcomponent',1);
```
### newWebComponent(name, type, x, y, width, height)

Creates a new JSWebComponent (spec based component) object on the form.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the JSWebComponent object\
[String](../JSLib/String.md) type the webcomponent name as it appears in the spec\
[Number](../JSLib/Number.md) x the horizontal "x" position of the JSWebComponent object in pixels\
[Number](../JSLib/Number.md) y the vertical "y" position of the JSWebComponent object in pixels\
[Number](../JSLib/Number.md) width the width of the JSWebComponent object in pixels\
[Number](../JSLib/Number.md) height the height of the JSWebComponent object in pixels

**Returns**\
[JSComponent](./JSComponent.md) a JSWebComponent object


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', 'db:/server1/table1', null, true, 800, 600);
var bean = form.newWebComponent('bean','mypackage-testcomponent',200,200,300,300);
forms['newForm1'].controller.show();
```
### putDesignTimeProperty(key, value)

Set a design-time property of a form.

**Parameters**\
[String](../JSLib/String.md) key the property name\
[Object](../JSLib/Object.md) value the value to set

**Returns**\
[Object](../JSLib/Object.md) 


**Sample**

```javascript
var frm = solutionModel.getForm('orders')
frm.putDesignTimeProperty('myprop', 'lemon')
```
### removeBean(name)

Removes a JSBean that has the specified name. Returns true if removal was successful, false otherwise.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the JSBean to be removed

**Returns**\
[Boolean](../JSLib/Boolean.md) true if the JSBean has been removed; false otherwise


**Sample**

```javascript
var form = solutionModel.getForm('myform');
form.removeBean('mybean')
```
### removeButton(name)

Removes a JSButton that has the specified name. Returns true if removal was successful, false otherwise.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the JSButton to be removed

**Returns**\
[Boolean](../JSLib/Boolean.md) true if the JSButton has been removed; false otherwise


**Sample**

```javascript
var form = solutionModel.newForm('newFormX',myDatasource,null,true,800,600);
var b1 = form.newButton('This is button1',100,100,200,50,null);
b1.name = 'b1';
var jsmethod = form.newMethod("function removeMe(event) { var form = solutionModel.getForm('newFormX'); if (form.removeButton('b1') == true) application.output('Button has been removed ok'); else application.output('Button could not be deleted'); forms['newFormX'].controller.recreateUI();}");
var b2 = form.newButton('Click here to remove button1',100,230,200,50,jsmethod);
b2.name = 'b2';
forms['newFormX'].controller.show();
```
### removeComponent(name)

Removes a component (JSLabel, JSButton, JSField, JSPortal, JSBean, JSTabpanel, JSWebComponent) that has the given name. It is the same as calling "if(!removeLabel(name) &amp;&amp; !removeButton(name) ....)".
Returns true if removal was successful, false otherwise.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the component to be deleted

**Returns**\
[Boolean](../JSLib/Boolean.md) true if component has been successfully deleted; false otherwise


**Sample**

```javascript
var form = solutionModel.newForm('newFormX','db:/server1/parent_table',null,true,1000,750);
var jsbutton = form.newButton('JSButton to delete',100,100,200,50,null);
jsbutton.name = 'jsb';
var jslabel = form.newLabel('JSLabel to delete',100,200,200,50,null);
jslabel.name = 'jsl';
jslabel.transparent = false;
jslabel.background = 'green';
var jsfield = form.newField('scopes.globals.myGlobalVariable',JSField.TEXT_FIELD,100,300,200,50);
jsfield.name = 'jsf';
var relation = solutionModel.newRelation('parentToChild','db:/server1/parent_table','db:/server1/child_table',JSRelation.INNER_JOIN);
relation.newRelationItem('parent_table_id', '=', 'child_table_id');
var jsportal = form.newPortal('jsp',relation,100,400,300,300);
jsportal.newField('child_table_id',JSField.TEXT_FIELD,200,200,120);
var childOne = solutionModel.newForm('childOne','db:/server1/child_table',null,false,400,300);
childOne.newField('child_table_id', JSField.TEXT_FIELD,10,10,100,20);
var childTwo = solutionModel.newForm('childTwo','server1','other_table',null,false,400,300);
childTwo.newField('some_table_id', JSField.TEXT_FIELD,10,10,100,100);
var jstabpanel = form.newTabPanel('jst',450,30,620,460);
jstabpanel.newTab('tab1','Child One',childOne,relation);
jstabpanel.newTab('tab2','Child Two',childTwo);
var jsmethod = form.newMethod("function removeMe(event) { var form = solutionModel.getForm('newFormX');\n if ((form.removeComponent('jsb') == true) && (form.removeComponent('jsl') == true) && (form.removeComponent('jsf') == true) && (form.removeComponent('jsp') == true) & (form.removeComponent('jst') == true)) application.output('Components removed ok'); else application.output('Some component(s) could not be deleted'); forms['newFormX'].controller.recreateUI();}");
var removerButton = form.newButton('Click here to remove form components',450,500,250,50,jsmethod);
removerButton.name = 'remover';
forms['newFormX'].controller.show();
```
### removeDesignTimeProperty(key)

Clear a design-time property of a form.

**Parameters**\
[String](../JSLib/String.md) key the property name

**Returns**\
[Object](../JSLib/Object.md) 


**Sample**

```javascript
var frm = solutionModel.getForm('orders')
frm.removeDesignTimeProperty('myprop')
```
### removeField(name)

Removes a JSField that has the given name. Returns true if removal was successful, false otherwise.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the JSField to remove

**Returns**\
[Boolean](../JSLib/Boolean.md) true is the JSField has been successfully removed; false otherwise


**Sample**

```javascript
var form = solutionModel.newForm('newFormX',myDatasource,null,true,800,600);
var jsfield = form.newField(scopes.globals.myGlobalVariable,JSField.TEXT_FIELD,100,300,200,50);
jsfield.name = 'jsf';
var jsmethod = form.newMethod("function removeMe(event) { var form = solutionModel.getForm('newFormX');\n if (form.removeComponent('jsf') == true) application.output('Field has been removed ok'); else application.output('Field could not be deleted'); forms['newFormX'].controller.recreateUI();}");
var removerButton = form.newButton('Click here to remove the field',450,500,250,50,jsmethod);
removerButton.name = 'remover';
forms['newFormX'].controller.show();
```
### removeLabel(name)

Removes a JSLabel that has the given name. Returns true if removal successful, false otherwise

**Parameters**\
[String](../JSLib/String.md) name the specified name of the JSLabel to be removed

**Returns**\
[Boolean](../JSLib/Boolean.md) true if the JSLabel with the given name has successfully been removed; false otherwise


**Sample**

```javascript
var form = solutionModel.newForm('newFormX',myDatasource,null,true,1000,750);
var jslabel = form.newLabel('JSLabel to delete',100,200,200,50,null);
jslabel.name = 'jsl';
jslabel.transparent = false;
jslabel.background = 'green';
var jsmethod = form.newMethod("function removeMe(event) { var form = solutionModel.getForm('newFormX'); if (form.removeComponent('jsl') == true) application.output('Label has been removed'); else application.output('Label could not be deleted'); forms['newFormX'].controller.recreateUI();}");
var removerButton = form.newButton('Click here to remove the green label',450,500,250,50,jsmethod);
removerButton.name = 'remover';
forms['newFormX'].controller.show();
```
### removeMethod(name)

Removes a  form JSMethod - based on the specified code.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the method

**Returns**\
[Boolean](../JSLib/Boolean.md) true if method was removed successfully , false otherwise


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', null, null, true, 800, 600);
var hello = form.newMethod('function aMethod(event){application.output("Hello world!");}');
var removeMethod = form.newMethod('function removeMethod(event){ \
									solutionModel.getForm(event.getFormName()).removeMethod("aMethod"); \
									forms[event.getFormName()].controller.recreateUI();\
									}');
var button1 = form.newButton('Call method!',50,50,120,30,hello);
var button2 = form.newButton('Remove Mehtod!',200,50,120,30,removeMethod);
forms['newForm1'].controller.show();
```
### removePart(type)

Removes a JSPart of the given type.

**Parameters**\
[Number](../JSLib/Number.md) type The type of the part that should be removed.

**Returns**\
[Boolean](../JSLib/Boolean.md) True if the part is successfully removed, false otherwise.


**Sample**

```javascript
form.removePart(JSPart.HEADER);
form.removePart(JSPart.LEADING_SUBSUMMARY, 160);
```
### removePart(type, height)

Removes a JSPart of the given type. The height parameter is for removing one of multiple subsummary parts.

**Parameters**\
[Number](../JSLib/Number.md) type The type of the part that should be removed.\
[Number](../JSLib/Number.md) height The height of the part that should be removed. This parameter is for
					removing one of multiple Leading/Trailing Subsummary parts.

**Returns**\
[Boolean](../JSLib/Boolean.md) True if the part is successfully removed, false otherwise.


**Sample**

```javascript
form.removePart(JSPart.HEADER);
form.removePart(JSPart.LEADING_SUBSUMMARY, 160);
```
### removePortal(name)

Removes a JSPortal that has the given name. Returns true if removal was successful, false otherwise.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the JSPortal to be removed

**Returns**\
[Boolean](../JSLib/Boolean.md) true if the JSPortal has successfully been removed; false otherwise


**Sample**

```javascript
var form = solutionModel.newForm('newFormX',myDatasource,null,true,800,600);
var relation = solutionModel.newRelation('parentToChild','db:/server1/myTable','db:/server1/myOtherTable',JSRelation.INNER_JOIN);
relation.newRelationItem('parent_table_id', '=', 'child_table_id');
var jsportal = form.newPortal('jsp',relation,100,400,300,300);
jsportal.newField('child_table_id',JSField.TEXT_FIELD,200,200,120);
var jsmethod = form.newMethod("function removeMe(event) { var form = solutionModel.getForm('newFormX');\n if (form.removeComponent('jsp') == true) application.output('Portal removed ok'); else application.output('Portal could not be deleted'); forms['newFormX'].controller.recreateUI();}");
var removerButton = form.newButton('Click here to remove the portal',450,500,250,50,jsmethod);
removerButton.name = 'remover';
forms['newFormX'].controller.show();
```
### removeTabPanel(name)

Removes a JSTabPanel that has the given name. Returns true if removal was successful, false otherwise.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the JSTabPanel to be removed

**Returns**\
[Boolean](../JSLib/Boolean.md) true is the JSTabPanel has been successfully removed, false otherwise


**Sample**

```javascript
var form = solutionModel.newForm('newFormX','db:/server1/parent_table',null,false,800,600);
var childOne = solutionModel.newForm('childOne','db:/server1/child_table',null,false,400,300);
childOne.newField('child_table_text', JSField.TEXT_FIELD,10,10,100,20);
var parentToChild = solutionModel.newRelation('parentToChild','db:/server1/parent_table','db:/server1/child_table',JSRelation.INNER_JOIN);
parentToChild.newRelationItem('parent_table_id','=','child_table_id');
var childTwo = solutionModel.newForm('childTwo','db:/server1/another_table',null,false,400,300);
childTwo.newField('columnDataProvider', JSField.TEXT_FIELD,10,10,100,100);
var tabPanel = form.newTabPanel('jst',10,10,620,460);
tabPanel.newTab('tab1','Child One',childOne,parentToChild);
tabPanel.newTab('tab2','Child Two',childTwo);
var jsmethod = form.newMethod("function removeMe(event) { var form = solutionModel.getForm('newFormX');\n if (form.removeComponent('jst') == true)\n application.output('TabPanel has been removed ok');\n else\n application.output('TabPanel could not be deleted');\n forms['newFormX'].controller.recreateUI();\n}");
var removerButton = form.newButton('Click here to remove the tab panel',450,500,250,50,jsmethod);
removerButton.name = 'remover';
forms['newFormX'].controller.show();
```
### removeVariable(name)

Removes a form JSVariable - based on the name of the variable object.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the variable

**Returns**\
[Boolean](../JSLib/Boolean.md) true if removed, false otherwise (ex: no var with that name)


**Sample**

```javascript
var form = solutionModel.newForm('newForm1', null, null, true, 800, 600);
var variable = form.newVariable('myVar', JSVariable.TEXT);
variable.defaultValue = "'This is a default value (with triple quotes)!'";
//variable.defaultValue = "{a:'First letter',b:'Second letter'}"
var field = form.newField(variable, JSField.TEXT_FIELD, 100, 100, 200, 200);
forms['newForm1'].controller.show();

variable = form.removeVariable('myVar');
application.sleep(4000);
forms['newForm1'].controller.recreateUI();
```
### removeWebComponent(name)

Removes a JSWebComponent that has the specified name. Returns true if removal was successful, false otherwise.

**Parameters**\
[String](../JSLib/String.md) name the specified name of the JSWebComponent to be removed

**Returns**\
[Boolean](../JSLib/Boolean.md) true if the JSWebComponent has been removed; false otherwise


**Sample**

```javascript
var form = solutionModel.getForm('myform');
form.removeWebComponent('mybean')
```

