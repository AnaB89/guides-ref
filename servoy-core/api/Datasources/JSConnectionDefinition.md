#  JSConnectionDefinition


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSConnectionDefinition](./JSConnectionDefinition.md) | [create()](JSConnectionDefinition.md#create)                   | Registers this JSConnectionDefinition to the server with the current configuration..                                    |
|void | [destroy()](JSConnectionDefinition.md#destroy)                   | Destoyes this JSConnectonDefintion, this unregisteres this on the server so it will not use this configuration anymore to create connections..                                    |
| [String](../JSLib/String.md) | [password()](JSConnectionDefinition.md#password)                   | returns the password that was set by password(string).                                    |
| [JSConnectionDefinition](./JSConnectionDefinition.md) | [password(password)](JSConnectionDefinition.md#password-password)                   | Sets the password to use for this client connection..                                    |
| [JSConnectionDefinition](./JSConnectionDefinition.md) | [setProperty(key, value)](JSConnectionDefinition.md#setproperty-key-value)                   | Set a key value pair that is used as a connection property for this connection definition.                                    |
| [String](../JSLib/String.md) | [username()](JSConnectionDefinition.md#username)                   | returns the username that was set by username(string).                                    |
| [JSConnectionDefinition](./JSConnectionDefinition.md) | [username(username)](JSConnectionDefinition.md#username-username)                   | Sets the username to use for this client connection..                                    |

## Methods Details

### create()

Registers this JSConnectionDefinition to the server with the current configuration.
 After this call all connections to that database will use the configuration of this definition.


**Returns**\
[JSConnectionDefinition](./JSConnectionDefinition.md) The this if it could be created, this will return null if there was a creating this definition (check logs)


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
[String](../JSLib/String.md) the password for this connection.


**Sample**

```javascript

```
### password(password)

Sets the password to use for this client connection.

**Parameters**\
[String](../JSLib/String.md) password  ;

**Returns**\
[JSConnectionDefinition](./JSConnectionDefinition.md) this


**Sample**

```javascript

```
### setProperty(key, value)

Set a key value pair that is used as a connection property for this connection definition

**Parameters**\
[String](../JSLib/String.md) key The propertie key\
[String](../JSLib/String.md) value The property value

**Returns**\
[JSConnectionDefinition](./JSConnectionDefinition.md) this


**Sample**

```javascript

```
### username()

returns the username that was set by username(string)


**Returns**\
[String](../JSLib/String.md) the username for this connection.


**Sample**

```javascript

```
### username(username)

Sets the username to use for this client connection.

**Parameters**\
[String](../JSLib/String.md) username  ;

**Returns**\
[JSConnectionDefinition](./JSConnectionDefinition.md) this


**Sample**

```javascript

```

