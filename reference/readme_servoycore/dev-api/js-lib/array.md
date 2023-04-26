# Array

## Property Summary

| Type                | Name                           | Summary                       |
| ------------------- | ------------------------------ | ----------------------------- |
| [Object](object.md) | [\[index\]](array.md#\[index]) | Get an element by index..     |
| [Number](number.md) | [length](array.md#length)      | Get the length of the array.. |

## Methods Summary

| Type                  | Name                                                                                                         | Summary                                                                                                                 |
| --------------------- | ------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------- |
| [Array](array.md)     | [concat(value1)](array.md#concat-value1)                                                                     | Returns a new array comprised of this array joined with other array(s) and/or value(s)..                                |
| [Array](array.md)     | [concat(value1, value2)](array.md#concat-value1-value2)                                                      | Returns a new array comprised of this array joined with other array(s) and/or value(s)..                                |
| [Array](array.md)     | [concat(value1, value2, valueN)](array.md#concat-value1-value2-valuen)                                       | Returns a new array comprised of this array joined with other array(s) and/or value(s)..                                |
| [Array](array.md)     | [copyWithin(target)](array.md#copywithin-target)                                                             | Shallow copies part of an array to another location in the same array and returns it without modifying its length.      |
| [Array](array.md)     | [copyWithin(target, start)](array.md#copywithin-target-start)                                                | Shallow copies part of an array to another location in the same array and returns it without modifying its length.      |
| [Array](array.md)     | [copyWithin(target, start, end)](array.md#copywithin-target-start-end)                                       | Shallow copies part of an array to another location in the same array and returns it without modifying its length.      |
| [Boolean](boolean.md) | [every(callback)](array.md#every-callback)                                                                   | Runs a function on items in the array while that function is returning true..                                           |
| [Boolean](boolean.md) | [every(callback, thisObject)](array.md#every-callback-thisobject)                                            | Runs a function on items in the array while that function is returning true..                                           |
| [Array](array.md)     | [fill(value)](array.md#fill-value)                                                                           | Changes all elements in an array to a static value, from a start index (default 0) to an end index (default array..     |
| [Array](array.md)     | [fill(value, start)](array.md#fill-value-start)                                                              | Changes all elements in an array to a static value, from a start index (default 0) to an end index (default array..     |
| [Array](array.md)     | [fill(value, start, end)](array.md#fill-value-start-end)                                                     | Changes all elements in an array to a static value, from a start index (default 0) to an end index (default array..     |
| [Array](array.md)     | [filter(callback)](array.md#filter-callback)                                                                 | Runs a function on every item in the array and returns an array of all items for which the function returns true..      |
| [Array](array.md)     | [filter(callback, thisObject)](array.md#filter-callback-thisobject)                                          | Runs a function on every item in the array and returns an array of all items for which the function returns true..      |
| [Object](object.md)   | [find(callback)](array.md#find-callback)                                                                     | Returns the value of the first element in the provided array that satisfies the provided testing function..             |
| [Number](number.md)   | [findIndex(callback)](array.md#findindex-callback)                                                           | Returns the index of the first element in the provided array which satisfies the provided testing function..            |
| void                  | [forEach(callback)](array.md#foreach-callback)                                                               | Runs a function (callback) on every item in the array..                                                                 |
| void                  | [forEach(callback, thisObject)](array.md#foreach-callback-thisobject)                                        | Runs a function (callback) on every item in the array..                                                                 |
| [Array](array.md)     | [from(value)](array.md#from-value)                                                                           | Creates a new, shallow-copied Array instance from an iterable or array-like object..                                    |
| [Array](array.md)     | [from(value, mapFunction, thisObject)](array.md#from-value-mapfunction-thisobject)                           | Creates a new, shallow-copied Array instance from an iterable or array-like object..                                    |
| [Boolean](boolean.md) | [includes(searchElement)](array.md#includes-searchelement)                                                   | Determines whether an array includes a certain value among its entries, returning true or false as appropriate..        |
| [Boolean](boolean.md) | [includes(searchElement, start)](array.md#includes-searchelement-start)                                      | Determines whether an array includes a certain value among its entries, returning true or false as appropriate..        |
| [Number](number.md)   | [indexOf(searchElement)](array.md#indexof-searchelement)                                                     | Returns the first index at which a given element can be found in the array, or -1 if it is not present..                |
| [Number](number.md)   | [indexOf(searchElement, fromIndex)](array.md#indexof-searchelement-fromindex)                                | Returns the first index at which a given element can be found in the array, or -1 if it is not present..                |
| [Boolean](boolean.md) | [isArray(obj)](array.md#isarray-obj)                                                                         | Checks whether an object is an array or not..                                                                           |
| [String](string.md)   | [join(delimiter)](array.md#join-delimiter)                                                                   | Puts all elements in the array into a string, separating each element with the specified delimiter.                     |
| [Number](number.md)   | [lastIndexOf(searchElement)](array.md#lastindexof-searchelement)                                             | Returns the last index at which a given element can be found in the array, or -1 if it is not present..                 |
| [Number](number.md)   | [lastIndexOf(searchElement, fromIndex)](array.md#lastindexof-searchelement-fromindex)                        | Returns the last index at which a given element can be found in the array, or -1 if it is not present..                 |
| [Array](array.md)     | [map(callback)](array.md#map-callback)                                                                       | Runs a function on every item in the array and returns the results in an array..                                        |
| [Array](array.md)     | [map(callback, thisObject)](array.md#map-callback-thisobject)                                                | Runs a function on every item in the array and returns the results in an array..                                        |
| [Array](array.md)     | [of(value)](array.md#of-value)                                                                               | Ccreates a new Array instance from a variable number of arguments..                                                     |
| [Object](object.md)   | [pop()](array.md#pop)                                                                                        | Pops the last string off the array and returns it..                                                                     |
| [Number](number.md)   | [push(value1)](array.md#push-value1)                                                                         | Mutates an array by appending the given elements and returning the new length of the array..                            |
| [Number](number.md)   | [push(value1, value2)](array.md#push-value1-value2)                                                          | Mutates an array by appending the given elements and returning the new length of the array..                            |
| [Number](number.md)   | [push(value1, value2, valueN)](array.md#push-value1-value2-valuen)                                           | Mutates an array by appending the given elements and returning the new length of the array..                            |
| [Object](object.md)   | [reduce(f, initialValue)](array.md#reduce-f-initialvalue)                                                    | Reduces the array to a single value by executing a provided function for each value of the array (from left-to-right).. |
| [Array](array.md)     | [reverse()](array.md#reverse)                                                                                | Puts array elements in reverse order..                                                                                  |
| [Object](object.md)   | [shift()](array.md#shift)                                                                                    | Decreases array element size by one by shifting the first element off the array and returning it..                      |
| [Array](array.md)     | [slice(begin)](array.md#slice-begin)                                                                         | The slice method creates a new array from a selected section of an array..                                              |
| [Array](array.md)     | [slice(begin, end)](array.md#slice-begin-end)                                                                | The slice method creates a new array from a selected section of an array..                                              |
| [Boolean](boolean.md) | [some(callback)](array.md#some-callback)                                                                     | Runs a function on items in the array while that function returns false..                                               |
| [Boolean](boolean.md) | [some(callback, thisObject)](array.md#some-callback-thisobject)                                              | Runs a function on items in the array while that function returns false..                                               |
| [Array](array.md)     | [sort()](array.md#sort)                                                                                      | Sorts the array elements in dictionary order or using a compare function passed to the method..                         |
| [Array](array.md)     | [sort(function)](array.md#sort-function)                                                                     | Sorts the array elements in dictionary order or using a compare function passed to the method..                         |
| [Array](array.md)     | [splice(arrayIndex, length)](array.md#splice-arrayindex-length)                                              | It is used to take elements out of an array and replace them with those specified..                                     |
| [Array](array.md)     | [splice(arrayIndex, length, value1)](array.md#splice-arrayindex-length-value1)                               | It is used to take elements out of an array and replace them with those specified..                                     |
| [Array](array.md)     | [splice(arrayIndex, length, value1, value2)](array.md#splice-arrayindex-length-value1-value2)                | It is used to take elements out of an array and replace them with those specified..                                     |
| [Array](array.md)     | [splice(arrayIndex, length, value1, value2, valueN)](array.md#splice-arrayindex-length-value1-value2-valuen) | It is used to take elements out of an array and replace them with those specified..                                     |
| [Number](number.md)   | [unshift(value1, value2, valueN)](array.md#unshift-value1-value2-valuen)                                     | Places element data at the start of an array..                                                                          |

## Properties Details

### \[index]

Get an element by index.

**Returns**\
[Object](object.md)

**Sample**

```javascript
array[0]
```

### length

Get the length of the array.

**Returns**\
[Number](number.md)

**Sample**

```javascript
array.length
```

## Methods Details

### concat(value1)

Returns a new array comprised of this array joined with other array(s) and/or value(s).

**Parameters**\
[Object](object.md) value1 ;

**Returns**\
[Array](array.md)

**Sample**

```javascript
array.concat();
```

### concat(value1, value2)

Returns a new array comprised of this array joined with other array(s) and/or value(s).

**Parameters**\
[Object](object.md) value1 ;\
[Object](object.md) value2 ;

**Returns**\
[Array](array.md)

**Sample**

```javascript
array.concat();
```

### concat(value1, value2, valueN)

Returns a new array comprised of this array joined with other array(s) and/or value(s).

**Parameters**\
[Object](object.md) value1 ;\
[Object](object.md) value2 ;\
[Object](object.md) valueN ;

**Returns**\
[Array](array.md)

**Sample**

```javascript
array.concat();
```

### copyWithin(target)

Shallow copies part of an array to another location in the same array and returns it without modifying its length

**Parameters**\
[Number](number.md) target Zero-based index at which to copy the sequence to. If negative, target will be counted from the end.

**Returns**\
[Array](array.md)

**Sample**

```javascript
array.copyWithin(2);
```

### copyWithin(target, start)

Shallow copies part of an array to another location in the same array and returns it without modifying its length

**Parameters**\
[Number](number.md) target Zero-based index at which to copy the sequence to. If negative, target will be counted from the end.\
[Number](number.md) start Zero-based index at which to start copying elements from. If negative, start will be counted from the end. If start is omitted, copyWithin will copy from index 0.

**Returns**\
[Array](array.md)

**Sample**

```javascript
array.copyWithin(2);
```

### copyWithin(target, start, end)

Shallow copies part of an array to another location in the same array and returns it without modifying its length

**Parameters**\
[Number](number.md) target Zero-based index at which to copy the sequence to. If negative, target will be counted from the end.\
[Number](number.md) start Zero-based index at which to start copying elements from. If negative, start will be counted from the end. If start is omitted, copyWithin will copy from index 0.\
[Number](number.md) end Zero-based index at which to end copying elements from. copyWithin copies up to but not including end. If negative, end will be counted from the end.

**Returns**\
[Array](array.md)

**Sample**

```javascript
array.copyWithin(2);
```

### every(callback)

Runs a function on items in the array while that function is returning true. It returns true if the function returns true for every item it could visit. The callback function is invoked with three arguments: the element value, the element index, the array being traversed.

**Parameters**\
[Function](function.md) callback ;

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
function isNumber(value) { return typeof value == 'number'; }
var a1 = [1, 2, 3];
application.output(a1.every(isNumber));
var a2 = [1, '2', 3];
application.output(a2.every(isNumber));
```

### every(callback, thisObject)

Runs a function on items in the array while that function is returning true. It returns true if the function returns true for every item it could visit. The callback function is invoked with three arguments: the element value, the element index, the array being traversed.

**Parameters**\
[Function](function.md) callback ;\
[Array](array.md) thisObject ;

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
function isNumber(value) { return typeof value == 'number'; }
var a1 = [1, 2, 3];
application.output(a1.every(isNumber));
var a2 = [1, '2', 3];
application.output(a2.every(isNumber));
```

### fill(value)

Changes all elements in an array to a static value, from a start index (default 0) to an end index (default array.length). It returns the modified array.

**Parameters**\
[Object](object.md) value Value to fill the array with.

**Returns**\
[Array](array.md)

**Sample**

```javascript
array.fill('test');
```

### fill(value, start)

Changes all elements in an array to a static value, from a start index (default 0) to an end index (default array.length). It returns the modified array.

**Parameters**\
[Object](object.md) value Value to fill the array with.\
[Number](number.md) start Zero-based index at which to start filling.

**Returns**\
[Array](array.md)

**Sample**

```javascript
array.fill('test');
```

### fill(value, start, end)

Changes all elements in an array to a static value, from a start index (default 0) to an end index (default array.length). It returns the modified array.

**Parameters**\
[Object](object.md) value Value to fill the array with.\
[Number](number.md) start Zero-based index at which to start filling.\
[Number](number.md) end Zero-based index at which to end filling.

**Returns**\
[Array](array.md)

**Sample**

```javascript
array.fill('test');
```

### filter(callback)

Runs a function on every item in the array and returns an array of all items for which the function returns true. The callback function is invoked with three arguments: the element value, the element index, the array being traversed.

**Parameters**\
[Function](function.md) callback ;

**Returns**\
[Array](array.md)

**Sample**

```javascript
var a1 = ['a', 10, 'b', 20, 'c', 30];
var a2 = a1.filter(function(item) { return typeof item == 'number'; });
application.output(a2);
```

### filter(callback, thisObject)

Runs a function on every item in the array and returns an array of all items for which the function returns true. The callback function is invoked with three arguments: the element value, the element index, the array being traversed.

**Parameters**\
[Function](function.md) callback ;\
[Array](array.md) thisObject ;

**Returns**\
[Array](array.md)

**Sample**

```javascript
var a1 = ['a', 10, 'b', 20, 'c', 30];
var a2 = a1.filter(function(item) { return typeof item == 'number'; });
application.output(a2);
```

### find(callback)

Returns the value of the first element in the provided array that satisfies the provided testing function. If no values satisfy the testing function, undefined is returned. The callback function can invoked with three arguments: the element value, the element index(optional), the array being traversed (optional).

**Parameters**\
[Function](function.md) callback a testing function

**Returns**\
[Object](object.md) the element which satisfies the function or undefined

**Sample**

```javascript
var array1 = [5, 12, 8, 130, 44];
 var found = array1.find(function(element) { return element > 10});
 application.output(found); // prints 12
```

### findIndex(callback)

Returns the index of the first element in the provided array which satisfies the provided testing function. If no values satisfy the testing function, -1 is returned. The callback function can invoked with three arguments: the element value, the element index (optional), the array being traversed (optional).

**Parameters**\
[Function](function.md) callback a testing function

**Returns**\
[Number](number.md) the index of the first element which satisfies the function or -1

**Sample**

```javascript
var array1 = [5, 12, 8, 130, 44];
 var found = array1.findIndex(function(element) { return element > 10});
 application.output(found); // prints 1
```

### forEach(callback)

Runs a function (callback) on every item in the array. The callback function is invoked only for indexes of the array which have assigned values. The callback function is invoked with three arguments: the element value, the element index, the array being traversed.

**Parameters**\
[Function](function.md) callback ;

**Returns**\
void

**Sample**

```javascript
function printThemOut(element, index, array) {
		application.output("a[" + index + "] = " + element);
}
var a = ['a', 'b', 'c'];
a.forEach(printThemOut);
```

### forEach(callback, thisObject)

Runs a function (callback) on every item in the array. The callback function is invoked only for indexes of the array which have assigned values. The callback function is invoked with three arguments: the element value, the element index, the array being traversed.

**Parameters**\
[Function](function.md) callback ;\
[Object](object.md) thisObject ;

**Returns**\
void

**Sample**

```javascript
function printThemOut(element, index, array) {
		application.output("a[" + index + "] = " + element);
}
var a = ['a', 'b', 'c'];
a.forEach(printThemOut);
```

### from(value)

Creates a new, shallow-copied Array instance from an iterable or array-like object.

**Parameters**\
[Object](object.md) value An iterable or array-like object to convert to an array.

**Returns**\
[Array](array.md)

**Sample**

```javascript
var a = Array.from([1, 2, 3]);
```

### from(value, mapFunction, thisObject)

Creates a new, shallow-copied Array instance from an iterable or array-like object.

**Parameters**\
[Object](object.md) value An iterable or array-like object to convert to an array.\
[Function](function.md) mapFunction Map function to call on every element of the array. If provided, every value to be added to the array is first passed through this function, and mapFunction's return value is added to the array instead.\
[Object](object.md) thisObject Value to use as this when executing mapFunction.

**Returns**\
[Array](array.md)

**Sample**

```javascript
var a = Array.from([1, 2, 3]);
```

### includes(searchElement)

Determines whether an array includes a certain value among its entries, returning true or false as appropriate.

**Parameters**\
[Object](object.md) searchElement The value to search for.

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
array.includes('test');
```

### includes(searchElement, start)

Determines whether an array includes a certain value among its entries, returning true or false as appropriate.

**Parameters**\
[Object](object.md) searchElement The value to search for.\
[Number](number.md) start Zero-based index at which to start searching.

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
array.includes('test');
```

### indexOf(searchElement)

Returns the first index at which a given element can be found in the array, or -1 if it is not present.

**Parameters**\
[Object](object.md) searchElement ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
var a = ['a', 'b', 'a', 'b', 'a'];
application.output(a.indexOf('b'));
application.output(a.indexOf('b', 2));
application.output(a.indexOf('z'));
```

### indexOf(searchElement, fromIndex)

Returns the first index at which a given element can be found in the array, or -1 if it is not present.

**Parameters**\
[Object](object.md) searchElement ;\
[Number](number.md) fromIndex ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
var a = ['a', 'b', 'a', 'b', 'a'];
application.output(a.indexOf('b'));
application.output(a.indexOf('b', 2));
application.output(a.indexOf('z'));
```

### isArray(obj)

Checks whether an object is an array or not.

**Parameters**\
[Object](object.md) obj ;

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
var a = [1, 2, 3];
application.output(Array.isArray(a)); //prints true
application.output(Array.isArray(23)); //prints false
```

### join(delimiter)

Puts all elements in the array into a string, separating each element with the specified delimiter

**Parameters**\
[String](string.md) delimiter ;

**Returns**\
[String](string.md)

**Sample**

```javascript
var words = new Array("limit","lines","finish","complete","In","Out");
var jwords = words.join(";");
```

### lastIndexOf(searchElement)

Returns the last index at which a given element can be found in the array, or -1 if it is not present. The array is searched backwards, starting at fromIndex.

**Parameters**\
[Object](object.md) searchElement ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
var a = ['a', 'b', 'c', 'd', 'a', 'b'];
application.output(a.lastIndexOf('b'));
application.output(a.lastIndexOf('b', 4));
application.output(a.lastIndexOf('z'));
```

### lastIndexOf(searchElement, fromIndex)

Returns the last index at which a given element can be found in the array, or -1 if it is not present. The array is searched backwards, starting at fromIndex.

**Parameters**\
[Object](object.md) searchElement ;\
[Number](number.md) fromIndex ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
var a = ['a', 'b', 'c', 'd', 'a', 'b'];
application.output(a.lastIndexOf('b'));
application.output(a.lastIndexOf('b', 4));
application.output(a.lastIndexOf('z'));
```

### map(callback)

Runs a function on every item in the array and returns the results in an array. The callback function is invoked with three arguments: the element value, the element index, the array being traversed.

**Parameters**\
[Object](object.md) callback ;

**Returns**\
[Array](array.md)

**Sample**

```javascript
var a = ['a', 'b', 'c'];
var a2 = a.map(function(item) { return item.toUpperCase(); });
application.output(a2);
```

### map(callback, thisObject)

Runs a function on every item in the array and returns the results in an array. The callback function is invoked with three arguments: the element value, the element index, the array being traversed.

**Parameters**\
[Object](object.md) callback ;\
[Array](array.md) thisObject ;

**Returns**\
[Array](array.md)

**Sample**

```javascript
var a = ['a', 'b', 'c'];
var a2 = a.map(function(item) { return item.toUpperCase(); });
application.output(a2);
```

### of(value)

Ccreates a new Array instance from a variable number of arguments.

**Parameters**\
[Array](array.md) value ;

**Returns**\
[Array](array.md)

**Sample**

```javascript
var a = Array.of(1, 2, 3);
```

### pop()

Pops the last string off the array and returns it.

**Returns**\
[Object](object.md)

**Sample**

```javascript
var words = new Array("limit","lines","finish","complete","In","Out");
var lastword = words.pop();
```

### push(value1)

Mutates an array by appending the given elements and returning the new length of the array.

**Parameters**\
[Object](object.md) value1 ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
var words = new Array("limit","lines","finish","complete");
words.push("In","Out");
```

### push(value1, value2)

Mutates an array by appending the given elements and returning the new length of the array.

**Parameters**\
[Object](object.md) value1 ;\
[Object](object.md) value2 ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
var words = new Array("limit","lines","finish","complete");
words.push("In","Out");
```

### push(value1, value2, valueN)

Mutates an array by appending the given elements and returning the new length of the array.

**Parameters**\
[Object](object.md) value1 ;\
[Object](object.md) value2 ;\
[Object](object.md) valueN ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
var words = new Array("limit","lines","finish","complete");
words.push("In","Out");
```

### reduce(f, initialValue)

Reduces the array to a single value by executing a provided function for each value of the array (from left-to-right).

**Parameters**\
[Function](function.md) f Function to execute on each element in the array, taking four arguments: -accumulator: accumulates the callback's return values; it is the accumulated value previously returned in the last invocation of the callback, or initialValue, if supplied (see below). -currentValue: the current element being processed in the array. -currentIndex (Optional): the index of the current element being processed in the array (starts at index 0, if an initialValue is provided, and at index 1 otherwise) -array (Optional): the array reduce() was called upon.\
[Object](object.md) initialValue Value to use as the first argument to the first call of the callback. If no initial value is supplied, the first element in the array will be used.

**Returns**\
[Object](object.md) Object

**Sample**

```javascript
var euros = [29.76, 41.85, 46.5];
var sum = euros.reduce( function(total, amount) {
  return total + amount
});
```

### reverse()

Puts array elements in reverse order.

**Returns**\
[Array](array.md)

**Sample**

```javascript
var words = new Array("limit","lines","finish","complete","In","Out");
words.reverse();
```

### shift()

Decreases array element size by one by shifting the first element off the array and returning it.

**Returns**\
[Object](object.md)

**Sample**

```javascript
var words = new Array("limit","lines","finish","complete","In","Out");
words.shift();
```

### slice(begin)

The slice method creates a new array from a selected section of an array.

**Parameters**\
[Object](object.md) begin ;

**Returns**\
[Array](array.md)

**Sample**

```javascript
var words = new Array("limit","lines","finish","complete","In","Out");
var nwords1 = words.slice(3, 5);
```

### slice(begin, end)

The slice method creates a new array from a selected section of an array.

**Parameters**\
[Object](object.md) begin ;\
[Object](object.md) end ;

**Returns**\
[Array](array.md)

**Sample**

```javascript
var words = new Array("limit","lines","finish","complete","In","Out");
var nwords1 = words.slice(3, 5);
```

### some(callback)

Runs a function on items in the array while that function returns false. It returns true if the function returns true for any item it could visit. The callback function is invoked with three arguments: the element value, the element index, the array being traversed.

**Parameters**\
[Function](function.md) callback ;

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
function isNumber(value) { return typeof value == 'number'; }
var a1 = [1, 2, 3];
application.output(a1.some(isNumber));
var a2 = [1, '2', 3];
application.output(a2.some(isNumber));
```

### some(callback, thisObject)

Runs a function on items in the array while that function returns false. It returns true if the function returns true for any item it could visit. The callback function is invoked with three arguments: the element value, the element index, the array being traversed.

**Parameters**\
[Function](function.md) callback ;\
[Array](array.md) thisObject ;

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
function isNumber(value) { return typeof value == 'number'; }
var a1 = [1, 2, 3];
application.output(a1.some(isNumber));
var a2 = [1, '2', 3];
application.output(a2.some(isNumber));
```

### sort()

Sorts the array elements in dictionary order or using a compare function passed to the method.

**Returns**\
[Array](array.md)

**Sample**

```javascript
var words = new Array("limit","lines","finish","complete","In","Out");
words.sort();
```

### sort(function)

Sorts the array elements in dictionary order or using a compare function passed to the method.

**Parameters**\
[Function](function.md) function ;

**Returns**\
[Array](array.md)

**Sample**

```javascript
var words = new Array("limit","lines","finish","complete","In","Out");
words.sort();
```

### splice(arrayIndex, length)

It is used to take elements out of an array and replace them with those specified.

**Parameters**\
[Object](object.md) arrayIndex ;\
[Object](object.md) length ;

**Returns**\
[Array](array.md)

**Sample**

```javascript
var words = new Array("limit","lines","finish","complete","In","Out");
var nwords1 = words.splice(3, 2, "done", "On");
```

### splice(arrayIndex, length, value1)

It is used to take elements out of an array and replace them with those specified.

**Parameters**\
[Object](object.md) arrayIndex ;\
[Object](object.md) length ;\
[Object](object.md) value1 ;

**Returns**\
[Array](array.md)

**Sample**

```javascript
var words = new Array("limit","lines","finish","complete","In","Out");
var nwords1 = words.splice(3, 2, "done", "On");
```

### splice(arrayIndex, length, value1, value2)

It is used to take elements out of an array and replace them with those specified.

**Parameters**\
[Object](object.md) arrayIndex ;\
[Object](object.md) length ;\
[Object](object.md) value1 ;\
[Object](object.md) value2 ;

**Returns**\
[Array](array.md)

**Sample**

```javascript
var words = new Array("limit","lines","finish","complete","In","Out");
var nwords1 = words.splice(3, 2, "done", "On");
```

### splice(arrayIndex, length, value1, value2, valueN)

It is used to take elements out of an array and replace them with those specified.

**Parameters**\
[Object](object.md) arrayIndex ;\
[Object](object.md) length ;\
[Object](object.md) value1 ;\
[Object](object.md) value2 ;\
[Object](object.md) valueN ;

**Returns**\
[Array](array.md)

**Sample**

```javascript
var words = new Array("limit","lines","finish","complete","In","Out");
var nwords1 = words.splice(3, 2, "done", "On");
```

### unshift(value1, value2, valueN)

Places element data at the start of an array.

**Parameters**\
[Object](object.md) value1 ;\
[Object](object.md) value2 ;\
[Object](object.md) valueN ;

**Returns**\
[Number](number.md)

**Sample**

```javascript
var words = new Array("finish","complete","In","Out");
words.unshift("limit","lines");
```
