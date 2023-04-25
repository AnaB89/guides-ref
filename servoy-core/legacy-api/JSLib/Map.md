#  Map

## **Supported Clients**

    SmartClient
    WebClient
    NGClient
    MobileClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](./Number.md) | [size](Map.md#size)                   | The size accessor property returns the number of elements in a Map object..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [clear()](Map.md#clear)                   | The clear() method removes all elements from a Map object..                                    |
| [Boolean](./Boolean.md) | [delete(key)](Map.md#delete-key)                   | The delete() method removes the specified element from a Map object by key..                                    |
| [Iterator](./Iterator.md) | [entries()](Map.md#entries)                   | The entries() method returns a new iterator object that contains the [key, value] pairs for each element in the Map object in insertion order..                                    |
|void | [forEach(callback, thisArgument)](Map.md#foreach-callback-thisargument)                   | The forEach() method executes a provided function once for each value in the Map object, in insertion order..                                    |
| [Object](./Object.md) | [get(key)](Map.md#get-key)                   | The get() method returns a specified element from a Map object..                                    |
| [Boolean](./Boolean.md) | [has(key)](Map.md#has-key)                   | The has() method returns a boolean indicating whether an element with the specified key exists in a Map object or not..                                    |
| [Iterator](./Iterator.md) | [keys()](Map.md#keys)                   | The keys() method returns a new iterator object that contains the keys for each element in the Map object in insertion order..                                    |
| [Map](./Map.md) | [set(key, value)](Map.md#set-key-value)                   | The set() method adds or updates an entry in a Map object with a specified key and a value..                                    |
| [Iterator](./Iterator.md) | [values()](Map.md#values)                   | The values() method returns a new iterator object that contains the values for each element in the Map object in insertion order..                                    |

## Properties Details

### size

The size accessor property returns the number of elements in a Map object.

**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
map.size;
```

## Methods Details

### clear()

The clear() method removes all elements from a Map object.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
map.clear();
```
### delete(key)

The delete() method removes the specified element from a Map object by key.

**Parameters**\
[Object](./Object.md) key  ;

**Returns**\
[Boolean](./Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var success = map.delete(key);
```
### entries()

The entries() method returns a new iterator object that contains the [key, value] pairs for each element in the Map object in insertion order. In this particular case, this iterator object is also an iterable, so the for-of loop can be used..


**Returns**\
[Iterator](./Iterator.md) the iterator that can be used in for of loops

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
for(var entry of map.entries()) {}
```
### forEach(callback, thisArgument)

The forEach() method executes a provided function once for each value in the Map object, in insertion order.

**Parameters**\
[Function](./Function.md) callback  ;\
[Object](./Object.md) thisArgument  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
map.forEach(function(keyValuePair) {});
```
### get(key)

The get() method returns a specified element from a Map object. If the value that is associated to the provided key is an object, then you will get a reference to that object and any change made to that object will effectively modify it inside the Map object.

**Parameters**\
[Object](./Object.md) key  ;

**Returns**\
[Object](./Object.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var value = map.get(key);
```
### has(key)

The has() method returns a boolean indicating whether an element with the specified key exists in a Map object or not.

**Parameters**\
[Object](./Object.md) key  ;

**Returns**\
[Boolean](./Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var containsKey = map.has(key);
```
### keys()

The keys() method returns a new iterator object that contains the keys for each element in the Map object in insertion order. In this particular case, this iterator object is also an iterable, so a for...of loop can be used.


**Returns**\
[Iterator](./Iterator.md) the iterator that can be used in for of loops

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var values = map.keys();
```
### set(key, value)

The set() method adds or updates an entry in a Map object with a specified key and a value.

**Parameters**\
[Object](./Object.md) key  ;\
[Object](./Object.md) value  ;

**Returns**\
[Map](./Map.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
map.set(keyObject, value);
```
### values()

The values() method returns a new iterator object that contains the values for each element in the Map object in insertion order.


**Returns**\
[Iterator](./Iterator.md) the iterator that can be used in for of loops

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var values = map.values();
```

