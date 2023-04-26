# RegExp

## Property Summary

| Type                  | Name                               | Summary                                                            |
| --------------------- | ---------------------------------- | ------------------------------------------------------------------ |
| [Boolean](boolean.md) | [global](regexp.md#global)         | Specifies if the "g" modifier is set..                             |
| [Boolean](boolean.md) | [ignoreCase](regexp.md#ignoreCase) | Specifies if the "i" modifier is set..                             |
| [Number](number.md)   | [lastIndex](regexp.md#lastIndex)   | An integer specifying the index at which to start the next match.. |
| [Boolean](boolean.md) | [multiline](regexp.md#multiline)   | Specifies if the "m" modifier is set..                             |
| [String](string.md)   | [source](regexp.md#source)         | The text used for pattern matching..                               |

## Methods Summary

| Type                  | Name                                  | Summary                                 |
| --------------------- | ------------------------------------- | --------------------------------------- |
| [String](string.md)   | [exec(string)](regexp.md#exec-string) | Search a string for a specified value.. |
| [Boolean](boolean.md) | [test(string)](regexp.md#test-string) | Search a string for a specified value.. |

## Properties Details

### global

Specifies if the "g" modifier is set.

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
var str = 'Visit www.servoy.com';	
var patt1 = new RegExp('www');	
application.output(patt1.global);
```

### ignoreCase

Specifies if the "i" modifier is set.

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
var str = 'Visit www.servoy.com';	
var patt1 = new RegExp('www');	
application.output(patt1.ignoreCase);
```

### lastIndex

An integer specifying the index at which to start the next match.

**Returns**\
[Number](number.md)

**Sample**

```javascript
var str = 'The rain in Spain stays mainly in the plain';	
var patt1 = new RegExp('ain', 'g');	
patt1.test(str);	
application.output('Match found. index now at: ' + patt1.lastIndex);
```

### multiline

Specifies if the "m" modifier is set.

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
var str = 'Visit www.servoy.com';	
var patt1 = new RegExp('www','m');	
application.output(patt1.multiline);
```

### source

The text used for pattern matching.

**Returns**\
[String](string.md)

**Sample**

```javascript
var str = 'Visit www.servoy.com';	
var patt1 = new RegExp('www.','g');	
application.output('The regular expression is: ' + patt1.source);
```

## Methods Details

### exec(string)

Search a string for a specified value. Returns the found value and remembers the position.

**Parameters**\
[Object](object.md) string ;

**Returns**\
[String](string.md) A String representing the found value.

**Sample**

```javascript
var str='Visit www.servoy.com';
var patt=new RegExp('servoy');
application.output(patt.exec(str));
```

### test(string)

Search a string for a specified value. Returns true or false.

**Parameters**\
[Object](object.md) string ;

**Returns**\
[Boolean](boolean.md) true if a match was found in the string. false otherwise.

**Sample**

```javascript
var str='Visit www.servoy.com';	
var patt=new RegExp('soft'); 
application.output(patt.test(str)==true);	
patt.compile('servoy');	
application.output(patt.test(str)==true)
```
