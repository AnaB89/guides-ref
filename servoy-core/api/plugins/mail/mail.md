#  mail

## **Return Types**
[MailMessage](./MailMessage.md),[Attachment](./Attachment.md),

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../../JSLib/String.md) | [from](mail.md#from)                   | Returns the value of the mail..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Attachment](./Attachment.md) | [createBinaryAttachment(filename, binarydata)](mail.md#createbinaryattachment-filename-binarydata)                   | Creates a binary attachment object..                                    |
| [Attachment](./Attachment.md) | [createBinaryAttachment(filename, binarydata, mimeType)](mail.md#createbinaryattachment-filename-binarydata-mimetype)                   | Creates a binary attachment object..                                    |
| [Attachment](./Attachment.md) | [createTextAttachment(filename, textdata)](mail.md#createtextattachment-filename-textdata)                   | Creates a text based attachment objec with the default 'text/plain' mimetype.                                    |
| [Attachment](./Attachment.md) | [createTextAttachment(filename, textdata, mimeType)](mail.md#createtextattachment-filename-textdata-mimetype)                   | Creates a text based attachment object..                                    |
| [String](../../JSLib/String.md) | [getLastSendMailExceptionMsg()](mail.md#getlastsendmailexceptionmsg)                   | Get the exception that occurred in the last sendMail attempt (null if no exception occurred)..                                    |
| [MailMessage](./MailMessage.md) | [getMailMessage(binaryblob/string)](mail.md#getmailmessage-binaryblob/string)                   | Helper method, returns MailMessage object from binary or 7bits string..                                    |
| [Array](../../JSLib/Array.md) | [getPlainMailAddresses(addressesString)](mail.md#getplainmailaddresses-addressesstring)                   | Helper method to only get the plain addresses..                                    |
| [Boolean](../../JSLib/Boolean.md) | [isValidEmailAddress(email)](mail.md#isvalidemailaddress-email)                   | Checks whether the given e-mail address is valid or not..                                    |
| [Array](../../JSLib/Array.md) | [receiveMail(username, password, leaveMsgsOnServer)](mail.md#receivemail-username-password-leavemsgsonserver)                   | Receive mails from pop3 account..                                    |
| [Array](../../JSLib/Array.md) | [receiveMail(username, password, leaveMsgsOnServer, receiveMode)](mail.md#receivemail-username-password-leavemsgsonserver-receivemode)                   | Receive mails from pop3 account..                                    |
| [Array](../../JSLib/Array.md) | [receiveMail(username, password, leaveMsgsOnServer, receiveMode, onlyReceiveMsgWithSentDate)](mail.md#receivemail-username-password-leavemsgsonserver-receivemode-onlyreceivemsgwithsentdate)                   | Receive mails from pop3 account..                                    |
| [Array](../../JSLib/Array.md) | [receiveMail(username, password, leaveMsgsOnServer, receiveMode, onlyReceiveMsgWithSentDate, pop3Host)](mail.md#receivemail-username-password-leavemsgsonserver-receivemode-onlyreceivemsgwithsentdate-pop3host)                   | Receive mails from pop3 account..                                    |
| [Array](../../JSLib/Array.md) | [receiveMail(username, password, leaveMsgsOnServer, receiveMode, onlyReceiveMsgWithSentDate, properties)](mail.md#receivemail-username-password-leavemsgsonserver-receivemode-onlyreceivemsgwithsentdate-properties)                   | Receive mails from pop3 account..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendBulkMail(to, from, subject, msgText)](mail.md#sendbulkmail-to-from-subject-msgtext)                   | Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendBulkMail(to, from, subject, msgText, cc)](mail.md#sendbulkmail-to-from-subject-msgtext-cc)                   | Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendBulkMail(to, from, subject, msgText, cc, bcc)](mail.md#sendbulkmail-to-from-subject-msgtext-cc-bcc)                   | Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendBulkMail(to, from, subject, msgText, cc, bcc, attachment)](mail.md#sendbulkmail-to-from-subject-msgtext-cc-bcc-attachment)                   | Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendBulkMail(to, from, subject, msgText, cc, bcc, attachment, smtpHost)](mail.md#sendbulkmail-to-from-subject-msgtext-cc-bcc-attachment-smtphost)                   | Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendBulkMail(to, from, subject, msgText, cc, bcc, attachment, overrideProperties)](mail.md#sendbulkmail-to-from-subject-msgtext-cc-bcc-attachment-overrideproperties)                   | Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendBulkMail(to, from, subject, msgText, cc, bcc, attachments)](mail.md#sendbulkmail-to-from-subject-msgtext-cc-bcc-attachments)                   | Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendBulkMail(to, from, subject, msgText, cc, bcc, attachments, smtpHost)](mail.md#sendbulkmail-to-from-subject-msgtext-cc-bcc-attachments-smtphost)                   | Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendBulkMail(to, from, subject, msgText, cc, bcc, attachments, overrideProperties)](mail.md#sendbulkmail-to-from-subject-msgtext-cc-bcc-attachments-overrideproperties)                   | Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendMail(to, from, subject, msgText)](mail.md#sendmail-to-from-subject-msgtext)                   | Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendMail(to, from, subject, msgText, cc)](mail.md#sendmail-to-from-subject-msgtext-cc)                   | Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendMail(to, from, subject, msgText, cc, bcc)](mail.md#sendmail-to-from-subject-msgtext-cc-bcc)                   | Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendMail(to, from, subject, msgText, cc, bcc, attachment)](mail.md#sendmail-to-from-subject-msgtext-cc-bcc-attachment)                   | Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendMail(to, from, subject, msgText, cc, bcc, attachment, smtpHost)](mail.md#sendmail-to-from-subject-msgtext-cc-bcc-attachment-smtphost)                   | Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendMail(to, from, subject, msgText, cc, bcc, attachment, overrideProperties)](mail.md#sendmail-to-from-subject-msgtext-cc-bcc-attachment-overrideproperties)                   | Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendMail(to, from, subject, msgText, cc, bcc, attachments)](mail.md#sendmail-to-from-subject-msgtext-cc-bcc-attachments)                   | Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendMail(to, from, subject, msgText, cc, bcc, attachments, smtpHost)](mail.md#sendmail-to-from-subject-msgtext-cc-bcc-attachments-smtphost)                   | Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |
| [Boolean](../../JSLib/Boolean.md) | [sendMail(to, from, subject, msgText, cc, bcc, attachments, overrideProperties)](mail.md#sendmail-to-from-subject-msgtext-cc-bcc-attachments-overrideproperties)                   | Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting)..                                    |

## Properties Details

### from

Returns the value of the mail.from property which is set on the admin page.

**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var from = plugins.mail.from
```

## Methods Details

### createBinaryAttachment(filename, binarydata)

Creates a binary attachment object.

**Parameters**\
[String](../../JSLib/String.md) filename  ;\
[Array](../../JSLib/Array.md) binarydata  ;

**Returns**\
[Attachment](./Attachment.md) 


**Sample**

```javascript
var attachment1 = plugins.mail.createBinaryAttachment('logo1.gif',plugins.file.readFile('c:/temp/a_logo.gif'));
var attachment2 = plugins.mail.createBinaryAttachment('logo2.gif',plugins.file.readFile('c:/temp/another_logo.gif'));
var success = plugins.mail.sendMail('to_someone@example.com', 'John Cobb <from_me@example.org>', 'subject', 'msgText',null,null,new Array(attachment1,attachment2));
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send mail','OK');
}
```
### createBinaryAttachment(filename, binarydata, mimeType)

Creates a binary attachment object.

**Parameters**\
[String](../../JSLib/String.md) filename  ;\
[Array](../../JSLib/Array.md) binarydata  ;\
[String](../../JSLib/String.md) mimeType  ;

**Returns**\
[Attachment](./Attachment.md) 


**Sample**

```javascript
var attachment1 = plugins.mail.createBinaryAttachment('logo1.gif',plugins.file.readFile('c:/temp/a_logo.gif', 'image/gif'));
var attachment2 = plugins.mail.createBinaryAttachment('logo2.gif',plugins.file.readFile('c:/temp/another_logo.gif', 'image/gif'));
var success = plugins.mail.sendMail('to_someone@example.com', 'John Cobb <from_me@example.org>', 'subject', 'msgText',null,null,new Array(attachment1,attachment2));
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send mail','OK');
}
```
### createTextAttachment(filename, textdata)

Creates a text based attachment objec with the default 'text/plain' mimetype

**Parameters**\
[String](../../JSLib/String.md) filename  ;\
[String](../../JSLib/String.md) textdata  ;

**Returns**\
[Attachment](./Attachment.md) 


**Sample**

```javascript
var attachment = plugins.mail.createTextAttachment('readme.html','<html>bla bla bla');
var success = plugins.mail.sendMail('to_someone@example.com', 'John Cobb <from_me@example.com>', 'subject', 'msgText',null,null,attachment);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send mail','OK');
}
```
### createTextAttachment(filename, textdata, mimeType)

Creates a text based attachment object.

**Parameters**\
[String](../../JSLib/String.md) filename  ;\
[String](../../JSLib/String.md) textdata  ;\
[String](../../JSLib/String.md) mimeType  ;

**Returns**\
[Attachment](./Attachment.md) 


**Sample**

```javascript
var attachment = plugins.mail.createTextAttachment('readme.html','<html>bla bla bla', 'text/html');
var success = plugins.mail.sendMail('to_someone@example.com', 'John Cobb <from_me@example.com>', 'subject', 'msgText',null,null,attachment);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send mail','OK');
}
```
### getLastSendMailExceptionMsg()

Get the exception that occurred in the last sendMail attempt (null if no exception occurred).


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var success = plugins.mail.sendMail('to_someone@example.com,to_someone_else@example.org', 'John Cobb <from_me@example.com>', 'subject', 'my message',null,'unnamed@example.com');
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert',plugins.mail.getLastSendMailExceptionMsg(),'OK');
}
```
### getMailMessage(binaryblob/string)

Helper method, returns MailMessage object from binary or 7bits string.

**Parameters**\
[Object](../../JSLib/Object.md) binaryblob/string  ;

**Returns**\
[MailMessage](./MailMessage.md) 


**Sample**

```javascript
var msg = plugins.mail.getMailMessage(myBlob);
if (msg != null) //if is null error occurred!
{
	application.output(msg.getFromAddresses())
}
```
### getPlainMailAddresses(addressesString)

Helper method to only get the plain addresses.

**Parameters**\
[Object](../../JSLib/Object.md) addressesString  ;

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
var plainArray = plugins.mail.getPlainMailAddresses('John Cobb <from_me@example.com>,Pete Cobb<from_pete@example.com>');
application.output(plainArray[0]) //will return 'from_me@example.com'
```
### isValidEmailAddress(email)

Checks whether the given e-mail address is valid or not.

**Parameters**\
[String](../../JSLib/String.md) email  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
plugins.mail.isValidEmailAddress("me@example.com");
```
### receiveMail(username, password, leaveMsgsOnServer)

Receive mails from pop3 account.

**Parameters**\
[String](../../JSLib/String.md) username  ;\
[String](../../JSLib/String.md) password  ;\
[Boolean](../../JSLib/Boolean.md) leaveMsgsOnServer  ;

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
var msgs = plugins.mail.receiveMail('mylogin', 'secretpass',  true);
if (msgs != null) //if is null error occurred!
{
	for (var i = 0 ; i < msgs.length ; i++)
	{
		var msg = msgs[i]
		application.output(msg.getFromAddresses())
		application.output(msg.getRecipientAddresses())
		application.output(msg.getReplyAddresses())
		application.output(msg.getSentDate())
		application.output(msg.getHeaders())
		application.output(msg.getSubject())
		application.output(msg.getHtmlMsg())
		application.output(msg.getPlainMsg())
		var attachments = msg.getAttachments()
		if (attachments != null)
		{
			for (var j = 0 ; j < attachments.length ; j++)
			{
				var attachment = attachments[j]
				application.output(attachment.getName())
				var attachmentDataByteArray = attachment.getData()
				//write attachmentDataByteArray to a file...
			}
		}
	}
}
```
### receiveMail(username, password, leaveMsgsOnServer, receiveMode)

Receive mails from pop3 account.

**Parameters**\
[String](../../JSLib/String.md) username  ;\
[String](../../JSLib/String.md) password  ;\
[Boolean](../../JSLib/Boolean.md) leaveMsgsOnServer  ;\
[Number](../../JSLib/Number.md) receiveMode  ;

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
var receiveMode = 1;//0=FULL,1=HEADERS_ONLY,2=NO_ATTACHMENTS
var msgs = plugins.mail.receiveMail('mylogin', 'secretpass',  true,  0);
if (msgs != null) //if is null error occurred!
{
	for (var i = 0 ; i < msgs.length ; i++)
	{
		var msg = msgs[i]
		application.output(msg.getFromAddresses())
		application.output(msg.getRecipientAddresses())
		application.output(msg.getReplyAddresses())
		application.output(msg.getSentDate())
		application.output(msg.getHeaders())
		application.output(msg.getSubject())
	}
}
```
### receiveMail(username, password, leaveMsgsOnServer, receiveMode, onlyReceiveMsgWithSentDate)

Receive mails from pop3 account.

**Parameters**\
[String](../../JSLib/String.md) username  ;\
[String](../../JSLib/String.md) password  ;\
[Boolean](../../JSLib/Boolean.md) leaveMsgsOnServer  ;\
[Number](../../JSLib/Number.md) receiveMode  ;\
[Date](../../JSLib/Date.md) onlyReceiveMsgWithSentDate  ;

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
//it is also possible to first receive the headers and later receive a full message with particular 'sentdate'
//var receiveMode = 1;//0=FULL,1=HEADERS_ONLY,2=NO_ATTACHMENTS
var msgs = plugins.mail.receiveMail('mylogin', 'secretpass',  true,  0,  theSentDateObjectFormPreviousHeaderLoading);
if (msgs != null) //if is null error occurred!
{
	for (var i = 0 ; i < msgs.length ; i++)
	{
		var msg = msgs[i]
		application.output(msg.getFromAddresses())
		application.output(msg.getRecipientAddresses())
		application.output(msg.getReplyAddresses())
		application.output(msg.getSentDate())
		application.output(msg.getHeaders())
		application.output(msg.getSubject())
	}
}
```
### receiveMail(username, password, leaveMsgsOnServer, receiveMode, onlyReceiveMsgWithSentDate, pop3Host)

Receive mails from pop3 account.

**Parameters**\
[String](../../JSLib/String.md) username  ;\
[String](../../JSLib/String.md) password  ;\
[Boolean](../../JSLib/Boolean.md) leaveMsgsOnServer  ;\
[Number](../../JSLib/Number.md) receiveMode  ;\
[Date](../../JSLib/Date.md) onlyReceiveMsgWithSentDate  ;\
[String](../../JSLib/String.md) pop3Host  ;

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
//it is also possible to first receive the headers and later receive a full message
var receiveMode = 0;//0=FULL,1=HEADERS_ONLY,2=NO_ATTACHMENTS
var pop3Host = 'myserver.com';
var msgs = plugins.mail.receiveMail('mylogin', 'secretpass',  true,  receiveMode,  null, pop3Host);
if (msgs != null) //if is null error occurred!
{
	for (var i = 0 ; i < msgs.length ; i++)
	{
		var msg = msgs[i]
		application.output(msg.getFromAddresses())
		application.output(msg.getRecipientAddresses())
		application.output(msg.getReplyAddresses())
		application.output(msg.getSentDate())
		application.output(msg.getHeaders())
		application.output(msg.getSubject())
		application.output(msg.getHtmlMsg())
		application.output(msg.getPlainMsg())
		var attachments = msg.getAttachments()
		if (attachments != null)
		{
			for (var j = 0 ; j < attachments.length ; j++)
			{
				var attachment = attachments[j]
				application.output(attachment.getName())
				var attachmentDataByteArray = attachment.getData()
				//write attachmentDataByteArray to a file...
			}
		}
	}
}
```
### receiveMail(username, password, leaveMsgsOnServer, receiveMode, onlyReceiveMsgWithSentDate, properties)

Receive mails from pop3 account.

**Parameters**\
[String](../../JSLib/String.md) username  ;\
[String](../../JSLib/String.md) password  ;\
[Boolean](../../JSLib/Boolean.md) leaveMsgsOnServer  ;\
[Number](../../JSLib/Number.md) receiveMode  ;\
[Date](../../JSLib/Date.md) onlyReceiveMsgWithSentDate  ;\
[Array](../../JSLib/Array.md) properties  ;

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
var receiveMode = 1;//0=FULL,1=HEADERS_ONLY,2=NO_ATTACHMENTS

var properties = new Array();
properties[0] = 'mail.pop3.port=995';
properties[1] = 'mail.pop3.ssl.enable=true';
properties[2] = 'mail.pop3.host=myserver.com';
properties[3] = 'mail.pop3.user=user@myserver.com';

var msgs = plugins.mail.receiveMail('mylogin', 'secretpass',  true,  receiveMode,  null, properties);
if (msgs != null) //if is null error occurred!
{
	for (var i = 0 ; i < msgs.length ; i++)
	{
		var msg = msgs[i]
		application.output(msg.getFromAddresses())
		application.output(msg.getRecipientAddresses())
		application.output(msg.getReplyAddresses())
		application.output(msg.getSentDate())
		application.output(msg.getHeaders())
		application.output(msg.getSubject())
	}
}
```
### sendBulkMail(to, from, subject, msgText)

Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
A bulk email makes it possible for one to not receive "out of office" emails back from receiver.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the bulk mail\
[String](../../JSLib/String.md) msgText The message text

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
var success = plugins.mail.sendBulkMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>,replyTo@example.com', 'subject', msgText);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send bulk mail','OK');
}
```
### sendBulkMail(to, from, subject, msgText, cc)

Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
A bulk email makes it possible for one to not receive "out of office" emails back from receiver.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the bulk mail\
[String](../../JSLib/String.md) msgText The message text\
[String](../../JSLib/String.md) cc One or more addresses separated by a comma

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
var success = plugins.mail.sendBulkMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>', 'subject', msgText,'cc1@example.com,cc2@example.com');
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send bulk mail','OK');
}
```
### sendBulkMail(to, from, subject, msgText, cc, bcc)

Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
A bulk email makes it possible for one to not receive "out of office" emails back from receiver.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the bulk mail\
[String](../../JSLib/String.md) msgText The message text\
[String](../../JSLib/String.md) cc One or more addresses separated by a comma\
[String](../../JSLib/String.md) bcc One or more addresses separated by a comma

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
var success = plugins.mail.sendBulkMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>', 'subject', msgText,null,'bcc1@example.com');
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send bulk mail','OK');
}
```
### sendBulkMail(to, from, subject, msgText, cc, bcc, attachment)

Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
A bulk email makes it possible for one to not receive "out of office" emails back from receiver.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the bulk mail\
[String](../../JSLib/String.md) msgText The message text\
[String](../../JSLib/String.md) cc One or more addresses separated by a comma\
[String](../../JSLib/String.md) bcc One or more addresses separated by a comma\
[Attachment](./Attachment.md) attachment A single attachment

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var attachment = plugins.mail.createBinaryAttachment('embedded',plugins.file.readFile('c:/temp/a_logo.gif'));
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
var success = plugins.mail.sendBulkMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>', 'subject', msgText,null,'bcc1@example.com,bcc2@example.com',attachment);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send bulk mail','OK');
}
```
### sendBulkMail(to, from, subject, msgText, cc, bcc, attachment, smtpHost)

Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
A bulk email makes it possible for one to not receive "out of office" emails back from receiver.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the bulk mail\
[String](../../JSLib/String.md) msgText The message text\
[String](../../JSLib/String.md) cc One or more addresses separated by a comma\
[String](../../JSLib/String.md) bcc One or more addresses separated by a comma\
[Attachment](./Attachment.md) attachment A single attachment\
[String](../../JSLib/String.md) smtpHost The smtp host

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var attachment = plugins.mail.createBinaryAttachment('embedded',plugins.file.readFile('c:/temp/a_logo.gif'));
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
var smtphost = 'myserver.com';
var success = plugins.mail.sendBulkMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>', 'subject', msgText,null,'unnamed@example.com',attachment,smtphost);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send bulk mail','OK');
}
```
### sendBulkMail(to, from, subject, msgText, cc, bcc, attachment, overrideProperties)

Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
A bulk email makes it possible for one to not receive "out of office" emails back from receiver.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the bulk mail\
[String](../../JSLib/String.md) msgText The message text\
[String](../../JSLib/String.md) cc One or more addresses separated by a comma\
[String](../../JSLib/String.md) bcc One or more addresses separated by a comma\
[Attachment](./Attachment.md) attachment A single attachment\
[Array](../../JSLib/Array.md) overrideProperties An array of properties

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var attachment = plugins.mail.createBinaryAttachment('embedded',plugins.file.readFile('c:/temp/a_logo.gif'));
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
//it is possbile to set all kind of smtp properties
var properties = new Array()
properties[0] = 'mail.smtp.host=myserver.com'
// properties specification can be found at:https://javaee.github.io/javamail/docs/api/com/sun/mail/smtp/package-summary.html
var success = plugins.mail.sendBulkMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>', 'subject', msgText,null,'unnamed@example.com',attachment,properties);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send bulk mail','OK');
}
```
### sendBulkMail(to, from, subject, msgText, cc, bcc, attachments)

Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
A bulk email makes it possible for one to not receive "out of office" emails back from receiver.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the bulk mail\
[String](../../JSLib/String.md) msgText The message text\
[String](../../JSLib/String.md) cc One or more addresses separated by a comma\
[String](../../JSLib/String.md) bcc One or more addresses separated by a comma\
[Array](../../JSLib/Array.md) attachments The attachments

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var attachment1 = plugins.mail.createBinaryAttachment('embedded',plugins.file.readFile('c:/temp/a_logo.gif'));
var attachment2 = plugins.mail.createTextAttachment('embedded','A text attachement');
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
var success = plugins.mail.sendBulkMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>', 'subject', msgText,null,'bcc1@example.com,bcc2@example.com',[attachment1,attachment2]);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send bulk mail','OK');
}
```
### sendBulkMail(to, from, subject, msgText, cc, bcc, attachments, smtpHost)

Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
A bulk email makes it possible for one to not receive "out of office" emails back from receiver.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the bulk mail\
[String](../../JSLib/String.md) msgText The message text\
[String](../../JSLib/String.md) cc One or more addresses separated by a comma\
[String](../../JSLib/String.md) bcc One or more addresses separated by a comma\
[Array](../../JSLib/Array.md) attachments The attachments\
[String](../../JSLib/String.md) smtpHost The smtp host

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var attachment1 = plugins.mail.createBinaryAttachment('embedded',plugins.file.readFile('c:/temp/a_logo.gif'));
var attachment2 = plugins.mail.createTextAttachment('embedded','A text attachement');
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
var smtphost = 'myserver.com';
var success = plugins.mail.sendBulkMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>', 'subject', msgText,null,'unnamed@example.com',[attachment1,attachement2],smtphost);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send bulk mail','OK');
}
```
### sendBulkMail(to, from, subject, msgText, cc, bcc, attachments, overrideProperties)

Send a bulk mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
A bulk email makes it possible for one to not receive "out of office" emails back from receiver.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the bulk mail\
[String](../../JSLib/String.md) msgText The message text\
[String](../../JSLib/String.md) cc One or more addresses separated by a comma\
[String](../../JSLib/String.md) bcc One or more addresses separated by a comma\
[Array](../../JSLib/Array.md) attachments The attachments\
[Array](../../JSLib/Array.md) overrideProperties An array of properties

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var attachment1 = plugins.mail.createBinaryAttachment('embedded',plugins.file.readFile('c:/temp/a_logo.gif'));
var attachment2 = plugins.mail.createTextAttachment('embedded','A text attachement');
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
//it is possbile to set all kind of smtp properties
var properties = new Array()
properties[0] = 'mail.smtp.host=myserver.com'
// properties specification can be found at:https://javaee.github.io/javamail/docs/api/com/sun/mail/smtp/package-summary.html
var success = plugins.mail.sendBulkMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>', 'subject', msgText,null,'unnamed@example.com',[attachment1,attachement2],properties);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send bulk mail','OK');
}
```
### sendMail(to, from, subject, msgText)

Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
If you want to have a different reply address than from, you can specify this with the from parameter by adding another email after it.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the mail\
[String](../../JSLib/String.md) msgText The message text

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
var success = plugins.mail.sendMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>,replyTo@example.com', 'subject', msgText);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send mail','OK');
}
```
### sendMail(to, from, subject, msgText, cc)

Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
If you want to have a different reply address than from, you can specify this with the from parameter by adding another email after it.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the mail\
[String](../../JSLib/String.md) msgText The message text\
[String](../../JSLib/String.md) cc One or more addresses separated by a comma

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
var success = plugins.mail.sendMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>', 'subject', msgText,'cc1@example.com,cc2@example.com');
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send mail','OK');
}
```
### sendMail(to, from, subject, msgText, cc, bcc)

Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
If you want to have a different reply address than from, you can specify this with the from parameter by adding another email after it.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the mail\
[String](../../JSLib/String.md) msgText The message text\
[String](../../JSLib/String.md) cc One or more addresses separated by a comma\
[String](../../JSLib/String.md) bcc One or more addresses separated by a comma

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
var success = plugins.mail.sendMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>', 'subject', msgText,null,'bcc1@example.com');
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send mail','OK');
}
```
### sendMail(to, from, subject, msgText, cc, bcc, attachment)

Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
If you want to have a different reply address than from, you can specify this with the from parameter by adding another email after it.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the mail\
[String](../../JSLib/String.md) msgText The message text\
[String](../../JSLib/String.md) cc One or more addresses separated by a comma\
[String](../../JSLib/String.md) bcc One or more addresses separated by a comma\
[Attachment](./Attachment.md) attachment A single attachment

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var attachment = plugins.mail.createBinaryAttachment('embedded',plugins.file.readFile('c:/temp/a_logo.gif'));
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
var success = plugins.mail.sendMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>', 'subject', msgText,null,'bcc1@example.com,bcc2@example.com',attachment);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send mail','OK');
}
```
### sendMail(to, from, subject, msgText, cc, bcc, attachment, smtpHost)

Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
If you want to have a different reply address than from, you can specify this with the from parameter by adding another email after it.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the mail\
[String](../../JSLib/String.md) msgText The message text\
[String](../../JSLib/String.md) cc One or more addresses separated by a comma\
[String](../../JSLib/String.md) bcc One or more addresses separated by a comma\
[Attachment](./Attachment.md) attachment A single attachment\
[String](../../JSLib/String.md) smtpHost The smtp host

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var attachment = plugins.mail.createBinaryAttachment('embedded',plugins.file.readFile('c:/temp/a_logo.gif'));
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
var smtphost = 'myserver.com';
var success = plugins.mail.sendMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>', 'subject', msgText,null,'unnamed@example.com',attachment,smtphost);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send mail','OK');
}
```
### sendMail(to, from, subject, msgText, cc, bcc, attachment, overrideProperties)

Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
If you want to have a different reply address than from, you can specify this with the from parameter by adding another email after it.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the mail\
[String](../../JSLib/String.md) msgText The message text\
[String](../../JSLib/String.md) cc One or more addresses separated by a comma\
[String](../../JSLib/String.md) bcc One or more addresses separated by a comma\
[Attachment](./Attachment.md) attachment A single attachment\
[Array](../../JSLib/Array.md) overrideProperties An array of properties

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var attachment = plugins.mail.createBinaryAttachment('embedded',plugins.file.readFile('c:/temp/a_logo.gif'));
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
//it is possbile to set all kind of smtp properties
var properties = new Array()
properties[0] = 'mail.smtp.host=myserver.com'
// properties specification can be found at:https://javaee.github.io/javamail/docs/api/com/sun/mail/smtp/package-summary.html
var success = plugins.mail.sendMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>', 'subject', msgText,null,'unnamed@example.com',attachment,properties);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send mail','OK');
}
```
### sendMail(to, from, subject, msgText, cc, bcc, attachments)

Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
If you want to have a different reply address than from, you can specify this with the from parameter by adding another email after it.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the mail\
[String](../../JSLib/String.md) msgText The message text\
[String](../../JSLib/String.md) cc One or more addresses separated by a comma\
[String](../../JSLib/String.md) bcc One or more addresses separated by a comma\
[Array](../../JSLib/Array.md) attachments The attachments

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var attachment1 = plugins.mail.createBinaryAttachment('embedded',plugins.file.readFile('c:/temp/a_logo.gif'));
var attachment2 = plugins.mail.createTextAttachment('embedded','A text attachement');
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
var success = plugins.mail.sendMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>', 'subject', msgText,null,'bcc1@example.com,bcc2@example.com',[attachment1,attachment2]);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send mail','OK');
}
```
### sendMail(to, from, subject, msgText, cc, bcc, attachments, smtpHost)

Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
If you want to have a different reply address than from, you can specify this with the from parameter by adding another email after it.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the mail\
[String](../../JSLib/String.md) msgText The message text\
[String](../../JSLib/String.md) cc One or more addresses separated by a comma\
[String](../../JSLib/String.md) bcc One or more addresses separated by a comma\
[Array](../../JSLib/Array.md) attachments The attachments\
[String](../../JSLib/String.md) smtpHost The smtp host

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var attachment1 = plugins.mail.createBinaryAttachment('embedded',plugins.file.readFile('c:/temp/a_logo.gif'));
var attachment2 = plugins.mail.createTextAttachment('embedded','A text attachement');
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
var smtphost = 'myserver.com';
var success = plugins.mail.sendMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>', 'subject', msgText,null,'unnamed@example.com',[attachment1,attachement2],smtphost);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send mail','OK');
}
```
### sendMail(to, from, subject, msgText, cc, bcc, attachments, overrideProperties)

Send a mail, if you make the msgText start with <html> the message will be sent in html (and you can use all html formatting).
If you want to have a different reply address than from, you can specify this with the from parameter by adding another email after it.

**Parameters**\
[String](../../JSLib/String.md) to A string containing 1 or multiple addresses separated by a comma.\
[String](../../JSLib/String.md) from A string containing an address and optional reply addresses, separated by commas.\
[String](../../JSLib/String.md) subject The subject of the mail\
[String](../../JSLib/String.md) msgText The message text\
[String](../../JSLib/String.md) cc One or more addresses separated by a comma\
[String](../../JSLib/String.md) bcc One or more addresses separated by a comma\
[Array](../../JSLib/Array.md) attachments The attachments\
[Array](../../JSLib/Array.md) overrideProperties An array of properties

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var attachment1 = plugins.mail.createBinaryAttachment('embedded',plugins.file.readFile('c:/temp/a_logo.gif'));
var attachment2 = plugins.mail.createTextAttachment('embedded','A text attachement');
var msgText = 'plain msg<html>styled html msg<img src="%%embedded%%"></html>';
//it is possbile to set all kind of smtp properties
var properties = new Array()
properties[0] = 'mail.smtp.host=myserver.com'
// properties specification can be found at:https://javaee.github.io/javamail/docs/api/com/sun/mail/smtp/package-summary.html
var success = plugins.mail.sendMail('to_someone@example.com,to_someone_else@example.net', 'John Cobb <from_me@example.com>', 'subject', msgText,null,'unnamed@example.com',[attachment1,attachement2],properties);
if (!success)
{
	plugins.dialogs.showWarningDialog('Alert','Failed to send mail','OK');
}
```

