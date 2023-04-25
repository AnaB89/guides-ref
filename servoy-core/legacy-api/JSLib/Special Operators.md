#  Special Operators

## **Supported Clients**

    SmartClient
    WebClient
    NGClient
    MobileClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [typeof()](Special%20Operators.md#typeof)                   | Returns the type of the given object, one of these strings get returned: "number", "string", "boolean", "object", "function" or undefined if the object doesn't exists..                                    |

## Methods Details

### typeof()

Returns the type of the given object, one of these strings get returned: "number", "string", "boolean", "object", "function" or undefined if the object doesn't exists.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
application.output(typeof "abc"); // string
application.output(typeof 10); // number
application.output(typeof 10.1); // number
application.output(typeof true); // boolean
application.output(typeof parseInt); // function
application.output(typeof application); // object
application.output(typeof somethingInexisting); // undefined
```

