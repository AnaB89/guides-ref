#  RegExp


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](./Boolean.md) | [global](RegExp.md#global)                   | Specifies if the "g" modifier is set..                                    |
| [Boolean](./Boolean.md) | [ignoreCase](RegExp.md#ignoreCase)                   | Specifies if the "i" modifier is set..                                    |
| [Number](./Number.md) | [lastIndex](RegExp.md#lastIndex)                   | An integer specifying the index at which to start the next match..                                    |
| [Boolean](./Boolean.md) | [multiline](RegExp.md#multiline)                   | Specifies if the "m" modifier is set..                                    |
| [String](./String.md) | [source](RegExp.md#source)                   | The text used for pattern matching..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](./String.md) | [exec(string)](RegExp.md#exec-string)                   | Search a string for a specified value..                                    |
| [Boolean](./Boolean.md) | [test(string)](RegExp.md#test-string)                   | Search a string for a specified value..                                    |

## Properties Details

### global

Specifies if the "g" modifier is set.

**Returns**\
[Boolean](./Boolean.md) 


**Sample**

```javascript
var str = 'Visit www.servoy.com';	
var patt1 = new RegExp('www');	
application.output(patt1.global);
```
### ignoreCase

Specifies if the "i" modifier is set.

**Returns**\
[Boolean](./Boolean.md) 


**Sample**

```javascript
var str = 'Visit www.servoy.com';	
var patt1 = new RegExp('www');	
application.output(patt1.ignoreCase);
```
### lastIndex

An integer specifying the index at which to start the next match.

**Returns**\
[Number](./Number.md) 


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
[Boolean](./Boolean.md) 


**Sample**

```javascript
var str = 'Visit www.servoy.com';	
var patt1 = new RegExp('www','m');	
application.output(patt1.multiline);
```
### source

The text used for pattern matching.

**Returns**\
[String](./String.md) 


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
[Object](./Object.md) string  ;

**Returns**\
[String](./String.md) A String representing the found value.


**Sample**

```javascript
var str='Visit www.servoy.com';
var patt=new RegExp('servoy');
application.output(patt.exec(str));
```
### test(string)

Search a string for a specified value. Returns true or false.

**Parameters**\
[Object](./Object.md) string  ;

**Returns**\
[Boolean](./Boolean.md) true if a match was found in the string. false otherwise.


**Sample**

```javascript
var str='Visit www.servoy.com';	
var patt=new RegExp('soft'); 
application.output(patt.test(str)==true);	
patt.compile('servoy');	
application.output(patt.test(str)==true)
```

