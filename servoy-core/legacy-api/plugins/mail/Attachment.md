#  Attachment

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Array](../../JSLib/Array.md) | [getData()](Attachment.md#getdata)                   | Returns a byte array with the content of this attachment..                                    |
| [String](../../JSLib/String.md) | [getMimeType()](Attachment.md#getmimetype)                   | Returns the Mime type of this attachment..                                    |
| [String](../../JSLib/String.md) | [getName()](Attachment.md#getname)                   | Returns the name of this attachment..                                    |
| [Boolean](../../JSLib/Boolean.md) | [isEmbedded()](Attachment.md#isembedded)                   | Returns true if this attachment is embedded, false otherwise..                                    |

## Methods Details

### getData()

Returns a byte array with the content of this attachment.


**Returns**\
[Array](../../JSLib/Array.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var logo = plugins.mail.createBinaryAttachment('logo.jpg', plugins.file.readFile('d:/logo.jpg'));
var invoice = plugins.mail.createTextAttachment('invoice.txt', plugins.file.readTXTFile('d:/invoice.txt'));
var attachments = new Array(logo, invoice);
var success = plugins.mail.sendMail(toAddress, fromAddress, 'subject line', 'message text', null, null, attachments, properties);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert', 'Failed to send mail', 'OK');
}
else
{
	plugins.dialogs.showInfoDialog('Success', 'Mail sent', 'OK');
	application.output('logo attachment name: ' + logo.getName());
	application.output('logo attachment mime type: ' + logo.getMimeType());
	application.output('logo attachment size: ' + logo.getData().length);
	application.output('logo attachment embedded state: ' + logo.isEmbedded());
	application.output('invoice attachment name: ' + invoice.getName());
	application.output('invoice attachment mime type: ' + invoice.getMimeType());
	application.output('invoice attachment size: ' + invoice.getData().length);
	application.output('invoice attachment embedded state: ' + invoice.isEmbedded());
}
```
### getMimeType()

Returns the Mime type of this attachment.


**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var logo = plugins.mail.createBinaryAttachment('logo.jpg', plugins.file.readFile('d:/logo.jpg'));
var invoice = plugins.mail.createTextAttachment('invoice.txt', plugins.file.readTXTFile('d:/invoice.txt'));
var attachments = new Array(logo, invoice);
var success = plugins.mail.sendMail(toAddress, fromAddress, 'subject line', 'message text', null, null, attachments, properties);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert', 'Failed to send mail', 'OK');
}
else
{
	plugins.dialogs.showInfoDialog('Success', 'Mail sent', 'OK');
	application.output('logo attachment name: ' + logo.getName());
	application.output('logo attachment mime type: ' + logo.getMimeType());
	application.output('logo attachment size: ' + logo.getData().length);
	application.output('logo attachment embedded state: ' + logo.isEmbedded());
	application.output('invoice attachment name: ' + invoice.getName());
	application.output('invoice attachment mime type: ' + invoice.getMimeType());
	application.output('invoice attachment size: ' + invoice.getData().length);
	application.output('invoice attachment embedded state: ' + invoice.isEmbedded());
}
```
### getName()

Returns the name of this attachment.


**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var logo = plugins.mail.createBinaryAttachment('logo.jpg', plugins.file.readFile('d:/logo.jpg'));
var invoice = plugins.mail.createTextAttachment('invoice.txt', plugins.file.readTXTFile('d:/invoice.txt'));
var attachments = new Array(logo, invoice);
var success = plugins.mail.sendMail(toAddress, fromAddress, 'subject line', 'message text', null, null, attachments, properties);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert', 'Failed to send mail', 'OK');
}
else
{
	plugins.dialogs.showInfoDialog('Success', 'Mail sent', 'OK');
	application.output('logo attachment name: ' + logo.getName());
	application.output('logo attachment mime type: ' + logo.getMimeType());
	application.output('logo attachment size: ' + logo.getData().length);
	application.output('logo attachment embedded state: ' + logo.isEmbedded());
	application.output('invoice attachment name: ' + invoice.getName());
	application.output('invoice attachment mime type: ' + invoice.getMimeType());
	application.output('invoice attachment size: ' + invoice.getData().length);
	application.output('invoice attachment embedded state: ' + invoice.isEmbedded());
}
```
### isEmbedded()

Returns true if this attachment is embedded, false otherwise. Attachments become embedded 
if they are references through tags from the body text of the message.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var logo = plugins.mail.createBinaryAttachment('logo.jpg', plugins.file.readFile('d:/logo.jpg'));
var invoice = plugins.mail.createTextAttachment('invoice.txt', plugins.file.readTXTFile('d:/invoice.txt'));
var attachments = new Array(logo, invoice);
var success = plugins.mail.sendMail(toAddress, fromAddress, 'subject line', 'message text', null, null, attachments, properties);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert', 'Failed to send mail', 'OK');
}
else
{
	plugins.dialogs.showInfoDialog('Success', 'Mail sent', 'OK');
	application.output('logo attachment name: ' + logo.getName());
	application.output('logo attachment mime type: ' + logo.getMimeType());
	application.output('logo attachment size: ' + logo.getData().length);
	application.output('logo attachment embedded state: ' + logo.isEmbedded());
	application.output('invoice attachment name: ' + invoice.getName());
	application.output('invoice attachment mime type: ' + invoice.getMimeType());
	application.output('invoice attachment size: ' + invoice.getData().length);
	application.output('invoice attachment embedded state: ' + invoice.isEmbedded());
}
```

