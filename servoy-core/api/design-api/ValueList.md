#  ValueList


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [addEmptyValue](ValueList.md#addEmptyValue)                   | Property that tells if an empty value must be shown next to the items in the value list..                                    |
| [String](../JSLib/String.md) | [comment](ValueList.md#comment)                   | .                                    |
| [String](../JSLib/String.md) | [customValues](ValueList.md#customValues)                   | A string with the elements in the valuelist..                                    |
| [String](../JSLib/String.md) | [dataProviderID1](ValueList.md#dataProviderID1)                   | This is the dataprovider selected in the fist list of dataproviders when a table or related valuelist is selected..                                    |
| [String](../JSLib/String.md) | [dataProviderID2](ValueList.md#dataProviderID2)                   | This is the dataprovider selected in the last list of dataproviders when a table or related valuelist is selected..                                    |
| [String](../JSLib/String.md) | [dataProviderID3](ValueList.md#dataProviderID3)                   | This is the dataprovider selected in the last list of dataproviders when a table or related valuelist is selected..                                    |
| [String](../JSLib/String.md) | [dataSource](ValueList.md#dataSource)                   | Compact representation of the names of the server and table that are used for loading the data from the database..                                    |
| [String](../JSLib/String.md) | [deprecated](ValueList.md#deprecated)                   | Gets the deprecate info for this element.                                    |
| [Number](../JSLib/Number.md) | [displayValueType](ValueList.md#displayValueType)                   | The type of the display value if this is a global or custom valuelist, servoy needs to know this for formatting purposes.                                    |
| [Number](../JSLib/Number.md) | [encapsulation](ValueList.md#encapsulation)                   | The encapsulation mode of this Valuelist..                                    |
| [Number](../JSLib/Number.md) | [fallbackValueList](ValueList.md#fallbackValueList)                   | If the valuelist only displays the "active" values that a user can choose, but you still need to be able to show also old values, then a fallback valuelist should be set..                                    |
| [Boolean](../JSLib/Boolean.md) | [lazyLoading](ValueList.md#lazyLoading)                   | A property special for NGClient and GlobalValuelist to only query the global valuelist when it is needed..                                    |
| [String](../JSLib/String.md) | [name](ValueList.md#name)                   | The name of the value list..                                    |
| [Number](../JSLib/Number.md) | [realValueType](ValueList.md#realValueType)                   | The type of the real value if this is a global or custom valuelist, servoy needs to know this so it can check if the types match on the record it is binded to..                                    |
| [String](../JSLib/String.md) | [relationName](ValueList.md#relationName)                   | The name of the relation that is used for loading data from the database..                                    |
| [Number](../JSLib/Number.md) | [returnDataProviders](ValueList.md#returnDataProviders)                   | Which of the dataprovers should be used as the return dataprovider, so set back into the records dataprovider..                                    |
| [String](../JSLib/String.md) | [separator](ValueList.md#separator)                   | A String representing the separator that should be used when multiple display dataproviders are set, when the value list has the type set to database values..                                    |
| [Number](../JSLib/Number.md) | [showDataProviders](ValueList.md#showDataProviders)                   | Gets the showDataProvider..                                    |
| [String](../JSLib/String.md) | [sortOptions](ValueList.md#sortOptions)                   | Sort options that are applied when the valuelist loads its data from the database..                                    |
| [Boolean](../JSLib/Boolean.md) | [useTableFilter](ValueList.md#useTableFilter)                   | Flag that tells if the name of the valuelist should be applied as a filter on the 'valuelist_name' column when retrieving the data from the database..                                    |
| [Number](../JSLib/Number.md) | [valueListType](ValueList.md#valueListType)                   | The type of the valuelist..                                    |

## Properties Details

### addEmptyValue

Property that tells if an empty value must be shown next to the items in the value list.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```
### comment



**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### customValues

A string with the elements in the valuelist. The elements
can be separated by linefeeds (custom1
custom2), optional with realvalues ((custom1|1
custom2|2)).

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### dataProviderID1

This is the dataprovider selected in the fist list of dataproviders when a table or related valuelist is selected.
This dataprovide can be marked as a display and/or return value

**Returns**\
[String](../JSLib/String.md) Returns a String


**Sample**

```javascript

```
### dataProviderID2

This is the dataprovider selected in the last list of dataproviders when a table or related valuelist is selected.
This dataprovide can be marked as a display and/or return value

**Returns**\
[String](../JSLib/String.md) Returns a String


**Sample**

```javascript

```
### dataProviderID3

This is the dataprovider selected in the last list of dataproviders when a table or related valuelist is selected.
This dataprovide can be marked as a display and/or return value

**Returns**\
[String](../JSLib/String.md) Returns a String


**Sample**

```javascript

```
### dataSource

Compact representation of the names of the server and table that
are used for loading the data from the database.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### deprecated

Gets the deprecate info for this element

**Returns**\
[String](../JSLib/String.md) the deprecate info for this element or null if it is not deprecated


**Sample**

```javascript

```
### displayValueType

The type of the display value if this is a global or custom valuelist, servoy needs to know this for formatting purposes

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```
### encapsulation

The encapsulation mode of this Valuelist. The following can be used:

- Public (available in both scripting and designer from any module)
- Module Scope - available in both scripting and designer but only in the same module.

**Returns**\
[Number](../JSLib/Number.md) the encapsulation mode/level of the persist.


**Sample**

```javascript

```
### fallbackValueList

If the valuelist only displays the "active" values that a user can choose, but you still need to be able to show also old values, then a fallback valuelist should be set.
 So that there is a backup list for getting a display value for a real value that is not in the normal valuelist anymore.

**Returns**\
[Number](../JSLib/Number.md) the valueback valuelist id.


**Sample**

```javascript

```
### lazyLoading

A property special for NGClient and GlobalValuelist to only query the global valuelist when it is needed.
This flag has to be set both on valuelist and in component spec, on the valuelist property.

IMPORTANT: Usage of real & display values is not fully supported with lazy loading. Don't set lazy load if your method returns both real and display values
This is because very likely we do need directly the display value for the given real to dispaly its value..

**Returns**\
[Boolean](../JSLib/Boolean.md) 


**Sample**

```javascript

```
### name

The name of the value list.

It is relevant when the "useTableFilter" property is set.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### realValueType

The type of the real value if this is a global or custom valuelist, servoy needs to know this so it can check if the types match on the record it is binded to.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```
### relationName

The name of the relation that is used for loading data from the database.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### returnDataProviders

Which of the dataprovers should be used as the return dataprovider, so set back into the records dataprovider.

**Returns**\
[Number](../JSLib/Number.md) Returns a int


**Sample**

```javascript

```
### separator

A String representing the separator that should be used when multiple
display dataproviders are set, when the value list has the type set to
database values.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### showDataProviders

Gets the showDataProvider.

**Returns**\
[Number](../JSLib/Number.md) Returns a int


**Sample**

```javascript

```
### sortOptions

Sort options that are applied when the valuelist loads its data
from the database.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript

```
### useTableFilter

Flag that tells if the name of the valuelist should be applied as a filter on the
'valuelist_name' column when retrieving the data from the database.

**Returns**\
[Boolean](../JSLib/Boolean.md) 


**Sample**

```javascript

```
### valueListType

The type of the valuelist. Can be either custom values or database values.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript

```

