#  JS Lib


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](./Number.md) | [Infinity](JS%20Lib.md#Infinity)                   | Numeric value representing infinity..                                    |
| [Number](./Number.md) | [NaN](JS%20Lib.md#NaN)                   | Value representing Not-a-Number..                                    |
| [Object](./Object.md) | [undefined](JS%20Lib.md#undefined)                   | The value undefined..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](./String.md) | [decodeURI(encodedURI)](JS%20Lib.md#decodeuri-encodeduri)                   | Decodes a URI previously encoded with encodeURI or another similar routine..                                    |
| [String](./String.md) | [decodeURIComponent(encodedURI)](JS%20Lib.md#decodeuricomponent-encodeduri)                   | Decodes a URI component previously created by encodeURIComponent or by a similar routine..                                    |
| [String](./String.md) | [encodeURI(URI)](JS%20Lib.md#encodeuri-uri)                   | Encodes a URI by replacing certain characters with escape sequences..                                    |
| [String](./String.md) | [encodeURIComponent(URI)](JS%20Lib.md#encodeuricomponent-uri)                   | Encodes a URI component by replacing all special characters with their corresponding UTF-8 escape sequences..                                    |
| [Object](./Object.md) | [eval(expression)](JS%20Lib.md#eval-expression)                   | Evaluates JavaScript code passed as a string..                                    |
| [Boolean](./Boolean.md) | [isFinite(n)](JS%20Lib.md#isfinite-n)                   | Returns true if the given number is a finite number..                                    |
|void | [isNaN(value)](JS%20Lib.md#isnan-value)                   | The NaN property indicates that a value is 'Not a Number'..                                    |
| [Boolean](./Boolean.md) | [isXMLName(name)](JS%20Lib.md#isxmlname-name)                   | Returns true if the given name can be used as a valid name for an XML element or attribute..                                    |
| [Number](./Number.md) | [parseFloat(text)](JS%20Lib.md#parsefloat-text)                   | Makes a floating point number from the starting numbers in a given string..                                    |
| [Number](./Number.md) | [parseInt(text)](JS%20Lib.md#parseint-text)                   | Makes a integer from the starting numbers in a given string in the base specified..                                    |
| [Number](./Number.md) | [parseInt(text, radix)](JS%20Lib.md#parseint-text-radix)                   | Makes a integer from the starting numbers in a given string in the base specified..                                    |
| [String](./String.md) | [uneval(obj)](JS%20Lib.md#uneval-obj)                   | Returns the string representation behind a given object..                                    |

## Properties Details

### Infinity

Numeric value representing infinity.

**Returns**\
[Number](./Number.md) 


**Sample**

```javascript
Infinity
```
### NaN

Value representing Not-a-Number.

**Returns**\
[Number](./Number.md) 


**Sample**

```javascript
NaN
```
### undefined

The value undefined.

**Returns**\
[Object](./Object.md) 


**Sample**

```javascript
undefined
```

## Methods Details

### decodeURI(encodedURI)

Decodes a URI previously encoded with encodeURI or another similar routine.

**Parameters**\
[String](./String.md) encodedURI  ;

**Returns**\
[String](./String.md) 


**Sample**

```javascript
var str = "http://www.mysite.com/my code.asp?name=[cool]";
var encoded = encodeURI(str);
var decoded = decodeURI(encoded);
application.output(encoded);//http://www.mysite.com/my%20code.asp?name=%5bcool%5d
application.output(decoded);//http://www.mysite.com/my code.asp?name=[cool]
```
### decodeURIComponent(encodedURI)

Decodes a URI component previously created by encodeURIComponent or by a similar routine.

**Parameters**\
[String](./String.md) encodedURI  ;

**Returns**\
[String](./String.md) 


**Sample**

```javascript
var str = "my code.asp?name=[cool]";
var encoded = encodeURIComponent(str);
var decoded = decodeURIComponent(encoded);
application.output(encoded); //my%20code.asp%3fname%3d%5bcool%5d
application.output(decoded); //my code.asp?name=[cool]
```
### encodeURI(URI)

Encodes a URI by replacing certain characters with escape sequences.

**Parameters**\
[String](./String.md) URI  ;

**Returns**\
[String](./String.md) 


**Sample**

```javascript
var str = "http://www.mysite.com/my code.asp?name=[cool]";
var encoded = encodeURI(str);
var decoded = decodeURI(encoded);
application.output(encoded);//http://www.mysite.com/my%20code.asp?name=%5bcool%5d
application.output(decoded);//http://www.mysite.com/my code.asp?name=[cool]
```
### encodeURIComponent(URI)

Encodes a URI component by replacing all special characters with their corresponding UTF-8 escape sequences.

**Parameters**\
[String](./String.md) URI  ;

**Returns**\
[String](./String.md) 


**Sample**

```javascript
var str = "my code.asp?name=[cool]";
var encoded = encodeURIComponent(str);
var decoded = decodeURIComponent(encoded);
application.output(encoded); //my%20code.asp%3fname%3d%5bcool%5d
application.output(decoded); //my code.asp?name=[cool]
```
### eval(expression)

Evaluates JavaScript code passed as a string. Returns the value returned by the evaluated code.

**Parameters**\
[String](./String.md) expression  ;

**Returns**\
[Object](./Object.md) 


**Sample**

```javascript
eval("var x = 2 + 3;");
application.output(x); // prints: 5.0
```
### isFinite(n)

Returns true if the given number is a finite number.

**Parameters**\
[Number](./Number.md) n  ;

**Returns**\
[Boolean](./Boolean.md) 


**Sample**

```javascript
application.output(isFinite(1)); // prints: true
application.output(isFinite(Infinity)); // prints: false
application.output(isFinite(isNaN)); // prints: false
```
### isNaN(value)

The NaN property indicates that a value is 'Not a Number'.

**Parameters**\
[Object](./Object.md) value  ;

**Returns**\
void 


**Sample**

```javascript
isNaN( value )
```
### isXMLName(name)

Returns true if the given name can be used as a valid name for an XML element or attribute.

**Parameters**\
[String](./String.md) name  ;

**Returns**\
[Boolean](./Boolean.md) 


**Sample**

```javascript
application.output(isXMLName("good_name")); // prints: true
application.output(isXMLName("bad name")); // because of the space, prints: false
```
### parseFloat(text)

Makes a floating point number from the starting numbers in a given string.

**Parameters**\
[String](./String.md) text  ;

**Returns**\
[Number](./Number.md) 


**Sample**

```javascript
parseFloat('string')
```
### parseInt(text)

Makes a integer from the starting numbers in a given string in the base specified.

**Parameters**\
[String](./String.md) text  ;

**Returns**\
[Number](./Number.md) 


**Sample**

```javascript
parseInt('0774')
```
### parseInt(text, radix)

Makes a integer from the starting numbers in a given string in the base specified.

**Parameters**\
[String](./String.md) text  ;\
[Number](./Number.md) radix  ;

**Returns**\
[Number](./Number.md) 


**Sample**

```javascript
parseInt('0774' , 8)
```
### uneval(obj)

Returns the string representation behind a given object.

**Parameters**\
[Object](./Object.md) obj  ;

**Returns**\
[String](./String.md) 


**Sample**

```javascript
application.output(uneval(isNaN)); // prints something like: function isNaN() { [native code for isNaN, arity=1] }
```

