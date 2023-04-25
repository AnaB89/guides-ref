#  Broadcaster

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [broadcastMessage(message)](Broadcaster.md#broadcastmessage-message)                   | Sends a message to the all other listeners of the channel of this broadcaster..                                    |
|void | [destroy()](Broadcaster.md#destroy)                   | Destroyes and unregister the listener for this channel..                                    |
| [String](../../JSLib/String.md) | [getChannelName()](Broadcaster.md#getchannelname)                   | get the channel name where this broadcaster listens and sends messages to..                                    |
| [String](../../JSLib/String.md) | [getName()](Broadcaster.md#getname)                   | Get the (nick) name for this broadcaster that will be send to other channel listeners..                                    |

## Methods Details

### broadcastMessage(message)

Sends a message to the all other listeners of the channel of this broadcaster.

**Parameters**\
[String](../../JSLib/String.md) message The message to send to the other users of this channel

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### destroy()

Destroyes and unregister the listener for this channel.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### getChannelName()

get the channel name where this broadcaster listens and sends messages to.


**Returns**\
[String](../../JSLib/String.md) String

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### getName()

Get the (nick) name for this broadcaster that will be send to other channel listeners.


**Returns**\
[String](../../JSLib/String.md) String

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```

