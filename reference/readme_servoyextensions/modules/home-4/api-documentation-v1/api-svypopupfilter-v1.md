# API svyPopupFilter v1

### Classes

[AbstractPopupFilter](api-svypopupfilter-v1.md#abstractpopupfilter)

[SvyDateFilter](api-svypopupfilter-v1.md#svydatefilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)

[SvyNumberFilter](api-svypopupfilter-v1.md#svynumberfilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)

[SvySelectFilter](api-svypopupfilter-v1.md#svyselectfilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)

[SvyTokenFilter](api-svypopupfilter-v1.md#svytokenfilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)

### Functions

[createDateFilter()](api-svypopupfilter-v1.md#createdatefilter-svydatefilter) ⇒ [`SvyDateFilter`](api-svypopupfilter-v1.md#svydatefilter-abstractpopupfilter)

[createNumberFilter()](api-svypopupfilter-v1.md#createnumberfilter-svynumberfilter) ⇒ [`SvyNumberFilter`](api-svypopupfilter-v1.md#svynumberfilter-abstractpopupfilter)

[createSelectFilter(dataProvider, lookup)](api-svypopupfilter-v1.md#createselectfilter-dataprovider-lookup-svyselectfilter) ⇒ [`SvySelectFilter`](api-svypopupfilter-v1.md#svyselectfilter-abstractpopupfilter)

[createTokenFilter()](api-svypopupfilter-v1.md#createtokenfilter-svytokenfilter) ⇒ [`SvyTokenFilter`](api-svypopupfilter-v1.md#svytokenfilter-abstractpopupfilter)

### AbstractPopupFilter

* [AbstractPopupFilter](api-svypopupfilter-v1.md#abstractpopupfilter)
  * [.addParam(param)](api-svypopupfilter-v1.md#abstractpopupfilter.addparam-param)
  * [.clearParams()](api-svypopupfilter-v1.md#abstractpopupfilter.clearparams)
  * [.createPopUp(callback)](api-svypopupfilter-v1.md#abstractpopupfilter.createpopup-callback-plugins.window.formpopup) ⇒ `plugins.window.FormPopup`
  * [.createWindow(\[x\], \[y\], \[width\], \[height\], \[jsWindowType\])](api-svypopupfilter-v1.md#abstractpopupfilter.createwindow-x-y-width-height-jswindowtype-jswindow) ⇒ `JSWindow`
  * [.getDataProvider()](api-svypopupfilter-v1.md#abstractpopupfilter.getdataprovider-string) ⇒ `String`
  * [.getID()](api-svypopupfilter-v1.md#abstractpopupfilter.getid-string) ⇒ `String`
  * [.getOperator()](api-svypopupfilter-v1.md#abstractpopupfilter.getoperator-string) ⇒ `String`
  * [.getParams()](api-svypopupfilter-v1.md#abstractpopupfilter.getparams-array) ⇒ `Array`
  * [.getState()](api-svypopupfilter-v1.md#abstractpopupfilter.getstate-object) ⇒ `Object`
  * [.getValues()](api-svypopupfilter-v1.md#abstractpopupfilter.getvalues-array) ⇒ `Array`
  * [.removeParam(index)](api-svypopupfilter-v1.md#abstractpopupfilter.removeparam-index)
  * [.restoreState(jsonState)](api-svypopupfilter-v1.md#abstractpopupfilter.restorestate-jsonstate-abstractpopupfilter) ⇒ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)
  * [.setDataProvider(dataProvider)](api-svypopupfilter-v1.md#abstractpopupfilter.setdataprovider-dataprovider)
  * [.setOperator(operator)](api-svypopupfilter-v1.md#abstractpopupfilter.setoperator-operator)
  * [.setRendererForm(popupFilterForm)](api-svypopupfilter-v1.md#abstractpopupfilter.setrendererform-popupfilterform)
  * [.setValues(values)](api-svypopupfilter-v1.md#abstractpopupfilter.setvalues-values)
  * [.showModalWindow(\[callback\], \[x\], \[y\], \[width\], \[height\])](api-svypopupfilter-v1.md#abstractpopupfilter.showmodalwindow-callback-x-y-width-height-array.less-than-jsrecord-greater-than) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`
  * [.showPopUp(callback, target, \[width\], \[height\])](api-svypopupfilter-v1.md#abstractpopupfilter.showpopup-callback-target-width-height)
  * [.showWindow(win, \[callback\])](api-svypopupfilter-v1.md#abstractpopupfilter.showwindow-win-callback-array-.less-than-string-or-date-or-number-greater-than) ⇒ `[ 'Array' ].<(String|Date|Number)>`

***

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

#### abstractPopupFilter.getValues() ⇒ `Array`

#### abstractPopupFilter.removeParam(index)

Removes a param at the specified index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### abstractPopupFilter.restoreState(jsonState) ⇒ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)

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

| Param           | Type                                                                                                                  |
| --------------- | --------------------------------------------------------------------------------------------------------------------- |
| popupFilterForm | [`RuntimeForm.<AbstractPopupFilter>`](api-svypopupfilter-v1.md#abstractpopupfilter) \| `RuntimeForm.<AbstractLookup>` |

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

***

### SvyDateFilter ⇐ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)

**Extends**: [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)

* [SvyDateFilter](api-svypopupfilter-v1.md#svydatefilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)
  * [.addParam(param)](api-svypopupfilter-v1.md#svydatefilter.addparam-param)
  * [.clearParams()](api-svypopupfilter-v1.md#svydatefilter.clearparams)
  * [.createPopUp(callback)](api-svypopupfilter-v1.md#svydatefilter.createpopup-callback-plugins.window.formpopup) ⇒ `plugins.window.FormPopup`
  * [.createWindow(\[x\], \[y\], \[width\], \[height\], \[jsWindowType\])](api-svypopupfilter-v1.md#svydatefilter.createwindow-x-y-width-height-jswindowtype-jswindow) ⇒ `JSWindow`
  * [.getDataProvider()](api-svypopupfilter-v1.md#svydatefilter.getdataprovider-string) ⇒ `String`
  * [.getID()](api-svypopupfilter-v1.md#svydatefilter.getid-string) ⇒ `String`
  * [.getOperator()](api-svypopupfilter-v1.md#svydatefilter.getoperator-string) ⇒ `String`
  * [.getParams()](api-svypopupfilter-v1.md#svydatefilter.getparams-array) ⇒ `Array`
  * [.getState()](api-svypopupfilter-v1.md#svydatefilter.getstate-object) ⇒ `Object`
  * [.getValues()](api-svypopupfilter-v1.md#svydatefilter.getvalues-array) ⇒ `Array`
  * [.removeParam(index)](api-svypopupfilter-v1.md#svydatefilter.removeparam-index)
  * [.restoreState(jsonState)](api-svypopupfilter-v1.md#svydatefilter.restorestate-jsonstate-abstractpopupfilter) ⇒ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)
  * [.setDataProvider(dataProvider)](api-svypopupfilter-v1.md#svydatefilter.setdataprovider-dataprovider)
  * [.setOperator(operator)](api-svypopupfilter-v1.md#svydatefilter.setoperator-operator)
  * [.setRendererForm(popupFilterForm)](api-svypopupfilter-v1.md#svydatefilter.setrendererform-popupfilterform)
  * [.setValues(values)](api-svypopupfilter-v1.md#svydatefilter.setvalues-values)
  * [.showModalWindow(\[callback\], \[x\], \[y\], \[width\], \[height\])](api-svypopupfilter-v1.md#svydatefilter.showmodalwindow-callback-x-y-width-height-array.less-than-jsrecord-greater-than-or-arr) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`
  * [.showPopUp(callback, target, \[width\], \[height\])](api-svypopupfilter-v1.md#svydatefilter.showpopup-callback-target-width-height)
  * [.showWindow(win, \[callback\])](api-svypopupfilter-v1.md#svydatefilter.showwindow-win-callback-array-.less-than-string-or-date-or-number-greater-than) ⇒ `[ 'Array' ].<(String|Date|Number)>`

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

#### svyDateFilter.getValues() ⇒ `Array`

#### svyDateFilter.removeParam(index)

Removes a param at the specified index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### svyDateFilter.restoreState(jsonState) ⇒ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)

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

| Param           | Type                                                                                                                  |
| --------------- | --------------------------------------------------------------------------------------------------------------------- |
| popupFilterForm | [`RuntimeForm.<AbstractPopupFilter>`](api-svypopupfilter-v1.md#abstractpopupfilter) \| `RuntimeForm.<AbstractLookup>` |

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

***

### SvyNumberFilter ⇐ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)

**Extends**: [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)

* [SvyNumberFilter](api-svypopupfilter-v1.md#svynumberfilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)
  * [.addParam(param)](api-svypopupfilter-v1.md#svynumberfilter.addparam-param)
  * [.clearParams()](api-svypopupfilter-v1.md#svynumberfilter.clearparams)
  * [.createPopUp(callback)](api-svypopupfilter-v1.md#svynumberfilter.createpopup-callback-plugins.window.formpopup) ⇒ `plugins.window.FormPopup`
  * [.createWindow(\[x\], \[y\], \[width\], \[height\], \[jsWindowType\])](api-svypopupfilter-v1.md#svynumberfilter.createwindow-x-y-width-height-jswindowtype-jswindow) ⇒ `JSWindow`
  * [.getDataProvider()](api-svypopupfilter-v1.md#svynumberfilter.getdataprovider-string) ⇒ `String`
  * [.getID()](api-svypopupfilter-v1.md#svynumberfilter.getid-string) ⇒ `String`
  * [.getOperator()](api-svypopupfilter-v1.md#svynumberfilter.getoperator-string) ⇒ `String`
  * [.getParams()](api-svypopupfilter-v1.md#svynumberfilter.getparams-array) ⇒ `Array`
  * [.getState()](api-svypopupfilter-v1.md#svynumberfilter.getstate-object) ⇒ `Object`
  * [.getValues()](api-svypopupfilter-v1.md#svynumberfilter.getvalues-array) ⇒ `Array`
  * [.removeParam(index)](api-svypopupfilter-v1.md#svynumberfilter.removeparam-index)
  * [.restoreState(jsonState)](api-svypopupfilter-v1.md#svynumberfilter.restorestate-jsonstate-abstractpopupfilter) ⇒ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)
  * [.setDataProvider(dataProvider)](api-svypopupfilter-v1.md#svynumberfilter.setdataprovider-dataprovider)
  * [.setOperator(operator)](api-svypopupfilter-v1.md#svynumberfilter.setoperator-operator)
  * [.setRendererForm(popupFilterForm)](api-svypopupfilter-v1.md#svynumberfilter.setrendererform-popupfilterform)
  * [.setValues(values)](api-svypopupfilter-v1.md#svynumberfilter.setvalues-values)
  * [.showModalWindow(\[callback\], \[x\], \[y\], \[width\], \[height\])](api-svypopupfilter-v1.md#svynumberfilter.showmodalwindow-callback-x-y-width-height-array.less-than-jsrecord-greater-than-or-a) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`
  * [.showPopUp(callback, target, \[width\], \[height\])](api-svypopupfilter-v1.md#svynumberfilter.showpopup-callback-target-width-height)
  * [.showWindow(win, \[callback\])](api-svypopupfilter-v1.md#svynumberfilter.showwindow-win-callback-array-.less-than-string-or-date-or-number-greater-than) ⇒ `[ 'Array' ].<(String|Date|Number)>`

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

#### svyNumberFilter.getValues() ⇒ `Array`

#### svyNumberFilter.removeParam(index)

Removes a param at the specified index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### svyNumberFilter.restoreState(jsonState) ⇒ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)

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

| Param           | Type                                                                                                                  |
| --------------- | --------------------------------------------------------------------------------------------------------------------- |
| popupFilterForm | [`RuntimeForm.<AbstractPopupFilter>`](api-svypopupfilter-v1.md#abstractpopupfilter) \| `RuntimeForm.<AbstractLookup>` |

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

### SvySelectFilter ⇐ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)

**Extends**: [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)

* [SvySelectFilter](api-svypopupfilter-v1.md#svyselectfilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)
  * [.addParam(param)](api-svypopupfilter-v1.md#svyselectfilter.addparam-param)
  * [.clearParams()](api-svypopupfilter-v1.md#svyselectfilter.clearparams)
  * [.createPopUp(callback)](api-svypopupfilter-v1.md#svyselectfilter.createpopup-callback-plugins.window.formpopup) ⇒ `plugins.window.FormPopup`
  * [.createWindow(\[x\], \[y\], \[width\], \[height\], \[jsWindowType\])](api-svypopupfilter-v1.md#svyselectfilter.createwindow-x-y-width-height-jswindowtype-jswindow) ⇒ `JSWindow`
  * [.getDataProvider()](api-svypopupfilter-v1.md#svyselectfilter.getdataprovider-string) ⇒ `String`
  * [.getID()](api-svypopupfilter-v1.md#svyselectfilter.getid-string) ⇒ `String`
  * [.getLookup()](api-svypopupfilter-v1.md#svyselectfilter.getlookup-scopes.svylookup.lookup) ⇒ `scopes.svyLookup.Lookup`
  * [.getOperator()](api-svypopupfilter-v1.md#svyselectfilter.getoperator-string) ⇒ `String`
  * [.getParams()](api-svypopupfilter-v1.md#svyselectfilter.getparams-array) ⇒ `Array`
  * [.getState()](api-svypopupfilter-v1.md#svyselectfilter.getstate-object) ⇒ `Object`
  * [.getValues()](api-svypopupfilter-v1.md#svyselectfilter.getvalues-array) ⇒ `Array`
  * [.removeParam(index)](api-svypopupfilter-v1.md#svyselectfilter.removeparam-index)
  * [.restoreState(jsonState)](api-svypopupfilter-v1.md#svyselectfilter.restorestate-jsonstate-abstractpopupfilter) ⇒ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)
  * [.setDataProvider(dataProvider)](api-svypopupfilter-v1.md#svyselectfilter.setdataprovider-dataprovider)
  * [.setOperator(operator)](api-svypopupfilter-v1.md#svyselectfilter.setoperator-operator)
  * [.setRendererForm(popupFilterForm)](api-svypopupfilter-v1.md#svyselectfilter.setrendererform-popupfilterform)
  * [.setValues(values)](api-svypopupfilter-v1.md#svyselectfilter.setvalues-values)
  * [.showModalWindow(\[callback\], \[x\], \[y\], \[width\], \[height\])](api-svypopupfilter-v1.md#svyselectfilter.showmodalwindow-callback-x-y-width-height-array.less-than-jsrecord-greater-than-or-a) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`
  * [.showPopUp(callback, target, \[width\], \[height\])](api-svypopupfilter-v1.md#svyselectfilter.showpopup-callback-target-width-height)
  * [.showWindow(win, \[callback\])](api-svypopupfilter-v1.md#svyselectfilter.showwindow-win-callback-array.less-than-jsrecord-greater-than-or-array.less-than-str) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`
  * [new SvySelectFilter(dataProvider, lookup)](api-svypopupfilter-v1.md#new-svyselectfilter-dataprovider-lookup)

#### svySelectFilter.addParam(param)

Add a params to be added into the onSelect callback arguments

| Param | Type     |
| ----- | -------- |
| param | `Object` |

#### svySelectFilter.clearParams()

Clear the params

#### svySelectFilter.createPopUp(callback) ⇒ `plugins.window.FormPopup`

Creates and returns the popupFilter

**Overrides**: [`createPopUp`](api-svypopupfilter-v1.md#abstractpopupfilter.createpopup-callback-plugins.window.formpopup)

| Param    | Type       | Description                                                                                                                             |
| -------- | ---------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| callback | `function` | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |

#### svySelectFilter.createWindow(\[x], \[y], \[width], \[height], \[jsWindowType]) ⇒ `JSWindow`

**Overrides**: [`createWindow`](api-svypopupfilter-v1.md#abstractpopupfilter.createwindow-x-y-width-height-jswindowtype-jswindow)\
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

**Overrides**: [`getState`](api-svypopupfilter-v1.md#abstractpopupfilter.getstate-object)

#### svySelectFilter.getValues() ⇒ `Array`

#### svySelectFilter.removeParam(index)

Removes a param at the specified index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### svySelectFilter.restoreState(jsonState) ⇒ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)

**Overrides**: [`restoreState`](api-svypopupfilter-v1.md#abstractpopupfilter.restorestate-jsonstate-abstractpopupfilter)

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

| Param           | Type                                                                                                                  |
| --------------- | --------------------------------------------------------------------------------------------------------------------- |
| popupFilterForm | [`RuntimeForm.<AbstractPopupFilter>`](api-svypopupfilter-v1.md#abstractpopupfilter) \| `RuntimeForm.<AbstractLookup>` |

#### svySelectFilter.setValues(values)

| Param  | Type    |
| ------ | ------- |
| values | `Array` |

#### svySelectFilter.showModalWindow(\[callback], \[x], \[y], \[width], \[height]) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`

Shows the popupFilter in a modal Window

**Overrides**: [`showModalWindow`](api-svypopupfilter-v1.md#abstractpopupfilter.showmodalwindow-callback-x-y-width-height-array.less-than-jsrecord-greater-than)\
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

**Overrides**: [`showPopUp`](api-svypopupfilter-v1.md#abstractpopupfilter.showpopup-callback-target-width-height)

| Param     | Type               | Description                                                                                                                             |
| --------- | ------------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| callback  | `function`         | The function that will be called when a selection is made; the callback returns the following arguments: {Array} record, {Array\<String |
| target    | `RuntimeComponent` | The component to show relative to                                                                                                       |
| \[width]  | `Number`           | The width of the popupFilter. Optional. Default is same as target component                                                             |
| \[height] | `Number`           | The height of the popupFilter. Optional. Default is implementation-specifc.                                                             |

#### svySelectFilter.showWindow(win, \[callback]) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`

Shows the popupFilter in a Window

**Overrides**: [`showWindow`](api-svypopupfilter-v1.md#abstractpopupfilter.showwindow-win-callback-array-.less-than-string-or-date-or-number-greater-than)\
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

### SvyTokenFilter ⇐ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)

**Extends**: [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)

* [SvyTokenFilter](api-svypopupfilter-v1.md#svytokenfilter-abstractpopupfilter) ⇐ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)
  * [.addParam(param)](api-svypopupfilter-v1.md#svytokenfilter.addparam-param)
  * [.clearParams()](api-svypopupfilter-v1.md#svytokenfilter.clearparams)
  * [.createPopUp(callback)](api-svypopupfilter-v1.md#svytokenfilter.createpopup-callback-plugins.window.formpopup) ⇒ `plugins.window.FormPopup`
  * [.createWindow(\[x\], \[y\], \[width\], \[height\], \[jsWindowType\])](api-svypopupfilter-v1.md#svytokenfilter.createwindow-x-y-width-height-jswindowtype-jswindow) ⇒ `JSWindow`
  * [.getDataProvider()](api-svypopupfilter-v1.md#svytokenfilter.getdataprovider-string) ⇒ `String`
  * [.getID()](api-svypopupfilter-v1.md#svytokenfilter.getid-string) ⇒ `String`
  * [.getOperator()](api-svypopupfilter-v1.md#svytokenfilter.getoperator-string) ⇒ `String`
  * [.getParams()](api-svypopupfilter-v1.md#svytokenfilter.getparams-array) ⇒ `Array`
  * [.getState()](api-svypopupfilter-v1.md#svytokenfilter.getstate-object) ⇒ `Object`
  * [.getValues()](api-svypopupfilter-v1.md#svytokenfilter.getvalues-array) ⇒ `Array`
  * [.removeParam(index)](api-svypopupfilter-v1.md#svytokenfilter.removeparam-index)
  * [.restoreState(jsonState)](api-svypopupfilter-v1.md#svytokenfilter.restorestate-jsonstate-abstractpopupfilter) ⇒ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)
  * [.setDataProvider(dataProvider)](api-svypopupfilter-v1.md#svytokenfilter.setdataprovider-dataprovider)
  * [.setOperator(operator)](api-svypopupfilter-v1.md#svytokenfilter.setoperator-operator)
  * [.setRendererForm(popupFilterForm)](api-svypopupfilter-v1.md#svytokenfilter.setrendererform-popupfilterform)
  * [.setValues(values)](api-svypopupfilter-v1.md#svytokenfilter.setvalues-values)
  * [.showModalWindow(\[callback\], \[x\], \[y\], \[width\], \[height\])](api-svypopupfilter-v1.md#svytokenfilter.showmodalwindow-callback-x-y-width-height-array.less-than-jsrecord-greater-than-or-ar) ⇒ `Array.<JSRecord>` | `Array.<(String|Date|Number)>`
  * [.showPopUp(callback, target, \[width\], \[height\])](api-svypopupfilter-v1.md#svytokenfilter.showpopup-callback-target-width-height)
  * [.showWindow(win, \[callback\])](api-svypopupfilter-v1.md#svytokenfilter.showwindow-win-callback-array-.less-than-string-or-date-or-number-greater-than) ⇒ `[ 'Array' ].<(String|Date|Number)>`

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

#### svyTokenFilter.getValues() ⇒ `Array`

#### svyTokenFilter.removeParam(index)

Removes a param at the specified index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### svyTokenFilter.restoreState(jsonState) ⇒ [`AbstractPopupFilter`](api-svypopupfilter-v1.md#abstractpopupfilter)

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

| Param           | Type                                                                                                                  |
| --------------- | --------------------------------------------------------------------------------------------------------------------- |
| popupFilterForm | [`RuntimeForm.<AbstractPopupFilter>`](api-svypopupfilter-v1.md#abstractpopupfilter) \| `RuntimeForm.<AbstractLookup>` |

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

***

### OPERATOR

**Properties**

| Name           | Default   |
| -------------- | --------- |
| EQUALS         | `eq`      |
| GREATER\_EQUAL | `ge`      |
| GREATER\_THEN  | `gt`      |
| SMALLER\_EQUAL | `le`      |
| SMALLER\_THEN  | `lt`      |
| BETWEEN        | `BETWEEN` |
| IS\_IN         | `IN`      |

### createDateFilter() ⇒ [`SvyDateFilter`](api-svypopupfilter-v1.md#svydatefilter-abstractpopupfilter)

### createNumberFilter() ⇒ [`SvyNumberFilter`](api-svypopupfilter-v1.md#svynumberfilter-abstractpopupfilter)

### createSelectFilter(dataProvider, lookup) ⇒ [`SvySelectFilter`](api-svypopupfilter-v1.md#svyselectfilter-abstractpopupfilter)

| Param        | Type                      |
| ------------ | ------------------------- |
| dataProvider | `String`                  |
| lookup       | `scopes.svyLookup.Lookup` |

### createTokenFilter() ⇒ [`SvyTokenFilter`](api-svypopupfilter-v1.md#svytokenfilter-abstractpopupfilter)

***
