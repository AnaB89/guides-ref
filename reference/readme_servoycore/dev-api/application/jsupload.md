# JSUpload

## Methods Summary

| Type                            | Name                                                  | Summary                                                                                                                                               |
| ------------------------------- | ----------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| void                            | [deleteFile()](jsupload.md#deletefile)                | Delets this uploaded file so it will be cleaned up if it was streamed in a temp file..                                                                |
| [Array](../js-lib/array.md)     | [getBytes()](jsupload.md#getbytes)                    | This returns the bytes of the uploaded file, try to using streaming or file operation on it (so the bytes don't have to be full loaded in to memory). |
| [String](../js-lib/string.md)   | [getContentType()](jsupload.md#getcontenttype)        | .                                                                                                                                                     |
| [String](../js-lib/string.md)   | [getFieldValue(name)](jsupload.md#getfieldvalue-name) | Returns the value for a give form field that was give as metadata to this uploaded file.                                                              |
| [Array](../js-lib/array.md)     | [getFields()](jsupload.md#getfields)                  | This returns the field names of the form fields that where give as metadata to this upload file..                                                     |
| [String](../js-lib/string.md)   | [getName()](jsupload.md#getname)                      | .                                                                                                                                                     |
| [Number](../js-lib/number.md)   | [getSize()](jsupload.md#getsize)                      | .                                                                                                                                                     |
| [String](../js-lib/string.md)   | [getString()](jsupload.md#getstring)                  | Returns the contents of the file as as string in UTF-8 encoding..                                                                                     |
| [Boolean](../js-lib/boolean.md) | [isInMemory()](jsupload.md#isinmemory)                | If this returns false, then a tmp file is created for it..                                                                                            |
| [Boolean](../js-lib/boolean.md) | [write(file)](jsupload.md#write-file)                 | Writes the contents of this upload right to a file..                                                                                                  |

## Methods Details

### deleteFile()

Delets this uploaded file so it will be cleaned up if it was streamed in a temp file. The system tries to clean this up for you, but that can take a while and depends on Garbage Collection. So it is better to be explicit and delete this file. if you use JSUpload.write(file) then the file is very likely moved instead of copied so the temp file is also removed.

**Returns**\
void

**Sample**

```javascript
```

### getBytes()

This returns the bytes of the uploaded file, try to using streaming or file operation on it (so the bytes don't have to be full loaded in to memory)

**Returns**\
[Array](../js-lib/array.md) the bytes of the upload file,

**Sample**

```javascript
```

### getContentType()

**Returns**\
[String](../js-lib/string.md) the content type of this upload

**Sample**

```javascript
```

### getFieldValue(name)

Returns the value for a give form field that was give as metadata to this uploaded file

**Parameters**\
[String](../js-lib/string.md) name The form fields name

**Returns**\
[String](../js-lib/string.md) the value that was given or null

**Sample**

```javascript
```

### getFields()

This returns the field names of the form fields that where give as metadata to this upload file.

**Returns**\
[Array](../js-lib/array.md) String\[] Array of names of the field names

**Sample**

```javascript
```

### getName()

**Returns**\
[String](../js-lib/string.md) the name of the upload file.

**Sample**

```javascript
```

### getSize()

**Returns**\
[Number](../js-lib/number.md) the size of the upload

**Sample**

```javascript
```

### getString()

Returns the contents of the file as as string in UTF-8 encoding.

**Returns**\
[String](../js-lib/string.md) the String contents

**Sample**

```javascript
```

### isInMemory()

If this returns false, then a tmp file is created for it. This means that you can also convert this to a JSFile and call rename() on it. But the method write(file) will always work by writing the contents of this upload file to a different file.

**Returns**\
[Boolean](../js-lib/boolean.md) true if this upload is fully in memory (not saved to a temp file)

**Sample**

```javascript
```

### write(file)

Writes the contents of this upload right to a file. Use the file plugin to create a JSFile object that can be given to this function. If this file was not fully in memory (isInMemory == false) then this will just stream the tmp file to the give file. If it was a temp file then it will try to move the file to the given location (so temp file is moved and because of that already deleted/cleaned up).

**Parameters**\
[Object](../js-lib/object.md) file the file object where to write to can be a JSFile or path string

**Returns**\
[Boolean](../js-lib/boolean.md) if write could be done

**Sample**

```javascript
```
