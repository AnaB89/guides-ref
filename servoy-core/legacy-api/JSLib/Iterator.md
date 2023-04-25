#  Iterator

## **Supported Clients**

    SmartClient
    WebClient
    NGClient
    MobileClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [IterableValue](./IterableValue.md) | [next()](Iterator.md#next)                   | An iterator is an object which defines a sequence and potentially a return value upon its termination Returns the next IterableValue  for this Iterable.                                    |

## Methods Details

### next()

An iterator is an object which defines a sequence and potentially a return value upon its termination
Returns the next IterableValue  for this Iterable


**Returns**\
[IterableValue](./IterableValue.md) the next IterableValue

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
for(var entry of set.value()) {}
```

