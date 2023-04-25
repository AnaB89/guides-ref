#  udp

## **Return Types**
[JSPacket](./JSPacket.md),

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [JSPacket](./JSPacket.md) | [createNewPacket()](udp.md#createnewpacket)                   | Create a new empty packet..                                    |
| [JSPacket](./JSPacket.md) | [getReceivedPacket()](udp.md#getreceivedpacket)                   | Get a packet from receive buffer, read buffer until empty (null is returned)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendPacket(destIpOrHostname, packet)](udp.md#sendpacket-destiporhostname-packet)                   | Send a packet..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendPacket(destIpOrHostname, packet, port)](udp.md#sendpacket-destiporhostname-packet-port)                   | Send a packet on another port..                                    |
| [Boolean](../../JSLib/Boolean.md) | [startSocket(port_number, method_to_call_when_packet_received_and_buffer_is_empty)](udp.md#startsocket-port_number-method_to_call_when_packet_received_and_buffer_is_empty)                   | Start a UDP socket for a port..                                    |
|void | [stopSocket()](udp.md#stopsocket)                   | Stop the UDP socket for a port..                                    |
| [Boolean](../../JSLib/Boolean.md) | [testPacket(packet)](udp.md#testpacket-packet)                   | Put a test packet in the receive buffer to test your method call and getReceivedPacket..                                    |

## Methods Details

### createNewPacket()

Create a new empty packet.


**Returns**\
[JSPacket](./JSPacket.md) 


**Sample**

```javascript
var packet = plugins.udp.createNewPacket()
packet.writeUTF('hello world!')//writes UTF
packet.writeInt(12348293)//writes 4 bytes
packet.writeShort(14823)//writes 2 bytes
packet.writeByte(123)//writes 1 byte
```
### getReceivedPacket()

Get a packet from receive buffer, read buffer until empty (null is returned).


**Returns**\
[JSPacket](./JSPacket.md) 


**Sample**

```javascript
var packet = null
while( ( packet = plugins.udp.getReceivedPacket() ) != null)
{
	var text = packet.readUTF()
	var count = packet.readInt()
}
```
### sendPacket(destIpOrHostname, packet)

Send a packet.

**Parameters**\
[String](../../JSLib/String.md) destIpOrHostname the ip of the destination or the hostname\
[JSPacket](./JSPacket.md) packet the JSPacket to send

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var packet = plugins.udp.createNewPacket()
packet.writeUTF('hello world!')
plugins.udp.sendPacket('10.0.0.1',packet)
```
### sendPacket(destIpOrHostname, packet, port)

Send a packet on another port.

**Parameters**\
[String](../../JSLib/String.md) destIpOrHostname the ip of the destination or the hostname\
[JSPacket](./JSPacket.md) packet the JSPacket to send\
[Number](../../JSLib/Number.md) port the port on which to send the packet

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var packet = plugins.udp.createNewPacket()
packet.writeUTF('hello world!')
plugins.udp.sendPacket('10.0.0.1',packet, 4321)
```
### startSocket(port_number, method_to_call_when_packet_received_and_buffer_is_empty)

Start a UDP socket for a port.

**Parameters**\
[Number](../../JSLib/Number.md) port_number the local port that this UDP socket will bind to.\
[Object](../../JSLib/Object.md) method_to_call_when_packet_received_and_buffer_is_empty when the socket receives one or more packages, it calls this method once.
The method will no longer be called even if new packages are received - until a call to UDPProvider#js_getReceivedPacket() returns null. So you should
consume all available packets before you expect this method to be called again.

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
plugins.udp.startSocket(1234,my_packet_process_method)
```
### stopSocket()

Stop the UDP socket for a port.


**Returns**\
void 


**Sample**

```javascript
plugins.udp.stopSocket()
```
### testPacket(packet)

Put a test packet in the receive buffer to test your method call and getReceivedPacket.

**Parameters**\
[JSPacket](./JSPacket.md) packet  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var packet = plugins.udp.createNewPacket()
packet.writeUTF('hello world!')
plugins.udp.testPacket(packet)
```

