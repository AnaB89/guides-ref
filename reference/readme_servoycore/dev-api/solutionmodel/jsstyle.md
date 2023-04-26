# JSStyle

## Property Summary

| Type                          | Name                    | Summary                            |
| ----------------------------- | ----------------------- | ---------------------------------- |
| [String](../js-lib/string.md) | [text](jsstyle.md#text) | The textual content of the style.. |

## Methods Summary

| Type                           | Name                            | Summary                               |
| ------------------------------ | ------------------------------- | ------------------------------------- |
| [String](../js-lib/string.md)  | [getName()](jsstyle.md#getname) | Gets the name of the style..          |
| [UUID](../application/uuid.md) | [getUUID()](jsstyle.md#getuuid) | Returns the UUID of the style object. |

## Properties Details

### text

The textual content of the style.

**Returns**\
[String](../js-lib/string.md)

**Sample**

```javascript
var st = solutionModel.newStyle('myStyle','form { background-color: yellow; }');
st.text = st.text + 'field { background-color: blue; }';
form.styleName = 'myStyle';
application.output('Style name is: ' + st.getName());
```

## Methods Details

### getName()

Gets the name of the style.

**Returns**\
[String](../js-lib/string.md) A String holding the name of the style.

**Sample**

```javascript
var st = solutionModel.newStyle('myStyle','form { background-color: yellow; }');
st.text = st.text + 'field { background-color: blue; }';
form.styleName = 'myStyle';
application.output('Style name is: ' + st.getName());
```

### getUUID()

Returns the UUID of the style object

**Returns**\
[UUID](../application/uuid.md)

**Sample**

```javascript
var st = solutionModel.newStyle('myStyle','form { background-color: yellow; }');
application.output(st.getUUID().toString());
```
