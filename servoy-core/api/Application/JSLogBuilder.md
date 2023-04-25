#  JSLogBuilder


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [log()](JSLogBuilder.md#log)                   | Logs an event without adding a message..                                    |
|void | [log(message, params)](JSLogBuilder.md#log-message-params)                   | Logs a message with or without parameters..                                    |
| [JSLogBuilder](./JSLogBuilder.md) | [withException(exception)](JSLogBuilder.md#withexception-exception)                   | Includes an exception in the log event..                                    |

## Methods Details

### log()

Logs an event without adding a message.
This can be useful in combination with withException(e) if no message is required.


**Returns**\
void 


**Sample**

```javascript
var log = application.getLogger();
log.warn.withException(myException).log();
```
### log(message, params)

Logs a message with or without parameters.

**Parameters**\
[Object](../JSLib/Object.md) message the message to log; the format depends on the message factory.\
[Array](../JSLib/Array.md) params parameters to the message.

**Returns**\
void 


**Sample**

```javascript
var log = application.getLogger();
log.warn.log("some message {} {} {}", "with", "multiple", "arguments");
```
### withException(exception)

Includes an exception in the log event.

**Parameters**\
[Object](../JSLib/Object.md) exception The exception to log.

**Returns**\
[JSLogBuilder](./JSLogBuilder.md) the LogBuilder.


**Sample**

```javascript
var log = application.getLogger();
log.warn.withException(myException).log("some message");
```

