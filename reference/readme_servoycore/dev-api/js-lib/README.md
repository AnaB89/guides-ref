# JS Lib

## Property Summary

| Type                | Name                      | Summary                               |
| ------------------- | ------------------------- | ------------------------------------- |
| [Number](number.md) | [Infinity](./#Infinity)   | Numeric value representing infinity.. |
| [Number](number.md) | [NaN](./#NaN)             | Value representing Not-a-Number..     |
| [Object](object.md) | [undefined](./#undefined) | The value undefined..                 |

## Methods Summary

| Type                  | Name                                                               | Summary                                                                                                       |
| --------------------- | ------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------- |
| [String](string.md)   | [decodeURI(encodedURI)](./#decodeuri-encodeduri)                   | Decodes a URI previously encoded with encodeURI or another similar routine..                                  |
| [String](string.md)   | [decodeURIComponent(encodedURI)](./#decodeuricomponent-encodeduri) | Decodes a URI component previously created by encodeURIComponent or by a similar routine..                    |
| [String](string.md)   | [encodeURI(URI)](./#encodeuri-uri)                                 | Encodes a URI by replacing certain characters with escape sequences..                                         |
| [String](string.md)   | [encodeURIComponent(URI)](./#encodeuricomponent-uri)               | Encodes a URI component by replacing all special characters with their corresponding UTF-8 escape sequences.. |
| [Object](object.md)   | [eval(expression)](./#eval-expression)                             | Evaluates JavaScript code passed as a string..                                                                |
| [Boolean](boolean.md) | [isFinite(n)](./#isfinite-n)                                       | Returns true if the given number is a finite number..                                                         |
| void                  | [isNaN(value)](./#isnan-value)                                     | The NaN property indicates that a value is 'Not a Number'..                                                   |
| [Boolean](boolean.md) | [isXMLName(name)](./#isxmlname-name)                               | Returns true if the given name can be used as a valid name for an XML element or attribute..                  |
| [Number](number.md)   | [parseFloat(text)](./#parsefloat-text)                             | Makes a floating point number from the starting numbers in a given string..                                   |
| [Number](number.md)   | [parseInt(text)](./#parseint-text)                                 | Makes a integer from the starting numbers in a given string in the base specified..                           |
| [Number](number.md)   | [parseInt(text, radix)](./#parseint-text-radix)                    | Makes a integer from the starting numbers in a given string in the base specified..                           |
| [String](string.md)   | [uneval(obj)](./#uneval-obj)                                       | Returns the string representation behind a given object..                                                     |

## Properties Details

### Infinity

Numeric value representing infinity.

**Returns**\
[Number](number.md)

**Sample**

```javascript
Infinity
```

### NaN

Value representing Not-a-Number.

**Returns**\
[Number](number.md)

**Sample**

```javascript
NaN
```

### undefined

The value undefined.

**Returns**\
[Object](object.md)

**Sample**

```javascript
undefined
```

## Methods Details

### decodeURI(encodedURI)

Decodes a URI previously encoded with encodeURI or another similar routine.

**Parameters**\
[String](string.md) encodedURI ;

**Returns**\
[String](string.md)

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
[String](string.md) encodedURI ;

**Returns**\
[String](string.md)

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
[String](string.md) URI ;

**Returns**\
[String](string.md)

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
[String](string.md) URI ;

**Returns**\
[String](string.md)

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
[String](string.md) expression ;

**Returns**\
[Object](object.md)

**Sample**

```javascript
eval("var x = 2 + 3;");
application.output(x); // prints: 5.0
```

### isFinite(n)

Returns true if the given number is a finite number.

**Parameters**\
[Number](number.md) n ;

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
application.output(isFinite(1)); // prints: true
application.output(isFinite(Infinity)); // prints: false
application.output(isFinite(isNaN)); // prints: false
```

### isNaN(value)

The NaN property indicates that a value is 'Not a Number'.

**Parameters**\
[Object](object.md) value ;

**Returns**\
void

**Sample**

```javascript
isNaN( value )
```

### isXMLName(name)

Returns true if the given name can be used as a valid name for an XML element or attribute.

**Parameters**\
[String](string.md) name ;

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
application.output(isXMLName("good_name")); // prints: true
application.output(isXMLName("bad name")); // because of the space, prints: false
```

### parseFloat(text)

Makes a floating point number from the starting numbers in a given string.

**Parameters**\
[String](string.md) text ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
parseFloat('string')
```

### parseInt(text)

Makes a integer from the starting numbers in a given string in the base specified.

**Parameters**\
[String](string.md) text ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
parseInt('0774')
```

### parseInt(text, radix)

Makes a integer from the starting numbers in a given string in the base specified.

**Parameters**\
[String](string.md) text ;\
[Number](number.md) radix ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
parseInt('0774' , 8)
```

### uneval(obj)

Returns the string representation behind a given object.

**Parameters**\
[Object](object.md) obj ;

**Returns**\
[String](string.md)

**Sample**

```javascript
application.output(uneval(isNaN)); // prints something like: function isNaN() { [native code for isNaN, arity=1] }
```
