#  JSUnit


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [assertEquals(expected, actual)](JSUnit.md#assertequals-expected-actual)                   | Asserts that two values are equal..                                    |
|void | [assertEquals(message, expected, actual)](JSUnit.md#assertequals-message-expected-actual)                   | Asserts that two values are equal..                                    |
|void | [assertFalse(boolean_condition)](JSUnit.md#assertfalse-boolean_condition)                   | Asserts that a condition is false..                                    |
|void | [assertFalse(message, boolean_condition)](JSUnit.md#assertfalse-message-boolean_condition)                   | Asserts that a condition is false..                                    |
|void | [assertFloatEquals(expectedFloat, actualFloat, tolerance)](JSUnit.md#assertfloatequals-expectedfloat-actualfloat-tolerance)                   | Asserts that two floating point values are equal to within a given tolerance..                                    |
|void | [assertFloatEquals(message, expectedFloat, actualFloat, tolerance)](JSUnit.md#assertfloatequals-message-expectedfloat-actualfloat-tolerance)                   | Asserts that two floating point values are equal to within a given tolerance..                                    |
|void | [assertMatches(regularExpression, actualString)](JSUnit.md#assertmatches-regularexpression-actualstring)                   | Asserts that a regular expression matches a string..                                    |
|void | [assertMatches(message, regularExpression, actualString)](JSUnit.md#assertmatches-message-regularexpression-actualstring)                   | Asserts that a regular expression matches a string..                                    |
|void | [assertNotNull(object)](JSUnit.md#assertnotnull-object)                   | Asserts that an object is not null..                                    |
|void | [assertNotNull(message, object)](JSUnit.md#assertnotnull-message-object)                   | Asserts that an object is not null..                                    |
|void | [assertNotSame(notExpected, actual)](JSUnit.md#assertnotsame-notexpected-actual)                   | Asserts that two values are not the same..                                    |
|void | [assertNotSame(message, notExpected, actual)](JSUnit.md#assertnotsame-message-notexpected-actual)                   | Asserts that two values are not the same..                                    |
|void | [assertNotUndefined(definedObject)](JSUnit.md#assertnotundefined-definedobject)                   | Asserts that an object is not undefined..                                    |
|void | [assertNotUndefined(message, definedObject)](JSUnit.md#assertnotundefined-message-definedobject)                   | Asserts that an object is not undefined..                                    |
|void | [assertNull(nullValue)](JSUnit.md#assertnull-nullvalue)                   | Asserts that an object is null..                                    |
|void | [assertNull(message, nullValue)](JSUnit.md#assertnull-message-nullvalue)                   | Asserts that an object is null..                                    |
|void | [assertSame(expected, actual)](JSUnit.md#assertsame-expected-actual)                   | Asserts that two values are the same..                                    |
|void | [assertSame(message, expected, actual)](JSUnit.md#assertsame-message-expected-actual)                   | Asserts that two values are the same..                                    |
|void | [assertTrue(boolean_condition)](JSUnit.md#asserttrue-boolean_condition)                   | Asserts that a condition is true..                                    |
|void | [assertTrue(message, boolean_condition)](JSUnit.md#asserttrue-message-boolean_condition)                   | Asserts that a condition is true..                                    |
|void | [assertUndefined(undefinedValue)](JSUnit.md#assertundefined-undefinedvalue)                   | Asserts that an object is undefined..                                    |
|void | [assertUndefined(message, undefinedValue)](JSUnit.md#assertundefined-message-undefinedvalue)                   | Asserts that an object is undefined..                                    |
|void | [fail(message)](JSUnit.md#fail-message)                   | Fails a test..                                    |
|void | [fail(message, instanceOfCallStack)](JSUnit.md#fail-message-instanceofcallstack)                   | Fails a test..                                    |
|void | [fail(message, instanceOfCallStack, userMessage)](JSUnit.md#fail-message-instanceofcallstack-usermessage)                   | Fails a test..                                    |

## Methods Details

### assertEquals(expected, actual)

Asserts that two values are equal. AssertionFailedError is thrown if the actual value does not match the regular expression.

**Parameters**\
[Object](JSLib/Object.md) expected the expected value.\
[Object](JSLib/Object.md) actual the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that two values are equal. AssertionFailedError is thrown if the actual value does not match the regular expression.
jsunit.assertEquals("Solution name test", "someSolution", application.getSolutionName());
jsunit.assertEquals("Simple math test", 2, 1 + 1);
```
### assertEquals(message, expected, actual)

Asserts that two values are equal. AssertionFailedError is thrown if the actual value does not match the regular expression.

**Parameters**\
[String](JSLib/String.md) message The test description/message.\
[Object](JSLib/Object.md) expected the expected value.\
[Object](JSLib/Object.md) actual the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that two values are equal. AssertionFailedError is thrown if the actual value does not match the regular expression.
jsunit.assertEquals("Solution name test", "someSolution", application.getSolutionName());
jsunit.assertEquals("Simple math test", 2, 1 + 1);
```
### assertFalse(boolean_condition)

Asserts that a condition is false. AssertionFailedError is thrown if the evaluation was not false.

**Parameters**\
[Boolean](JSLib/Boolean.md) boolean_condition the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that a condition is false. AssertionFailedError is thrown if the evaluation was not false.
jsunit.assertFalse("False test", application.isLastPrintPreviewPrinted());
```
### assertFalse(message, boolean_condition)

Asserts that a condition is false. AssertionFailedError is thrown if the evaluation was not false.

**Parameters**\
[String](JSLib/String.md) message The test description/message.\
[Boolean](JSLib/Boolean.md) boolean_condition the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that a condition is false. AssertionFailedError is thrown if the evaluation was not false.
jsunit.assertFalse("False test", application.isLastPrintPreviewPrinted());
```
### assertFloatEquals(expectedFloat, actualFloat, tolerance)

Asserts that two floating point values are equal to within a given tolerance. AssertionFailedError is thrown if the expected value is not within the tolerance of the actual one.

**Parameters**\
[Number](JSLib/Number.md) expectedFloat the expected value.\
[Number](JSLib/Number.md) actualFloat the actual value.\
[Number](JSLib/Number.md) tolerance tolerance when comparing.

**Returns**\
void 


**Sample**

```javascript
// Asserts that two floating point values are equal to within a given tolerance. AssertionFailedError is thrown if the expected value is not within the tolerance of the actual one.
jsunit.assertFloatEquals("Float equals test", 3.12, 3.121, 0.0015);
```
### assertFloatEquals(message, expectedFloat, actualFloat, tolerance)

Asserts that two floating point values are equal to within a given tolerance. AssertionFailedError is thrown if the expected value is not within the tolerance of the actual one.

**Parameters**\
[String](JSLib/String.md) message The test description/message.\
[Number](JSLib/Number.md) expectedFloat the expected value.\
[Number](JSLib/Number.md) actualFloat the actual value.\
[Number](JSLib/Number.md) tolerance tolerance when comparing.

**Returns**\
void 


**Sample**

```javascript
// Asserts that two floating point values are equal to within a given tolerance. AssertionFailedError is thrown if the expected value is not within the tolerance of the actual one.
jsunit.assertFloatEquals("Float equals test", 3.12, 3.121, 0.0015);
```
### assertMatches(regularExpression, actualString)

Asserts that a regular expression matches a string. AssertionFailedError is thrown if the expected value is not the actual one.

**Parameters**\
[Object](JSLib/Object.md) regularExpression the regular expression used for matching.\
[String](JSLib/String.md) actualString the actual value to be matched.

**Returns**\
void 


**Sample**

```javascript
// Asserts that a regular expression matches a string. AssertionFailedError is thrown if the expected value is not the actual one.
jsunit.assertMatches(new RegExp("gr(a|e)y"), "gray");
```
### assertMatches(message, regularExpression, actualString)

Asserts that a regular expression matches a string. AssertionFailedError is thrown if the expected value is not the actual one.

**Parameters**\
[String](JSLib/String.md) message The test description/message.\
[Object](JSLib/Object.md) regularExpression the regular expression used for matching.\
[String](JSLib/String.md) actualString the actual value to be matched.

**Returns**\
void 


**Sample**

```javascript
// Asserts that a regular expression matches a string. AssertionFailedError is thrown if the expected value is not the actual one.
jsunit.assertMatches("Match test", new RegExp("gr(a|e)y"), "gray");
```
### assertNotNull(object)

Asserts that an object is not null. AssertionFailedError is thrown if the object is not null.

**Parameters**\
[Object](JSLib/Object.md) object the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that an object is not null. AssertionFailedError is thrown if the object is not null.
var a; // this is undefined, not null
jsunit.assertNotNull(a);
```
### assertNotNull(message, object)

Asserts that an object is not null. AssertionFailedError is thrown if the object is not null.

**Parameters**\
[String](JSLib/String.md) message The test description/message.\
[Object](JSLib/Object.md) object the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that an object is not null. AssertionFailedError is thrown if the object is not null.
var a; // this is undefined, not null
jsunit.assertNotNull("Not null test", a);
```
### assertNotSame(notExpected, actual)

Asserts that two values are not the same. AssertionFailedError is thrown if the expected value is the actual one.

**Parameters**\
[Object](JSLib/Object.md) notExpected the value that is not expected.\
[Object](JSLib/Object.md) actual the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that two values are not the same. AssertionFailedError is thrown if the expected value is the actual one.
var a = new Date(1990, 1, 1);
var b = new Date(1990, 1, 1);
jsunit.assertNotSame(a, b);
jsunit.assertEquals("But equals", a, b);
```
### assertNotSame(message, notExpected, actual)

Asserts that two values are not the same. AssertionFailedError is thrown if the expected value is the actual one.

**Parameters**\
[String](JSLib/String.md) message The test description/message.\
[Object](JSLib/Object.md) notExpected the value that is not expected.\
[Object](JSLib/Object.md) actual the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that two values are not the same. AssertionFailedError is thrown if the expected value is the actual one.
var a = new Date(1990, 1, 1);
var b = new Date(1990, 1, 1);
jsunit.assertNotSame("Not same test", a, b);
jsunit.assertEquals("But equals", a, b);
```
### assertNotUndefined(definedObject)

Asserts that an object is not undefined. AssertionFailedError is thrown if the object is undefined.

**Parameters**\
[Object](JSLib/Object.md) definedObject the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that an object is not undefined. AssertionFailedError is thrown if the object is undefined.
var a = 0;
jsunit.assertNotUndefined(a);
```
### assertNotUndefined(message, definedObject)

Asserts that an object is not undefined. AssertionFailedError is thrown if the object is undefined.

**Parameters**\
[String](JSLib/String.md) message The test description/message.\
[Object](JSLib/Object.md) definedObject the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that an object is not undefined. AssertionFailedError is thrown if the object is undefined.
var a = 0;
jsunit.assertNotUndefined("Not undefined test", a);
```
### assertNull(nullValue)

Asserts that an object is null. AssertionFailedError is thrown if the object is not null.

**Parameters**\
[Object](JSLib/Object.md) nullValue the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that an object is null. AssertionFailedError is thrown if the object is not null.
jsunit.assertNull("Null test", null);
```
### assertNull(message, nullValue)

Asserts that an object is null. AssertionFailedError is thrown if the object is not null.

**Parameters**\
[String](JSLib/String.md) message The test description/message.\
[Object](JSLib/Object.md) nullValue the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that an object is null. AssertionFailedError is thrown if the object is not null.
jsunit.assertNull("Null test", null);
```
### assertSame(expected, actual)

Asserts that two values are the same. AssertionFailedError is thrown if the expected value is not the actual one.

**Parameters**\
[Object](JSLib/Object.md) expected the expected value.\
[Object](JSLib/Object.md) actual the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that two values are the same. AssertionFailedError is thrown if the expected value is not the actual one.
var a = new Date(1990, 1, 1);
var b = a;
jsunit.assertSame(a, b);
```
### assertSame(message, expected, actual)

Asserts that two values are the same. AssertionFailedError is thrown if the expected value is not the actual one.

**Parameters**\
[String](JSLib/String.md) message The test description/message.\
[Object](JSLib/Object.md) expected the expected value.\
[Object](JSLib/Object.md) actual the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that two values are the same. AssertionFailedError is thrown if the expected value is not the actual one.
var a = new Date(1990, 1, 1);
var b = a;
jsunit.assertSame("Same test", a, b);
```
### assertTrue(boolean_condition)

Asserts that a condition is true. AssertionFailedError is thrown if the evaluation was not true.

**Parameters**\
[Boolean](JSLib/Boolean.md) boolean_condition the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that a condition is true. AssertionFailedError is thrown if the evaluation was not true.
jsunit.assertTrue("True test", application.isLastPrintPreviewPrinted());
```
### assertTrue(message, boolean_condition)

Asserts that a condition is true. AssertionFailedError is thrown if the evaluation was not true.

**Parameters**\
[String](JSLib/String.md) message The test description/message.\
[Boolean](JSLib/Boolean.md) boolean_condition the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that a condition is true. AssertionFailedError is thrown if the evaluation was not true.
jsunit.assertTrue("True test", application.isLastPrintPreviewPrinted());
```
### assertUndefined(undefinedValue)

Asserts that an object is undefined. AssertionFailedError is thrown if the object is defined.

**Parameters**\
[Object](JSLib/Object.md) undefinedValue the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that an object is undefined. AssertionFailedError is thrown if the object is defined.
jsunit.assertUndefined("Undefined test", thisIsUndefined);
```
### assertUndefined(message, undefinedValue)

Asserts that an object is undefined. AssertionFailedError is thrown if the object is defined.

**Parameters**\
[String](JSLib/String.md) message The test description/message.\
[Object](JSLib/Object.md) undefinedValue the actual value.

**Returns**\
void 


**Sample**

```javascript
// Asserts that an object is undefined. AssertionFailedError is thrown if the object is defined.
jsunit.assertUndefined(thisIsUndefined);
```
### fail(message)

Fails a test. AssertionFailedError is always thrown.

**Parameters**\
[String](JSLib/String.md) message The test description/message. This is usually the only parameter specified when calling this method.

**Returns**\
void 


**Sample**

```javascript
// Fails a test. AssertionFailedError is always thrown.
jsunit.fail("Fail test");
jsunit.fail("test", null, "Fail"); // 2nd param is not used in Servoy, params 3 and 1 get merged to form a message. The result is the same as in the line above.
```
### fail(message, instanceOfCallStack)

Fails a test. AssertionFailedError is always thrown.

**Parameters**\
[String](JSLib/String.md) message The test description/message. This is usually the only parameter specified when calling this method.\
[Object](JSLib/Object.md) instanceOfCallStack an internal JSUnit call stack. Use null for this if you want to get to the next optional parameter. Usually not specified.

**Returns**\
void 


**Sample**

```javascript
// Fails a test. AssertionFailedError is always thrown.
jsunit.fail("Fail test");
jsunit.fail("test", null, "Fail"); // 2nd param is not used in Servoy, params 3 and 1 get merged to form a message. The result is the same as in the line above.
```
### fail(message, instanceOfCallStack, userMessage)

Fails a test. AssertionFailedError is always thrown.

**Parameters**\
[String](JSLib/String.md) message The test description/message. This is usually the only parameter specified when calling this method.\
[Object](JSLib/Object.md) instanceOfCallStack an internal JSUnit call stack. Use null for this if you want to get to the next optional parameter. Usually not specified.\
[String](JSLib/String.md) userMessage a user message. Usually not specified.

**Returns**\
void 


**Sample**

```javascript
// Fails a test. AssertionFailedError is always thrown.
jsunit.fail("Fail test");
jsunit.fail("test", null, "Fail"); // 2nd param is not used in Servoy, params 3 and 1 get merged to form a message. The result is the same as in the line above.
```

