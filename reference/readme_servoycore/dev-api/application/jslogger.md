# JSLogger

## Property Summary

| Type                            | Name                                     | Summary                                                                          |
| ------------------------------- | ---------------------------------------- | -------------------------------------------------------------------------------- |
| [JSLogBuilder](jslogbuilder.md) | [always](jslogger.md#always)             | Construct a log event that will always be logged..                               |
| [JSLogBuilder](jslogbuilder.md) | [debug](jslogger.md#debug)               | Construct a debug log event..                                                    |
| [Boolean](../js-lib/boolean.md) | [debugEnabled](jslogger.md#debugEnabled) | Check if the current logger's logging level enables logging on the debug level.. |
| [JSLogBuilder](jslogbuilder.md) | [error](jslogger.md#error)               | Construct an error log event..                                                   |
| [Boolean](../js-lib/boolean.md) | [errorEnabled](jslogger.md#errorEnabled) | Check if the current logger's logging level enables logging on the error level.. |
| [JSLogBuilder](jslogbuilder.md) | [fatal](jslogger.md#fatal)               | Construct a fatal log event..                                                    |
| [Boolean](../js-lib/boolean.md) | [fatalEnabled](jslogger.md#fatalEnabled) | Check if the current logger's logging level enables logging on the fatal level.. |
| [JSLogBuilder](jslogbuilder.md) | [info](jslogger.md#info)                 | Construct an info log event..                                                    |
| [Boolean](../js-lib/boolean.md) | [infoEnabled](jslogger.md#infoEnabled)   | Check if the current logger's logging level enables logging on the info level..  |
| [String](../js-lib/string.md)   | [level](jslogger.md#level)               | Get the logging level of this logger.                                            |
| [JSLogBuilder](jslogbuilder.md) | [trace](jslogger.md#trace)               | Construct a trace log event..                                                    |
| [Boolean](../js-lib/boolean.md) | [traceEnabled](jslogger.md#traceEnabled) | Check if the current logger's logging level enables logging on the trace level.. |
| [JSLogBuilder](jslogbuilder.md) | [warn](jslogger.md#warn)                 | Construct a warn log event..                                                     |
| [Boolean](../js-lib/boolean.md) | [warnEnabled](jslogger.md#warnEnabled)   | Check if the current logger's logging level enables logging on the warn level..  |

## Methods Summary

| Type | Name                                          | Summary                         |
| ---- | --------------------------------------------- | ------------------------------- |
| void | [setLevel(level)](jslogger.md#setlevel-level) | Set the level for this logger.. |

## Properties Details

### always

Construct a log event that will always be logged.

**Returns**\
[JSLogBuilder](jslogbuilder.md) a LogBuilder

**Sample**

```javascript
var log = application.getLogger();
log.always.log("some message and {} {}", "some", "arguments");
```

### debug

Construct a debug log event.

**Returns**\
[JSLogBuilder](jslogbuilder.md) a LogBuilder

**Sample**

```javascript
var log = application.getLogger();
log.debug.log("some message and {} {}", "some", "arguments");
```

### debugEnabled

Check if the current logger's logging level enables logging on the debug level. Return true if the logger's level is set to debug or trace.

**Returns**\
[Boolean](../js-lib/boolean.md) true if 'debug' level is enabled for logging

**Sample**

```javascript
```

### error

Construct an error log event.

**Returns**\
[JSLogBuilder](jslogbuilder.md) a LogBuilder

**Sample**

```javascript
var log = application.getLogger();
log.error.log("some message and {} {}", "some", "arguments");
```

### errorEnabled

Check if the current logger's logging level enables logging on the error level. Return true if the logger's level is set to error, warn, info, debug or trace.

**Returns**\
[Boolean](../js-lib/boolean.md) true if 'error' level is enabled for logging

**Sample**

```javascript
```

### fatal

Construct a fatal log event.

**Returns**\
[JSLogBuilder](jslogbuilder.md) a LogBuilder

**Sample**

```javascript
var log = application.getLogger();
log.fatal.log("some message and {} {}", "some", "arguments");
```

### fatalEnabled

Check if the current logger's logging level enables logging on the fatal level. Return true if the logger's level is set to fatal, error, warn, info, debug or trace.

**Returns**\
[Boolean](../js-lib/boolean.md) true if 'fatal' level is enabled for logging

**Sample**

```javascript
```

### info

Construct an info log event.

**Returns**\
[JSLogBuilder](jslogbuilder.md) a LogBuilder

**Sample**

```javascript
var log = application.getLogger();
log.info.log("some message and {} {}", "some", "arguments");
```

### infoEnabled

Check if the current logger's logging level enables logging on the info level. Return true if the logger's level is set to info, debug or trace.

**Returns**\
[Boolean](../js-lib/boolean.md) true if 'info' level is enabled for logging

**Sample**

```javascript
```

### level

Get the logging level of this logger

**Returns**\
[String](../js-lib/string.md) the logging level of this logger

**Sample**

```javascript
```

### trace

Construct a trace log event.

**Returns**\
[JSLogBuilder](jslogbuilder.md) a LogBuilder

**Sample**

```javascript
var log = application.getLogger();
log.trace.log("some message and {} {}", "some", "arguments");
```

### traceEnabled

Check if the current logger's logging level enables logging on the trace level. Return true if the logger's level is set to trace.

**Returns**\
[Boolean](../js-lib/boolean.md) true if 'trace' level is enabled for logging

**Sample**

```javascript
```

### warn

Construct a warn log event.

**Returns**\
[JSLogBuilder](jslogbuilder.md) a LogBuilder

**Sample**

```javascript
var log = application.getLogger();
log.warn.log("some message and {} {}", "some", "arguments");
```

### warnEnabled

Check if the current logger's logging level enables logging on the warn level. Return true if the logger's level is set to warn, info, debug or trace.

**Returns**\
[Boolean](../js-lib/boolean.md) true if 'warn' level is enabled for logging

**Sample**

```javascript
```

## Methods Details

### setLevel(level)

Set the level for this logger. Be aware that this will override the logging level as configured in log4j.xml, meaning it affects all JSLogger instances based on that configuration. This changes the global configuration, meaning that restarting the client will not reset the logging level to it's default state. Only restarting the application server will reset the logging level to it's default state.

**Parameters**\
[JSLogBuilder](jslogbuilder.md) level the desired logging level for this logger

**Returns**\
void

**Sample**

```javascript
var log = application.getLogger("myLogger");
log.setLevel(log.info);
```
