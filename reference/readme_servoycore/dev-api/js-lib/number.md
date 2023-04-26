# Number

## Property Summary

| Type                | Name                                               | Summary                                                              |
| ------------------- | -------------------------------------------------- | -------------------------------------------------------------------- |
| [Number](number.md) | [MAX\_VALUE](number.md#MAX\_VALUE)                 | The largest representable number..                                   |
| [Number](number.md) | [MIN\_VALUE](number.md#MIN\_VALUE)                 | The smallest representable number..                                  |
| [Number](number.md) | [NEGATIVE\_INFINITY](number.md#NEGATIVE\_INFINITY) | Special value representing negative infinity; returned on overflow.. |
| [Object](object.md) | [NaN](number.md#NaN)                               | Special "not a number" value..                                       |
| [Number](number.md) | [POSITIVE\_INFINITY](number.md#POSITIVE\_INFINITY) | Special value representing infinity; returned on overflow..          |

## Methods Summary

| Type                | Name                                                                    | Summary                                                                                                    |
| ------------------- | ----------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| [String](string.md) | [toExponential()](number.md#toexponential)                              | Returns a string representing the number in exponential notation..                                         |
| [String](string.md) | [toExponential(fractionDigits)](number.md#toexponential-fractiondigits) | Returns a string representing the number in exponential notation..                                         |
| [String](string.md) | [toFixed()](number.md#tofixed)                                          | Returns a string representing the number in fixed-point notation..                                         |
| [String](string.md) | [toFixed(digits)](number.md#tofixed-digits)                             | Returns a string representing the number in fixed-point notation..                                         |
| [String](string.md) | [toLocaleString()](number.md#tolocalestring)                            | Converts the number into a string which is suitable for presentation in the given locale..                 |
| [String](string.md) | [toPrecision()](number.md#toprecision)                                  | Returns a string representing the number to a specified precision in fixed-point or exponential notation.. |
| [String](string.md) | [toPrecision(precision)](number.md#toprecision-precision)               | Returns a string representing the number to a specified precision in fixed-point or exponential notation.. |
| [String](string.md) | [toString()](number.md#tostring)                                        | Returns a string representing the specified Number object..                                                |
| [String](string.md) | [toString(radix)](number.md#tostring-radix)                             | Returns a string representing the specified Number object..                                                |

## Properties Details

### MAX\_VALUE

The largest representable number.

**Returns**\
[Number](number.md)

**Sample**

```javascript
application.output("Largest number: " + Number.MAX_VALUE);
```

### MIN\_VALUE

The smallest representable number.

**Returns**\
[Number](number.md)

**Sample**

```javascript
application.output("Smallest number: " + Number.MIN_VALUE);
```

### NEGATIVE\_INFINITY

Special value representing negative infinity; returned on overflow.

**Returns**\
[Number](number.md)

**Sample**

```javascript
application.output("Negative infinity: " + Number.NEGATIVE_INFINITY);
```

### NaN

Special "not a number" value.

**Returns**\
[Object](object.md)

**Sample**

```javascript
application.output("NaN: " + Number.NaN);
```

### POSITIVE\_INFINITY

Special value representing infinity; returned on overflow.

**Returns**\
[Number](number.md)

**Sample**

```javascript
application.output("Positive infinity: " + Number.POSITIVE_INFINITY);
```

## Methods Details

### toExponential()

Returns a string representing the number in exponential notation.

**Returns**\
[String](string.md) A string representing the number in exponential notation.

**Sample**

```javascript
var n = 123.45678;
application.output(n.toExponential(3));
```

### toExponential(fractionDigits)

Returns a string representing the number in exponential notation.

**Parameters**\
[Number](number.md) fractionDigits An integer specifying the number of digits after the decimal point. Defaults to as many digits as necessary to specify the number.

**Returns**\
[String](string.md) A string representing the number in exponential notation.

**Sample**

```javascript
var n = 123.45678;
application.output(n.toExponential(3));
```

### toFixed()

Returns a string representing the number in fixed-point notation.

**Returns**\
[String](string.md) A string representing the number in fixed-point notation.

**Sample**

```javascript
var n = 123.45678;
application.output(n.toFixed(3));
```

### toFixed(digits)

Returns a string representing the number in fixed-point notation.

**Parameters**\
[Number](number.md) digits The number of digits to appear after the decimal point. Defaults to 0.

**Returns**\
[String](string.md) A string representing the number in fixed-point notation.

**Sample**

```javascript
var n = 123.45678;
application.output(n.toFixed(3));
```

### toLocaleString()

Converts the number into a string which is suitable for presentation in the given locale.

**Returns**\
[String](string.md) A string representing the number in the current locale.

**Sample**

```javascript
var n = 1000000;
application.output(n.toLocaleString());
```

### toPrecision()

Returns a string representing the number to a specified precision in fixed-point or exponential notation.

**Returns**\
[String](string.md) A string representing the number to a specified precision in fixed-point or exponential notation.

**Sample**

```javascript
var n = 123.45678;
application.output(n.toPrecision(5));
```

### toPrecision(precision)

Returns a string representing the number to a specified precision in fixed-point or exponential notation.

**Parameters**\
[Number](number.md) precision An integer specifying the number of significant digits.

**Returns**\
[String](string.md) A string representing the number to a specified precision in fixed-point or exponential notation.

**Sample**

```javascript
var n = 123.45678;
application.output(n.toPrecision(5));
```

### toString()

Returns a string representing the specified Number object.

**Returns**\
[String](string.md) A string representing the specified Number object.

**Sample**

```javascript
var n = 7;
application.output(n.toString()); //displays "7"
application.output(n.toString(2)); //displays "111"
```

### toString(radix)

Returns a string representing the specified Number object.

**Parameters**\
[Number](number.md) radix An integer between 2 and 36 specifying the base to use for representing numeric values

**Returns**\
[String](string.md) A string representing the specified Number object.

**Sample**

```javascript
var n = 7;
application.output(n.toString()); //displays "7"
application.output(n.toString(2)); //displays "111"
```
