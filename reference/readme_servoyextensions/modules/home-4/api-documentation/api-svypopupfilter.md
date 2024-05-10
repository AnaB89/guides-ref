# API svyPopupFilter

### Classes

[AbstractPopupFilter](api-svypopupfilter.md#abstractpopupfilter)

[SvyCheckFilter](api-svypopupfilter.md#svycheckfilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

[SvyDateFilter](api-svypopupfilter.md#svydatefilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

[SvyIntegerFilter](api-svypopupfilter.md#svyintegerfilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

[SvyNumberFilter](api-svypopupfilter.md#svynumberfilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

[SvySelectFilter](api-svypopupfilter.md#svyselectfilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

[SvyTokenFilter](api-svypopupfilter.md#svytokenfilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

### Functions

[applyLocaleStrings(formName, formType)](api-svypopupfilter.md#applylocalestrings-formname-formtype)

Applies the locale strings set on svyToolbarFilter.TOOLBAR\_LOCALE to the matching elements for the given form identifier which is one of TOOLBAR\_LOCALE's main properties

[createCheckFilter()](api-svypopupfilter.md#createcheckfilter-svycheckfilter) ⇒ [`SvyCheckFilter`](api-svypopupfilter.md#svycheckfilter-abstractpopupfilter)

[createDateFilter()](api-svypopupfilter.md#createdatefilter-svydatefilter) ⇒ [`SvyDateFilter`](api-svypopupfilter.md#svydatefilter-abstractpopupfilter)

[createIntegerFilter()](api-svypopupfilter.md#createintegerfilter-svyintegerfilter) ⇒ [`SvyIntegerFilter`](api-svypopupfilter.md#svyintegerfilter-abstractpopupfilter)

[createNumberFilter()](api-svypopupfilter.md#createnumberfilter-svynumberfilter) ⇒ [`SvyNumberFilter`](api-svypopupfilter.md#svynumberfilter-abstractpopupfilter)

[createSelectFilter(dataProvider, lookup)](api-svypopupfilter.md#createselectfilter-dataprovider-lookup-svyselectfilter) ⇒ [`SvySelectFilte`](api-svypopupfilter.md#svyselectfilter-abstractpopupfilter)

[createTokenFilter()](api-svypopupfilter.md#createtokenfilter-svytokenfilter) ⇒ [`SvyTokenFilter`](api-svypopupfilter.md#svytokenfilter-abstractpopupfilter)

[getVersion()](api-svypopupfilter.md#getversion-string) ⇒ `String`

Gets the version of this module

### AbstractPopupFilter

* [AbstractPopupFilter](api-svypopupfilter.md#abstractpopupfilter)
  * [.addParam(param)](api-svypopupfilter.md#abstractpopupfilter.addparam-param)
  * [.clearParams()](api-svypopupfilter.md#abstractpopupfilter.clearparams)
  * [.createPopUp(callback)](api-svypopupfilter.md#abstractpopupfilter.createpopup-callback-plugins.window.formpopup) ⇒ `plugins.window.FormPopup`
  * [.createWindow(\[x\], \[y\], \[width\], \[height\], \[jsWindowType\])](api-svypopupfilter.md#abstractpopupfilter.createwindow-x-y-width-height-jswindowtype-jswindow) ⇒ `JSWindow`
  * [.getDataProvider()](api-svypopupfilter.md#abstractpopupfilter.getdataprovider-string) ⇒ `String`
  * [.getID()](api-svypopupfilter.md#abstractpopupfilter.getid-string) ⇒ `String`
  * [.getOperator()](api-svypopupfilter.md#abstractpopupfilter.getoperator-string) ⇒ `String`
  * [.getParams()](api-svypopupfilter.md#abstractpopupfilter.getparams-array) ⇒ `Array`
  * [.getState()](api-svypopupfilter.md#abstractpopupfilter.getstate-object) ⇒ `Object`
  * [.getText()](api-svypopupfilter.md#abstractpopupfilter.gettext-string) ⇒ `String`
  * [.getValues()](api-svypopupfilter.md#abstractpopupfilter.getvalues-array) ⇒ `Array`
  * [.removeParam(index)](api-svypopupfilter.md#abstractpopupfilter.removeparam-index)
  * [.restoreState(jsonState)](api-svypopupfilter.md#abstractpopupfilter.restorestate-jsonstate-abstractpopupfilter) ⇒ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)
  * [.setDataProvider(dataProvider)](api-svypopupfilter.md#abstractpopupfilter.setdataprovider-dataprovider)
  * [.setOperator(operator)](api-svypopupfilter.md#abstractpopupfilter.setoperator-operator)
  * [.setRendererForm(popupFilterForm)](api-svypopupfilter.md#abstractpopupfilter.setrendererform-popupfilterform)
  * [.setText(text)](api-svypopupfilter.md#abstractpopupfilter.settext-text)
  * [.setValues(values)](api-svypopupfilter.md#abstractpopupfilter.setvalues-values)
  * [.showModalWindow(\[callback\], \[x\], \[y\], \[width\], \[height\])](api-svypopupfilter.md#abstractpopupfilter.showmodalwindow-callback-x-y-width-height-array.less-than-jsrecord-greater-than) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`
  * [.showPopUp(callback, target, \[width\], \[height\])](api-svypopupfilter.md#abstractpopupfilter.showpopup-callback-target-width-height)
  * [.showWindow(win, \[callback\])](api-svypopupfilter.md#abstractpopupfilter.showwindow-win-callback-array-.less-than-string-or-date-or-number-greater-than) ⇒ `[ 'Array' ].<(String|Date|Number)>`

#### abstractPopupFilter.addParam(param)

Add a params to be added into the onSelect callback arguments

| Param | Type     |
| ----- | -------- |
| param | `Object` |

#### abstractPopupFilter.clearParams()

Clear the params

#### abstractPopupFilter.createPopUp(callback) ⇒ `plugins.window.FormPopup`

Creates and returns the popupFilter

| Param    | Type       | Description                                                                                                                             |
| -------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| callback | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |

#### abstractPopupFilter.createWindow(\[x], \[y], \[width], \[height], \[jsWindowType]) ⇒ `JSWindow`

**Returns**: `JSWindow` - returns a JSWindow which can be used to show the popupFilter in it using popupFilter.showWindow(window)

| Param           | Type     | Description                                                                     |
| --------------- | -------- | ------------------------------------------------------------------------------- |
| \[x]            | `Number` |                                                                                 |
| \[y]            | `Number` |                                                                                 |
| \[width]        | `Number` | The width of the pop-up. Optional. Default is component width                   |
| \[height]       | `Number` | The height of the pop-up. Optional. Default is form height.                     |
| \[jsWindowType] | `Number` | Type of window; should be an option of JSWindow, Default JSWindow.MODAL\_DIALOG |

#### abstractPopupFilter.getDataProvider() ⇒ `String`

Gets the popupFilter dataprovider

#### abstractPopupFilter.getID() ⇒ `String`

Gets the filter name

#### abstractPopupFilter.getOperator() ⇒ `String`

#### abstractPopupFilter.getParams() ⇒ `Array`

#### abstractPopupFilter.getState() ⇒ `Object`

#### abstractPopupFilter.getText() ⇒ `String`

Gets the popupFilter text

#### abstractPopupFilter.getValues() ⇒ `Array`

#### abstractPopupFilter.removeParam(index)

Removes a param at the specified index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### abstractPopupFilter.restoreState(jsonState) ⇒ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

| Param     | Type     |
| --------- | -------- |
| jsonState | `Object` |

#### abstractPopupFilter.setDataProvider(dataProvider)

Sets the popupFilter dataprovider

| Param        | Type     |
| ------------ | -------- |
| dataProvider | `String` |

#### abstractPopupFilter.setOperator(operator)

| Param    | Type     | Description                                 |
| -------- | -------- | ------------------------------------------- |
| operator | `String` | a value from scopes.svyPopupFilter.OPERATOR |

#### abstractPopupFilter.setRendererForm(popupFilterForm)

| Param           | Type                                                                                                               |
| --------------- | ------------------------------------------------------------------------------------------------------------------ |
| popupFilterForm | [`RuntimeForm.<AbstractPopupFilter>`](api-svypopupfilter.md#abstractpopupfilter) \| `RuntimeForm.<AbstractLookup>` |

#### abstractPopupFilter.setText(text)

Sets the popupFilter text

| Param | Type     |
| ----- | -------- |
| text  | `String` |

#### abstractPopupFilter.setValues(values)

| Param  | Type    |
| ------ | ------- |
| values | `Array` |

#### abstractPopupFilter.showModalWindow(\[callback], \[x], \[y], \[width], \[height]) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`

Shows the popupFilter in a modal Window

**Returns**: `Array.<JSRecord>` | `Array.<(String|Date|Number)>` - returns the selected records; if the popupFilterDataprovider has been set instead it returns the popupFilterDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection

| Param       | Type       | Description                                                                                                                             |
| ----------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| \[callback] | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| \[x]        | `Number`   |                                                                                                                                         |
| \[y]        | `Number`   |                                                                                                                                         |
| \[width]    | `Number`   | The width of the popupFilter. Optional. Default is same as target component                                                             |
| \[height]   | `Number`   | The height of the popupFilter. Optional. Default is implementation-specifc.                                                             |

#### abstractPopupFilter.showPopUp(callback, target, \[width], \[height])

Shows the popupFilter

| Param     | Type               | Description                                                                                                                             |
| --------- | ------------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| callback  | `function`         | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| target    | `RuntimeComponent` | The component to show relative to                                                                                                       |
| \[width]  | `Number`           | The width of the popupFilter. Optional. Default is same as target component                                                             |
| \[height] | `Number`           | The height of the popupFilter. Optional. Default is implementation-specifc.                                                             |

#### abstractPopupFilter.showWindow(win, \[callback]) ⇒ `[ 'Array' ].<(String|Date|Number)>`

Shows the popupFilter in a Window

**Returns**: `[ 'Array' ].<(String|Date|Number)>` - returns the selected records; if the popupFilterDataprovider has been set instead it returns the popupFilterDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection

| Param       | Type       | Description                                                                                                                             |
| ----------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| win         | `JSWindow` | the JSWindow object to show                                                                                                             |
| \[callback] | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |

### SvyCheckFilter ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

**Extends**: [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

* [SvyCheckFilter](api-svypopupfilter.md#svycheckfilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)
  * [.addParam(param)](api-svypopupfilter.md#svycheckfilter.addparam-param)
  * [.clearParams()](api-svypopupfilter.md#svycheckfilter.clearparams)
  * [.createPopUp(callback)](api-svypopupfilter.md#svycheckfilter.createpopup-callback-plugins.window.formpopup) ⇒ `plugins.window.FormPopup`
  * [.createWindow(\[x\], \[y\], \[width\], \[height\], \[jsWindowType\])](api-svypopupfilter.md#svycheckfilter.createwindow-x-y-width-height-jswindowtype-jswindow) ⇒ `JSWindow`
  * [.getDataProvider()](api-svypopupfilter.md#svycheckfilter.getdataprovider-string) ⇒ `String`
  * [.getID()](api-svypopupfilter.md#svycheckfilter.getid-string) ⇒ `String`
  * [.getOperator()](api-svypopupfilter.md#svycheckfilter.getoperator-string) ⇒ `String`
  * [.getParams()](api-svypopupfilter.md#svycheckfilter.getparams-array) ⇒ `Array`
  * [.getState()](api-svypopupfilter.md#svycheckfilter.getstate-object) ⇒ `Object`
  * [.getText()](api-svypopupfilter.md#svycheckfilter.gettext-string) ⇒ `String`
  * [.getValues()](api-svypopupfilter.md#svycheckfilter.getvalues-array) ⇒ `Array`
  * [.removeParam(index)](api-svypopupfilter.md#svycheckfilter.removeparam-index)
  * [.restoreState(jsonState)](api-svypopupfilter.md#svycheckfilter.restorestate-jsonstate-abstractpopupfilter) ⇒ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)
  * [.setDataProvider(dataProvider)](api-svypopupfilter.md#svycheckfilter.setdataprovider-dataprovider)
  * [.setOperator(operator)](api-svypopupfilter.md#svycheckfilter.setoperator-operator)
  * [.setRendererForm(popupFilterForm)](api-svypopupfilter.md#svycheckfilter.setrendererform-popupfilterform)
  * [.setText(text)](api-svypopupfilter.md#svycheckfilter.settext-text)
  * [.setValues(values)](api-svypopupfilter.md#svycheckfilter.setvalues-values)
  * [.showModalWindow(\[callback\], \[x\], \[y\], \[width\], \[height\])](api-svypopupfilter.md#svycheckfilter.showmodalwindow-callback-x-y-width-height-array.less-than-jsrecord-greater-than-or-ar) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`
  * [.showPopUp(callback, target, \[width\], \[height\])](api-svypopupfilter.md#svycheckfilter.showpopup-callback-target-width-height)
  * [.showWindow(win, \[callback\])](api-svypopupfilter.md#svycheckfilter.showwindow-win-callback-array-.less-than-string-or-date-or-number-greater-than) ⇒ `[ 'Array' ].<(String|Date|Number)>`

#### svyCheckFilter.addParam(param)

Add a params to be added into the onSelect callback arguments

| Param | Type     |
| ----- | -------- |
| param | `Object` |

#### svyCheckFilter.clearParams()

Clear the params

#### svyCheckFilter.createPopUp(callback) ⇒ `plugins.window.FormPopup`

Creates and returns the popupFilter

| Param    | Type       | Description                                                                                                                             |
| -------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| callback | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |

#### svyCheckFilter.createWindow(\[x], \[y], \[width], \[height], \[jsWindowType]) ⇒ `JSWindow`

**Returns**: `JSWindow` - returns a JSWindow which can be used to show the popupFilter in it using popupFilter.showWindow(window)

| Param           | Type     | Description                                                                     |
| --------------- | -------- | ------------------------------------------------------------------------------- |
| \[x]            | `Number` |                                                                                 |
| \[y]            | `Number` |                                                                                 |
| \[width]        | `Number` | The width of the pop-up. Optional. Default is component width                   |
| \[height]       | `Number` | The height of the pop-up. Optional. Default is form height.                     |
| \[jsWindowType] | `Number` | Type of window; should be an option of JSWindow, Default JSWindow.MODAL\_DIALOG |

#### svyCheckFilter.getDataProvider() ⇒ `String`

Gets the popupFilter dataprovider

#### svyCheckFilter.getID() ⇒ `String`

Gets the filter name

#### svyCheckFilter.getOperator() ⇒ `String`

#### svyCheckFilter.getParams() ⇒ `Array`

#### svyCheckFilter.getState() ⇒ `Object`

#### svyCheckFilter.getText() ⇒ `String`

Gets the popupFilter text

#### svyCheckFilter.getValues() ⇒ `Array`

#### svyCheckFilter.removeParam(index)

Removes a param at the specified index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### svyCheckFilter.restoreState(jsonState) ⇒ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

| Param     | Type     |
| --------- | -------- |
| jsonState | `Object` |

#### svyCheckFilter.setDataProvider(dataProvider)

Sets the popupFilter dataprovider

| Param        | Type     |
| ------------ | -------- |
| dataProvider | `String` |

#### svyCheckFilter.setOperator(operator)

| Param    | Type     | Description                                 |
| -------- | -------- | ------------------------------------------- |
| operator | `String` | a value from scopes.svyPopupFilter.OPERATOR |

#### svyCheckFilter.setRendererForm(popupFilterForm)

| Param           | Type                                                                                                               |
| --------------- | ------------------------------------------------------------------------------------------------------------------ |
| popupFilterForm | [`RuntimeForm.<AbstractPopupFilter>`](api-svypopupfilter.md#abstractpopupfilter) \| `RuntimeForm.<AbstractLookup>` |

#### svyCheckFilter.setText(text)

Sets the popupFilter text

| Param | Type     |
| ----- | -------- |
| text  | `String` |

#### svyCheckFilter.setValues(values)

| Param  | Type    |
| ------ | ------- |
| values | `Array` |

#### svyCheckFilter.showModalWindow(\[callback], \[x], \[y], \[width], \[height]) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`

Shows the popupFilter in a modal Window

**Returns**: `Array.<JSRecord>` | `Array.<(String|Date|Number)>` - returns the selected records; if the popupFilterDataprovider has been set instead it returns the popupFilterDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection

| Param       | Type       | Description                                                                                                                             |
| ----------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| \[callback] | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| \[x]        | `Number`   |                                                                                                                                         |
| \[y]        | `Number`   |                                                                                                                                         |
| \[width]    | `Number`   | The width of the popupFilter. Optional. Default is same as target component                                                             |
| \[height]   | `Number`   | The height of the popupFilter. Optional. Default is implementation-specifc.                                                             |

#### svyCheckFilter.showPopUp(callback, target, \[width], \[height])

Shows the popupFilter

| Param     | Type               | Description                                                                                                                             |
| --------- | ------------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| callback  | `function`         | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| target    | `RuntimeComponent` | The component to show relative to                                                                                                       |
| \[width]  | `Number`           | The width of the popupFilter. Optional. Default is same as target component                                                             |
| \[height] | `Number`           | The height of the popupFilter. Optional. Default is implementation-specifc.                                                             |

#### svyCheckFilter.showWindow(win, \[callback]) ⇒ `[ 'Array' ].<(String|Date|Number)>`

Shows the popupFilter in a Window

**Returns**: `[ 'Array' ].<(String|Date|Number)>` - returns the selected records; if the popupFilterDataprovider has been set instead it returns the popupFilterDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection

| Param       | Type       | Description                                                                                                                             |
| ----------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| win         | `JSWindow` | the JSWindow object to show                                                                                                             |
| \[callback] | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |

***

### SvyDateFilter ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

**Extends**: [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

* [SvyDateFilter](api-svypopupfilter.md#svydatefilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)
  * [.addParam(param)](api-svypopupfilter.md#svydatefilter.addparam-param)
  * [.clearParams()](api-svypopupfilter.md#svydatefilter.clearparams)
  * [.createPopUp(callback)](api-svypopupfilter.md#svydatefilter.createpopup-callback-plugins.window.formpopup) ⇒ `plugins.window.FormPopup`
  * [.createWindow(\[x\], \[y\], \[width\], \[height\], \[jsWindowType\])](api-svypopupfilter.md#svydatefilter.createwindow-x-y-width-height-jswindowtype-jswindow) ⇒ `JSWindow`
  * [.getDataProvider()](api-svypopupfilter.md#svydatefilter.getdataprovider-string) ⇒ `String`
  * [.getID()](api-svypopupfilter.md#svydatefilter.getid-string) ⇒ `String`
  * [.getOperator()](api-svypopupfilter.md#svydatefilter.getoperator-string) ⇒ `String`
  * [.getParams()](api-svypopupfilter.md#svydatefilter.getparams-array) ⇒ `Array`
  * [.getState()](api-svypopupfilter.md#svydatefilter.getstate-object) ⇒ `Object`
  * [.getText()](api-svypopupfilter.md#svydatefilter.gettext-string) ⇒ `String`
  * [.getValues()](api-svypopupfilter.md#svydatefilter.getvalues-array) ⇒ `Array`
  * [.removeParam(index)](api-svypopupfilter.md#svydatefilter.removeparam-index)
  * [.restoreState(jsonState)](api-svypopupfilter.md#svydatefilter.restorestate-jsonstate-abstractpopupfilter) ⇒ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)
  * [.setDataProvider(dataProvider)](api-svypopupfilter.md#svydatefilter.setdataprovider-dataprovider)
  * [.setOperator(operator)](api-svypopupfilter.md#svydatefilter.setoperator-operator)
  * [.setRendererForm(popupFilterForm)](api-svypopupfilter.md#svydatefilter.setrendererform-popupfilterform)
  * [.setText(text)](api-svypopupfilter.md#svydatefilter.settext-text)
  * [.setValues(values)](api-svypopupfilter.md#svydatefilter.setvalues-values)
  * [.showModalWindow(\[callback\], \[x\], \[y\], \[width\], \[height\])](api-svypopupfilter.md#svydatefilter.showmodalwindow-callback-x-y-width-height-array.less-than-jsrecord-greater-than-or-arr) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`
  * [.showPopUp(callback, target, \[width\], \[height\])](api-svypopupfilter.md#svydatefilter.showpopup-callback-target-width-height)
  * [.showWindow(win, \[callback\])](api-svypopupfilter.md#svydatefilter.showwindow-win-callback-array-.less-than-string-or-date-or-number-greater-than) ⇒ `[ 'Array' ].<(String|Date|Number)>`

#### svyDateFilter.addParam(param)

Add a params to be added into the onSelect callback arguments

| Param | Type     |
| ----- | -------- |
| param | `Object` |

#### svyDateFilter.clearParams()

Clear the params

#### svyDateFilter.createPopUp(callback) ⇒ `plugins.window.FormPopup`

Creates and returns the popupFilter

| Param    | Type       | Description                                                                                                                             |
| -------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| callback | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |

#### svyDateFilter.createWindow(\[x], \[y], \[width], \[height], \[jsWindowType]) ⇒ `JSWindow`

**Returns**: `JSWindow` - returns a JSWindow which can be used to show the popupFilter in it using popupFilter.showWindow(window)

| Param           | Type     | Description                                                                     |
| --------------- | -------- | ------------------------------------------------------------------------------- |
| \[x]            | `Number` |                                                                                 |
| \[y]            | `Number` |                                                                                 |
| \[width]        | `Number` | The width of the pop-up. Optional. Default is component width                   |
| \[height]       | `Number` | The height of the pop-up. Optional. Default is form height.                     |
| \[jsWindowType] | `Number` | Type of window; should be an option of JSWindow, Default JSWindow.MODAL\_DIALOG |

#### svyDateFilter.getDataProvider() ⇒ `String`

Gets the popupFilter dataprovider

#### svyDateFilter.getID() ⇒ `String`

Gets the filter name

#### svyDateFilter.getOperator() ⇒ `String`

#### svyDateFilter.getParams() ⇒ `Array`

#### svyDateFilter.getState() ⇒ `Object`

#### svyDateFilter.getText() ⇒ `String`

Gets the popupFilter text

#### svyDateFilter.getValues() ⇒ `Array`

#### svyDateFilter.removeParam(index)

Removes a param at the specified index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### svyDateFilter.restoreState(jsonState) ⇒ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

| Param     | Type     |
| --------- | -------- |
| jsonState | `Object` |

#### svyDateFilter.setDataProvider(dataProvider)

Sets the popupFilter dataprovider

| Param        | Type     |
| ------------ | -------- |
| dataProvider | `String` |

#### svyDateFilter.setOperator(operator)

| Param    | Type     | Description                                 |
| -------- | -------- | ------------------------------------------- |
| operator | `String` | a value from scopes.svyPopupFilter.OPERATOR |

#### svyDateFilter.setRendererForm(popupFilterForm)

| Param           | Type                                                                                                               |
| --------------- | ------------------------------------------------------------------------------------------------------------------ |
| popupFilterForm | [`RuntimeForm.<AbstractPopupFilter>`](api-svypopupfilter.md#abstractpopupfilter) \| `RuntimeForm.<AbstractLookup>` |

#### svyDateFilter.setText(text)

Sets the popupFilter text

| Param | Type     |
| ----- | -------- |
| text  | `String` |

#### svyDateFilter.setValues(values)

| Param  | Type    |
| ------ | ------- |
| values | `Array` |

#### svyDateFilter.showModalWindow(\[callback], \[x], \[y], \[width], \[height]) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`

Shows the popupFilter in a modal Window

**Returns**: `Array.<JSRecord>` | `Array.<(String|Date|Number)>` - returns the selected records; if the popupFilterDataprovider has been set instead it returns the popupFilterDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection

| Param       | Type       | Description                                                                                                                             |
| ----------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| \[callback] | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| \[x]        | `Number`   |                                                                                                                                         |
| \[y]        | `Number`   |                                                                                                                                         |
| \[width]    | `Number`   | The width of the popupFilter. Optional. Default is same as target component                                                             |
| \[height]   | `Number`   | The height of the popupFilter. Optional. Default is implementation-specifc.                                                             |

#### svyDateFilter.showPopUp(callback, target, \[width], \[height])

Shows the popupFilter

| Param     | Type               | Description                                                                                                                             |
| --------- | ------------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| callback  | `function`         | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| target    | `RuntimeComponent` | The component to show relative to                                                                                                       |
| \[width]  | `Number`           | The width of the popupFilter. Optional. Default is same as target component                                                             |
| \[height] | `Number`           | The height of the popupFilter. Optional. Default is implementation-specifc.                                                             |

#### svyDateFilter.showWindow(win, \[callback]) ⇒ `[ 'Array' ].<(String|Date|Number)>`

Shows the popupFilter in a Window

**Returns**: `[ 'Array' ].<(String|Date|Number)>` - returns the selected records; if the popupFilterDataprovider has been set instead it returns the popupFilterDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection

| Param       | Type       | Description                                                                                                                             |
| ----------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| win         | `JSWindow` | the JSWindow object to show                                                                                                             |
| \[callback] | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |

### SvyIntegerFilter ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

**Extends**: [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

* [SvyIntegerFilter](api-svypopupfilter.md#svyintegerfilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)
  * [.addParam(param)](api-svypopupfilter.md#svyintegerfilter.addparam-param)
  * [.clearParams()](api-svypopupfilter.md#svyintegerfilter.clearparams)
  * [.createPopUp(callback)](api-svypopupfilter.md#svyintegerfilter.createpopup-callback-plugins.window.formpopup) ⇒ `plugins.window.FormPopup`
  * [.createWindow(\[x\], \[y\], \[width\], \[height\], \[jsWindowType\])](api-svypopupfilter.md#svyintegerfilter.createwindow-x-y-width-height-jswindowtype-jswindow) ⇒ `JSWindow`
  * [.getDataProvider()](api-svypopupfilter.md#svyintegerfilter.getdataprovider-string) ⇒ `String`
  * [.getID()](api-svypopupfilter.md#svyintegerfilter.getid-string) ⇒ `String`
  * [.getOperator()](api-svypopupfilter.md#svyintegerfilter.getoperator-string) ⇒ `String`
  * [.getParams()](api-svypopupfilter.md#svyintegerfilter.getparams-array) ⇒ `Array`
  * [.getState()](api-svypopupfilter.md#svyintegerfilter.getstate-object) ⇒ `Object`
  * [.getText()](api-svypopupfilter.md#svyintegerfilter.gettext-string) ⇒ `String`
  * [.getValues()](api-svypopupfilter.md#svyintegerfilter.getvalues-array) ⇒ `Array`
  * [.removeParam(index)](api-svypopupfilter.md#svyintegerfilter.removeparam-index)
  * [.restoreState(jsonState)](api-svypopupfilter.md#svyintegerfilter.restorestate-jsonstate-abstractpopupfilter) ⇒ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)
  * [.setDataProvider(dataProvider)](api-svypopupfilter.md#svyintegerfilter.setdataprovider-dataprovider)
  * [.setOperator(operator)](api-svypopupfilter.md#svyintegerfilter.setoperator-operator)
  * [.setRendererForm(popupFilterForm)](api-svypopupfilter.md#svyintegerfilter.setrendererform-popupfilterform)
  * [.setText(text)](api-svypopupfilter.md#svyintegerfilter.settext-text)
  * [.setValues(values)](api-svypopupfilter.md#svyintegerfilter.setvalues-values)
  * [.showModalWindow(\[callback\], \[x\], \[y\], \[width\], \[height\])](api-svypopupfilter.md#svyintegerfilter.showmodalwindow-callback-x-y-width-height-array.less-than-jsrecord-greater-than-or) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`
  * [.showPopUp(callback, target, \[width\], \[height\])](api-svypopupfilter.md#svyintegerfilter.showpopup-callback-target-width-height)
  * [.showWindow(win, \[callback\])](api-svypopupfilter.md#svyintegerfilter.showwindow-win-callback-array-.less-than-string-or-date-or-number-greater-than) ⇒ `[ 'Array' ].<(String|Date|Number)>`

#### svyIntegerFilter.addParam(param)

Add a params to be added into the onSelect callback arguments

| Param | Type     |
| ----- | -------- |
| param | `Object` |

#### svyIntegerFilter.clearParams()

Clear the params

#### svyIntegerFilter.createPopUp(callback) ⇒ `plugins.window.FormPopup`

Creates and returns the popupFilter

| Param    | Type       | Description                                                                                                                             |
| -------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| callback | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |

#### svyIntegerFilter.createWindow(\[x], \[y], \[width], \[height], \[jsWindowType]) ⇒ `JSWindow`

**Returns**: `JSWindow` - returns a JSWindow which can be used to show the popupFilter in it using popupFilter.showWindow(window)

| Param           | Type     | Description                                                                     |
| --------------- | -------- | ------------------------------------------------------------------------------- |
| \[x]            | `Number` |                                                                                 |
| \[y]            | `Number` |                                                                                 |
| \[width]        | `Number` | The width of the pop-up. Optional. Default is component width                   |
| \[height]       | `Number` | The height of the pop-up. Optional. Default is form height.                     |
| \[jsWindowType] | `Number` | Type of window; should be an option of JSWindow, Default JSWindow.MODAL\_DIALOG |

#### svyIntegerFilter.getDataProvider() ⇒ `String`

Gets the popupFilter dataprovider

#### svyIntegerFilter.getID() ⇒ `String`

Gets the filter name

#### svyIntegerFilter.getOperator() ⇒ `String`

#### svyIntegerFilter.getParams() ⇒ `Array`

#### svyIntegerFilter.getState() ⇒ `Object`

#### svyIntegerFilter.getText() ⇒ `String`

Gets the popupFilter text

#### svyIntegerFilter.getValues() ⇒ `Array`

#### svyIntegerFilter.removeParam(index)

Removes a param at the specified index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### svyIntegerFilter.restoreState(jsonState) ⇒ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

| Param     | Type     |
| --------- | -------- |
| jsonState | `Object` |

#### svyIntegerFilter.setDataProvider(dataProvider)

Sets the popupFilter dataprovider

| Param        | Type     |
| ------------ | -------- |
| dataProvider | `String` |

#### svyIntegerFilter.setOperator(operator)

| Param    | Type     | Description                                 |
| -------- | -------- | ------------------------------------------- |
| operator | `String` | a value from scopes.svyPopupFilter.OPERATOR |

#### svyIntegerFilter.setRendererForm(popupFilterForm)

| Param           | Type                                                                                                               |
| --------------- | ------------------------------------------------------------------------------------------------------------------ |
| popupFilterForm | [`RuntimeForm.<AbstractPopupFilter>`](api-svypopupfilter.md#abstractpopupfilter) \| `RuntimeForm.<AbstractLookup>` |

#### svyIntegerFilter.setText(text)

Sets the popupFilter text

| Param | Type     |
| ----- | -------- |
| text  | `String` |

#### svyIntegerFilter.setValues(values)

| Param  | Type    |
| ------ | ------- |
| values | `Array` |

#### svyIntegerFilter.showModalWindow(\[callback], \[x], \[y], \[width], \[height]) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`

Shows the popupFilter in a modal Window

**Returns**: `Array.<JSRecord>` | `Array.<(String|Date|Number)>` - returns the selected records; if the popupFilterDataprovider has been set instead it returns the popupFilterDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection

| Param       | Type       | Description                                                                                                                             |
| ----------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| \[callback] | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| \[x]        | `Number`   |                                                                                                                                         |
| \[y]        | `Number`   |                                                                                                                                         |
| \[width]    | `Number`   | The width of the popupFilter. Optional. Default is same as target component                                                             |
| \[height]   | `Number`   | The height of the popupFilter. Optional. Default is implementation-specifc.                                                             |

#### svyIntegerFilter.showPopUp(callback, target, \[width], \[height])

Shows the popupFilter

| Param     | Type               | Description                                                                                                                             |
| --------- | ------------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| callback  | `function`         | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| target    | `RuntimeComponent` | The component to show relative to                                                                                                       |
| \[width]  | `Number`           | The width of the popupFilter. Optional. Default is same as target component                                                             |
| \[height] | `Number`           | The height of the popupFilter. Optional. Default is implementation-specifc.                                                             |

#### svyIntegerFilter.showWindow(win, \[callback]) ⇒ `[ 'Array' ].<(String|Date|Number)>`

Shows the popupFilter in a Window

**Returns**: `[ 'Array' ].<(String|Date|Number)>` - returns the selected records; if the popupFilterDataprovider has been set instead it returns the popupFilterDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection

| Param       | Type       | Description                                                                                                                             |
| ----------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| win         | `JSWindow` | the JSWindow object to show                                                                                                             |
| \[callback] | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |

### SvyNumberFilter ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

**Extends**: [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

* [SvyNumberFilter](api-svypopupfilter.md#svynumberfilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)
  * [.addParam(param)](api-svypopupfilter.md#svynumberfilter.addparam-param)
  * [.clearParams()](api-svypopupfilter.md#svynumberfilter.clearparams)
  * [.createPopUp(callback)](api-svypopupfilter.md#svynumberfilter.createpopup-callback-plugins.window.formpopup) ⇒ `plugins.window.FormPopup`
  * [.createWindow(\[x\], \[y\], \[width\], \[height\], \[jsWindowType\])](api-svypopupfilter.md#svynumberfilter.createwindow-x-y-width-height-jswindowtype-jswindow) ⇒ `JSWindow`
  * [.getDataProvider()](api-svypopupfilter.md#svynumberfilter.getdataprovider-string) ⇒ `String`
  * [.getID()](api-svypopupfilter.md#svynumberfilter.getid-string) ⇒ `String`
  * [.getOperator()](api-svypopupfilter.md#svynumberfilter.getoperator-string) ⇒ `String`
  * [.getParams()](api-svypopupfilter.md#svynumberfilter.getparams-array) ⇒ `Array`
  * [.getState()](api-svypopupfilter.md#svynumberfilter.getstate-object) ⇒ `Object`
  * [.getText()](api-svypopupfilter.md#svynumberfilter.gettext-string) ⇒ `String`
  * [.getValues()](api-svypopupfilter.md#svynumberfilter.getvalues-array) ⇒ `Array`
  * [.removeParam(index)](api-svypopupfilter.md#svynumberfilter.removeparam-index)
  * [.restoreState(jsonState)](api-svypopupfilter.md#svynumberfilter.restorestate-jsonstate-abstractpopupfilter) ⇒ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)
  * [.setDataProvider(dataProvider)](api-svypopupfilter.md#svynumberfilter.setdataprovider-dataprovider)
  * [.setOperator(operator)](api-svypopupfilter.md#svynumberfilter.setoperator-operator)
  * [.setRendererForm(popupFilterForm)](api-svypopupfilter.md#svynumberfilter.setrendererform-popupfilterform)
  * [.setText(text)](api-svypopupfilter.md#svynumberfilter.settext-text)
  * [.setValues(values)](api-svypopupfilter.md#svynumberfilter.setvalues-values)
  * [.showModalWindow(\[callback\], \[x\], \[y\], \[width\], \[height\])](api-svypopupfilter.md#svynumberfilter.showmodalwindow-callback-x-y-width-height-array.less-than-jsrecord-greater-than-or-a) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`
  * [.showPopUp(callback, target, \[width\], \[height\])](api-svypopupfilter.md#svynumberfilter.showpopup-callback-target-width-height)
  * [.showWindow(win, \[callback\])](api-svypopupfilter.md#svynumberfilter.showwindow-win-callback-array-.less-than-string-or-date-or-number-greater-than) ⇒ `[ 'Array' ].<(String|Date|Number)>`

#### svyNumberFilter.addParam(param)

Add a params to be added into the onSelect callback arguments

| Param | Type     |
| ----- | -------- |
| param | `Object` |

#### svyNumberFilter.clearParams()

Clear the params

#### svyNumberFilter.createPopUp(callback) ⇒ `plugins.window.FormPopup`

Creates and returns the popupFilter

| Param    | Type       | Description                                                                                                                             |
| -------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| callback | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |

#### svyNumberFilter.createWindow(\[x], \[y], \[width], \[height], \[jsWindowType]) ⇒ `JSWindow`

**Returns**: `JSWindow` - returns a JSWindow which can be used to show the popupFilter in it using popupFilter.showWindow(window)

| Param           | Type     | Description                                                                     |
| --------------- | -------- | ------------------------------------------------------------------------------- |
| \[x]            | `Number` |                                                                                 |
| \[y]            | `Number` |                                                                                 |
| \[width]        | `Number` | The width of the pop-up. Optional. Default is component width                   |
| \[height]       | `Number` | The height of the pop-up. Optional. Default is form height.                     |
| \[jsWindowType] | `Number` | Type of window; should be an option of JSWindow, Default JSWindow.MODAL\_DIALOG |

#### svyNumberFilter.getDataProvider() ⇒ `String`

Gets the popupFilter dataprovider

#### svyNumberFilter.getID() ⇒ `String`

Gets the filter name

#### svyNumberFilter.getOperator() ⇒ `String`

#### svyNumberFilter.getParams() ⇒ `Array`

#### svyNumberFilter.getState() ⇒ `Object`

#### svyNumberFilter.getText() ⇒ `String`

Gets the popupFilter text

#### svyNumberFilter.getValues() ⇒ `Array`

#### svyNumberFilter.removeParam(index)

Removes a param at the specified index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### svyNumberFilter.restoreState(jsonState) ⇒ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

| Param     | Type     |
| --------- | -------- |
| jsonState | `Object` |

#### svyNumberFilter.setDataProvider(dataProvider)

Sets the popupFilter dataprovider

| Param        | Type     |
| ------------ | -------- |
| dataProvider | `String` |

#### svyNumberFilter.setOperator(operator)

| Param    | Type     | Description                                 |
| -------- | -------- | ------------------------------------------- |
| operator | `String` | a value from scopes.svyPopupFilter.OPERATOR |

#### svyNumberFilter.setRendererForm(popupFilterForm)

| Param           | Type                                                                                                               |
| --------------- | ------------------------------------------------------------------------------------------------------------------ |
| popupFilterForm | [`RuntimeForm.<AbstractPopupFilter>`](api-svypopupfilter.md#abstractpopupfilter) \| `RuntimeForm.<AbstractLookup>` |

#### svyNumberFilter.setText(text)

Sets the popupFilter text

| Param | Type     |
| ----- | -------- |
| text  | `String` |

#### svyNumberFilter.setValues(values)

| Param  | Type    |
| ------ | ------- |
| values | `Array` |

#### svyNumberFilter.showModalWindow(\[callback], \[x], \[y], \[width], \[height]) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`

Shows the popupFilter in a modal Window

**Returns**: `Array.<JSRecord>` | `Array.<(String|Date|Number)>` - returns the selected records; if the popupFilterDataprovider has been set instead it returns the popupFilterDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection

| Param       | Type       | Description                                                                                                                             |
| ----------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| \[callback] | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| \[x]        | `Number`   |                                                                                                                                         |
| \[y]        | `Number`   |                                                                                                                                         |
| \[width]    | `Number`   | The width of the popupFilter. Optional. Default is same as target component                                                             |
| \[height]   | `Number`   | The height of the popupFilter. Optional. Default is implementation-specifc.                                                             |

#### svyNumberFilter.showPopUp(callback, target, \[width], \[height])

Shows the popupFilter

| Param     | Type               | Description                                                                                                                             |
| --------- | ------------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| callback  | `function`         | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| target    | `RuntimeComponent` | The component to show relative to                                                                                                       |
| \[width]  | `Number`           | The width of the popupFilter. Optional. Default is same as target component                                                             |
| \[height] | `Number`           | The height of the popupFilter. Optional. Default is implementation-specifc.                                                             |

#### svyNumberFilter.showWindow(win, \[callback]) ⇒ `[ 'Array' ].<(String|Date|Number)>`

Shows the popupFilter in a Window

**Returns**: `[ 'Array' ].<(String|Date|Number)>` - returns the selected records; if the popupFilterDataprovider has been set instead it returns the popupFilterDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection

| Param       | Type       | Description                                                                                                                             |
| ----------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| win         | `JSWindow` | the JSWindow object to show                                                                                                             |
| \[callback] | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |

***

### SvySelectFilter ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

**Extends**: [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

* [SvySelectFilter](api-svypopupfilter.md#svyselectfilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)
  * [.addParam(param)](api-svypopupfilter.md#svyselectfilter.addparam-param)
  * [.clearParams()](api-svypopupfilter.md#svyselectfilter.clearparams)
  * [.createPopUp(callback)](api-svypopupfilter.md#svyselectfilter.createpopup-callback-plugins.window.formpopup) ⇒ `plugins.window.FormPopup`
  * [.createWindow(\[x\], \[y\], \[width\], \[height\], \[jsWindowType\])](api-svypopupfilter.md#svyselectfilter.createwindow-x-y-width-height-jswindowtype-jswindow) ⇒ `JSWindow`
  * [.getDataProvider()](api-svypopupfilter.md#svyselectfilter.getdataprovider-string) ⇒ `String`
  * [.getID()](api-svypopupfilter.md#svyselectfilter.getid-string) ⇒ `String`
  * [.getLookup()](api-svypopupfilter.md#svyselectfilter.getlookup-scopes.svylookup.lookup) ⇒ `scopes.svyLookup.Lookup`
  * [.getOperator()](api-svypopupfilter.md#svyselectfilter.getoperator-string) ⇒ `String`
  * [.getParams()](api-svypopupfilter.md#svyselectfilter.getparams-array) ⇒ `Array`
  * [.getState()](api-svypopupfilter.md#svyselectfilter.getstate-object) ⇒ `Object`
  * [.getText()](api-svypopupfilter.md#svyselectfilter.gettext-string) ⇒ `String`
  * [.getValues()](api-svypopupfilter.md#svyselectfilter.getvalues-array) ⇒ `Array`
  * [.removeParam(index)](api-svypopupfilter.md#svyselectfilter.removeparam-index)
  * [.restoreState(jsonState)](api-svypopupfilter.md#svyselectfilter.restorestate-jsonstate-abstractpopupfilter) ⇒ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)
  * [.setDataProvider(dataProvider)](api-svypopupfilter.md#svyselectfilter.setdataprovider-dataprovider)
  * [.setOperator(operator)](api-svypopupfilter.md#svyselectfilter.setoperator-operator)
  * [.setRendererForm(popupFilterForm)](api-svypopupfilter.md#svyselectfilter.setrendererform-popupfilterform)
  * [.setText(text)](api-svypopupfilter.md#svyselectfilter.settext-text)
  * [.setValues(values)](api-svypopupfilter.md#svyselectfilter.setvalues-values)
  * [.showModalWindow(\[callback\], \[x\], \[y\], \[width\], \[height\])](api-svypopupfilter.md#svyselectfilter.showmodalwindow-callback-x-y-width-height-array.less-than-jsrecord-greater-than-or-a) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`
  * [.showPopUp(callback, target, \[width\], \[height\])](api-svypopupfilter.md#svyselectfilter.showpopup-callback-target-width-height)
  * [.showWindow(win, \[callback\])](api-svypopupfilter.md#svyselectfilter.showwindow-win-callback-array.less-than-jsrecord-greater-than-or-array.less-than-str) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`
  * [new SvySelectFilter(dataProvider, lookup)](api-svypopupfilter.md#new-svyselectfilter-dataprovider-lookup)

#### svySelectFilter.addParam(param)

Add a params to be added into the onSelect callback arguments

| Param | Type     |
| ----- | -------- |
| param | `Object` |

#### svySelectFilter.clearParams()

Clear the params

#### svySelectFilter.createPopUp(callback) ⇒ `plugins.window.FormPopup`

Creates and returns the popupFilter

**Overrides**: [`createPopUp`](api-svypopupfilter.md#abstractpopupfilter.createpopup-callback-plugins.window.formpopup)

#### svySelectFilter.createWindow(\[x], \[y], \[width], \[height], \[jsWindowType]) ⇒ `JSWindow`

**Overrides**: [`createWindow`](api-svypopupfilter.md#abstractpopupfilter.createwindow-x-y-width-height-jswindowtype-jswindow)\
**Returns**: `JSWindow` - returns a JSWindow which can be used to show the popupFilter in it using popupFilter.showWindow(window)

| Param           | Type     | Description                                                                     |
| --------------- | -------- | ------------------------------------------------------------------------------- |
| \[x]            | `Number` |                                                                                 |
| \[y]            | `Number` |                                                                                 |
| \[width]        | `Number` | The width of the pop-up. Optional. Default is component width                   |
| \[height]       | `Number` | The height of the pop-up. Optional. Default is form height.                     |
| \[jsWindowType] | `Number` | Type of window; should be an option of JSWindow, Default JSWindow.MODAL\_DIALOG |

#### svySelectFilter.getDataProvider() ⇒ `String`

Gets the popupFilter dataprovider

#### svySelectFilter.getID() ⇒ `String`

Gets the filter name

#### svySelectFilter.getLookup() ⇒ `scopes.svyLookup.Lookup`

#### svySelectFilter.getOperator() ⇒ `String`

#### svySelectFilter.getParams() ⇒ `Array`

#### svySelectFilter.getState() ⇒ `Object`

**Overrides**: [`getState`](api-svypopupfilter.md#abstractpopupfilter.getstate-object)

#### svySelectFilter.getText() ⇒ `String`

Gets the popupFilter text

#### svySelectFilter.getValues() ⇒ `Array`

#### svySelectFilter.removeParam(index)

Removes a param at the specified index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### svySelectFilter.restoreState(jsonState) ⇒ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

**Overrides**: [`restoreState`](api-svypopupfilter.md#abstractpopupfilter.restorestate-jsonstate-abstractpopupfilter)

| Param     | Type     |
| --------- | -------- |
| jsonState | `Object` |

#### svySelectFilter.setDataProvider(dataProvider)

Sets the popupFilter dataprovider

| Param        | Type     |
| ------------ | -------- |
| dataProvider | `String` |

#### svySelectFilter.setOperator(operator)

| Param    | Type     | Description                                 |
| -------- | -------- | ------------------------------------------- |
| operator | `String` | a value from scopes.svyPopupFilter.OPERATOR |

#### svySelectFilter.setRendererForm(popupFilterForm)

| Param           | Type                                                                                                               |
| --------------- | ------------------------------------------------------------------------------------------------------------------ |
| popupFilterForm | [`RuntimeForm.<AbstractPopupFilter>`](api-svypopupfilter.md#abstractpopupfilter) \| `RuntimeForm.<AbstractLookup>` |

#### svySelectFilter.setText(text)

Sets the popupFilter text

| Param | Type     |
| ----- | -------- |
| text  | `String` |

#### svySelectFilter.setValues(values)

**Overrides**: [`setValues`](api-svypopupfilter.md#abstractpopupfilter.setvalues-values)

| Param  | Type    |
| ------ | ------- |
| values | `Array` |

#### svySelectFilter.showModalWindow(\[callback], \[x], \[y], \[width], \[height]) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`

Shows the popupFilter in a modal Window

**Overrides**: [`showModalWindow`](api-svypopupfilter.md#abstractpopupfilter.showmodalwindow-callback-x-y-width-height-array.less-than-jsrecord-greater-than)\
**Returns**: `Array.<JSRecord>` | `Array.<(String|Date|Number)>` - returns the selected records; if the popupFilterDataprovider has been set instead it returns the popupFilterDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection

| Param       | Type       | Description                                                                                                                             |
| ----------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| \[callback] | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| \[x]        | `Number`   |                                                                                                                                         |
| \[y]        | `Number`   |                                                                                                                                         |
| \[width]    | `Number`   | The width of the popupFilter. Optional. Default is same as target component                                                             |
| \[height]   | `Number`   | The height of the popupFilter. Optional. Default is implementation-specifc.                                                             |

#### svySelectFilter.showPopUp(callback, target, \[width], \[height])

Shows the popupFilter

**Overrides**: [`showPopUp`](api-svypopupfilter.md#abstractpopupfilter.showpopup-callback-target-width-height)

| Param     | Type               | Description                                                                                                                             |
| --------- | ------------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| callback  | `function`         | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| target    | `RuntimeComponent` | The component to show relative to                                                                                                       |
| \[width]  | `Number`           | The width of the popupFilter. Optional. Default is same as target component                                                             |
| \[height] | `Number`           | The height of the popupFilter. Optional. Default is implementation-specifc.                                                             |

#### svySelectFilter.showWindow(win, \[callback]) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`

Shows the popupFilter in a Window

**Overrides**: [`showWindow`](api-svypopupfilter.md#abstractpopupfilter.showwindow-win-callback-array-.less-than-string-or-date-or-number-greater-than)\
**Returns**: `Array.<JSRecord>` | `Array.<(String|Date|Number)>` - returns the selected records; if the popupFilterDataprovider has been set instead it returns the popupFilterDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection

| Param       | Type       | Description                                                                                                             |
| ----------- | ---------- | ----------------------------------------------------------------------------------------------------------------------- |
| win         | `JSWindow` | the JSWindow object to show                                                                                             |
| \[callback] | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array\<String |

#### new SvySelectFilter(dataProvider, lookup)

| Param        | Type                      | Description                          |
| ------------ | ------------------------- | ------------------------------------ |
| dataProvider | `String`                  | will override the lookupDataProvider |
| lookup       | `scopes.svyLookup.Lookup` |                                      |

***

### SvyTokenFilter ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

**Extends**: [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

* [SvyTokenFilter](api-svypopupfilter.md#svytokenfilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)
  * [.addParam(param)](api-svypopupfilter.md#svytokenfilter.addparam-param)
  * [.clearParams()](api-svypopupfilter.md#svytokenfilter.clearparams)
  * [.createPopUp(callback)](api-svypopupfilter.md#svytokenfilter.createpopup-callback-plugins.window.formpopup) ⇒ `plugins.window.FormPopup`
  * [.createWindow(\[x\], \[y\], \[width\], \[height\], \[jsWindowType\])](api-svypopupfilter.md#svytokenfilter.createwindow-x-y-width-height-jswindowtype-jswindow) ⇒ `JSWindow`
  * [.getDataProvider()](api-svypopupfilter.md#svytokenfilter.getdataprovider-string) ⇒ `String`
  * [.getID()](api-svypopupfilter.md#svytokenfilter.getid-string) ⇒ `String`
  * [.getOperator()](api-svypopupfilter.md#svytokenfilter.getoperator-string) ⇒ `String`
  * [.getParams()](api-svypopupfilter.md#svytokenfilter.getparams-array) ⇒ `Array`
  * [.getState()](api-svypopupfilter.md#svytokenfilter.getstate-object) ⇒ `Object`
  * [.getText()](api-svypopupfilter.md#svytokenfilter.gettext-string) ⇒ `String`
  * [.getValues()](api-svypopupfilter.md#svytokenfilter.getvalues-array) ⇒ `Array`
  * [.removeParam(index)](api-svypopupfilter.md#svytokenfilter.removeparam-index)
  * [.restoreState(jsonState)](api-svypopupfilter.md#svytokenfilter.restorestate-jsonstate-abstractpopupfilter) ⇒ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)
  * [.setDataProvider(dataProvider)](api-svypopupfilter.md#svytokenfilter.setdataprovider-dataprovider)
  * [.setOperator(operator)](api-svypopupfilter.md#svytokenfilter.setoperator-operator)
  * [.setRendererForm(popupFilterForm)](api-svypopupfilter.md#svytokenfilter.setrendererform-popupfilterform)
  * [.setText(text)](api-svypopupfilter.md#svytokenfilter.settext-text)
  * [.setValues(values)](api-svypopupfilter.md#svytokenfilter.setvalues-values)
  * [.showModalWindow(\[callback\], \[x\], \[y\], \[width\], \[height\])](api-svypopupfilter.md#svytokenfilter.showmodalwindow-callback-x-y-width-height-array.less-than-jsrecord-greater-than-or-ar) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`
  * [.showPopUp(callback, target, \[width\], \[height\])](api-svypopupfilter.md#svytokenfilter.showpopup-callback-target-width-height)
  * [.showWindow(win, \[callback\])](api-svypopupfilter.md#svytokenfilter.showwindow-win-callback-array-.less-than-string-or-date-or-number-greater-than) ⇒ `[ 'Array' ].<(String|Date|Number)>`

#### svyTokenFilter.addParam(param)

Add a params to be added into the onSelect callback arguments

| Param | Type     |
| ----- | -------- |
| param | `Object` |

#### svyTokenFilter.clearParams()

Clear the params

#### svyTokenFilter.createPopUp(callback) ⇒ `plugins.window.FormPopup`

Creates and returns the popupFilter

| Param    | Type       | Description                                                                                                                             |
| -------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| callback | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |

#### svyTokenFilter.createWindow(\[x], \[y], \[width], \[height], \[jsWindowType]) ⇒ `JSWindow`

**Returns**: `JSWindow` - returns a JSWindow which can be used to show the popupFilter in it using popupFilter.showWindow(window)

| Param           | Type     | Description                                                                     |
| --------------- | -------- | ------------------------------------------------------------------------------- |
| \[x]            | `Number` |                                                                                 |
| \[y]            | `Number` |                                                                                 |
| \[width]        | `Number` | The width of the pop-up. Optional. Default is component width                   |
| \[height]       | `Number` | The height of the pop-up. Optional. Default is form height.                     |
| \[jsWindowType] | `Number` | Type of window; should be an option of JSWindow, Default JSWindow.MODAL\_DIALOG |

#### svyTokenFilter.getDataProvider() ⇒ `String`

Gets the popupFilter dataprovider

#### svyTokenFilter.getID() ⇒ `String`

Gets the filter name

#### svyTokenFilter.getOperator() ⇒ `String`

#### svyTokenFilter.getParams() ⇒ `Array`

#### svyTokenFilter.getState() ⇒ `Object`

#### svyTokenFilter.getText() ⇒ `String`

Gets the popupFilter text

#### svyTokenFilter.getValues() ⇒ `Array`

#### svyTokenFilter.removeParam(index)

Removes a param at the specified index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### svyTokenFilter.restoreState(jsonState) ⇒ [`AbstractPopupFilter`](api-svypopupfilter.md#abstractpopupfilter)

| Param     | Type     |
| --------- | -------- |
| jsonState | `Object` |

#### svyTokenFilter.setDataProvider(dataProvider)

Sets the popupFilter dataprovider

| Param        | Type     |
| ------------ | -------- |
| dataProvider | `String` |

#### svyTokenFilter.setOperator(operator)

| Param    | Type     | Description                                 |
| -------- | -------- | ------------------------------------------- |
| operator | `String` | a value from scopes.svyPopupFilter.OPERATOR |

#### svyTokenFilter.setRendererForm(popupFilterForm)

| Param           | Type                                                                                                               |
| --------------- | ------------------------------------------------------------------------------------------------------------------ |
| popupFilterForm | [`RuntimeForm.<AbstractPopupFilter>`](api-svypopupfilter.md#abstractpopupfilter) \| `RuntimeForm.<AbstractLookup>` |

#### svyTokenFilter.setText(text)

Sets the popupFilter text

| Param | Type     |
| ----- | -------- |
| text  | `String` |

#### svyTokenFilter.setValues(values)

| Param  | Type    |
| ------ | ------- |
| values | `Array` |

#### svyTokenFilter.showModalWindow(\[callback], \[x], \[y], \[width], \[height]) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`

Shows the popupFilter in a modal Window

**Returns**: `Array.<JSRecord>` | `Array.<(String|Date|Number)>` - returns the selected records; if the popupFilterDataprovider has been set instead it returns the popupFilterDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection

| Param       | Type       | Description                                                                                                                             |
| ----------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| \[callback] | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| \[x]        | `Number`   |                                                                                                                                         |
| \[y]        | `Number`   |                                                                                                                                         |
| \[width]    | `Number`   | The width of the popupFilter. Optional. Default is same as target component                                                             |
| \[height]   | `Number`   | The height of the popupFilter. Optional. Default is implementation-specifc.                                                             |

#### svyTokenFilter.showPopUp(callback, target, \[width], \[height])

Shows the popupFilter

| Param     | Type               | Description                                                                                                                             |
| --------- | ------------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| callback  | `function`         | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| target    | `RuntimeComponent` | The component to show relative to                                                                                                       |
| \[width]  | `Number`           | The width of the popupFilter. Optional. Default is same as target component                                                             |
| \[height] | `Number`           | The height of the popupFilter. Optional. Default is implementation-specifc.                                                             |

#### svyTokenFilter.showWindow(win, \[callback]) ⇒ `[ 'Array' ].<(String|Date|Number)>`

Shows the popupFilter in a Window

**Returns**: `[ 'Array' ].<(String|Date|Number)>` - returns the selected records; if the popupFilterDataprovider has been set instead it returns the popupFilterDataprovider values on the selected records. Returns null if the window is closed without a selection or an empty selection

| Param       | Type       | Description                                                                                                                             |
| ----------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| win         | `JSWindow` | the JSWindow object to show                                                                                                             |
| \[callback] | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |

### LOCALE

**Properties**

| Name                  | Default                                                                                                                                                                                                                                                           |
| --------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| filterPopupMenu       | `{"addFilter":"Add filter"}`                                                                                                                                                                                                                                      |
| svyCheckPopupFilter   | `{"labelChecked":"Yes","labelUnchecked":"No"}`                                                                                                                                                                                                                    |
| svyDatePopupFilter    | `{"labelTitle":"Date","labelToday":"Today","labelTomorrow":"Tomorrow","labelThisWeek":"This week","labelNextWeek":"Next week","labelThisMonth":"This month","labelNextMonth":"Next month","labelThisYear":"This year","labelLastYear":"Last year","operator":""}` |
| svyTokenPopupFilter   | `{"searchbox":"","labelRemoveAll":"Remove all"}`                                                                                                                                                                                                                  |
| svySelectPopupFilter  | `{"searchText":"","labelSelectAll":"Select all","labelDeselectAll":"Deselect all"}`                                                                                                                                                                               |
| svyIntegerPopupFilter | `{"labelTitle":"Type filter value...","labelEqualTo":"Equal to","labelGreater":"Bigger than","labelSmaller":"Smaller than","labelBetween":"Between"}`                                                                                                             |
| svyNumberPopupFilter  | `{"labelTitle":"Type filter value...","labelEqualTo":"Equal to","labelGreater":"Bigger than","labelSmaller":"Smaller than","labelBetween":"Between"}`                                                                                                             |

### OPERATOR

**Properties**

| Name             | Default         | Description                                                   |
| ---------------- | --------------- | ------------------------------------------------------------- |
| IS\_NULL         | `isNull`        |                                                               |
| NOT\_NULL        | `!isNull`       |                                                               |
| EQUALS           | `eq`            |                                                               |
| EQUALS\_OR\_NULL | `^`             | eq                                                            |
| LIKE             | `like`          | All values starting with search input e.g. LIKE SEARCH\_WORD% |
| LIKE\_CONTAINS   | `like_contains` | All values containing search input e.g. LIKE %SEARCH\_WORD%   |
| GREATER\_EQUAL   | `ge`            |                                                               |
| GREATER\_THEN    | `gt`            |                                                               |
| SMALLER\_EQUAL   | `le`            |                                                               |
| SMALLER\_THEN    | `lt`            |                                                               |
| BETWEEN          | `BETWEEN`       |                                                               |
| IS\_IN           | `IN`            |                                                               |

### STYLING

**Properties**

| Name                               | Default               |
| ---------------------------------- | --------------------- |
| MUTLI\_SELECT\_ICON\_COLUMN\_WIDTH | `50`                  |
| MULTI\_SELECT\_SHOW\_TILE\_HEADERS | `true`                |
| CLOSE\_ICON                        | `fa fa-close`         |
| REMOVE\_ICON                       | `fa fa-trash`         |
| EXCLUDE\_ICON                      | `fas fa-minus-circle` |
| INCLUDE\_ICON                      | `fas fa-check-circle` |
| OPEN\_FILTER\_ICON                 | `fas fa-angle-down`   |
| REMOVE\_FILTER\_ICON               | `fas fa-times`        |

### applyLocaleStrings(formName, formType)

Applies the locale strings set on svyToolbarFilter.TOOLBAR\_LOCALE to the matching elements for the given form identifier which is one of TOOLBAR\_LOCALE's main properties

| Param    | Type     |
| -------- | -------- |
| formName | `String` |
| formType | `String` |

### createCheckFilter() ⇒ [`SvyCheckFilter`](api-svypopupfilter.md#svycheckfilter-abstractpopupfilter)

### createDateFilter() ⇒ [`SvyDateFilter`](api-svypopupfilter.md#svydatefilter-abstractpopupfilter)

### createIntegerFilter() ⇒ [`SvyIntegerFilter`](api-svypopupfilter.md#svyintegerfilter-abstractpopupfilter)

### createNumberFilter() ⇒ [`SvyNumberFilter`](api-svypopupfilter.md#svynumberfilter-abstractpopupfilter)

### createSelectFilter(dataProvider, lookup) ⇒ [`SvySelectFilter`](api-svypopupfilter.md#svyselectfilter-abstractpopupfilter)

| Param        | Type                      |
| ------------ | ------------------------- |
| dataProvider | `String`                  |
| lookup       | `scopes.svyLookup.Lookup` |

### createTokenFilter() ⇒ [`SvyTokenFilter`](api-svypopupfilter.md#svytokenfilter-abstractpopupfilter)

### getVersion() ⇒ `String`

Gets the version of this module

**Returns**: `String` - the version of the module using the format Major.Minor.Revision

***
