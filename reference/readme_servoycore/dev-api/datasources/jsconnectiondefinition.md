# JSConnectionDefinition

## Methods Summary

| Type                                                | Name                                                                       | Summary                                                                                                                                        |
| --------------------------------------------------- | -------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| [JSConnectionDefinition](jsconnectiondefinition.md) | [create()](jsconnectiondefinition.md#create)                               | Registers this JSConnectionDefinition to the server with the current configuration..                                                           |
| void                                                | [destroy()](jsconnectiondefinition.md#destroy)                             | Destoyes this JSConnectonDefintion, this unregisteres this on the server so it will not use this configuration anymore to create connections.. |
| [String](../js-lib/string.md)                       | [password()](jsconnectiondefinition.md#password)                           | returns the password that was set by password(string).                                                                                         |
| [JSConnectionDefinition](jsconnectiondefinition.md) | [password(password)](jsconnectiondefinition.md#password-password)          | Sets the password to use for this client connection..                                                                                          |
| [JSConnectionDefinition](jsconnectiondefinition.md) | [setProperty(key, value)](jsconnectiondefinition.md#setproperty-key-value) | Set a key value pair that is used as a connection property for this connection definition.                                                     |
| [String](../js-lib/string.md)                       | [username()](jsconnectiondefinition.md#username)                           | returns the username that was set by username(string).                                                                                         |
| [JSConnectionDefinition](jsconnectiondefinition.md) | [username(username)](jsconnectiondefinition.md#username-username)          | Sets the username to use for this client connection..                                                                                          |

## Methods Details

### create()

Registers this JSConnectionDefinition to the server with the current configuration. After this call all connections to that database will use the configuration of this definition.

**Returns**\
[JSConnectionDefinition](jsconnectiondefinition.md) The this if it could be created, this will return null if there was a creating this definition (check logs)

**Sample**

```javascript
```

### destroy()

Destoyes this JSConnectonDefintion, this unregisteres this on the server so it will not use this configuration anymore to create connections.

**Returns**\
void

**Sample**

```javascript
```

### password()

returns the password that was set by password(string)

**Returns**\
[String](../js-lib/string.md) the password for this connection.

**Sample**

```javascript
```

### password(password)

Sets the password to use for this client connection.

**Parameters**\
[String](../js-lib/string.md) password ;

**Returns**\
[JSConnectionDefinition](jsconnectiondefinition.md) this

**Sample**

```javascript
```

### setProperty(key, value)

Set a key value pair that is used as a connection property for this connection definition

**Parameters**\
[String](../js-lib/string.md) key The propertie key\
[String](../js-lib/string.md) value The property value

**Returns**\
[JSConnectionDefinition](jsconnectiondefinition.md) this

**Sample**

```javascript
```

### username()

returns the username that was set by username(string)

**Returns**\
[String](../js-lib/string.md) the username for this connection.

**Sample**

```javascript
```

### username(username)

Sets the username to use for this client connection.

**Parameters**\
[String](../js-lib/string.md) username ;

**Returns**\
[JSConnectionDefinition](jsconnectiondefinition.md) this

**Sample**

```javascript
```
