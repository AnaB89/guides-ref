#  JSUpload

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [deleteFile()](JSUpload.md#deletefile)                   | Delets this uploaded file so it will be cleaned up if it was streamed in a temp file..                                    |
| [Array](../JSLib/Array.md) | [getBytes()](JSUpload.md#getbytes)                   | This returns the bytes of the uploaded file, try to using streaming or file operation on it (so the bytes don't have to be full loaded in to memory).                                    |
| [String](../JSLib/String.md) | [getContentType()](JSUpload.md#getcontenttype)                   | .                                    |
| [String](../JSLib/String.md) | [getFieldValue(name)](JSUpload.md#getfieldvalue-name)                   | Returns the value for a give form field that was give as metadata to this uploaded file.                                    |
| [Array](../JSLib/Array.md) | [getFields()](JSUpload.md#getfields)                   | This returns the field names of the form fields that where give as metadata to this upload file..                                    |
| [String](../JSLib/String.md) | [getName()](JSUpload.md#getname)                   | .                                    |
| [Number](../JSLib/Number.md) | [getSize()](JSUpload.md#getsize)                   | .                                    |
| [String](../JSLib/String.md) | [getString()](JSUpload.md#getstring)                   | Returns the contents of the file as as string in UTF-8 encoding..                                    |
| [Boolean](../JSLib/Boolean.md) | [isInMemory()](JSUpload.md#isinmemory)                   | If this returns false, then a tmp file is created for it..                                    |
| [Boolean](../JSLib/Boolean.md) | [write(file)](JSUpload.md#write-file)                   | Writes the contents of this upload right to a file..                                    |

## Methods Details

### deleteFile()

Delets this uploaded file so it will be cleaned up if it was streamed in a temp file.
The system tries to clean this up for you, but that can take a while and depends on Garbage Collection.
So it is better to be explicit and delete this file.
if you use JSUpload.write(file) then the file is very likely moved instead of copied so the temp file is also removed.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### getBytes()

This returns the bytes of the uploaded file, try to using streaming or file operation on it (so the bytes don't have to be full loaded in to memory)


**Returns**\
[Array](../JSLib/Array.md) the bytes of the upload file,

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### getContentType()




**Returns**\
[String](../JSLib/String.md) the content type of this upload

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### getFieldValue(name)

Returns the value for a give form field that was give as metadata to this uploaded file

**Parameters**\
[String](../JSLib/String.md) name The form fields name

**Returns**\
[String](../JSLib/String.md) the value that was given or null

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### getFields()

This returns the field names of the form fields that where give as metadata to this upload file.


**Returns**\
[Array](../JSLib/Array.md) String[] Array of names of the field names

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### getName()




**Returns**\
[String](../JSLib/String.md) the name of the upload file.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### getSize()




**Returns**\
[Number](../JSLib/Number.md) the size of the upload

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### getString()

Returns the contents of the file as as string in UTF-8 encoding.


**Returns**\
[String](../JSLib/String.md) the String contents

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### isInMemory()

If this returns false, then a tmp file is created for it. This means that you can also convert this to a JSFile and call rename() on it.
But the method write(file) will always work by writing the contents of this upload file to a different file.


**Returns**\
[Boolean](../JSLib/Boolean.md) true if this upload is fully in memory (not saved to a temp file)

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### write(file)

Writes the contents of this upload right to a file. Use the file plugin to create a JSFile object that can be given to this function.
If this file was not fully in memory (isInMemory == false) then this will just stream the tmp file to the give file.
If it was a temp file then it will try to move the file to the given location (so temp file is moved and because of that already deleted/cleaned up).

**Parameters**\
[Object](../JSLib/Object.md) file the file object where to write to can be a JSFile or path string

**Returns**\
[Boolean](../JSLib/Boolean.md) if write could be done

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```

