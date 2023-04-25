#  serialize


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Object](../../JSLib/Object.md) | [fromJSON(data)](serialize.md#fromjson-data)                   | Deserialize from JSON text to an object..                                    |
| [String](../../JSLib/String.md) | [toJSON(obj)](serialize.md#tojson-obj)                   | Serialize an object to JSON text..                                    |

## Methods Details

### fromJSON(data)

Deserialize from JSON text to an object.

**Parameters**\
[String](../../JSLib/String.md) data  ;

**Returns**\
[Object](../../JSLib/Object.md) 


**Sample**

```javascript
var org_array = new Array('A1','F1','Paris-Dakar');
var string_data = plugins.serialize.toJSON(org_array);
var new_array = plugins.serialize.fromJSON(string_data);
application.output(new_array.join('#'));
```
### toJSON(obj)

Serialize an object to JSON text.

**Parameters**\
[Object](../../JSLib/Object.md) obj  ;

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var org_array = new Array('A1','F1','Paris-Dakar');
var string_data = plugins.serialize.toJSON(org_array);
var new_array = plugins.serialize.fromJSON(string_data);
application.output(new_array.join('#'));
```

