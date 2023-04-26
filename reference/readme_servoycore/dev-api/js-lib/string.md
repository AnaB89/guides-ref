# String

## Property Summary

| Type                | Name                       | Summary                          |
| ------------------- | -------------------------- | -------------------------------- |
| [Number](number.md) | [length](string.md#length) | Gives the length of the string.. |

## Methods Summary

| Type                  | Name                                                                               | Summary                                                                                                                                             |
| --------------------- | ---------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| [String](string.md)   | [anchor(nameAttribute)](string.md#anchor-nameattribute)                            | returns a copy of the string embedded within an anchor \<A> tag set..                                                                               |
| [String](string.md)   | [big()](string.md#big)                                                             | returns a copy of the string embedded within an \<BIG> tag set..                                                                                    |
| [String](string.md)   | [blink()](string.md#blink)                                                         | returns a copy of the string embedded within an \<BLINK> tag set..                                                                                  |
| [String](string.md)   | [bold()](string.md#bold)                                                           | returns a copy of the string embedded within an \<B> tag set..                                                                                      |
| [Number](number.md)   | [charAt(index)](string.md#charat-index)                                            | returns a character of the string..                                                                                                                 |
| [Number](number.md)   | [charCodeAt(index)](string.md#charcodeat-index)                                    | returns a decimal code of the char in the string..                                                                                                  |
| [Number](number.md)   | [codePointAt(index)](string.md#codepointat-index)                                  | returns a non-negative integer that is the Unicode code point value at the given position..                                                         |
| [String](string.md)   | [concat(string2)](string.md#concat-string2)                                        | returns a string that appends the parameter string to the string..                                                                                  |
| [String](string.md)   | [concat(string2, stringN)](string.md#concat-string2-stringn)                       | returns a string that appends the parameter string to the string..                                                                                  |
| [String](string.md)   | [endsWith(searchString)](string.md#endswith-searchstring)                          | Determines whether a string ends with the characters of a specified string, returning true or false as appropriate..                                |
| [String](string.md)   | [endsWith(searchString, length)](string.md#endswith-searchstring-length)           | Determines whether a string ends with the characters of a specified string, returning true or false as appropriate..                                |
| [Boolean](boolean.md) | [equals(other)](string.md#equals-other)                                            | returns a boolean that checks if the given string is equal to the string.                                                                           |
| [Boolean](boolean.md) | [equalsIgnoreCase(other)](string.md#equalsignorecase-other)                        | returns a boolean that checks if the given string is equal to the string ignoring case.                                                             |
| [String](string.md)   | [fixed()](string.md#fixed)                                                         | returns a copy of the string embedded within an anchor \<TT> tag set..                                                                              |
| [String](string.md)   | [fontcolor(color)](string.md#fontcolor-color)                                      | returns a copy of the string embedded within an \<FONT> tag set, the color param is assigned the the color attribute..                              |
| [String](string.md)   | [fontsize(size)](string.md#fontsize-size)                                          | returns a copy of the string embedded within an \<FONT> tag set, The size param is set to the SIZE attribute.                                       |
| [String](string.md)   | [fromCharCode(num)](string.md#fromcharcode-num)                                    | Static method that returns a string created from the specified sequence of UTF-16 code units..                                                      |
| [String](string.md)   | [fromCodePoint(num)](string.md#fromcodepoint-num)                                  | Static method that returns a string created by using the specified sequence of code points..                                                        |
| [String](string.md)   | [includes()](string.md#includes)                                                   | Determines whether one string may be found within another string..                                                                                  |
| [Number](number.md)   | [indexOf(searchValue, fromIndex)](string.md#indexof-searchvalue-fromindex)         | returns the found index of the given string in string..                                                                                             |
| [String](string.md)   | [italics()](string.md#italics)                                                     | returns a copy of the string embedded within an \<I> tag set.                                                                                       |
| [Number](number.md)   | [lastIndexOf(searchValue, fromIndex)](string.md#lastindexof-searchvalue-fromindex) | returns the found index of the given string in string from the end..                                                                                |
| [String](string.md)   | [link(hrefAttribute)](string.md#link-hrefattribute)                                | returns a copy of the string embedded within an \<A> tag set..                                                                                      |
| [Number](number.md)   | [localeCompare(otherString)](string.md#localecompare-otherstring)                  | .                                                                                                                                                   |
| [Array](array.md)     | [match(regexp)](string.md#match-regexp)                                            | returns an array of strings within the current string that matches the regexp..                                                                     |
| [String](string.md)   | [normalize()](string.md#normalize)                                                 | Returns the Unicode Normalization Form of the string..                                                                                              |
| [String](string.md)   | [normalize(form)](string.md#normalize-form)                                        | Returns the Unicode Normalization Form of the string..                                                                                              |
| [String](string.md)   | [padEnd(targetLength)](string.md#padend-targetlength)                              | The padEnd() method pads the current string with a given string (repeated, if needed) so that the resulting string reaches a given length..         |
| [String](string.md)   | [padEnd(targetLength, padString)](string.md#padend-targetlength-padstring)         | The padEnd() method pads the current string with a given string (repeated, if needed) so that the resulting string reaches a given length..         |
| [String](string.md)   | [padStart(targetLength)](string.md#padstart-targetlength)                          | The padStart() method pads the current string with another string (multiple times, if needed) until the resulting string reaches the given length.. |
| [String](string.md)   | [padStart(targetLength, padString)](string.md#padstart-targetlength-padstring)     | The padStart() method pads the current string with another string (multiple times, if needed) until the resulting string reaches the given length.. |
| [String](string.md)   | [repeat(count)](string.md#repeat-count)                                            | Constructs and returns a new string which contains the specified number of copies of the string on which it was called, concatenated together..     |
| [String](string.md)   | [replace(regexp, function)](string.md#replace-regexp-function)                     | returns a new string where the matches of the given regexp are replaced by the return value of the function..                                       |
| [String](string.md)   | [replace(regexp, newSubStr)](string.md#replace-regexp-newsubstr)                   | returns a new string where the matches of the given reg exp are replaced by newSubStr..                                                             |
| [String](string.md)   | [replace(substr, function)](string.md#replace-substr-function)                     | returns a new string where the first match of the given substr is replaced by the return value of the function..                                    |
| [String](string.md)   | [replace(substr, newSubStr)](string.md#replace-substr-newsubstr)                   | returns a new string where the first match of the given substr is replaced by newSubStr..                                                           |
| [Number](number.md)   | [search(regexp)](string.md#search-regexp)                                          | returns an index where the first match is found of the regexp.                                                                                      |
| [String](string.md)   | [slice(beginSlice)](string.md#slice-beginslice)                                    | returns a substring of the string..                                                                                                                 |
| [String](string.md)   | [slice(beginSlice, endSlice)](string.md#slice-beginslice-endslice)                 | returns a substring of the string..                                                                                                                 |
| [String](string.md)   | [small()](string.md#small)                                                         | returns a copy of the string embedded within an \<SMALL> tag set..                                                                                  |
| [String](string.md)   | [split(separator, limit)](string.md#split-separator-limit)                         | returns an array of objects whose elements are segments of the current string..                                                                     |
| [String](string.md)   | [split(separator, limit)](string.md#split-separator-limit)                         | returns an array of objects whose elements are segments of the current string..                                                                     |
| [String](string.md)   | [startsWith(searchString)](string.md#startswith-searchstring)                      | Determines whether a string begins with the characters of a specified string, returning true or false as appropriate..                              |
| [String](string.md)   | [startsWith(searchString, position)](string.md#startswith-searchstring-position)   | Determines whether a string begins with the characters of a specified string, returning true or false as appropriate..                              |
| [String](string.md)   | [strike()](string.md#strike)                                                       | returns a copy of the string embedded within an \<STRIKE> tag set..                                                                                 |
| [String](string.md)   | [sub()](string.md#sub)                                                             | returns a copy of the string embedded within an \<SUB> tag set..                                                                                    |
| [String](string.md)   | [substr(start)](string.md#substr-start)                                            | returns a substring of the string from the start with the number of chars specified..                                                               |
| [String](string.md)   | [substr(start, length)](string.md#substr-start-length)                             | returns a substring of the string from the start with the number of chars specified..                                                               |
| [String](string.md)   | [substring(indexA)](string.md#substring-indexa)                                    | Returns a substring of the string from the start index until the end index..                                                                        |
| [String](string.md)   | [substring(indexA, indexB)](string.md#substring-indexa-indexb)                     | Returns a substring of the string from the start index until the end index..                                                                        |
| [String](string.md)   | [sup()](string.md#sup)                                                             | returns a copy of the string embedded within an \<SUP> tag set..                                                                                    |
| [String](string.md)   | [toLocaleLowerCase()](string.md#tolocalelowercase)                                 | .                                                                                                                                                   |
| [String](string.md)   | [toLocaleUpperCase()](string.md#tolocaleuppercase)                                 | .                                                                                                                                                   |
| [String](string.md)   | [toLowerCase()](string.md#tolowercase)                                             | returns a string with all lowercase letters of the current string..                                                                                 |
| [String](string.md)   | [toUpperCase()](string.md#touppercase)                                             | returns a string with all uppercase letters of the current string..                                                                                 |
| [String](string.md)   | [trim()](string.md#trim)                                                           | Returns the string stripped of whitespace from both ends..                                                                                          |
| [String](string.md)   | [trimEnd()](string.md#trimend)                                                     | Removes whitespace from the ending of a string and returns a new string, without modifying the original string..                                    |
| [String](string.md)   | [trimStart()](string.md#trimstart)                                                 | Removes whitespace from the beginning of a string and returns a new string, without modifying the original string..                                 |

## Properties Details

### length

Gives the length of the string.

**Returns**\
[Number](number.md)

**Sample**

```javascript
string.length;
```

## Methods Details

### anchor(nameAttribute)

returns a copy of the string embedded within an anchor \<A> tag set.

**Parameters**\
[String](string.md) nameAttribute ;

**Returns**\
[String](string.md)

**Sample**

```javascript
string.anchor();
```

### big()

returns a copy of the string embedded within an \<BIG> tag set.

**Returns**\
[String](string.md)

**Sample**

```javascript
string.big();
```

### blink()

returns a copy of the string embedded within an \<BLINK> tag set.

**Returns**\
[String](string.md)

**Sample**

```javascript
string.blink();
```

### bold()

returns a copy of the string embedded within an \<B> tag set.

**Returns**\
[String](string.md)

**Sample**

```javascript
string.bold();
```

### charAt(index)

returns a character of the string.

**Parameters**\
[Number](number.md) index ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
string.charAt(integer_position);
```

### charCodeAt(index)

returns a decimal code of the char in the string.

**Parameters**\
[Number](number.md) index ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
string.charCodeAt(integer_position);
```

### codePointAt(index)

returns a non-negative integer that is the Unicode code point value at the given position. Note that this function does not give the nth code point in a string, but the code point starting at the specified string index.

**Parameters**\
[Number](number.md) index ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
string.codePointAt(integer_position);
```

### concat(string2)

returns a string that appends the parameter string to the string.

**Parameters**\
[String](string.md) string2 ;

**Returns**\
[String](string.md)

**Sample**

```javascript
string.concat(string);
```

### concat(string2, stringN)

returns a string that appends the parameter string to the string.

**Parameters**\
[String](string.md) string2 ;\
[String](string.md) stringN ;

**Returns**\
[String](string.md)

**Sample**

```javascript
string.concat(string);
```

### endsWith(searchString)

Determines whether a string ends with the characters of a specified string, returning true or false as appropriate.

**Parameters**\
[String](string.md) searchString The characters to be searched for at the end of str.

**Returns**\
[String](string.md) true if the given characters are found at the end of the string; otherwise, false

**Sample**

```javascript
var str1 = 'Cats are the best!';
 application.output(str1.endsWith('best', 17));
```

### endsWith(searchString, length)

Determines whether a string ends with the characters of a specified string, returning true or false as appropriate.

**Parameters**\
[String](string.md) searchString The characters to be searched for at the end of str.\
[Number](number.md) length If provided, it is used as the length of str. Defaults to str.length.

**Returns**\
[String](string.md) true if the given characters are found at the end of the string; otherwise, false

**Sample**

```javascript
var str1 = 'Cats are the best!';
 application.output(str1.endsWith('best', 17));
```

### equals(other)

returns a boolean that checks if the given string is equal to the string

**Parameters**\
[String](string.md) other ;

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
string.equals(string);
```

### equalsIgnoreCase(other)

returns a boolean that checks if the given string is equal to the string ignoring case

**Parameters**\
[String](string.md) other ;

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
string.equalsIgnoreCase(string);
```

### fixed()

returns a copy of the string embedded within an anchor \<TT> tag set.

**Returns**\
[String](string.md)

**Sample**

```javascript
string.fixed();
```

### fontcolor(color)

returns a copy of the string embedded within an \<FONT> tag set, the color param is assigned the the color attribute.

**Parameters**\
[String](string.md) color ;

**Returns**\
[String](string.md)

**Sample**

```javascript
string.fontcolor(color);
```

### fontsize(size)

returns a copy of the string embedded within an \<FONT> tag set, The size param is set to the SIZE attribute

**Parameters**\
[Number](number.md) size ;

**Returns**\
[String](string.md)

**Sample**

```javascript
string.fontsize(size);
```

### fromCharCode(num)

Static method that returns a string created from the specified sequence of UTF-16 code units.

**Parameters**\
[Array](array.md) num A sequence of numbers that are UTF-16 code units. The range is between 0 and 65535 (0xFFFF). Numbers greater than 0xFFFF are truncated. No validity checks are performed.

**Returns**\
[String](string.md) A string of length N consisting of the N specified UTF-16 code units.

**Sample**

```javascript
String.fromCharCode(0x2014); // returns "—"
String.fromCharCode(65, 66, 67); // returns "ABC"
```

### fromCodePoint(num)

Static method that returns a string created by using the specified sequence of code points. String.fromCharCode() cannot return supplementary characters (i.e. code points 0x010000 – 0x10FFFF) by specifying their code point. Instead, it requires the UTF-16 surrogate pair for that. String.fromCodePoint(), on the other hand, can return 4-byte supplementary characters, as well as the more common 2-byte BMP characters, by specifying their code point (which is equivalent to the UTF-32 code unit).

RangeError is thrown if an invalid Unicode code point is given (e.g. "RangeError: NaN is not a valid code point").

**Parameters**\
[Array](array.md) num A sequence of code points.

**Returns**\
[String](string.md) A string created by using the specified sequence of code points.

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
[String](string.md)

**Sample**

```javascript
string.includes('foo');
```

### indexOf(searchValue, fromIndex)

returns the found index of the given string in string.

**Parameters**\
[String](string.md) searchValue ;\
[Number](number.md) fromIndex ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
string.indexOf(string,startPosition);
```

### italics()

returns a copy of the string embedded within an \<I> tag set

**Returns**\
[String](string.md)

**Sample**

```javascript
string.italics();
```

### lastIndexOf(searchValue, fromIndex)

returns the found index of the given string in string from the end.

**Parameters**\
[String](string.md) searchValue ;\
[Number](number.md) fromIndex ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
string.lastIndexOf(string,startPosition);
```

### link(hrefAttribute)

returns a copy of the string embedded within an \<A> tag set.

**Parameters**\
[String](string.md) hrefAttribute ;

**Returns**\
[String](string.md)

**Sample**

```javascript
string.link(url);
```

### localeCompare(otherString)

**Parameters**\
[String](string.md) otherString ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
var s = "Have a nice day!";
application.output(s.localeCompare("Hello"));
```

### match(regexp)

returns an array of strings within the current string that matches the regexp.

**Parameters**\
[RegExp](regexp.md) regexp ;

**Returns**\
[Array](array.md)

**Sample**

```javascript
string.match(regexpr);
```

### normalize()

Returns the Unicode Normalization Form of the string. (defaults to "NFC" form)

**Returns**\
[String](string.md) A string containing the Unicode Normalization Form of the given string.

**Sample**

```javascript
```

### normalize(form)

Returns the Unicode Normalization Form of the string. form param can be one of "NFC", "NFD", "NFKC", or "NFKD", specifying the Unicode Normalization Form. If omitted or undefined, "NFC" is used.

These values have the following meanings:

"NFC" Canonical Decomposition, followed by Canonical Composition. "NFD" Canonical Decomposition. "NFKC" Compatibility Decomposition, followed by Canonical Composition. "NFKD" Compatibility Decomposition.

**Parameters**\
[String](string.md) form param can be one of "NFC", "NFD", "NFKC", or "NFKD",

**Returns**\
[String](string.md) A string containing the Unicode Normalization Form of the given string.

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

The padEnd() method pads the current string with a given string (repeated, if needed) so that the resulting string reaches a given length. The padding is applied from the end of the current string. The default value used for padding is the unicode "space" character (U+0020) - if no padString argument is used.

**Parameters**\
[Number](number.md) targetLength The length of the resulting string once the current str has been padded. If the value is less than or equal to str.length, then str is returned as-is.

**Returns**\
[String](string.md) A String of the specified targetLength with spaces applied at the end of the current str.

**Sample**

```javascript
string.padEnd(10, '*');
```

### padEnd(targetLength, padString)

The padEnd() method pads the current string with a given string (repeated, if needed) so that the resulting string reaches a given length. The padding is applied from the end of the current string.

**Parameters**\
[Number](number.md) targetLength The length of the resulting string once the current str has been padded. If the value is less than or equal to str.length, then str is returned as-is.\
[String](string.md) padString The string to pad the current str with. If padString is too long to stay within the targetLength, it will be truncated from the end. The default value is the unicode "space" character (U+0020).

**Returns**\
[String](string.md) A String of the specified targetLength with the padString applied at the end of the current str.

**Sample**

```javascript
string.padEnd(10, '*');
```

### padStart(targetLength)

The padStart() method pads the current string with another string (multiple times, if needed) until the resulting string reaches the given length. The padding is applied from the start of the current string. The default value used for padding is the unicode "space" character (U+0020) - if no padString argument is used.

**Parameters**\
[Number](number.md) targetLength The length of the resulting string once the current str has been padded. If the value is less than or equal to str.length, then str is returned as-is.

**Returns**\
[String](string.md) A String of the specified targetLength with spaces applied from the start.

**Sample**

```javascript
string.padStart(10);
```

### padStart(targetLength, padString)

The padStart() method pads the current string with another string (multiple times, if needed) until the resulting string reaches the given length. The padding is applied from the start of the current string.

**Parameters**\
[Number](number.md) targetLength The length of the resulting string once the current str has been padded. If the value is less than or equal to str.length, then str is returned as-is.\
[String](string.md) padString The string to pad the current str with. If padString is too long to stay within the targetLength, it will be truncated from the end. The default value is the unicode "space" character (U+0020).

**Returns**\
[String](string.md) A String of the specified targetLength with padString applied from the start.

**Sample**

```javascript
string.padStart(10, '*');
```

### repeat(count)

Constructs and returns a new string which contains the specified number of copies of the string on which it was called, concatenated together.

**Parameters**\
[Number](number.md) count An integer between 0 and +Infinity, indicating the number of times to repeat the string.

**Returns**\
[String](string.md) A new string containing the specified number of copies of the given string.

**Sample**

```javascript
var str = 'abc'.repeat(2); // 'abcabc'
```

### replace(regexp, function)

returns a new string where the matches of the given regexp are replaced by the return value of the function. The function parameter is the function to be invoked to create the new substring (to put in place of the substring received from parameter #1).

**Parameters**\
[RegExp](regexp.md) regexp ;\
[Function](function.md) function ;

**Returns**\
[String](string.md)

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
[RegExp](regexp.md) regexp ;\
[String](string.md) newSubStr ;

**Returns**\
[String](string.md)

**Sample**

```javascript
string.replace(regexp,newSubStr);
//var re = /(\w+)\s(\w+)/;
//var str = "John Smith";
//var newstr = str.replace(re, "$2, $1");
//application.output(newstr);
```

### replace(substr, function)

returns a new string where the first match of the given substr is replaced by the return value of the function. The function parameter is the function to be invoked to create the new substring (to put in place of the substring received from parameter #1).

**Parameters**\
[String](string.md) substr ;\
[Function](function.md) function ;

**Returns**\
[String](string.md)

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
[String](string.md) substr ;\
[String](string.md) newSubStr ;

**Returns**\
[String](string.md)

**Sample**

```javascript
string.replace(substr,newSubStr);
```

### search(regexp)

returns an index where the first match is found of the regexp

**Parameters**\
[RegExp](regexp.md) regexp ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
string.search(regexpr);
```

### slice(beginSlice)

returns a substring of the string.

**Parameters**\
[Number](number.md) beginSlice ;

**Returns**\
[String](string.md)

**Sample**

```javascript
string.slice(start,end);
```

### slice(beginSlice, endSlice)

returns a substring of the string.

**Parameters**\
[Number](number.md) beginSlice ;\
[Number](number.md) endSlice ;

**Returns**\
[String](string.md)

**Sample**

```javascript
string.slice(start,end);
```

### small()

returns a copy of the string embedded within an \<SMALL> tag set.

**Returns**\
[String](string.md)

**Sample**

```javascript
string.small();
```

### split(separator, limit)

returns an array of objects whose elements are segments of the current string.

**Parameters**\
[RegExp](regexp.md) separator Specifies the string which denotes the points at which each split should occur. If separator is an empty string, str is converted to an array of characters.\
[Number](number.md) limit Optional integer specifying a limit on the number of splits to be found.

**Returns**\
[String](string.md)

**Sample**

```javascript
var myString = 'Hello 1 word. Sentence number 2.';
var splits = myString.split(new RegExp(/(\d)/), 2);
application.output(splits); //prints [Hello , 1]
```

### split(separator, limit)

returns an array of objects whose elements are segments of the current string.

**Parameters**\
[String](string.md) separator Specifies the string which denotes the points at which each split should occur. If separator is an empty string, str is converted to an array of characters.\
[Number](number.md) limit Optional integer specifying a limit on the number of splits to be found.

**Returns**\
[String](string.md)

**Sample**

```javascript
var myString = 'Hello 1 word. Sentence number 2.';
var splits = myString.split(' ');
application.output(splits);
```

### startsWith(searchString)

Determines whether a string begins with the characters of a specified string, returning true or false as appropriate.

**Parameters**\
[String](string.md) searchString The characters to be searched for at the start of this string.

**Returns**\
[String](string.md) true if the given characters are found at the beginning of the string; otherwise, false

**Sample**

```javascript
var str1 = 'Cats are the best!';
 application.output(str1.startsWith('Cats'));
```

### startsWith(searchString, position)

Determines whether a string begins with the characters of a specified string, returning true or false as appropriate.

**Parameters**\
[String](string.md) searchString The characters to be searched for at the start of this string.\
[Number](number.md) position The position in this string at which to begin searching for searchString. Defaults to 0.

**Returns**\
[String](string.md) true if the given characters are found at the beginning of the string; otherwise, false

**Sample**

```javascript
var str1 = 'Cats are the best!';
 application.output(str1.startsWith('Cats'));
```

### strike()

returns a copy of the string embedded within an \<STRIKE> tag set.

**Returns**\
[String](string.md)

**Sample**

```javascript
string.strike();
```

### sub()

returns a copy of the string embedded within an \<SUB> tag set.

**Returns**\
[String](string.md)

**Sample**

```javascript
string.sub();
```

### substr(start)

returns a substring of the string from the start with the number of chars specified.

**Parameters**\
[Number](number.md) start ;

**Returns**\
[String](string.md)

**Sample**

```javascript
string.substr(start, number_of_chars);
```

### substr(start, length)

returns a substring of the string from the start with the number of chars specified.

**Parameters**\
[Number](number.md) start ;\
[Number](number.md) length ;

**Returns**\
[String](string.md)

**Sample**

```javascript
string.substr(start, number_of_chars);
```

### substring(indexA)

Returns a substring of the string from the start index until the end index.

**Parameters**\
[Number](number.md) indexA ;

**Returns**\
[String](string.md)

**Sample**

```javascript
string.substring(start, end);
```

### substring(indexA, indexB)

Returns a substring of the string from the start index until the end index.

**Parameters**\
[Number](number.md) indexA ;\
[Number](number.md) indexB ;

**Returns**\
[String](string.md)

**Sample**

```javascript
string.substring(start, end);
```

### sup()

returns a copy of the string embedded within an \<SUP> tag set.

**Returns**\
[String](string.md)

**Sample**

```javascript
string.sup();
```

### toLocaleLowerCase()

**Returns**\
[String](string.md)

**Sample**

```javascript
var s = "Have a nice day!";
application.output(s.toLocaleLowerCase());
```

### toLocaleUpperCase()

**Returns**\
[String](string.md)

**Sample**

```javascript
var s = "Have a nice day!";
application.output(s.toLocaleUpperCase());
```

### toLowerCase()

returns a string with all lowercase letters of the current string.

**Returns**\
[String](string.md)

**Sample**

```javascript
string.toLowerCase();
```

### toUpperCase()

returns a string with all uppercase letters of the current string.

**Returns**\
[String](string.md)

**Sample**

```javascript
string.toUpperCase();
```

### trim()

Returns the string stripped of whitespace from both ends.

**Returns**\
[String](string.md)

**Sample**

```javascript
string.trim();
```

### trimEnd()

Removes whitespace from the ending of a string and returns a new string, without modifying the original string.

**Returns**\
[String](string.md)

**Sample**

```javascript
string.trimEnd();
```

### trimStart()

Removes whitespace from the beginning of a string and returns a new string, without modifying the original string.

**Returns**\
[String](string.md)

**Sample**

```javascript
string.trimStart();
```
