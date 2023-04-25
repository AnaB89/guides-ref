#  Function


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Function](./Function.md) | [constructor](Function.md#constructor)                   | Specifies the function that creates an object's prototype..                                    |
| [Number](./Number.md) | [length](Function.md#length)                   | Specifies the number of arguments expected by the function..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [apply()](Function.md#apply)                   | Applies the method of another object in the context of a different object (the calling object); arguments can be passed as an Array object..                                    |
|void | [bind()](Function.md#bind)                   | Creates a new function which, when called, itself calls this function in the context of the provided value, with a given sequence of arguments preceding any provided when the new function was called..                                    |
|void | [call()](Function.md#call)                   | Calls (executes) a method of another object in the context of a different object (the calling object); arguments can be passed as they are..                                    |
| [String](./String.md) | [toString()](Function.md#tostring)                   | Returns a string representing the source code of the function..                                    |

## Properties Details

### constructor

Specifies the function that creates an object's prototype.

**Returns**\
[Function](./Function.md) 


**Sample**

```javascript
function Tree(name) {
	this.name = name;
}
theTree = new Tree("Redwood");
console.log("theTree.constructor is " + theTree.constructor);
```
### length

Specifies the number of arguments expected by the function.

**Returns**\
[Number](./Number.md) 


**Sample**

```javascript
function addNumbers(x, y){
	if (addNumbers.length == 2) {
		return (x + y);
	} else
		return 0;
}
```

## Methods Details

### apply()

Applies the method of another object in the context of a different object (the calling object); arguments can be passed as an Array object.


**Returns**\
void 


**Sample**

```javascript
function book(name, author) {
	this.name = name;
	this.author = author;
}

function book_with_topic(name, author, topic) {
	this.topic = topic;
	book.apply(this, arguments);
}
book_with_topic.prototype = new book();

var aBook = new book_with_topic("name","author","topic");
```
### bind()

Creates a new function which, when called, itself calls this function in the context of the provided value, with a given sequence of arguments preceding any provided when the new function was called.


**Returns**\
void 


**Sample**

```javascript
var x = 9, 
	module = {
		getX: function() { 
		     return this.x;
		},
		x: 81
	};
//  "module.getX()" called, "module" is "this", "module.x" is returned
module.getX(); // > 81
//  "getX()" called, "this" is global, "x" is returned
getX(); // > 9
//  store a reference with "module" bound as "this"
var boundGetX = getX.bind(module);
//  "boundGetX()" called, "module" is "this" again, "module.x" is returned
boundGetX(); // > 81
```
### call()

Calls (executes) a method of another object in the context of a different object (the calling object); arguments can be passed as they are.


**Returns**\
void 


**Sample**

```javascript
function book(name) {
	this.name = name;
}

function book_with_author(name, author) {
	this.author = author;
	book.call(this, name);
}
book_with_author.prototype = new book();

var aBook = new book_with_author("name","author");
```
### toString()

Returns a string representing the source code of the function. Overrides the Object.toString method.


**Returns**\
[String](./String.md) 


**Sample**

```javascript
function printHello() {
	return "Hello";
}
application.output(printHello.toString());
```

