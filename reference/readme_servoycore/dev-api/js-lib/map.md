# Map

## Property Summary

| Type                | Name                | Summary                                                                     |
| ------------------- | ------------------- | --------------------------------------------------------------------------- |
| [Number](number.md) | [size](map.md#size) | The size accessor property returns the number of elements in a Map object.. |

## Methods Summary

| Type                    | Name                                                                    | Summary                                                                                                                                          |
| ----------------------- | ----------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| void                    | [clear()](map.md#clear)                                                 | The clear() method removes all elements from a Map object..                                                                                      |
| [Boolean](boolean.md)   | [delete(key)](map.md#delete-key)                                        | The delete() method removes the specified element from a Map object by key..                                                                     |
| [Iterator](iterator.md) | [entries()](map.md#entries)                                             | The entries() method returns a new iterator object that contains the \[key, value] pairs for each element in the Map object in insertion order.. |
| void                    | [forEach(callback, thisArgument)](map.md#foreach-callback-thisargument) | The forEach() method executes a provided function once for each value in the Map object, in insertion order..                                    |
| [Object](object.md)     | [get(key)](map.md#get-key)                                              | The get() method returns a specified element from a Map object..                                                                                 |
| [Boolean](boolean.md)   | [has(key)](map.md#has-key)                                              | The has() method returns a boolean indicating whether an element with the specified key exists in a Map object or not..                          |
| [Iterator](iterator.md) | [keys()](map.md#keys)                                                   | The keys() method returns a new iterator object that contains the keys for each element in the Map object in insertion order..                   |
| [Map](map.md)           | [set(key, value)](map.md#set-key-value)                                 | The set() method adds or updates an entry in a Map object with a specified key and a value..                                                     |
| [Iterator](iterator.md) | [values()](map.md#values)                                               | The values() method returns a new iterator object that contains the values for each element in the Map object in insertion order..               |

## Properties Details

### size

The size accessor property returns the number of elements in a Map object.

**Returns**\
[Number](number.md)

**Sample**

```javascript
map.size;
```

## Methods Details

### clear()

The clear() method removes all elements from a Map object.

**Returns**\
void

**Sample**

```javascript
map.clear();
```

### delete(key)

The delete() method removes the specified element from a Map object by key.

**Parameters**\
[Object](object.md) key ;

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
var success = map.delete(key);
```

### entries()

The entries() method returns a new iterator object that contains the \[key, value] pairs for each element in the Map object in insertion order. In this particular case, this iterator object is also an iterable, so the for-of loop can be used..

**Returns**\
[Iterator](iterator.md) the iterator that can be used in for of loops

**Sample**

```javascript
for(var entry of map.entries()) {}
```

### forEach(callback, thisArgument)

The forEach() method executes a provided function once for each value in the Map object, in insertion order.

**Parameters**\
[Function](function.md) callback ;\
[Object](object.md) thisArgument ;

**Returns**\
void

**Sample**

```javascript
map.forEach(function(keyValuePair) {});
```

### get(key)

The get() method returns a specified element from a Map object. If the value that is associated to the provided key is an object, then you will get a reference to that object and any change made to that object will effectively modify it inside the Map object.

**Parameters**\
[Object](object.md) key ;

**Returns**\
[Object](object.md)

**Sample**

```javascript
var value = map.get(key);
```

### has(key)

The has() method returns a boolean indicating whether an element with the specified key exists in a Map object or not.

**Parameters**\
[Object](object.md) key ;

**Returns**\
[Boolean](boolean.md)

**Sample**

```javascript
var containsKey = map.has(key);
```

### keys()

The keys() method returns a new iterator object that contains the keys for each element in the Map object in insertion order. In this particular case, this iterator object is also an iterable, so a for...of loop can be used.

**Returns**\
[Iterator](iterator.md) the iterator that can be used in for of loops

**Sample**

```javascript
var values = map.keys();
```

### set(key, value)

The set() method adds or updates an entry in a Map object with a specified key and a value.

**Parameters**\
[Object](object.md) key ;\
[Object](object.md) value ;

**Returns**\
[Map](map.md)

**Sample**

```javascript
map.set(keyObject, value);
```

### values()

The values() method returns a new iterator object that contains the values for each element in the Map object in insertion order.

**Returns**\
[Iterator](iterator.md) the iterator that can be used in for of loops

**Sample**

```javascript
var values = map.values();
```
