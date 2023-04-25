#  Number


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](./Number.md) | [MAX_VALUE](Number.md#MAX_VALUE)                   | The largest representable number..                                    |
| [Number](./Number.md) | [MIN_VALUE](Number.md#MIN_VALUE)                   | The smallest representable number..                                    |
| [Number](./Number.md) | [NEGATIVE_INFINITY](Number.md#NEGATIVE_INFINITY)                   | Special value representing negative infinity; returned on overflow..                                    |
| [Object](./Object.md) | [NaN](Number.md#NaN)                   | Special "not a number" value..                                    |
| [Number](./Number.md) | [POSITIVE_INFINITY](Number.md#POSITIVE_INFINITY)                   | Special value representing infinity; returned on overflow..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](./String.md) | [toExponential()](Number.md#toexponential)                   | Returns a string representing the number in exponential notation..                                    |
| [String](./String.md) | [toExponential(fractionDigits)](Number.md#toexponential-fractiondigits)                   | Returns a string representing the number in exponential notation..                                    |
| [String](./String.md) | [toFixed()](Number.md#tofixed)                   | Returns a string representing the number in fixed-point notation..                                    |
| [String](./String.md) | [toFixed(digits)](Number.md#tofixed-digits)                   | Returns a string representing the number in fixed-point notation..                                    |
| [String](./String.md) | [toLocaleString()](Number.md#tolocalestring)                   | Converts the number into a string which is suitable for presentation in the given locale..                                    |
| [String](./String.md) | [toPrecision()](Number.md#toprecision)                   | Returns a string representing the number to a specified precision in fixed-point or exponential notation..                                    |
| [String](./String.md) | [toPrecision(precision)](Number.md#toprecision-precision)                   | Returns a string representing the number to a specified precision in fixed-point or exponential notation..                                    |
| [String](./String.md) | [toString()](Number.md#tostring)                   | Returns a string representing the specified Number object..                                    |
| [String](./String.md) | [toString(radix)](Number.md#tostring-radix)                   | Returns a string representing the specified Number object..                                    |

## Properties Details

### MAX_VALUE

The largest representable number.

**Returns**\
[Number](./Number.md) 


**Sample**

```javascript
application.output("Largest number: " + Number.MAX_VALUE);
```
### MIN_VALUE

The smallest representable number.

**Returns**\
[Number](./Number.md) 


**Sample**

```javascript
application.output("Smallest number: " + Number.MIN_VALUE);
```
### NEGATIVE_INFINITY

Special value representing negative infinity; returned on overflow.

**Returns**\
[Number](./Number.md) 


**Sample**

```javascript
application.output("Negative infinity: " + Number.NEGATIVE_INFINITY);
```
### NaN

Special "not a number" value.

**Returns**\
[Object](./Object.md) 


**Sample**

```javascript
application.output("NaN: " + Number.NaN);
```
### POSITIVE_INFINITY

Special value representing infinity; returned on overflow.

**Returns**\
[Number](./Number.md) 


**Sample**

```javascript
application.output("Positive infinity: " + Number.POSITIVE_INFINITY);
```

## Methods Details

### toExponential()

Returns a string representing the number in exponential notation.


**Returns**\
[String](./String.md) A string representing the number in exponential notation.


**Sample**

```javascript
var n = 123.45678;
application.output(n.toExponential(3));
```
### toExponential(fractionDigits)

Returns a string representing the number in exponential notation.

**Parameters**\
[Number](./Number.md) fractionDigits An integer specifying the number of digits after the decimal point. Defaults to as many digits as necessary to specify the number.

**Returns**\
[String](./String.md) A string representing the number in exponential notation.


**Sample**

```javascript
var n = 123.45678;
application.output(n.toExponential(3));
```
### toFixed()

Returns a string representing the number in fixed-point notation.


**Returns**\
[String](./String.md) A string representing the number in fixed-point notation.


**Sample**

```javascript
var n = 123.45678;
application.output(n.toFixed(3));
```
### toFixed(digits)

Returns a string representing the number in fixed-point notation.

**Parameters**\
[Number](./Number.md) digits The number of digits to appear after the decimal point. Defaults to 0.

**Returns**\
[String](./String.md) A string representing the number in fixed-point notation.


**Sample**

```javascript
var n = 123.45678;
application.output(n.toFixed(3));
```
### toLocaleString()

Converts the number into a string which is suitable for presentation in the given locale.


**Returns**\
[String](./String.md) A string representing the number in the current locale.


**Sample**

```javascript
var n = 1000000;
application.output(n.toLocaleString());
```
### toPrecision()

Returns a string representing the number to a specified precision in fixed-point or exponential notation.


**Returns**\
[String](./String.md) A string representing the number to a specified precision in fixed-point or exponential notation.


**Sample**

```javascript
var n = 123.45678;
application.output(n.toPrecision(5));
```
### toPrecision(precision)

Returns a string representing the number to a specified precision in fixed-point or exponential notation.

**Parameters**\
[Number](./Number.md) precision An integer specifying the number of significant digits.

**Returns**\
[String](./String.md) A string representing the number to a specified precision in fixed-point or exponential notation.


**Sample**

```javascript
var n = 123.45678;
application.output(n.toPrecision(5));
```
### toString()

Returns a string representing the specified Number object.


**Returns**\
[String](./String.md) A string representing the specified Number object.


**Sample**

```javascript
var n = 7;
application.output(n.toString()); //displays "7"
application.output(n.toString(2)); //displays "111"
```
### toString(radix)

Returns a string representing the specified Number object.

**Parameters**\
[Number](./Number.md) radix An integer between 2 and 36 specifying the base to use for representing numeric values

**Returns**\
[String](./String.md) A string representing the specified Number object.


**Sample**

```javascript
var n = 7;
application.output(n.toString()); //displays "7"
application.output(n.toString(2)); //displays "111"
```

