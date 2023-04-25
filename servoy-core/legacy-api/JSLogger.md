#  JSLogger

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSLogBuilder](./JSLogBuilder.md) | [always](JSLogger.md#always)                   | Construct a log event that will always be logged..                                    |
| [JSLogBuilder](./JSLogBuilder.md) | [debug](JSLogger.md#debug)                   | Construct a debug log event..                                    |
| [Boolean](JSLib/Boolean.md) | [debugEnabled](JSLogger.md#debugEnabled)                   | Check if the current logger's logging level enables logging on the debug level..                                    |
| [JSLogBuilder](./JSLogBuilder.md) | [error](JSLogger.md#error)                   | Construct an error log event..                                    |
| [Boolean](JSLib/Boolean.md) | [errorEnabled](JSLogger.md#errorEnabled)                   | Check if the current logger's logging level enables logging on the error level..                                    |
| [JSLogBuilder](./JSLogBuilder.md) | [fatal](JSLogger.md#fatal)                   | Construct a fatal log event..                                    |
| [Boolean](JSLib/Boolean.md) | [fatalEnabled](JSLogger.md#fatalEnabled)                   | Check if the current logger's logging level enables logging on the fatal level..                                    |
| [JSLogBuilder](./JSLogBuilder.md) | [info](JSLogger.md#info)                   | Construct an info log event..                                    |
| [Boolean](JSLib/Boolean.md) | [infoEnabled](JSLogger.md#infoEnabled)                   | Check if the current logger's logging level enables logging on the info level..                                    |
| [String](JSLib/String.md) | [level](JSLogger.md#level)                   | Get the logging level of this logger.                                    |
| [JSLogBuilder](./JSLogBuilder.md) | [trace](JSLogger.md#trace)                   | Construct a trace log event..                                    |
| [Boolean](JSLib/Boolean.md) | [traceEnabled](JSLogger.md#traceEnabled)                   | Check if the current logger's logging level enables logging on the trace level..                                    |
| [JSLogBuilder](./JSLogBuilder.md) | [warn](JSLogger.md#warn)                   | Construct a warn log event..                                    |
| [Boolean](JSLib/Boolean.md) | [warnEnabled](JSLogger.md#warnEnabled)                   | Check if the current logger's logging level enables logging on the warn level..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [setLevel(level)](JSLogger.md#setlevel-level)                   | Set the level for this logger..                                    |

## Properties Details

### always

Construct a log event that will always be logged.

**Returns**\
[JSLogBuilder](./JSLogBuilder.md) a LogBuilder

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var log = application.getLogger();
log.always.log("some message and {} {}", "some", "arguments");
```
### debug

Construct a debug log event.

**Returns**\
[JSLogBuilder](./JSLogBuilder.md) a LogBuilder

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var log = application.getLogger();
log.debug.log("some message and {} {}", "some", "arguments");
```
### debugEnabled

Check if the current logger's logging level enables logging on the debug level.
Return true if the logger's level is set to debug or trace.

**Returns**\
[Boolean](JSLib/Boolean.md) true if 'debug' level is enabled for logging

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### error

Construct an error log event.

**Returns**\
[JSLogBuilder](./JSLogBuilder.md) a LogBuilder

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var log = application.getLogger();
log.error.log("some message and {} {}", "some", "arguments");
```
### errorEnabled

Check if the current logger's logging level enables logging on the error level.
Return true if the logger's level is set to error, warn, info, debug or trace.

**Returns**\
[Boolean](JSLib/Boolean.md) true if 'error' level is enabled for logging

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### fatal

Construct a fatal log event.

**Returns**\
[JSLogBuilder](./JSLogBuilder.md) a LogBuilder

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var log = application.getLogger();
log.fatal.log("some message and {} {}", "some", "arguments");
```
### fatalEnabled

Check if the current logger's logging level enables logging on the fatal level.
Return true if the logger's level is set to fatal, error, warn, info, debug or trace.

**Returns**\
[Boolean](JSLib/Boolean.md) true if 'fatal' level is enabled for logging

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### info

Construct an info log event.

**Returns**\
[JSLogBuilder](./JSLogBuilder.md) a LogBuilder

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var log = application.getLogger();
log.info.log("some message and {} {}", "some", "arguments");
```
### infoEnabled

Check if the current logger's logging level enables logging on the info level.
Return true if the logger's level is set to info, debug or trace.

**Returns**\
[Boolean](JSLib/Boolean.md) true if 'info' level is enabled for logging

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### level

Get the logging level of this logger

**Returns**\
[String](JSLib/String.md) the logging level of this logger

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### trace

Construct a trace log event.

**Returns**\
[JSLogBuilder](./JSLogBuilder.md) a LogBuilder

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var log = application.getLogger();
log.trace.log("some message and {} {}", "some", "arguments");
```
### traceEnabled

Check if the current logger's logging level enables logging on the trace level.
Return true if the logger's level is set to trace.

**Returns**\
[Boolean](JSLib/Boolean.md) true if 'trace' level is enabled for logging

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### warn

Construct a warn log event.

**Returns**\
[JSLogBuilder](./JSLogBuilder.md) a LogBuilder

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var log = application.getLogger();
log.warn.log("some message and {} {}", "some", "arguments");
```
### warnEnabled

Check if the current logger's logging level enables logging on the warn level.
Return true if the logger's level is set to warn, info, debug or trace.

**Returns**\
[Boolean](JSLib/Boolean.md) true if 'warn' level is enabled for logging

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```

## Methods Details

### setLevel(level)

Set the level for this logger.
Be aware that this will override the logging level as configured in log4j.xml,
meaning it affects all JSLogger instances based on that configuration.
This changes the global configuration,
meaning that restarting the client will not reset the logging level to it's default state.
Only restarting the application server will reset the logging level to it's default state.

**Parameters**\
[JSLogBuilder](./JSLogBuilder.md) level the desired logging level for this logger

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var log = application.getLogger("myLogger");
log.setLevel(log.info);
```

