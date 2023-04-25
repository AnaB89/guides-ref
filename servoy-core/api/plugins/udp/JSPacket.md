#  JSPacket


## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](../../JSLib/Number.md) | [index](JSPacket.md#index)                   | Returns the current position in the byte array of the packet..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Array](../../JSLib/Array.md) | [getByteArray()](JSPacket.md#getbytearray)                   | Returns the content of the package into a byte array..                                    |
| [String](../../JSLib/String.md) | [getHost()](JSPacket.md#gethost)                   | Returns the name of the host that sent the packet..                                    |
| [Number](../../JSLib/Number.md) | [getLength()](JSPacket.md#getlength)                   | Returns the length of the packet in bytes..                                    |
| [Number](../../JSLib/Number.md) | [getPort()](JSPacket.md#getport)                   | Returns the port where the packet originated from..                                    |
| [Number](../../JSLib/Number.md) | [readByte()](JSPacket.md#readbyte)                   | Reads an 8 bits byte value from the packet, starting from the current index..                                    |
| [Number](../../JSLib/Number.md) | [readInt()](JSPacket.md#readint)                   | Reads a 32 bits int value from the packet, starting from the current index..                                    |
| [Number](../../JSLib/Number.md) | [readShort()](JSPacket.md#readshort)                   | Reads a 32 bits short value from the packet, starting from the current index..                                    |
| [String](../../JSLib/String.md) | [readUTF()](JSPacket.md#readutf)                   | Reads a UTF-8 string from the packet, starting from the current index..                                    |
| [String](../../JSLib/String.md) | [readUTF(length)](JSPacket.md#readutf-length)                   | Reads a UTF-8 string from the packet, starting from the current index..                                    |
|void | [writeByte(number)](JSPacket.md#writebyte-number)                   | Writes one byte into the packet, at the current index..                                    |
|void | [writeBytes(bytes)](JSPacket.md#writebytes-bytes)                   | Writes an array of bytes into the packet, at the current index..                                    |
|void | [writeInt(number)](JSPacket.md#writeint-number)                   | Writes a 32 bits int into the packet, at the current index..                                    |
|void | [writeShort(number)](JSPacket.md#writeshort-number)                   | Writes a 16 bits short value into the packet, at the current index..                                    |
| [Number](../../JSLib/Number.md) | [writeUTF(string)](JSPacket.md#writeutf-string)                   | Writes an UTF-8 encoded string into the packet, at the current index..                                    |

## Properties Details

### index

Returns the current position in the byte array of the packet. The next read/write operation will occur at this position.
This is a 0 based index.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var packet;
while (packet = plugins.udp.getReceivedPacket()) {
	application.output('packet received from ' + packet.getHost() + ':' + packet.getPort());
	if (packet.getLength() > 0) {
		application.output('an int is: ' + packet.readInt());
		application.output('moved to index: ' + packet.index);
		application.output('a short is: ' + packet.readShort());
		application.output('moved to index: ' + packet.index);
		application.output('a byte is: ' + packet.readByte());
		application.output('moved to index: ' + packet.index);
		application.output('a byte is: ' + packet.readByte());
		application.output('moved to index: ' + packet.index);
	}
	else {
		application.output('end of communication.');
		break;
	}
}
```

## Methods Details

### getByteArray()

Returns the content of the package into a byte array.


**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
var packet;
while (packet = plugins.udp.getReceivedPacket()) {
	application.output('packet received from ' + packet.getHost() + ':' + packet.getPort());
	if (packet.getLength() > 0) {
		var bytes = packet.getByteArray();
		application.output('received a packet of length: ' + bytes.length);
		for (var i=0; i<bytes.length; i++)
			application.output(bytes[i]);
		}
	else {
		application.output('end of communication.');
		break;
	}
}
```
### getHost()

Returns the name of the host that sent the packet.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var packet;
while (packet = plugins.udp.getReceivedPacket()) {
	application.output('packet received from ' + packet.getHost() + ':' + packet.getPort());
	if (packet.getLength() > 0) {
		application.output('message is: ' + packet.readUTF());
	}
	else {
		application.output('end of communication.');
		break;
	}
}
```
### getLength()

Returns the length of the packet in bytes.


**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var packet;
while (packet = plugins.udp.getReceivedPacket()) {
	application.output('packet received from ' + packet.getHost() + ':' + packet.getPort());
	if (packet.getLength() > 0) {
		application.output('message is: ' + packet.readUTF());
	}
	else {
		application.output('end of communication.');
		break;
	}
}
```
### getPort()

Returns the port where the packet originated from.


**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var packet;
while (packet = plugins.udp.getReceivedPacket()) {
	application.output('packet received from ' + packet.getHost() + ':' + packet.getPort());
	if (packet.getLength() > 0) {
		application.output('message is: ' + packet.readUTF());
	}
	else {
		application.output('end of communication.');
		break;
	}
}
```
### readByte()

Reads an 8 bits byte value from the packet, starting from the current index. Advances the index with one position.


**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var packet;
while (packet = plugins.udp.getReceivedPacket()) {
	application.output('packet received from ' + packet.getHost() + ':' + packet.getPort());
	if (packet.getLength() > 0) {
		application.output('an int is: ' + packet.readInt());
		application.output('moved to index: ' + packet.index);
		application.output('a short is: ' + packet.readShort());
		application.output('moved to index: ' + packet.index);
		application.output('a byte is: ' + packet.readByte());
		application.output('moved to index: ' + packet.index);
		application.output('a byte is: ' + packet.readByte());
		application.output('moved to index: ' + packet.index);
	}
	else {
		application.output('end of communication.');
		break;
	}
}
```
### readInt()

Reads a 32 bits int value from the packet, starting from the current index. Advances the index with 4 positions.


**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var packet;
while (packet = plugins.udp.getReceivedPacket()) {
	application.output('packet received from ' + packet.getHost() + ':' + packet.getPort());
	if (packet.getLength() > 0) {
		application.output('an int is: ' + packet.readInt());
		application.output('moved to index: ' + packet.index);
		application.output('a short is: ' + packet.readShort());
		application.output('moved to index: ' + packet.index);
		application.output('a byte is: ' + packet.readByte());
		application.output('moved to index: ' + packet.index);
		application.output('a byte is: ' + packet.readByte());
		application.output('moved to index: ' + packet.index);
	}
	else {
		application.output('end of communication.');
		break;
	}
}
```
### readShort()

Reads a 32 bits short value from the packet, starting from the current index. Advances the index with 2 positions.


**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var packet;
while (packet = plugins.udp.getReceivedPacket()) {
	application.output('packet received from ' + packet.getHost() + ':' + packet.getPort());
	if (packet.getLength() > 0) {
		application.output('an int is: ' + packet.readInt());
		application.output('moved to index: ' + packet.index);
		application.output('a short is: ' + packet.readShort());
		application.output('moved to index: ' + packet.index);
		application.output('a byte is: ' + packet.readByte());
		application.output('moved to index: ' + packet.index);
		application.output('a byte is: ' + packet.readByte());
		application.output('moved to index: ' + packet.index);
	}
	else {
		application.output('end of communication.');
		break;
	}
}
```
### readUTF()

Reads a UTF-8 string from the packet, starting from the current index. If an argument is specified, then it represents the length (in UTF-8 encoded bytes, not characters) of the string to read. If no argument is specified, then first a 32 bits (4 byte) int is read from the packet and that will be the byte length of the string. Advances the index with a number of positions that depends on the length of the read string.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var packet;
while (packet = plugins.udp.getReceivedPacket()) {
	application.output('packet received from ' + packet.getHost() + ':' + packet.getPort());
	if (packet.getLength() > 0) {
		application.output('message is: ' + packet.readUTF());
	}
	else {
		application.output('end of communication.');
		break;
	}
}
```
### readUTF(length)

Reads a UTF-8 string from the packet, starting from the current index. If an argument is specified, then it represents the length (in UTF-8 encoded bytes, not characters) of the string to read. If no argument is specified, then first a 32 bits (4 byte) int is read from the packet and that will be the byte length of the string. Advances the index with a number of positions that depends on the length of the read string.

**Parameters**\
[Number](../../JSLib/Number.md) length  ;

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var packet;
while (packet = plugins.udp.getReceivedPacket()) {
	application.output('packet received from ' + packet.getHost() + ':' + packet.getPort());
	if (packet.getLength() > 0) {
		application.output('message is: ' + packet.readUTF());
	}
	else {
		application.output('end of communication.');
		break;
	}
}
```
### writeByte(number)

Writes one byte into the packet, at the current index. The index is advanced with one position.

**Parameters**\
[Number](../../JSLib/Number.md) number  ;

**Returns**\
void 


**Sample**

```javascript
if (!plugins.udp.startSocket('5555', packetReceived)) {
	application.output('Failed to start socket.');
} else {
	var packet = plugins.udp.createNewPacket();
	packet.writeUTF('hello world!');
	plugins.udp.sendPacket('localhost', packet, 1234);
	packet = plugins.udp.createNewPacket();
	packet.writeByte(0xFF);
	packet.writeShort(10001);
	packet.writeInt(2000000001);
	plugins.udp.sendPacket('localhost', packet, 1234);
	var imgBytes = plugins.file.readFile('logo.jpg', 1024);
	packet = plugins.udp.createNewPacket();
	packet.writeBytes(imgBytes);
	plugins.udp.sendPacket('localhost', packet, 1234);
	plugins.udp.stopSocket();
}
```
### writeBytes(bytes)

Writes an array of bytes into the packet, at the current index. The index is advanced with a number of positions equal to the length of the written array.

**Parameters**\
[Array](../../JSLib/Array.md) bytes  ;

**Returns**\
void 


**Sample**

```javascript
if (!plugins.udp.startSocket('5555', packetReceived)) {
	application.output('Failed to start socket.');
} else {
	var packet = plugins.udp.createNewPacket();
	packet.writeUTF('hello world!');
	plugins.udp.sendPacket('localhost', packet, 1234);
	packet = plugins.udp.createNewPacket();
	packet.writeByte(0xFF);
	packet.writeShort(10001);
	packet.writeInt(2000000001);
	plugins.udp.sendPacket('localhost', packet, 1234);
	var imgBytes = plugins.file.readFile('logo.jpg', 1024);
	packet = plugins.udp.createNewPacket();
	packet.writeBytes(imgBytes);
	plugins.udp.sendPacket('localhost', packet, 1234);
	plugins.udp.stopSocket();
}
```
### writeInt(number)

Writes a 32 bits int into the packet, at the current index. The index is advances with 4 positions.

**Parameters**\
[Number](../../JSLib/Number.md) number  ;

**Returns**\
void 


**Sample**

```javascript
if (!plugins.udp.startSocket('5555', packetReceived)) {
	application.output('Failed to start socket.');
} else {
	var packet = plugins.udp.createNewPacket();
	packet.writeUTF('hello world!');
	plugins.udp.sendPacket('localhost', packet, 1234);
	packet = plugins.udp.createNewPacket();
	packet.writeByte(0xFF);
	packet.writeShort(10001);
	packet.writeInt(2000000001);
	plugins.udp.sendPacket('localhost', packet, 1234);
	var imgBytes = plugins.file.readFile('logo.jpg', 1024);
	packet = plugins.udp.createNewPacket();
	packet.writeBytes(imgBytes);
	plugins.udp.sendPacket('localhost', packet, 1234);
	plugins.udp.stopSocket();
}
```
### writeShort(number)

Writes a 16 bits short value into the packet, at the current index. The index is advances with 2 positions.

**Parameters**\
[Number](../../JSLib/Number.md) number  ;

**Returns**\
void 


**Sample**

```javascript
if (!plugins.udp.startSocket('5555', packetReceived)) {
	application.output('Failed to start socket.');
} else {
	var packet = plugins.udp.createNewPacket();
	packet.writeUTF('hello world!');
	plugins.udp.sendPacket('localhost', packet, 1234);
	packet = plugins.udp.createNewPacket();
	packet.writeByte(0xFF);
	packet.writeShort(10001);
	packet.writeInt(2000000001);
	plugins.udp.sendPacket('localhost', packet, 1234);
	var imgBytes = plugins.file.readFile('logo.jpg', 1024);
	packet = plugins.udp.createNewPacket();
	packet.writeBytes(imgBytes);
	plugins.udp.sendPacket('localhost', packet, 1234);
	plugins.udp.stopSocket();
}
```
### writeUTF(string)

Writes an UTF-8 encoded string into the packet, at the current index. First the length of the string is written on 4 bytes, then the string is written. The index is advanced with a number of positions equal to the length of the string plus 4.

**Parameters**\
[String](../../JSLib/String.md) string  ;

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
if (!plugins.udp.startSocket('5555', packetReceived)) {
	application.output('Failed to start socket.');
} else {
	var packet = plugins.udp.createNewPacket();
	packet.writeUTF('hello world!');
	plugins.udp.sendPacket('localhost', packet, 1234);
	packet = plugins.udp.createNewPacket();
	packet.writeByte(0xFF);
	packet.writeShort(10001);
	packet.writeInt(2000000001);
	plugins.udp.sendPacket('localhost', packet, 1234);
	var imgBytes = plugins.file.readFile('logo.jpg', 1024);
	packet = plugins.udp.createNewPacket();
	packet.writeBytes(imgBytes);
	plugins.udp.sendPacket('localhost', packet, 1234);
	plugins.udp.stopSocket();
}
```

