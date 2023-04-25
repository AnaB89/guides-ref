#  Object


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Object](./Object.md) | [assign(target, sources)](Object.md#assign-target-sources)                   | Copy the values of all enumerable own properties from one or more source objects to a target object..                                    |
| [Object](./Object.md) | [create(object)](Object.md#create-object)                   | Creates a new object, using an existing object to provide the newly created object's prototype..                                    |
| [Object](./Object.md) | [create(object, properties)](Object.md#create-object-properties)                   | Creates a new object, using an existing object to provide the newly created object's prototype and properties..                                    |
| [Object](./Object.md) | [defineProperties(object, properties)](Object.md#defineproperties-object-properties)                   | Defines new or modifies existing properties directly on an object, returning the object..                                    |
| [Object](./Object.md) | [defineProperty(object, property, descriptor)](Object.md#defineproperty-object-property-descriptor)                   | Allows a precise addition to or modification of a property on an object..                                    |
| [Array](./Array.md) | [entries(object1)](Object.md#entries-object1)                   | Returns an array whose elements are arrays corresponding to the enumerable string-keyed property key-value pairs found directly upon object..                                    |
| [Object](./Object.md) | [freeze(object)](Object.md#freeze-object)                   | Freezes an object: that is, prevents new properties from being added to it; prevents existing properties from being removed; and prevents existing properties, or their enumerability, configurability, or writability, from being changed..                                    |
| [Object](./Object.md) | [fromEntries(entries)](Object.md#fromentries-entries)                   | Transforms a list of key-value pairs into an object.                                    |
| [Object](./Object.md) | [getOwnPropertyDescriptor(object, property)](Object.md#getownpropertydescriptor-object-property)                   | Permits examination of the precise description of a property..                                    |
| [Array](./Array.md) | [getOwnPropertyNames(object)](Object.md#getownpropertynames-object)                   | Returns an array of all properties (including non-enumerable properties) found directly upon a given object..                                    |
| [Object](./Object.md) | [getPrototypeOf(object)](Object.md#getprototypeof-object)                   | Returns the prototype of the specified object..                                    |
| [Boolean](./Boolean.md) | [hasOwnProperty(prop)](Object.md#hasownproperty-prop)                   | Determine whether the object has the specified property as its own property (as opposed to inheriting it)..                                    |
| [Boolean](./Boolean.md) | [is(value1, value2)](Object.md#is-value1-value2)                   | Determines whether two values are the same value..                                    |
| [Boolean](./Boolean.md) | [isExtensible(object)](Object.md#isextensible-object)                   | Determines if an object is extensible (whether it can have new properties added to it)..                                    |
| [Boolean](./Boolean.md) | [isFrozen(object)](Object.md#isfrozen-object)                   | Determines if an object is frozen..                                    |
| [Boolean](./Boolean.md) | [isPrototypeOf(object)](Object.md#isprototypeof-object)                   | Checks if an object exists in another object's prototype chain..                                    |
| [Boolean](./Boolean.md) | [isSealed(object)](Object.md#issealed-object)                   | Determines if an object is sealed..                                    |
| [Array](./Array.md) | [keys(object)](Object.md#keys-object)                   | Returns an array of all own enumerable properties found upon a given object, in the same order as that provided by a for-in loop (the difference being that a for-in loop enumerates properties in the prototype chain as well)..                                    |
| [Object](./Object.md) | [preventExtensions(object)](Object.md#preventextensions-object)                   | Prevents new properties from ever being added to an object (i..                                    |
| [Boolean](./Boolean.md) | [propertyIsEnumerable(prop)](Object.md#propertyisenumerable-prop)                   | Indicates whether the specified property is enumerable..                                    |
| [Object](./Object.md) | [seal(object)](Object.md#seal-object)                   | Seals an object, preventing new properties from being added to it and marking all existing properties as non-configurable..                                    |
| [String](./String.md) | [toLocaleString()](Object.md#tolocalestring)                   | Returns a string representing the object..                                    |
| [String](./String.md) | [toString()](Object.md#tostring)                   | Returns a string representing the specified object..                                    |
| [Object](./Object.md) | [valueOf()](Object.md#valueof)                   | Returns the primitive value of the specified object..                                    |
| [Array](./Array.md) | [values(object1)](Object.md#values-object1)                   | Returns an array whose elements are strings corresponding to the enumerable string-keyed property values found directly upon object..                                    |

## Methods Details

### assign(target, sources)

Copy the values of all enumerable own properties from one or more source objects to a target object.

**Parameters**\
[Object](./Object.md) target The target object.\
[Array](./Array.md) sources The source object(s).

**Returns**\
[Object](./Object.md) The target object.


**Sample**

```javascript
var object1 = { a: 1, b: 2, c: 3};
var object2 = Object.assign({c: 4, d: 5}, object1);
application.output(object2.c, object2.d);
```
### create(object)

Creates a new object, using an existing object to provide the newly created object's prototype.

**Parameters**\
[Object](./Object.md) object The object which should be the prototype of the newly-created object.

**Returns**\
[Object](./Object.md) A new object with the specified prototype object.


**Sample**

```javascript
const person = {
	isHuman: false,
	printIntroduction: function () {
		application.output("My name is " + this.name + ". Am I human? " + this.isHuman);
	}
};
var me = Object.create(person);
me.name = "Matthew"; // "name" is a property set on "me", but not on "person"
me.isHuman = true; // inherited properties can be overwritten
me.printIntroduction(); // expected output: "My name is Matthew. Am I human? true"
```
### create(object, properties)

Creates a new object, using an existing object to provide the newly created object's prototype and properties.

**Parameters**\
[Object](./Object.md) object The object which should be the prototype of the newly-created object.\
[Object](./Object.md) properties  ;

**Returns**\
[Object](./Object.md) A new object with the specified prototype object.


**Sample**

```javascript
var o = Object.create({}, { p: { value: 42 } });
application.output(o.p);
```
### defineProperties(object, properties)

Defines new or modifies existing properties directly on an object, returning the object.

**Parameters**\
[Object](./Object.md) object The object on which to define or modify properties.\
[Object](./Object.md) properties An object whose own enumerable properties constitute descriptors for the properties to be defined or modified.
			Descriptors have the following keys:
			configurable - true if and only if the type of this property descriptor may be changed and if the property may be deleted
							from the corresponding object. Defaults to false.
			enumerable - true if and only if this property shows up during enumeration of the properties on the corresponding object.
							Defaults to false.
			value - The value associated with the property. Can be any valid JavaScript value (number, object, function, etc).
							Defaults to undefined.
			writable - true if and only if the value associated with the property may be changed with an assignment operator.
							Defaults to false.
			get - A function which serves as a getter for the property, or undefined if there is no getter. The function return will
				  be used as the value of property. Defaults to undefined.
			set - A function which serves as a setter for the property, or undefined if there is no setter. The function will receive
				  as only argument the new value being assigned to the property. Defaults to undefined.

**Returns**\
[Object](./Object.md) The object that was passed to the function.


**Sample**

```javascript
const object1 = {};
Object.defineProperties(object1, {property1: {value: 42, writable: true},   property2: {}});
application.output(object1.property1);
```
### defineProperty(object, property, descriptor)

Allows a precise addition to or modification of a property on an object.

**Parameters**\
[Object](./Object.md) object The object on which to define or modify properties.\
[Object](./Object.md) property The name of the property to be defined or modified.\
[Object](./Object.md) descriptor The descriptor for the property being defined or modified.

**Returns**\
[Object](./Object.md) The object that was passed to the function.


**Sample**

```javascript
const object1 = {};
Object.defineProperty(object1, 'property1', {value: 42, writable: false});
application.output(object1.property1);
```
### entries(object1)

Returns an array whose elements are arrays corresponding to the enumerable string-keyed property key-value pairs found directly upon object.

**Parameters**\
[Object](./Object.md) object1 An object.

**Returns**\
[Array](./Array.md) An array of the given object's own enumerable string-keyed property key-value pairs. Each key-value pair is an array with two elements: the first element is the property key (which is always a string), and the second element is the property value.


**Sample**

```javascript
const object1 = { a: 'somestring',  b: 42,  c: false};
application.output(Object.entries(object1));
```
### freeze(object)

Freezes an object: that is, prevents new properties from being added to it; prevents existing properties from being removed; and prevents
existing properties, or their enumerability, configurability, or writability, from being changed. In essence the object is made effectively immutable.

**Parameters**\
[Object](./Object.md) object The object to freeze.

**Returns**\
[Object](./Object.md) The object that was passed to the function.


**Sample**

```javascript
const object1 = { property1: 42 };
const object2 = Object.freeze(object1);
object2.property1 = 33;
application.output(object2.property1); //expected result is 42
```
### fromEntries(entries)

Transforms a list of key-value pairs into an object

**Parameters**\
[Array](./Array.md) entries A list of objects. Each object is an array with two values, first value is the key second one is the value.

**Returns**\
[Object](./Object.md) A new object whose properties are given by the entries of the array.


**Sample**

```javascript
application.output(Object.fromEntries(entries));
```
### getOwnPropertyDescriptor(object, property)

Permits examination of the precise description of a property.

**Parameters**\
[Object](./Object.md) object The object in which to look for the property.\
[Object](./Object.md) property The name of the property whose description is to be retrieved.

**Returns**\
[Object](./Object.md) A property descriptor of the given property if it exists on the object, undefined otherwise.


**Sample**

```javascript
const object1 = { property1: 42 };
const descriptor1 = Object.getOwnPropertyDescriptor(object1, 'property1');
application.output(descriptor1.configurable); // expected output: true
application.output(descriptor1.value); //expected result is 42
```
### getOwnPropertyNames(object)

Returns an array of all properties (including non-enumerable properties) found directly upon a given object.

**Parameters**\
[Object](./Object.md) object The object whose enumerable and non-enumerable own properties are to be returned.

**Returns**\
[Array](./Array.md) An array of strings that correspond to the properties found directly upon the given object.


**Sample**

```javascript
const object1 = { a: 1, b: 2, c: 3};
application.output(Object.getOwnPropertyNames(object1));
```
### getPrototypeOf(object)

Returns the prototype of the specified object.

**Parameters**\
[Object](./Object.md) object The object whose prototype is to be returned.

**Returns**\
[Object](./Object.md) The prototype of the given object. If there are no inherited properties, null is returned.


**Sample**

```javascript
const prototype1 = {};
const object1 = Object.create(prototype1);
application.output(Object.getPrototypeOf(object1) === prototype1); // expected output: true
```
### hasOwnProperty(prop)

Determine whether the object has the specified property as its own property (as opposed to inheriting it).

**Parameters**\
[String](./String.md) prop The name of the property to test.

**Returns**\
[Boolean](./Boolean.md) A Boolean indicating whether or not the object has the specified property as own property.


**Sample**

```javascript
const object1 = new Object();
 object1.property1 = 42;
 application.output(object1.hasOwnProperty('property1')); // expected output: true
 application.output(object1.hasOwnProperty('toString')); // expected output: false
 application.output(object1.hasOwnProperty('hasOwnProperty')); // expected output: false
```
### is(value1, value2)

Determines whether two values are the same value.

**Parameters**\
[Object](./Object.md) value1 The first value to compare.\
[Object](./Object.md) value2 The second value to compare.

**Returns**\
[Boolean](./Boolean.md) a Boolean indicating whether or not the two arguments are the same value.


**Sample**

```javascript
Object.is('foo', 'foo');
```
### isExtensible(object)

Determines if an object is extensible (whether it can have new properties added to it).
Objects are extensible by default, can be marked as non-extensible using Object.preventExtensions(), Object.seal(), or Object.freeze().

**Parameters**\
[Object](./Object.md) object The object which should be checked.

**Returns**\
[Boolean](./Boolean.md) A Boolean indicating whether or not the given object is extensible.


**Sample**

```javascript
var empty = {};
Object.isExtensible(empty); // === true

Object.preventExtensions(empty);
Object.isExtensible(empty); // === false

var sealed = Object.seal({});
Object.isExtensible(sealed); // === false

var frozen = Object.freeze({});
Object.isExtensible(frozen); // === false
```
### isFrozen(object)

Determines if an object is frozen. An object is frozen if and only if it is not extensible, all its properties are non-configurable, and all its data properties
(that is, properties which are not accessor properties with getter or setter components) are non-writable.

**Parameters**\
[Object](./Object.md) object The object which should be checked.

**Returns**\
[Boolean](./Boolean.md) A Boolean indicating whether or not the given object is frozen.


**Sample**

```javascript
const object1 = { property1: 42 };
application.output(Object.isFrozen(object1)); // expected output: false
Object.freeze(object1);
application.output(Object.isFrozen(object1)); // expected output: true
```
### isPrototypeOf(object)

Checks if an object exists in another object's prototype chain.

**Parameters**\
[Object](./Object.md) object The object whose prototype chain will be searched.

**Returns**\
[Boolean](./Boolean.md) A Boolean indicating whether the calling object lies in the prototype chain of the specified object.


**Sample**

```javascript
function object1() {}
function object2() {}
object1.prototype = Object.create(object2.prototype);
const object3 = new object1();
application.output(object1.prototype.isPrototypeOf(object3)); // expected output: true
application.output(object2.prototype.isPrototypeOf(object3)); // expected output: true
```
### isSealed(object)

Determines if an object is sealed. An object is sealed if it is not extensible and if all its properties are non-configurable and therefore not removable (but
not necessarily non-writable).

**Parameters**\
[Object](./Object.md) object The object which should be checked.

**Returns**\
[Boolean](./Boolean.md) A Boolean indicating whether or not the given object is sealed.


**Sample**

```javascript
const object1 = { property1: 42 };
application.output(Object.isSealed(object1)); // expected output: false
Object.seal(object1);
application.output(Object.isSealed(object1)); // expected output: true
```
### keys(object)

Returns an array of all own enumerable properties found upon a given object, in the same order as that provided by a for-in loop (the difference
being that a for-in loop enumerates properties in the prototype chain as well).

**Parameters**\
[Object](./Object.md) object An array of strings that represent all the enumerable properties of the given object.

**Returns**\
[Array](./Array.md) The object of which the enumerable's own properties are to be returned.


**Sample**

```javascript
const object1 = {a: 'somestring', b: 42, c: false };
application.outout(Object.keys(object1)); // expected output: Array ["a", "b", "c"]
```
### preventExtensions(object)

Prevents new properties from ever being added to an object (i.e. prevents future extensions to the object).

**Parameters**\
[Object](./Object.md) object The object which should be made non-extensible.

**Returns**\
[Object](./Object.md) The object being made non-extensible.


**Sample**

```javascript
const object1 = {};
Object.preventExtensions(object1);
try {
  Object.defineProperty(object1, 'property1', {
      value: 42
 });
 } catch (e) {
   application.output(e);
}
```
### propertyIsEnumerable(prop)

Indicates whether the specified property is enumerable.

**Parameters**\
[Object](./Object.md) prop The name or symbol of the property to test.

**Returns**\
[Boolean](./Boolean.md) A Boolean indicating whether the specified property is enumerable.


**Sample**

```javascript
const array1 = [];
object1.property1 = 42;
array1[0] = 42;
application.output(object1.propertyIsEnumerable('property1')); // expected output: true
application.output(array1.propertyIsEnumerable(0)); // expected output: true
application.output(array1.propertyIsEnumerable('length')); // expected output: false
```
### seal(object)

Seals an object, preventing new properties from being added to it and marking all existing properties as non-configurable.
Values of present properties can still be changed as long as they are writable.

**Parameters**\
[Object](./Object.md) object The object which should be sealed.

**Returns**\
[Object](./Object.md) The object being sealed.


**Sample**

```javascript
const object1 = { property1: 42 };
Object.seal(object1);
object1.property1 = 33;
application.output(object1.property1); // expected output: 33

delete object1.property1; // cannot delete when sealed
application.output(object1.property1); // expected output: 33
```
### toLocaleString()

Returns a string representing the object. This method is meant to be overriden by derived objects for locale-specific purposes.


**Returns**\
[String](./String.md) A string representing the object.


**Sample**

```javascript
const number1 = 123456.789;
application.output(number1.toLocaleString()); // expected output: "123.456,789"
```
### toString()

Returns a string representing the specified object.


**Returns**\
[String](./String.md) A string representing the object.


**Sample**

```javascript
function Dog(name) {
  this.name = name;
}
var dog1 = new Dog('Spike');
Dog.prototype.toString = function dogToString() { return this.name; }

application.output(dog1.toString());
```
### valueOf()

Returns the primitive value of the specified object. By default, the valueOf method is inherited by every object descended from Object.
Every built-in core object overrides this method to return an appropriate value.
If an object has no primitive value, valueOf returns the object itself.


**Returns**\
[Object](./Object.md) The primitive value of the specified object.


**Sample**

```javascript
function MyNumberType(n) {
 this.number = n;
}
MyNumberType.prototype.valueOf = function() { return this.number; };

const object1 = new MyNumberType(4);
application.output(object1 + 3); // expected output: 7
```
### values(object1)

Returns an array whose elements are strings corresponding to the enumerable string-keyed property values found directly upon object.

**Parameters**\
[Object](./Object.md) object1 An object.

**Returns**\
[Array](./Array.md) an array of a given object's own enumerable string-keyed property values.


**Sample**

```javascript
const object1 = { a: 'somestring',  b: 42,  c: false};
Object.values(object1);
```

