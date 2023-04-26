# LOGGINGLEVEL

## Constants Summary

| Type                          | Name                               | Summary         |
| ----------------------------- | ---------------------------------- | --------------- |
| [Number](../js-lib/number.md) | [DEBUG](logginglevel.md#DEBUG)     | Logging level.. |
| [Number](../js-lib/number.md) | [ERROR](logginglevel.md#ERROR)     | Logging level.. |
| [Number](../js-lib/number.md) | [FATAL](logginglevel.md#FATAL)     | Logging level.. |
| [Number](../js-lib/number.md) | [INFO](logginglevel.md#INFO)       | Logging level.. |
| [Number](../js-lib/number.md) | [WARNING](logginglevel.md#WARNING) | Logging level.. |

## Constants Details

### DEBUG

Logging level.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
application.output('my message',LOGGINGLEVEL.DEBUG)
```

### ERROR

Logging level.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
application.output('my message',LOGGINGLEVEL.ERROR)
```

### FATAL

Logging level. This level will for the most part be mapped on ERROR, because of java loggign api's

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
application.output('my message',LOGGINGLEVEL.FATAL)
```

### INFO

Logging level.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
application.output('my message',LOGGINGLEVEL.INFO)
```

### WARNING

Logging level.

**Returns**\
[Number](../js-lib/number.md)

**Sample**

```javascript
application.output('my message',LOGGINGLEVEL.WARNING)
```
