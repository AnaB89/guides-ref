#  MailMessage

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Array](../../JSLib/Array.md) | [getAttachments()](MailMessage.md#getattachments)                   | Returns an array of Attachment instances corresponding to the attachments of this message..                                    |
| [String](../../JSLib/String.md) | [getCCAddresses()](MailMessage.md#getccaddresses)                   | Returns a String with all addresses present in the CC field of this message..                                    |
| [String](../../JSLib/String.md) | [getFromAddresses()](MailMessage.md#getfromaddresses)                   | Returns a String with all addresses present in the From field of this message..                                    |
| [String](../../JSLib/String.md) | [getHeaders()](MailMessage.md#getheaders)                   | Returns a String with all headers of this message..                                    |
| [String](../../JSLib/String.md) | [getHtmlMsg()](MailMessage.md#gethtmlmsg)                   | Returns a String with the HTML content of this message..                                    |
| [String](../../JSLib/String.md) | [getPlainMsg()](MailMessage.md#getplainmsg)                   | Returns a String with the plain content of this message..                                    |
| [String](../../JSLib/String.md) | [getRecipientAddresses()](MailMessage.md#getrecipientaddresses)                   | Returns a String with all addresses in the To field of this message..                                    |
| [String](../../JSLib/String.md) | [getReplyAddresses()](MailMessage.md#getreplyaddresses)                   | Returns a String with all addresses in the Reply-To field of this message..                                    |
| [Date](../../JSLib/Date.md) | [getSentDate()](MailMessage.md#getsentdate)                   | Returns a Date instance corresponding to the moment when this message was sent..                                    |
| [String](../../JSLib/String.md) | [getSubject()](MailMessage.md#getsubject)                   | Returns a String with the subject of this message..                                    |

## Methods Details

### getAttachments()

Returns an array of Attachment instances corresponding to the attachments of this message.


**Returns**\
[Array](../../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var msgs = plugins.mail.receiveMail(username, password, true, 0, null, properties);
if (msgs != null)
{
	for (var i=0; i < msgs.length; i++)
	{
		var msg = msgs[i];
		var str = '';
		str += 'From: ' + msg.getFromAddresses() + '\n';
		str += 'To: ' + msg.getRecipientAddresses() + '\n';
		str += 'CC: ' + msg.getCCAddresses() + '\n';
		str += 'Reply to: ' + msg.getReplyAddresses() + '\n';
		str += 'Received on: ' + msg.getReceivedDate() + '\n';
		str += 'Sent on: ' + msg.getSentDate() + '\n\n';
		str += 'Subject: ' + msg.getSubject() + '\n\n';
		str += 'Plain message: ' + msg.getPlainMsg() + '\n\n';
		str += 'HTML message: ' + msg.getHtmlMsg() + '\n\n';
		str += 'Headers: ' + msg.getHeaders() + '\n\n';
		var attachments = msg.getAttachments();
		if (attachments != null) {
			str += 'Number of attachments: ' + attachments.length + '\n\n';
			for (var j=0; j < attachments.length; j++)
			{
				var attachment = attachments[j];
				str += 'Attachment ' + j + '\n';
				str += '	Name: ' + attachment.getName() + '\n';
				str += '	Size: ' + attachment.getData().length + '\n\n';
			}
		}
		plugins.file.writeTXTFile('msg' + i + '.txt', str);
		application.output('Message ' + i + ' retrieved.');
	}
}
else
{
	application.output("Failed to retrieve messages.");
}
```
### getCCAddresses()

Returns a String with all addresses present in the CC field of this message.


**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var msgs = plugins.mail.receiveMail(username, password, true, 0, null, properties);
if (msgs != null)
{
	for (var i=0; i < msgs.length; i++)
	{
		var msg = msgs[i];
		var str = '';
		str += 'From: ' + msg.getFromAddresses() + '\n';
		str += 'To: ' + msg.getRecipientAddresses() + '\n';
		str += 'CC: ' + msg.getCCAddresses() + '\n';
		str += 'Reply to: ' + msg.getReplyAddresses() + '\n';
		str += 'Received on: ' + msg.getReceivedDate() + '\n';
		str += 'Sent on: ' + msg.getSentDate() + '\n\n';
		str += 'Subject: ' + msg.getSubject() + '\n\n';
		str += 'Plain message: ' + msg.getPlainMsg() + '\n\n';
		str += 'HTML message: ' + msg.getHtmlMsg() + '\n\n';
		str += 'Headers: ' + msg.getHeaders() + '\n\n';
		var attachments = msg.getAttachments();
		if (attachments != null) {
			str += 'Number of attachments: ' + attachments.length + '\n\n';
			for (var j=0; j < attachments.length; j++)
			{
				var attachment = attachments[j];
				str += 'Attachment ' + j + '\n';
				str += '	Name: ' + attachment.getName() + '\n';
				str += '	Size: ' + attachment.getData().length + '\n\n';
			}
		}
		plugins.file.writeTXTFile('msg' + i + '.txt', str);
		application.output('Message ' + i + ' retrieved.');
	}
}
else
{
	application.output("Failed to retrieve messages.");
}
```
### getFromAddresses()

Returns a String with all addresses present in the From field of this message.


**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var msgs = plugins.mail.receiveMail(username, password, true, 0, null, properties);
if (msgs != null)
{
	for (var i=0; i < msgs.length; i++)
	{
		var msg = msgs[i];
		var str = '';
		str += 'From: ' + msg.getFromAddresses() + '\n';
		str += 'To: ' + msg.getRecipientAddresses() + '\n';
		str += 'CC: ' + msg.getCCAddresses() + '\n';
		str += 'Reply to: ' + msg.getReplyAddresses() + '\n';
		str += 'Received on: ' + msg.getReceivedDate() + '\n';
		str += 'Sent on: ' + msg.getSentDate() + '\n\n';
		str += 'Subject: ' + msg.getSubject() + '\n\n';
		str += 'Plain message: ' + msg.getPlainMsg() + '\n\n';
		str += 'HTML message: ' + msg.getHtmlMsg() + '\n\n';
		str += 'Headers: ' + msg.getHeaders() + '\n\n';
		var attachments = msg.getAttachments();
		if (attachments != null) {
			str += 'Number of attachments: ' + attachments.length + '\n\n';
			for (var j=0; j < attachments.length; j++)
			{
				var attachment = attachments[j];
				str += 'Attachment ' + j + '\n';
				str += '	Name: ' + attachment.getName() + '\n';
				str += '	Size: ' + attachment.getData().length + '\n\n';
			}
		}
		plugins.file.writeTXTFile('msg' + i + '.txt', str);
		application.output('Message ' + i + ' retrieved.');
	}
}
else
{
	application.output("Failed to retrieve messages.");
}
```
### getHeaders()

Returns a String with all headers of this message.


**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var msgs = plugins.mail.receiveMail(username, password, true, 0, null, properties);
if (msgs != null)
{
	for (var i=0; i < msgs.length; i++)
	{
		var msg = msgs[i];
		var str = '';
		str += 'From: ' + msg.getFromAddresses() + '\n';
		str += 'To: ' + msg.getRecipientAddresses() + '\n';
		str += 'CC: ' + msg.getCCAddresses() + '\n';
		str += 'Reply to: ' + msg.getReplyAddresses() + '\n';
		str += 'Received on: ' + msg.getReceivedDate() + '\n';
		str += 'Sent on: ' + msg.getSentDate() + '\n\n';
		str += 'Subject: ' + msg.getSubject() + '\n\n';
		str += 'Plain message: ' + msg.getPlainMsg() + '\n\n';
		str += 'HTML message: ' + msg.getHtmlMsg() + '\n\n';
		str += 'Headers: ' + msg.getHeaders() + '\n\n';
		var attachments = msg.getAttachments();
		if (attachments != null) {
			str += 'Number of attachments: ' + attachments.length + '\n\n';
			for (var j=0; j < attachments.length; j++)
			{
				var attachment = attachments[j];
				str += 'Attachment ' + j + '\n';
				str += '	Name: ' + attachment.getName() + '\n';
				str += '	Size: ' + attachment.getData().length + '\n\n';
			}
		}
		plugins.file.writeTXTFile('msg' + i + '.txt', str);
		application.output('Message ' + i + ' retrieved.');
	}
}
else
{
	application.output("Failed to retrieve messages.");
}
```
### getHtmlMsg()

Returns a String with the HTML content of this message.


**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var msgs = plugins.mail.receiveMail(username, password, true, 0, null, properties);
if (msgs != null)
{
	for (var i=0; i < msgs.length; i++)
	{
		var msg = msgs[i];
		var str = '';
		str += 'From: ' + msg.getFromAddresses() + '\n';
		str += 'To: ' + msg.getRecipientAddresses() + '\n';
		str += 'CC: ' + msg.getCCAddresses() + '\n';
		str += 'Reply to: ' + msg.getReplyAddresses() + '\n';
		str += 'Received on: ' + msg.getReceivedDate() + '\n';
		str += 'Sent on: ' + msg.getSentDate() + '\n\n';
		str += 'Subject: ' + msg.getSubject() + '\n\n';
		str += 'Plain message: ' + msg.getPlainMsg() + '\n\n';
		str += 'HTML message: ' + msg.getHtmlMsg() + '\n\n';
		str += 'Headers: ' + msg.getHeaders() + '\n\n';
		var attachments = msg.getAttachments();
		if (attachments != null) {
			str += 'Number of attachments: ' + attachments.length + '\n\n';
			for (var j=0; j < attachments.length; j++)
			{
				var attachment = attachments[j];
				str += 'Attachment ' + j + '\n';
				str += '	Name: ' + attachment.getName() + '\n';
				str += '	Size: ' + attachment.getData().length + '\n\n';
			}
		}
		plugins.file.writeTXTFile('msg' + i + '.txt', str);
		application.output('Message ' + i + ' retrieved.');
	}
}
else
{
	application.output("Failed to retrieve messages.");
}
```
### getPlainMsg()

Returns a String with the plain content of this message.


**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var msgs = plugins.mail.receiveMail(username, password, true, 0, null, properties);
if (msgs != null)
{
	for (var i=0; i < msgs.length; i++)
	{
		var msg = msgs[i];
		var str = '';
		str += 'From: ' + msg.getFromAddresses() + '\n';
		str += 'To: ' + msg.getRecipientAddresses() + '\n';
		str += 'CC: ' + msg.getCCAddresses() + '\n';
		str += 'Reply to: ' + msg.getReplyAddresses() + '\n';
		str += 'Received on: ' + msg.getReceivedDate() + '\n';
		str += 'Sent on: ' + msg.getSentDate() + '\n\n';
		str += 'Subject: ' + msg.getSubject() + '\n\n';
		str += 'Plain message: ' + msg.getPlainMsg() + '\n\n';
		str += 'HTML message: ' + msg.getHtmlMsg() + '\n\n';
		str += 'Headers: ' + msg.getHeaders() + '\n\n';
		var attachments = msg.getAttachments();
		if (attachments != null) {
			str += 'Number of attachments: ' + attachments.length + '\n\n';
			for (var j=0; j < attachments.length; j++)
			{
				var attachment = attachments[j];
				str += 'Attachment ' + j + '\n';
				str += '	Name: ' + attachment.getName() + '\n';
				str += '	Size: ' + attachment.getData().length + '\n\n';
			}
		}
		plugins.file.writeTXTFile('msg' + i + '.txt', str);
		application.output('Message ' + i + ' retrieved.');
	}
}
else
{
	application.output("Failed to retrieve messages.");
}
```
### getRecipientAddresses()

Returns a String with all addresses in the To field of this message.


**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var msgs = plugins.mail.receiveMail(username, password, true, 0, null, properties);
if (msgs != null)
{
	for (var i=0; i < msgs.length; i++)
	{
		var msg = msgs[i];
		var str = '';
		str += 'From: ' + msg.getFromAddresses() + '\n';
		str += 'To: ' + msg.getRecipientAddresses() + '\n';
		str += 'CC: ' + msg.getCCAddresses() + '\n';
		str += 'Reply to: ' + msg.getReplyAddresses() + '\n';
		str += 'Received on: ' + msg.getReceivedDate() + '\n';
		str += 'Sent on: ' + msg.getSentDate() + '\n\n';
		str += 'Subject: ' + msg.getSubject() + '\n\n';
		str += 'Plain message: ' + msg.getPlainMsg() + '\n\n';
		str += 'HTML message: ' + msg.getHtmlMsg() + '\n\n';
		str += 'Headers: ' + msg.getHeaders() + '\n\n';
		var attachments = msg.getAttachments();
		if (attachments != null) {
			str += 'Number of attachments: ' + attachments.length + '\n\n';
			for (var j=0; j < attachments.length; j++)
			{
				var attachment = attachments[j];
				str += 'Attachment ' + j + '\n';
				str += '	Name: ' + attachment.getName() + '\n';
				str += '	Size: ' + attachment.getData().length + '\n\n';
			}
		}
		plugins.file.writeTXTFile('msg' + i + '.txt', str);
		application.output('Message ' + i + ' retrieved.');
	}
}
else
{
	application.output("Failed to retrieve messages.");
}
```
### getReplyAddresses()

Returns a String with all addresses in the Reply-To field of this message.


**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var msgs = plugins.mail.receiveMail(username, password, true, 0, null, properties);
if (msgs != null)
{
	for (var i=0; i < msgs.length; i++)
	{
		var msg = msgs[i];
		var str = '';
		str += 'From: ' + msg.getFromAddresses() + '\n';
		str += 'To: ' + msg.getRecipientAddresses() + '\n';
		str += 'CC: ' + msg.getCCAddresses() + '\n';
		str += 'Reply to: ' + msg.getReplyAddresses() + '\n';
		str += 'Received on: ' + msg.getReceivedDate() + '\n';
		str += 'Sent on: ' + msg.getSentDate() + '\n\n';
		str += 'Subject: ' + msg.getSubject() + '\n\n';
		str += 'Plain message: ' + msg.getPlainMsg() + '\n\n';
		str += 'HTML message: ' + msg.getHtmlMsg() + '\n\n';
		str += 'Headers: ' + msg.getHeaders() + '\n\n';
		var attachments = msg.getAttachments();
		if (attachments != null) {
			str += 'Number of attachments: ' + attachments.length + '\n\n';
			for (var j=0; j < attachments.length; j++)
			{
				var attachment = attachments[j];
				str += 'Attachment ' + j + '\n';
				str += '	Name: ' + attachment.getName() + '\n';
				str += '	Size: ' + attachment.getData().length + '\n\n';
			}
		}
		plugins.file.writeTXTFile('msg' + i + '.txt', str);
		application.output('Message ' + i + ' retrieved.');
	}
}
else
{
	application.output("Failed to retrieve messages.");
}
```
### getSentDate()

Returns a Date instance corresponding to the moment when this message was sent.


**Returns**\
[Date](../../JSLib/Date.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var msgs = plugins.mail.receiveMail(username, password, true, 0, null, properties);
if (msgs != null)
{
	for (var i=0; i < msgs.length; i++)
	{
		var msg = msgs[i];
		var str = '';
		str += 'From: ' + msg.getFromAddresses() + '\n';
		str += 'To: ' + msg.getRecipientAddresses() + '\n';
		str += 'CC: ' + msg.getCCAddresses() + '\n';
		str += 'Reply to: ' + msg.getReplyAddresses() + '\n';
		str += 'Received on: ' + msg.getReceivedDate() + '\n';
		str += 'Sent on: ' + msg.getSentDate() + '\n\n';
		str += 'Subject: ' + msg.getSubject() + '\n\n';
		str += 'Plain message: ' + msg.getPlainMsg() + '\n\n';
		str += 'HTML message: ' + msg.getHtmlMsg() + '\n\n';
		str += 'Headers: ' + msg.getHeaders() + '\n\n';
		var attachments = msg.getAttachments();
		if (attachments != null) {
			str += 'Number of attachments: ' + attachments.length + '\n\n';
			for (var j=0; j < attachments.length; j++)
			{
				var attachment = attachments[j];
				str += 'Attachment ' + j + '\n';
				str += '	Name: ' + attachment.getName() + '\n';
				str += '	Size: ' + attachment.getData().length + '\n\n';
			}
		}
		plugins.file.writeTXTFile('msg' + i + '.txt', str);
		application.output('Message ' + i + ' retrieved.');
	}
}
else
{
	application.output("Failed to retrieve messages.");
}
```
### getSubject()

Returns a String with the subject of this message.


**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var msgs = plugins.mail.receiveMail(username, password, true, 0, null, properties);
if (msgs != null)
{
	for (var i=0; i < msgs.length; i++)
	{
		var msg = msgs[i];
		var str = '';
		str += 'From: ' + msg.getFromAddresses() + '\n';
		str += 'To: ' + msg.getRecipientAddresses() + '\n';
		str += 'CC: ' + msg.getCCAddresses() + '\n';
		str += 'Reply to: ' + msg.getReplyAddresses() + '\n';
		str += 'Received on: ' + msg.getReceivedDate() + '\n';
		str += 'Sent on: ' + msg.getSentDate() + '\n\n';
		str += 'Subject: ' + msg.getSubject() + '\n\n';
		str += 'Plain message: ' + msg.getPlainMsg() + '\n\n';
		str += 'HTML message: ' + msg.getHtmlMsg() + '\n\n';
		str += 'Headers: ' + msg.getHeaders() + '\n\n';
		var attachments = msg.getAttachments();
		if (attachments != null) {
			str += 'Number of attachments: ' + attachments.length + '\n\n';
			for (var j=0; j < attachments.length; j++)
			{
				var attachment = attachments[j];
				str += 'Attachment ' + j + '\n';
				str += '	Name: ' + attachment.getName() + '\n';
				str += '	Size: ' + attachment.getData().length + '\n\n';
			}
		}
		plugins.file.writeTXTFile('msg' + i + '.txt', str);
		application.output('Message ' + i + ' retrieved.');
	}
}
else
{
	application.output("Failed to retrieve messages.");
}
```

