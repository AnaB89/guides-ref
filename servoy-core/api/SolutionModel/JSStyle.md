#  JSStyle


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [text](JSStyle.md#text)                   | The textual content of the style..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [getName()](JSStyle.md#getname)                   | Gets the name of the style..                                    |
| [UUID](../Application/UUID.md) | [getUUID()](JSStyle.md#getuuid)                   | Returns the UUID of the style object.                                    |

## Properties Details

### text

The textual content of the style.

**Returns**\
[String](../JSLib/String.md) 


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
[String](../JSLib/String.md) A String holding the name of the style.


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
[UUID](../Application/UUID.md) 


**Sample**

```javascript
var st = solutionModel.newStyle('myStyle','form { background-color: yellow; }');
application.output(st.getUUID().toString());
```

