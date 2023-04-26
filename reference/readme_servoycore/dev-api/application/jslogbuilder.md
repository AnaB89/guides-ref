# JSLogBuilder

## Methods Summary

| Type                            | Name                                                                | Summary                                     |
| ------------------------------- | ------------------------------------------------------------------- | ------------------------------------------- |
| void                            | [log()](jslogbuilder.md#log)                                        | Logs an event without adding a message..    |
| void                            | [log(message, params)](jslogbuilder.md#log-message-params)          | Logs a message with or without parameters.. |
| [JSLogBuilder](jslogbuilder.md) | [withException(exception)](jslogbuilder.md#withexception-exception) | Includes an exception in the log event..    |

## Methods Details

### log()

Logs an event without adding a message. This can be useful in combination with withException(e) if no message is required.

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
[Object](../js-lib/object.md) message the message to log; the format depends on the message factory.\
[Array](../js-lib/array.md) params parameters to the message.

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
[Object](../js-lib/object.md) exception The exception to log.

**Returns**\
[JSLogBuilder](jslogbuilder.md) the LogBuilder.

**Sample**

```javascript
var log = application.getLogger();
log.warn.withException(myException).log("some message");
```
