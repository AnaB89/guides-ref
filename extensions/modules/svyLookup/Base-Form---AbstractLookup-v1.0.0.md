# Base Form AbstractLookup v1.0.0

### AbstractLookup

Provides base form implementation of a lookup form. In general, direct use of this form is not needed. But developers can subclass this form to create a custom implementation.

### Members

[lookup](Base-Form---AbstractLookup-v1.0.0.md#lookup-scopes.svylookup.lookup) : `scopes.svyLookup.Lookup`

The lookup object used by this lokup form

[searchText](Base-Form---AbstractLookup-v1.0.0.md#searchtext-string) : `String`

User input for text searching

### Functions

[dismiss()](Base-Form---AbstractLookup-v1.0.0.md#dismiss)

Dismisses the popup

[newInstance(lookupObj)](Base-Form---AbstractLookup-v1.0.0.md#newinstance-lookupobj-runtimeform.less-than-abstractlookup-greater-than) ⇒ `RuntimeForm.<AbstractLookup>`[onCreateInstance(jsForm, lookupObj)](Base-Form---AbstractLookup-v1.0.0.md#oncreateinstance-jsform-lookupobj)

Hook for sub form(s) to implement specific sol model additions

[onSelect()](Base-Form---AbstractLookup-v1.0.0.md#onselect)

Callback when item is selected

[search()](Base-Form---AbstractLookup-v1.0.0.md#search)

Runs the search. Loads records in the foundset.

[showPopUp(callback, target, \[width\], \[height\], \[initialValue\])](Base-Form---AbstractLookup-v1.0.0.md#showpopup-callback-target-width-height-initialvalue)

Shows this form as pop-up, returns selection in callback

### dismiss()

Dismisses the popup

***

### newInstance(lookupObj) ⇒ `RuntimeForm.<AbstractLookup>`

| Param     | Type                      |
| --------- | ------------------------- |
| lookupObj | `scopes.svyLookup.Lookup` |

***

#### newInstance\~form : `RuntimeForm.<AbstractLookup>`

***

### onCreateInstance(jsForm, lookupObj)

Hook for sub form(s) to implement specific sol model additions

| Param     | Type                      |
| --------- | ------------------------- |
| jsForm    | `JSForm`                  |
| lookupObj | `scopes.svyLookup.Lookup` |

***

### onSelect()

Callback when item is selected

***

### search()

Runs the search. Loads records in the foundset.

***

### showPopUp(callback, target, \[width], \[height], \[initialValue])

Shows this form as pop-up, returns selection in callback

| Param           | Type               | Description                                                   |
| --------------- | ------------------ | ------------------------------------------------------------- |
| callback        | `function`         | The function that is called when selection happens            |
| target          | `RuntimeComponent` | The component which will be shown                             |
| \[width]        | `Number`           | The width of the pop-up. Optional. Default is component width |
| \[height]       | `Number`           | The height of the pop-up. Optional. Default is form height.   |
| \[initialValue] | `String`           | Initial value in search. Optional. Default is empty.          |

***

### lookup : `scopes.svyLookup.Lookup`

The lookup object used by this lokup form

***

### searchText : `String`

User input for text searching

***
