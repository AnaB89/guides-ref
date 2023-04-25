#  JSPart


## **Extends**

## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [BODY](JSPart.md#BODY)                   | Constant use for specifying the type of form parts..                                    |
| [Number](../JSLib/Number.md) | [FOOTER](JSPart.md#FOOTER)                   | Constant use for specifying the type of form parts..                                    |
| [Number](../JSLib/Number.md) | [HEADER](JSPart.md#HEADER)                   | Constant use for specifying the type of form parts..                                    |
| [Number](../JSLib/Number.md) | [TITLE_HEADER](JSPart.md#TITLE_HEADER)                   | Constant use for specifying the type of form parts..                                    |

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [background](JSPart.md#background)                   | The background color of the form part..                                    |
| [String](../JSLib/String.md) | [groupbyDataProviderIDs](JSPart.md#groupbyDataProviderIDs)                   | For Leading Subsummary or Trailing Subsummary parts, one or more dataproviders can be added as Break (GroupBy) dataproviders..                                    |
| [Number](../JSLib/Number.md) | [height](JSPart.md#height)                   | The height of a selected part; specified in pixels..                                    |
| [String](../JSLib/String.md) | [styleClass](JSPart.md#styleClass)                   | The Cascading Style Sheet (CSS) class name applied to the part..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [getComment()](JSPart.md#getcomment)                   | Returns the comment of this component..                                    |
| [Number](../JSLib/Number.md) | [getPartType()](JSPart.md#getparttype)                   | The type of this part..                                    |
| [Number](../JSLib/Number.md) | [getPartYOffset()](JSPart.md#getpartyoffset)                   | The Y offset of the part on the form, this will include all the super forms parts if this form extends a form..                                    |
| [UUID](../Application/UUID.md) | [getUUID()](JSPart.md#getuuid)                   | Returns the UUID of this component..                                    |

## Constants Details

### BODY

Constant use for specifying the type of form parts.

This is the default part that is repeated for each record (being
displayed and/or printed).

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var body = form.newPart(JSPart.BODY, 320);
```
### FOOTER

Constant use for specifying the type of form parts.

A footer is displayed at the bottom of each page when printed ad can
contain summaries of the current selection of records. In List view, the
footer is displayed at the bottom of the list of records.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var footer = form.newPart(JSPart.FOOTER, 440);
```
### HEADER

Constant use for specifying the type of form parts.

A header is displayed at the top of each page when printed and can contain
summaries of the current selection of records. In List view the header is
displayed above the list of records. In tableview the default column headers will
not be there if this is specified.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var header = form.newPart(JSPart.HEADER, 80);
```
### TITLE_HEADER

Constant use for specifying the type of form parts.

Appears only once on the first page of a printed report or on top of the first screen
of a foundset. If a Header is available it is replace by the Title Header on the first
page.
This part is also shown in a normal none printing form, because it can be used to place components
in a tableview form and keep the default table header columns. Other parts as the HEADER will remove
the default header columns.

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var titleHeader = form.newPart(JSPart.TITLE_HEADER, 40);
```

## Properties Details

### background

The background color of the form part.

NOTE: When no background color has been set, the default background
color will be determined by the Look and Feel (LAF) that has been selected
in Application Preferences.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var body = form.newPart(JSPart.BODY, 320);
body.background = 'green';
```
### groupbyDataProviderIDs

For Leading Subsummary or Trailing Subsummary parts, one or more
dataproviders can be added as Break (GroupBy) dataproviders. The
Leading/Trailing Subsummary parts will be displayed once for each
resulted group of data.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var leadingSubsummary = form.newPart(JSPart.LEADING_SUBSUMMARY, 160);
leadingSubsummary.groupbyDataProviderIDs = 'my_table_text';
```
### height

The height of a selected part; specified in pixels.

This height property is the lowerbound as its ending Y value (0 == top of the form).

**Returns**\
[Number](../JSLib/Number.md) 


**Sample**

```javascript
var part = form.newPart(JSPart.HEADER, 100);
part.height = 200;
```
### styleClass

The Cascading Style Sheet (CSS) class name applied to the part.

**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var body = form.newPart(JSPart.BODY, 320);
body.styleClass = 'myBody';
```

## Methods Details

### getComment()

Returns the comment of this component.


**Returns**\
[String](../JSLib/String.md) 


**Sample**

```javascript
var comment = solutionModel.getForm("my_form").getButton("my_button").getComment();
application.output(comment);
```
### getPartType()

The type of this part.


**Returns**\
[Number](../JSLib/Number.md) A number representing the type of the form part.


**Sample**

```javascript
var allParts = form.getParts()
for (var i=0; i<allParts.length; i++) {
	if (allParts[i].getPartType() == JSPart.BODY)
		application.output('body Y offset: ' + allParts[i].getPartYOffset());
}
```
### getPartYOffset()

The Y offset of the part on the form, this will include all the super forms parts if this form extends a form.


**Returns**\
[Number](../JSLib/Number.md) A number holding the Y offset of the form part.


**Sample**

```javascript
var allParts = form.getParts()
for (var i=0; i<allParts.length; i++) {
	if (allParts[i].getPartType() == JSPart.BODY)
		application.output('body Y offset: ' + allParts[i].getPartYOffset());
}
```
### getUUID()

Returns the UUID of this component.


**Returns**\
[UUID](../Application/UUID.md) 


**Sample**

```javascript
var button_uuid = solutionModel.getForm("my_form").getButton("my_button").getUUID();
application.output(button_uuid.toString());
```

