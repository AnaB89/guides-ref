#  Part

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../../JSLib/Boolean.md) | [allowBreakAcrossPageBounds](Part.md#allowBreakAcrossPageBounds)                   | When set, the remainder of a selected part that does not fit on the page currently being printed, will not be transported to the next page - it will break where the page ends and continue on the next page..                                    |
| [String](../../JSLib/String.md) | [background](Part.md#background)                   | The background color of the form part..                                    |
| [Boolean](../../JSLib/Boolean.md) | [discardRemainderAfterBreak](Part.md#discardRemainderAfterBreak)                   | When set, the remainder of a selected part that is broken due to the page ending will not be printed on the next page - it will be discarded..                                    |
| [String](../../JSLib/String.md) | [groupbyDataProviderIDs](Part.md#groupbyDataProviderIDs)                   | For Leading Subsummary or Trailing Subsummary parts, one or more dataproviders can be added as Break (GroupBy) dataproviders..                                    |
| [Number](../../JSLib/Number.md) | [height](Part.md#height)                   | The height of a selected part; specified in pixels..                                    |
| [Number](../../JSLib/Number.md) | [pageBreakAfterOccurrence](Part.md#pageBreakAfterOccurrence)                   | A page break will be inserted after a specified number of occurences of a selected part..                                    |
| [Boolean](../../JSLib/Boolean.md) | [pageBreakBefore](Part.md#pageBreakBefore)                   | When set, a page break will be inserted before each occurrence of a selected part..                                    |
| [Number](../../JSLib/Number.md) | [partType](Part.md#partType)                   | The type of this part..                                    |
| [Boolean](../../JSLib/Boolean.md) | [restartPageNumber](Part.md#restartPageNumber)                   | When set, page numbering will be restarted after each occurrence of a selected part..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sinkWhenLast](Part.md#sinkWhenLast)                   | When set, the last part on a page (such as a Trailing Grand Summary part) will "sink" to the lowest part of the page when there is free space..                                    |
| [String](../../JSLib/String.md) | [styleClass](Part.md#styleClass)                   | The Cascading Style Sheet (CSS) class name applied to the part..                                    |

## Properties Details

### allowBreakAcrossPageBounds

When set, the remainder of a selected part that does not fit on the page currently
being printed, will not be transported to the next page - it will break where the page
ends and continue on the next page.

NOTE: Make sure to set this option when you are printing more than one page per record.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript

```
### background

The background color of the form part.

NOTE: When no background color has been set, the default background
color will be determined by the Look and Feel (LAF) that has been selected
in Application Preferences.

**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### discardRemainderAfterBreak

When set, the remainder of a selected part that is broken due to the page
ending will not be printed on the next page - it will be discarded.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript

```
### groupbyDataProviderIDs

For Leading Subsummary or Trailing Subsummary parts, one or more
dataproviders can be added as Break (GroupBy) dataproviders. The
Leading/Trailing Subsummary parts will be displayed once for each
resulted group of data.

**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### height

The height of a selected part; specified in pixels.

This height property is the lowerbound as its ending Y value (0 == top of the form).

**Returns**\
[Number](../../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### pageBreakAfterOccurrence

A page break will be inserted after a specified number of occurences of a selected part.

**Returns**\
[Number](../../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript

```
### pageBreakBefore

When set, a page break will be inserted before each occurrence of a selected part.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript

```
### partType

The type of this part.

**Returns**\
[Number](../../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### restartPageNumber

When set, page numbering will be restarted after each occurrence of a selected part.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript

```
### sinkWhenLast

When set, the last part on a page (such as a Trailing Grand Summary part) will
"sink" to the lowest part of the page when there is free space.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript

```
### styleClass

The Cascading Style Sheet (CSS) class name applied to the part.

**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```

