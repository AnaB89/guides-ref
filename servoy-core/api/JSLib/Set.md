#  Set


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](./Number.md) | [size](Set.md#size)                   | The size accessor property returns the number of elements in a Set object..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Set](./Set.md) | [add(value)](Set.md#add-value)                   | The set() method adds or updates an entry in a Set object with a specified key and a value..                                    |
|void | [clear()](Set.md#clear)                   | The clear() method removes all elements from a Set object..                                    |
| [Boolean](./Boolean.md) | [delete(value)](Set.md#delete-value)                   | The delete() method removes the specified element from a Set object by key..                                    |
| [Iterator](./Iterator.md) | [entries()](Set.md#entries)                   | The entries() method returns a new iterator object that contains the [key, value] pairs for each element in the Set object in insertion order..                                    |
|void | [forEach(callback, thisArgument)](Set.md#foreach-callback-thisargument)                   | The forEach() method executes a provided function once for each value in the Set object, in insertion order..                                    |
| [Boolean](./Boolean.md) | [has(key)](Set.md#has-key)                   | The has() method returns a boolean indicating whether an element with the specified value exists in a Set object or not..                                    |
| [Iterator](./Iterator.md) | [keys()](Set.md#keys)                   | The keys() method returns a new iterator object that contains the keys for each element in the Set object in insertion order..                                    |
| [Iterator](./Iterator.md) | [values()](Set.md#values)                   | The values() method returns a new iterator object that contains the values for each element in the Set object in insertion order..                                    |

## Properties Details

### size

The size accessor property returns the number of elements in a Set object.

**Returns**\
[Number](./Number.md) 


**Sample**

```javascript
set.size;
```

## Methods Details

### add(value)

The set() method adds or updates an entry in a Set object with a specified key and a value.

**Parameters**\
[Object](./Object.md) value  ;

**Returns**\
[Set](./Set.md) the Set itself


**Sample**

```javascript
set.add(value);
```
### clear()

The clear() method removes all elements from a Set object.


**Returns**\
void 


**Sample**

```javascript
set.clear();
```
### delete(value)

The delete() method removes the specified element from a Set object by key.

**Parameters**\
[Object](./Object.md) value  ;

**Returns**\
[Boolean](./Boolean.md) 


**Sample**

```javascript
var success = set.delete(key);
```
### entries()

The entries() method returns a new iterator object that contains the [key, value] pairs for each element in the Set object in insertion order. In this particular case, this iterator object is also an iterable, so the for-of loop can be used..


**Returns**\
[Iterator](./Iterator.md) the iterator that can be used in for of loops


**Sample**

```javascript
for(var entry of set.entries()) {}
```
### forEach(callback, thisArgument)

The forEach() method executes a provided function once for each value in the Set object, in insertion order.

**Parameters**\
[Function](./Function.md) callback  ;\
[Object](./Object.md) thisArgument  ;

**Returns**\
void 


**Sample**

```javascript
set.forEach(function(keyValuePair) {});
```
### has(key)

The has() method returns a boolean indicating whether an element with the specified value exists in a Set object or not.

**Parameters**\
[Object](./Object.md) key  ;

**Returns**\
[Boolean](./Boolean.md) 


**Sample**

```javascript
var containsKey = set.has(key);
```
### keys()

The keys() method returns a new iterator object that contains the keys for each element in the Set object in insertion order. In this particular case, this iterator object is also an iterable, so a for...of loop can be used.


**Returns**\
[Iterator](./Iterator.md) the iterator that can be used in for of loops


**Sample**

```javascript
var values = set.keys();
```
### values()

The values() method returns a new iterator object that contains the values for each element in the Set object in insertion order.


**Returns**\
[Iterator](./Iterator.md) the iterator that can be used in for of loops


**Sample**

```javascript
var values = set.values();
```

