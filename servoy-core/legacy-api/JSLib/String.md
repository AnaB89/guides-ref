#  String

## **Supported Clients**

    SmartClient
    WebClient
    NGClient
    MobileClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](./Number.md) | [length](String.md#length)                   | Gives the length of the string..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](./String.md) | [anchor(nameAttribute)](String.md#anchor-nameattribute)                   | returns a copy of the string embedded within an anchor &lt;A&gt; tag set..                                    |
| [String](./String.md) | [big()](String.md#big)                   | returns a copy of the string embedded within an &lt;BIG&gt; tag set..                                    |
| [String](./String.md) | [blink()](String.md#blink)                   | returns a copy of the string embedded within an &lt;BLINK&gt; tag set..                                    |
| [String](./String.md) | [bold()](String.md#bold)                   | returns a copy of the string embedded within an &lt;B&gt; tag set..                                    |
| [Number](./Number.md) | [charAt(index)](String.md#charat-index)                   | returns a character of the string..                                    |
| [Number](./Number.md) | [charCodeAt(index)](String.md#charcodeat-index)                   | returns a decimal code of the char in the string..                                    |
| [Number](./Number.md) | [codePointAt(index)](String.md#codepointat-index)                   | returns a non-negative integer that is the Unicode code point value at the given position..                                    |
| [String](./String.md) | [concat(string2)](String.md#concat-string2)                   | returns a string that appends the parameter string to the string..                                    |
| [String](./String.md) | [concat(string2, stringN)](String.md#concat-string2-stringn)                   | returns a string that appends the parameter string to the string..                                    |
| [String](./String.md) | [endsWith(searchString)](String.md#endswith-searchstring)                   | Determines whether a string ends with the characters of a specified string, returning true or false as appropriate..                                    |
| [String](./String.md) | [endsWith(searchString, length)](String.md#endswith-searchstring-length)                   | Determines whether a string ends with the characters of a specified string, returning true or false as appropriate..                                    |
| [Boolean](./Boolean.md) | [equals(other)](String.md#equals-other)                   | returns a boolean that checks if the given string is equal to the string.                                    |
| [Boolean](./Boolean.md) | [equalsIgnoreCase(other)](String.md#equalsignorecase-other)                   | returns a boolean that checks if the given string is equal to the string ignoring case.                                    |
| [String](./String.md) | [fixed()](String.md#fixed)                   | returns a copy of the string embedded within an anchor &lt;TT&gt; tag set..                                    |
| [String](./String.md) | [fontcolor(color)](String.md#fontcolor-color)                   | returns a copy of the string embedded within an &lt;FONT&gt; tag set, the color param is assigned the the color attribute..                                    |
| [String](./String.md) | [fontsize(size)](String.md#fontsize-size)                   | returns a copy of the string embedded within an &lt;FONT&gt; tag set, The size param is set to the SIZE attribute.                                    |
| [String](./String.md) | [fromCharCode(num)](String.md#fromcharcode-num)                   | Static method that returns a string created from the specified sequence of UTF-16 code units..                                    |
| [String](./String.md) | [fromCodePoint(num)](String.md#fromcodepoint-num)                   | Static method that returns a string created by using the specified sequence of code points..                                    |
| [String](./String.md) | [includes()](String.md#includes)                   | Determines whether one string may be found within another string..                                    |
| [Number](./Number.md) | [indexOf(searchValue, fromIndex)](String.md#indexof-searchvalue-fromindex)                   | returns the found index of the given string in string..                                    |
| [String](./String.md) | [italics()](String.md#italics)                   | returns a copy of the string embedded within an &lt;I&gt; tag set.                                    |
| [Number](./Number.md) | [lastIndexOf(searchValue, fromIndex)](String.md#lastindexof-searchvalue-fromindex)                   | returns the found index of the given string in string from the end..                                    |
| [String](./String.md) | [link(hrefAttribute)](String.md#link-hrefattribute)                   | returns a copy of the string embedded within an &lt;A&gt; tag set..                                    |
| [Number](./Number.md) | [localeCompare(otherString)](String.md#localecompare-otherstring)                   | .                                    |
| [Array](./Array.md) | [match(regexp)](String.md#match-regexp)                   | returns an array of strings within the current string that matches the regexp..                                    |
| [String](./String.md) | [normalize()](String.md#normalize)                   | Returns the Unicode Normalization Form of the string..                                    |
| [String](./String.md) | [normalize(form)](String.md#normalize-form)                   | Returns the Unicode Normalization Form of the string..                                    |
| [String](./String.md) | [padEnd(targetLength)](String.md#padend-targetlength)                   | The padEnd() method pads the current string with a given string (repeated, if needed) so that the resulting string reaches a given length..                                    |
| [String](./String.md) | [padEnd(targetLength, padString)](String.md#padend-targetlength-padstring)                   | The padEnd() method pads the current string with a given string (repeated, if needed) so that the resulting string reaches a given length..                                    |
| [String](./String.md) | [padStart(targetLength)](String.md#padstart-targetlength)                   | The padStart() method pads the current string with another string (multiple times, if needed) until the resulting string reaches the given length..                                    |
| [String](./String.md) | [padStart(targetLength, padString)](String.md#padstart-targetlength-padstring)                   | The padStart() method pads the current string with another string (multiple times, if needed) until the resulting string reaches the given length..                                    |
| [String](./String.md) | [repeat(count)](String.md#repeat-count)                   | Constructs and returns a new string which contains the specified number of copies of the string on which it was called, concatenated together..                                    |
| [String](./String.md) | [replace(regexp, function)](String.md#replace-regexp-function)                   | returns a new string where the matches of the given regexp are replaced by the return value of the function..                                    |
| [String](./String.md) | [replace(regexp, newSubStr)](String.md#replace-regexp-newsubstr)                   | returns a new string where the matches of the given reg exp are replaced by newSubStr..                                    |
| [String](./String.md) | [replace(substr, function)](String.md#replace-substr-function)                   | returns a new string where the first match of the given substr is replaced by the return value of the function..                                    |
| [String](./String.md) | [replace(substr, newSubStr)](String.md#replace-substr-newsubstr)                   | returns a new string where the first match of the given substr is replaced by newSubStr..                                    |
| [Number](./Number.md) | [search(regexp)](String.md#search-regexp)                   | returns an index where the first match is found of the regexp.                                    |
| [String](./String.md) | [slice(beginSlice)](String.md#slice-beginslice)                   | returns a substring of the string..                                    |
| [String](./String.md) | [slice(beginSlice, endSlice)](String.md#slice-beginslice-endslice)                   | returns a substring of the string..                                    |
| [String](./String.md) | [small()](String.md#small)                   | returns a copy of the string embedded within an &lt;SMALL&gt; tag set..                                    |
| [String](./String.md) | [split(separator, limit)](String.md#split-separator-limit)                   | returns an array of objects whose elements are segments of the current string..                                    |
| [String](./String.md) | [split(separator, limit)](String.md#split-separator-limit)                   | returns an array of objects whose elements are segments of the current string..                                    |
| [String](./String.md) | [startsWith(searchString)](String.md#startswith-searchstring)                   | Determines whether a string begins with the characters of a specified string, returning true or false as appropriate..                                    |
| [String](./String.md) | [startsWith(searchString, position)](String.md#startswith-searchstring-position)                   | Determines whether a string begins with the characters of a specified string, returning true or false as appropriate..                                    |
| [String](./String.md) | [strike()](String.md#strike)                   | returns a copy of the string embedded within an &lt;STRIKE&gt; tag set..                                    |
| [String](./String.md) | [sub()](String.md#sub)                   | returns a copy of the string embedded within an &lt;SUB&gt; tag set..                                    |
| [String](./String.md) | [substr(start)](String.md#substr-start)                   | returns a substring of the string from the start with the number of chars specified..                                    |
| [String](./String.md) | [substr(start, length)](String.md#substr-start-length)                   | returns a substring of the string from the start with the number of chars specified..                                    |
| [String](./String.md) | [substring(indexA)](String.md#substring-indexa)                   | Returns a substring of the string from the start index until the end index..                                    |
| [String](./String.md) | [substring(indexA, indexB)](String.md#substring-indexa-indexb)                   | Returns a substring of the string from the start index until the end index..                                    |
| [String](./String.md) | [sup()](String.md#sup)                   | returns a copy of the string embedded within an &lt;SUP&gt; tag set..                                    |
| [String](./String.md) | [toLocaleLowerCase()](String.md#tolocalelowercase)                   | .                                    |
| [String](./String.md) | [toLocaleUpperCase()](String.md#tolocaleuppercase)                   | .                                    |
| [String](./String.md) | [toLowerCase()](String.md#tolowercase)                   | returns a string with all lowercase letters of the current string..                                    |
| [String](./String.md) | [toUpperCase()](String.md#touppercase)                   | returns a string with all uppercase letters of the current string..                                    |
| [String](./String.md) | [trim()](String.md#trim)                   | Returns the string stripped of whitespace from both ends..                                    |
| [String](./String.md) | [trimEnd()](String.md#trimend)                   | Removes whitespace from the ending of a string and returns a new string, without modifying the original string..                                    |
| [String](./String.md) | [trimStart()](String.md#trimstart)                   | Removes whitespace from the beginning of a string and returns a new string, without modifying the original string..                                    |

## Properties Details

### length

Gives the length of the string.

**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.length;
```

## Methods Details

### anchor(nameAttribute)

returns a copy of the string embedded within an anchor &lt;A&gt; tag set.

**Parameters**\
[String](./String.md) nameAttribute  ;

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.anchor();
```
### big()

returns a copy of the string embedded within an &lt;BIG&gt; tag set.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.big();
```
### blink()

returns a copy of the string embedded within an &lt;BLINK&gt; tag set.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.blink();
```
### bold()

returns a copy of the string embedded within an &lt;B&gt; tag set.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.bold();
```
### charAt(index)

returns a character of the string.

**Parameters**\
[Number](./Number.md) index  ;

**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.charAt(integer_position);
```
### charCodeAt(index)

returns a decimal code of the char in the string.

**Parameters**\
[Number](./Number.md) index  ;

**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.charCodeAt(integer_position);
```
### codePointAt(index)

returns a non-negative integer that is the Unicode code point value at the given position. Note that this function does not give the nth code point in a string, but the code point starting at the specified string index.

**Parameters**\
[Number](./Number.md) index  ;

**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.codePointAt(integer_position);
```
### concat(string2)

returns a string that appends the parameter string to the string.

**Parameters**\
[String](./String.md) string2  ;

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.concat(string);
```
### concat(string2, stringN)

returns a string that appends the parameter string to the string.

**Parameters**\
[String](./String.md) string2  ;\
[String](./String.md) stringN  ;

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.concat(string);
```
### endsWith(searchString)

Determines whether a string ends with the characters of a specified string, returning true or false as appropriate.

**Parameters**\
[String](./String.md) searchString The characters to be searched for at the end of str.

**Returns**\
[String](./String.md) true if the given characters are found at the end of the string; otherwise, false

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var str1 = 'Cats are the best!';
 application.output(str1.endsWith('best', 17));
```
### endsWith(searchString, length)

Determines whether a string ends with the characters of a specified string, returning true or false as appropriate.

**Parameters**\
[String](./String.md) searchString The characters to be searched for at the end of str.\
[Number](./Number.md) length If provided, it is used as the length of str. Defaults to str.length.

**Returns**\
[String](./String.md) true if the given characters are found at the end of the string; otherwise, false

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var str1 = 'Cats are the best!';
 application.output(str1.endsWith('best', 17));
```
### equals(other)

returns a boolean that checks if the given string is equal to the string

**Parameters**\
[String](./String.md) other  ;

**Returns**\
[Boolean](./Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.equals(string);
```
### equalsIgnoreCase(other)

returns a boolean that checks if the given string is equal to the string ignoring case

**Parameters**\
[String](./String.md) other  ;

**Returns**\
[Boolean](./Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.equalsIgnoreCase(string);
```
### fixed()

returns a copy of the string embedded within an anchor &lt;TT&gt; tag set.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.fixed();
```
### fontcolor(color)

returns a copy of the string embedded within an &lt;FONT&gt; tag set, the color param is assigned the the color attribute.

**Parameters**\
[String](./String.md) color  ;

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.fontcolor(color);
```
### fontsize(size)

returns a copy of the string embedded within an &lt;FONT&gt; tag set, The size param is set to the SIZE attribute

**Parameters**\
[Number](./Number.md) size  ;

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.fontsize(size);
```
### fromCharCode(num)

Static method that returns a string created from the specified sequence of UTF-16 code units.

**Parameters**\
[Array](./Array.md) num A sequence of numbers that are UTF-16 code units. The range is between 0 and 65535 (0xFFFF). Numbers greater than 0xFFFF are truncated. No validity checks are performed.

**Returns**\
[String](./String.md) A string of length N consisting of the N specified UTF-16 code units.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
String.fromCharCode(0x2014); // returns "—"
String.fromCharCode(65, 66, 67); // returns "ABC"
```
### fromCodePoint(num)

Static method that returns a string created by using the specified sequence of code points.
String.fromCharCode() cannot return supplementary characters (i.e. code points 0x010000 – 0x10FFFF) by specifying their code point. Instead, it requires the UTF-16 surrogate pair for that. String.fromCodePoint(), on the other hand, can return 4-byte supplementary characters, as well as the more common 2-byte BMP characters, by specifying their code point (which is equivalent to the UTF-32 code unit).

RangeError is thrown if an invalid Unicode code point is given (e.g. "RangeError: NaN is not a valid code point").

**Parameters**\
[Array](./Array.md) num A sequence of code points.

**Returns**\
[String](./String.md) A string created by using the specified sequence of code points.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
String.fromCodePoint(42); // "*"
String.fromCodePoint(65, 90); // "AZ"
String.fromCodePoint(0x2f804); // "\uD87E\uDC04"
String.fromCodePoint(-1); // RangeError
String.fromCodePoint(3.14); // RangeError
```
### includes()

Determines whether one string may be found within another string.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.includes('foo');
```
### indexOf(searchValue, fromIndex)

returns the found index of the given string in string.

**Parameters**\
[String](./String.md) searchValue  ;\
[Number](./Number.md) fromIndex  ;

**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.indexOf(string,startPosition);
```
### italics()

returns a copy of the string embedded within an &lt;I&gt; tag set


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.italics();
```
### lastIndexOf(searchValue, fromIndex)

returns the found index of the given string in string from the end.

**Parameters**\
[String](./String.md) searchValue  ;\
[Number](./Number.md) fromIndex  ;

**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.lastIndexOf(string,startPosition);
```
### link(hrefAttribute)

returns a copy of the string embedded within an &lt;A&gt; tag set.

**Parameters**\
[String](./String.md) hrefAttribute  ;

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.link(url);
```
### localeCompare(otherString)



**Parameters**\
[String](./String.md) otherString  ;

**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var s = "Have a nice day!";
application.output(s.localeCompare("Hello"));
```
### match(regexp)

returns an array of strings within the current string that matches the regexp.

**Parameters**\
[RegExp](./RegExp.md) regexp  ;

**Returns**\
[Array](./Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.match(regexpr);
```
### normalize()

Returns the Unicode Normalization Form of the string. (defaults to "NFC" form)


**Returns**\
[String](./String.md) A string containing the Unicode Normalization Form of the given string.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### normalize(form)

Returns the Unicode Normalization Form of the string.
form param can be one of "NFC", "NFD", "NFKC", or "NFKD", specifying the Unicode Normalization Form. If omitted or undefined, "NFC" is used.

These values have the following meanings:

"NFC"
Canonical Decomposition, followed by Canonical Composition.
"NFD"
Canonical Decomposition.
"NFKC"
Compatibility Decomposition, followed by Canonical Composition.
"NFKD"
Compatibility Decomposition.

**Parameters**\
[String](./String.md) form param can be one of "NFC", "NFD", "NFKC", or "NFKD",

**Returns**\
[String](./String.md) A string containing the Unicode Normalization Form of the given string.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var string1 = '\u00F1';           // �
var string2 = '\u006E\u0303';     // �

string1 = string1.normalize('NFD');
string2 = string2.normalize('NFD');

application.output(string1 === string2); // true
application.output(string1.length);      // 2
application.output(string2.length);      // 2
```
### padEnd(targetLength)

The padEnd() method pads the current string with a given string (repeated, if needed) so that the resulting string reaches a given length. The padding is applied from the end of the current string.
The default value used for padding is the unicode "space" character (U+0020) - if no padString argument is used.

**Parameters**\
[Number](./Number.md) targetLength The length of the resulting string once the current str has been padded. If the value is less than or equal to str.length, then str is returned as-is.

**Returns**\
[String](./String.md) A String of the specified targetLength with spaces applied at the end of the current str.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.padEnd(10, '*');
```
### padEnd(targetLength, padString)

The padEnd() method pads the current string with a given string (repeated, if needed) so that the resulting string reaches a given length. The padding is applied from the end of the current string.

**Parameters**\
[Number](./Number.md) targetLength The length of the resulting string once the current str has been padded. If the value is less than or equal to str.length, then str is returned as-is.\
[String](./String.md) padString The string to pad the current str with. If padString is too long to stay within the targetLength, it will be truncated from the end. The default value is the unicode "space" character (U+0020).

**Returns**\
[String](./String.md) A String of the specified targetLength with the padString applied at the end of the current str.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.padEnd(10, '*');
```
### padStart(targetLength)

The padStart() method pads the current string with another string (multiple times, if needed) until the resulting string reaches the given length. The padding is applied from the start of the current string.
The default value used for padding is the unicode "space" character (U+0020) - if no padString argument is used.

**Parameters**\
[Number](./Number.md) targetLength The length of the resulting string once the current str has been padded. If the value is less than or equal to str.length, then str is returned as-is.

**Returns**\
[String](./String.md) A String of the specified targetLength with spaces applied from the start.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.padStart(10);
```
### padStart(targetLength, padString)

The padStart() method pads the current string with another string (multiple times, if needed) until the resulting string reaches the given length. The padding is applied from the start of the current string.

**Parameters**\
[Number](./Number.md) targetLength The length of the resulting string once the current str has been padded. If the value is less than or equal to str.length, then str is returned as-is.\
[String](./String.md) padString The string to pad the current str with. If padString is too long to stay within the targetLength, it will be truncated from the end. The default value is the unicode "space" character (U+0020).

**Returns**\
[String](./String.md) A String of the specified targetLength with padString applied from the start.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.padStart(10, '*');
```
### repeat(count)

Constructs and returns a new string which contains the specified number of copies of the string on which it was called, concatenated together.

**Parameters**\
[Number](./Number.md) count An integer between 0 and +Infinity, indicating the number of times to repeat the string.

**Returns**\
[String](./String.md) A new string containing the specified number of copies of the given string.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var str = 'abc'.repeat(2); // 'abcabc'
```
### replace(regexp, function)

returns a new string where the matches of the given regexp are replaced by the return value of the function.
The function parameter is the function to be invoked to create the new substring (to put in place of the substring received from parameter #1).

**Parameters**\
[RegExp](./RegExp.md) regexp  ;\
[Function](./Function.md) function  ;

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
//the callback definition
function replacer(match, p1, p2, p3, offset, string){
		// match is the matched substring
		// p1 is non-digits, p2 digits, and p3 non-alphanumerics
		// offset is the offset of the matched substring within the total string being examined
		// string is the total string being examined
 	return [p1, p2, p3].join(' - ');
}
// using replace method with replacer callback
newString = "abc12345#$*%".replace(/([^\d]*)(\d*)([^\w]*)/, replacer);
```
### replace(regexp, newSubStr)

returns a new string where the matches of the given reg exp are replaced by newSubStr.

**Parameters**\
[RegExp](./RegExp.md) regexp  ;\
[String](./String.md) newSubStr  ;

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.replace(regexp,newSubStr);
//var re = /(\w+)\s(\w+)/;
//var str = "John Smith";
//var newstr = str.replace(re, "$2, $1");
//application.output(newstr);
```
### replace(substr, function)

returns a new string where the first match of the given substr is replaced by the return value of the function.
The function parameter is the function to be invoked to create the new substring (to put in place of the substring received from parameter #1).

**Parameters**\
[String](./String.md) substr  ;\
[Function](./Function.md) function  ;

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
// the callback definition
function replacer(match){
		return match.toUpperCase()
}
// using replace method with replacer callback
var newString = "abc".replace("a", replacer);
```
### replace(substr, newSubStr)

returns a new string where the first match of the given substr is replaced by newSubStr.

**Parameters**\
[String](./String.md) substr  ;\
[String](./String.md) newSubStr  ;

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.replace(substr,newSubStr);
```
### search(regexp)

returns an index where the first match is found of the regexp

**Parameters**\
[RegExp](./RegExp.md) regexp  ;

**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.search(regexpr);
```
### slice(beginSlice)

returns a substring of the string.

**Parameters**\
[Number](./Number.md) beginSlice  ;

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.slice(start,end);
```
### slice(beginSlice, endSlice)

returns a substring of the string.

**Parameters**\
[Number](./Number.md) beginSlice  ;\
[Number](./Number.md) endSlice  ;

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.slice(start,end);
```
### small()

returns a copy of the string embedded within an &lt;SMALL&gt; tag set.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.small();
```
### split(separator, limit)

returns an array of objects whose elements are segments of the current string.

**Parameters**\
[RegExp](./RegExp.md) separator Specifies the string which denotes the points at which each split should occur. If separator is an empty string, str is converted to an array of characters.\
[Number](./Number.md) limit Optional integer specifying a limit on the number of splits to be found.

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var myString = 'Hello 1 word. Sentence number 2.';
var splits = myString.split(new RegExp(/(\d)/), 2);
application.output(splits); //prints [Hello , 1]
```
### split(separator, limit)

returns an array of objects whose elements are segments of the current string.

**Parameters**\
[String](./String.md) separator Specifies the string which denotes the points at which each split should occur. If separator is an empty string, str is converted to an array of characters.\
[Number](./Number.md) limit Optional integer specifying a limit on the number of splits to be found.

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var myString = 'Hello 1 word. Sentence number 2.';
var splits = myString.split(' ');
application.output(splits);
```
### startsWith(searchString)

Determines whether a string begins with the characters of a specified string, returning true or false as appropriate.

**Parameters**\
[String](./String.md) searchString The characters to be searched for at the start of this string.

**Returns**\
[String](./String.md) true if the given characters are found at the beginning of the string; otherwise, false

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var str1 = 'Cats are the best!';
 application.output(str1.startsWith('Cats'));
```
### startsWith(searchString, position)

Determines whether a string begins with the characters of a specified string, returning true or false as appropriate.

**Parameters**\
[String](./String.md) searchString The characters to be searched for at the start of this string.\
[Number](./Number.md) position The position in this string at which to begin searching for searchString. Defaults to 0.

**Returns**\
[String](./String.md) true if the given characters are found at the beginning of the string; otherwise, false

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var str1 = 'Cats are the best!';
 application.output(str1.startsWith('Cats'));
```
### strike()

returns a copy of the string embedded within an &lt;STRIKE&gt; tag set.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.strike();
```
### sub()

returns a copy of the string embedded within an &lt;SUB&gt; tag set.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.sub();
```
### substr(start)

returns a substring of the string from the start with the number of chars specified.

**Parameters**\
[Number](./Number.md) start  ;

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.substr(start, number_of_chars);
```
### substr(start, length)

returns a substring of the string from the start with the number of chars specified.

**Parameters**\
[Number](./Number.md) start  ;\
[Number](./Number.md) length  ;

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.substr(start, number_of_chars);
```
### substring(indexA)

Returns a substring of the string from the start index until the end index.

**Parameters**\
[Number](./Number.md) indexA  ;

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.substring(start, end);
```
### substring(indexA, indexB)

Returns a substring of the string from the start index until the end index.

**Parameters**\
[Number](./Number.md) indexA  ;\
[Number](./Number.md) indexB  ;

**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.substring(start, end);
```
### sup()

returns a copy of the string embedded within an &lt;SUP&gt; tag set.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.sup();
```
### toLocaleLowerCase()




**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var s = "Have a nice day!";
application.output(s.toLocaleLowerCase());
```
### toLocaleUpperCase()




**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var s = "Have a nice day!";
application.output(s.toLocaleUpperCase());
```
### toLowerCase()

returns a string with all lowercase letters of the current string.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.toLowerCase();
```
### toUpperCase()

returns a string with all uppercase letters of the current string.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.toUpperCase();
```
### trim()

Returns the string stripped of whitespace from both ends.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.trim();
```
### trimEnd()

Removes whitespace from the ending of a string and returns a new string, without modifying the original string.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.trimEnd();
```
### trimStart()

Removes whitespace from the beginning of a string and returns a new string, without modifying the original string.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
string.trimStart();
```

