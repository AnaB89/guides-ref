# JSUnit

## Methods Summary

| Type | Name                                                                                                                                         | Summary                                                                        |
| ---- | -------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| void | [assertEquals(expected, actual)](jsunit.md#assertequals-expected-actual)                                                                     | Asserts that two values are equal..                                            |
| void | [assertEquals(message, expected, actual)](jsunit.md#assertequals-message-expected-actual)                                                    | Asserts that two values are equal..                                            |
| void | [assertFalse(boolean\_condition)](jsunit.md#assertfalse-boolean\_condition)                                                                  | Asserts that a condition is false..                                            |
| void | [assertFalse(message, boolean\_condition)](jsunit.md#assertfalse-message-boolean\_condition)                                                 | Asserts that a condition is false..                                            |
| void | [assertFloatEquals(expectedFloat, actualFloat, tolerance)](jsunit.md#assertfloatequals-expectedfloat-actualfloat-tolerance)                  | Asserts that two floating point values are equal to within a given tolerance.. |
| void | [assertFloatEquals(message, expectedFloat, actualFloat, tolerance)](jsunit.md#assertfloatequals-message-expectedfloat-actualfloat-tolerance) | Asserts that two floating point values are equal to within a given tolerance.. |
| void | [assertMatches(regularExpression, actualString)](jsunit.md#assertmatches-regularexpression-actualstring)                                     | Asserts that a regular expression matches a string..                           |
| void | [assertMatches(message, regularExpression, actualString)](jsunit.md#assertmatches-message-regularexpression-actualstring)                    | Asserts that a regular expression matches a string..                           |
| void | [assertNotNull(object)](jsunit.md#assertnotnull-object)                                                                                      | Asserts that an object is not null..                                           |
| void | [assertNotNull(message, object)](jsunit.md#assertnotnull-message-object)                                                                     | Asserts that an object is not null..                                           |
| void | [assertNotSame(notExpected, actual)](jsunit.md#assertnotsame-notexpected-actual)                                                             | Asserts that two values are not the same..                                     |
| void | [assertNotSame(message, notExpected, actual)](jsunit.md#assertnotsame-message-notexpected-actual)                                            | Asserts that two values are not the same..                                     |
| void | [assertNotUndefined(definedObject)](jsunit.md#assertnotundefined-definedobject)                                                              | Asserts that an object is not undefined..                                      |
| void | [assertNotUndefined(message, definedObject)](jsunit.md#assertnotundefined-message-definedobject)                                             | Asserts that an object is not undefined..                                      |
| void | [assertNull(nullValue)](jsunit.md#assertnull-nullvalue)                                                                                      | Asserts that an object is null..                                               |
| void | [assertNull(message, nullValue)](jsunit.md#assertnull-message-nullvalue)                                                                     | Asserts that an object is null..                                               |
| void | [assertSame(expected, actual)](jsunit.md#assertsame-expected-actual)                                                                         | Asserts that two values are the same..                                         |
| void | [assertSame(message, expected, actual)](jsunit.md#assertsame-message-expected-actual)                                                        | Asserts that two values are the same..                                         |
| void | [assertTrue(boolean\_condition)](jsunit.md#asserttrue-boolean\_condition)                                                                    | Asserts that a condition is true..                                             |
| void | [assertTrue(message, boolean\_condition)](jsunit.md#asserttrue-message-boolean\_condition)                                                   | Asserts that a condition is true..                                             |
| void | [assertUndefined(undefinedValue)](jsunit.md#assertundefined-undefinedvalue)                                                                  | Asserts that an object is undefined..                                          |
| void | [assertUndefined(message, undefinedValue)](jsunit.md#assertundefined-message-undefinedvalue)                                                 | Asserts that an object is undefined..                                          |
| void | [fail(message)](jsunit.md#fail-message)                                                                                                      | Fails a test..                                                                 |
| void | [fail(message, instanceOfCallStack)](jsunit.md#fail-message-instanceofcallstack)                                                             | Fails a test..                                                                 |
| void | [fail(message, instanceOfCallStack, userMessage)](jsunit.md#fail-message-instanceofcallstack-usermessage)                                    | Fails a test..                                                                 |

## Methods Details

### assertEquals(expected, actual)

Asserts that two values are equal. AssertionFailedError is thrown if the actual value does not match the regular expression.

**Parameters**\
[Object](js-lib/object.md) expected the expected value.\
[Object](js-lib/object.md) actual the actual value.

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
[String](js-lib/string.md) message The test description/message.\
[Object](js-lib/object.md) expected the expected value.\
[Object](js-lib/object.md) actual the actual value.

**Returns**\
void

**Sample**

```javascript
// Asserts that two values are equal. AssertionFailedError is thrown if the actual value does not match the regular expression.
jsunit.assertEquals("Solution name test", "someSolution", application.getSolutionName());
jsunit.assertEquals("Simple math test", 2, 1 + 1);
```

### assertFalse(boolean\_condition)

Asserts that a condition is false. AssertionFailedError is thrown if the evaluation was not false.

**Parameters**\
[Boolean](js-lib/boolean.md) boolean\_condition the actual value.

**Returns**\
void

**Sample**

```javascript
// Asserts that a condition is false. AssertionFailedError is thrown if the evaluation was not false.
jsunit.assertFalse("False test", application.isLastPrintPreviewPrinted());
```

### assertFalse(message, boolean\_condition)

Asserts that a condition is false. AssertionFailedError is thrown if the evaluation was not false.

**Parameters**\
[String](js-lib/string.md) message The test description/message.\
[Boolean](js-lib/boolean.md) boolean\_condition the actual value.

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
[Number](js-lib/number.md) expectedFloat the expected value.\
[Number](js-lib/number.md) actualFloat the actual value.\
[Number](js-lib/number.md) tolerance tolerance when comparing.

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
[String](js-lib/string.md) message The test description/message.\
[Number](js-lib/number.md) expectedFloat the expected value.\
[Number](js-lib/number.md) actualFloat the actual value.\
[Number](js-lib/number.md) tolerance tolerance when comparing.

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
[Object](js-lib/object.md) regularExpression the regular expression used for matching.\
[String](js-lib/string.md) actualString the actual value to be matched.

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
[String](js-lib/string.md) message The test description/message.\
[Object](js-lib/object.md) regularExpression the regular expression used for matching.\
[String](js-lib/string.md) actualString the actual value to be matched.

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
[Object](js-lib/object.md) object the actual value.

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
[String](js-lib/string.md) message The test description/message.\
[Object](js-lib/object.md) object the actual value.

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
[Object](js-lib/object.md) notExpected the value that is not expected.\
[Object](js-lib/object.md) actual the actual value.

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
[String](js-lib/string.md) message The test description/message.\
[Object](js-lib/object.md) notExpected the value that is not expected.\
[Object](js-lib/object.md) actual the actual value.

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
[Object](js-lib/object.md) definedObject the actual value.

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
[String](js-lib/string.md) message The test description/message.\
[Object](js-lib/object.md) definedObject the actual value.

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
[Object](js-lib/object.md) nullValue the actual value.

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
[String](js-lib/string.md) message The test description/message.\
[Object](js-lib/object.md) nullValue the actual value.

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
[Object](js-lib/object.md) expected the expected value.\
[Object](js-lib/object.md) actual the actual value.

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
[String](js-lib/string.md) message The test description/message.\
[Object](js-lib/object.md) expected the expected value.\
[Object](js-lib/object.md) actual the actual value.

**Returns**\
void

**Sample**

```javascript
// Asserts that two values are the same. AssertionFailedError is thrown if the expected value is not the actual one.
var a = new Date(1990, 1, 1);
var b = a;
jsunit.assertSame("Same test", a, b);
```

### assertTrue(boolean\_condition)

Asserts that a condition is true. AssertionFailedError is thrown if the evaluation was not true.

**Parameters**\
[Boolean](js-lib/boolean.md) boolean\_condition the actual value.

**Returns**\
void

**Sample**

```javascript
// Asserts that a condition is true. AssertionFailedError is thrown if the evaluation was not true.
jsunit.assertTrue("True test", application.isLastPrintPreviewPrinted());
```

### assertTrue(message, boolean\_condition)

Asserts that a condition is true. AssertionFailedError is thrown if the evaluation was not true.

**Parameters**\
[String](js-lib/string.md) message The test description/message.\
[Boolean](js-lib/boolean.md) boolean\_condition the actual value.

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
[Object](js-lib/object.md) undefinedValue the actual value.

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
[String](js-lib/string.md) message The test description/message.\
[Object](js-lib/object.md) undefinedValue the actual value.

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
[String](js-lib/string.md) message The test description/message. This is usually the only parameter specified when calling this method.

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
[String](js-lib/string.md) message The test description/message. This is usually the only parameter specified when calling this method.\
[Object](js-lib/object.md) instanceOfCallStack an internal JSUnit call stack. Use null for this if you want to get to the next optional parameter. Usually not specified.

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
[String](js-lib/string.md) message The test description/message. This is usually the only parameter specified when calling this method.\
[Object](js-lib/object.md) instanceOfCallStack an internal JSUnit call stack. Use null for this if you want to get to the next optional parameter. Usually not specified.\
[String](js-lib/string.md) userMessage a user message. Usually not specified.

**Returns**\
void

**Sample**

```javascript
// Fails a test. AssertionFailedError is always thrown.
jsunit.fail("Fail test");
jsunit.fail("test", null, "Fail"); // 2nd param is not used in Servoy, params 3 and 1 get merged to form a message. The result is the same as in the line above.
```
