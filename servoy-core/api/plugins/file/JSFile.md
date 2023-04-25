#  JSFile


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../../JSLib/Boolean.md) | [canRead()](JSFile.md#canread)                   | Returns true if the file exists and is readable (has access to it) - works on remote files too..                                    |
| [Boolean](../../JSLib/Boolean.md) | [canWrite()](JSFile.md#canwrite)                   | Returns true if the file exists and can be modified - works on remote files too..                                    |
| [Boolean](../../JSLib/Boolean.md) | [createNewFile()](JSFile.md#createnewfile)                   | Creates the file on disk if needed..                                    |
| [Boolean](../../JSLib/Boolean.md) | [deleteFile()](JSFile.md#deletefile)                   | Deletes the file from the disk if possible..                                    |
| [Boolean](../../JSLib/Boolean.md) | [exists()](JSFile.md#exists)                   | Returns true if the file/directory exists on the filesystem - works on remote files too..                                    |
| [JSFile](./JSFile.md) | [getAbsoluteFile()](JSFile.md#getabsolutefile)                   | Returns a JSFile instance that corresponds to the absolute form of this pathname - works on remote files too..                                    |
| [String](../../JSLib/String.md) | [getAbsolutePath()](JSFile.md#getabsolutepath)                   | Returns a String representation of the absolute form of this pathname - works on remote files too..                                    |
| [Array](../../JSLib/Array.md) | [getBytes()](JSFile.md#getbytes)                   | Gets the contents (bytes) for the file data..                                    |
| [String](../../JSLib/String.md) | [getContentType()](JSFile.md#getcontenttype)                   | Returns the contenttype of this file, like for example 'application/pdf' - works on remote files too..                                    |
| [String](../../JSLib/String.md) | [getName()](JSFile.md#getname)                   | Returns the name of the file..                                    |
| [String](../../JSLib/String.md) | [getParent()](JSFile.md#getparent)                   | Returns the String representation of the path of the parent of this file - works on remote files too..                                    |
| [JSFile](./JSFile.md) | [getParentFile()](JSFile.md#getparentfile)                   | Returns a JSFile instance that corresponds to the parent of this file - works on remote files too..                                    |
| [String](../../JSLib/String.md) | [getPath()](JSFile.md#getpath)                   | Returns a String holding the path to the file - works on remote files too..                                    |
| [Boolean](../../JSLib/Boolean.md) | [isAbsolute()](JSFile.md#isabsolute)                   | Returns true if the path is absolute..                                    |
| [Boolean](../../JSLib/Boolean.md) | [isDirectory()](JSFile.md#isdirectory)                   | Returns true if the file is a directory - works on remote files too..                                    |
| [Boolean](../../JSLib/Boolean.md) | [isFile()](JSFile.md#isfile)                   | Returns true if the file is a file and not a regular file - works on remote files too..                                    |
| [Boolean](../../JSLib/Boolean.md) | [isHidden()](JSFile.md#ishidden)                   | Returns true if the file is hidden (a file system attribute) - works on remote files too..                                    |
| [Date](../../JSLib/Date.md) | [lastModified()](JSFile.md#lastmodified)                   | Returns the time/date of the last modification on the file - works on remote files too..                                    |
| [Array](../../JSLib/Array.md) | [list()](JSFile.md#list)                   | Returns an array of strings naming the files and directories located inside the file, if the file is a directory - works on remote files too..                                    |
| [Array](../../JSLib/Array.md) | [listFiles()](JSFile.md#listfiles)                   | Returns an array of JSFiles naming the files and directories located inside the file, if the file is a directory - works on remote files too..                                    |
| [Boolean](../../JSLib/Boolean.md) | [mkdir()](JSFile.md#mkdir)                   | Creates a directory on disk if possible..                                    |
| [Boolean](../../JSLib/Boolean.md) | [mkdirs()](JSFile.md#mkdirs)                   | Creates a directory on disk, together with all its parent directories, if possible..                                    |
| [Boolean](../../JSLib/Boolean.md) | [renameTo(destination)](JSFile.md#renameto-destination)                   | Renames the file to a different name..                                    |
| [Boolean](../../JSLib/Boolean.md) | [setBytes(bytes)](JSFile.md#setbytes-bytes)                   | Set the content of the file (local or remote) to the bytes provided<br/> Will not create a new file if one doesn't exist.                                    |
| [Boolean](../../JSLib/Boolean.md) | [setBytes(bytes, createFile)](JSFile.md#setbytes-bytes-createfile)                   | Set the content of the file (local or remote) to the bytes provided.                                    |
| [Boolean](../../JSLib/Boolean.md) | [setLastModified(date)](JSFile.md#setlastmodified-date)                   | Sets the date/time of the last modification on the file..                                    |
| [Boolean](../../JSLib/Boolean.md) | [setReadOnly()](JSFile.md#setreadonly)                   | Sets the readonly attribute of the file/directory..                                    |
| [Number](../../JSLib/Number.md) | [size()](JSFile.md#size)                   | Returns the size in bytes of the file..                                    |

## Methods Details

### canRead()

Returns true if the file exists and is readable (has access to it) - works on remote files too.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('./big.jpg');
// or for a remote file:
// var f = plugins.convertToRemoteJSFile('/images/big.jpg');
if (f && f.exists()) {
	application.output('is absolute: ' + f.isAbsolute());
	application.output('is dir: ' + f.isDirectory());
	application.output('is file: ' + f.isFile());
	application.output('is hidden: ' + f.isHidden());
	application.output('can read: ' + f.canRead());
	application.output('can write: ' + f.canWrite());
	application.output('last modified: ' + f.lastModified());
	application.output('name: ' + f.getName());
	application.output('path: ' + f.getPath());
	application.output('absolute path: ' + f.getAbsolutePath());
	application.output('content type: ' + f.getContentType());
	application.output('size: ' + f.size());
}
else {
	application.output('File/folder not found.');
}
```
### canWrite()

Returns true if the file exists and can be modified - works on remote files too.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('./big.jpg');
// or for a remote file:
// var f = plugins.convertToRemoteJSFile('/images/big.jpg');
if (f && f.exists()) {
	application.output('is absolute: ' + f.isAbsolute());
	application.output('is dir: ' + f.isDirectory());
	application.output('is file: ' + f.isFile());
	application.output('is hidden: ' + f.isHidden());
	application.output('can read: ' + f.canRead());
	application.output('can write: ' + f.canWrite());
	application.output('last modified: ' + f.lastModified());
	application.output('name: ' + f.getName());
	application.output('path: ' + f.getPath());
	application.output('absolute path: ' + f.getAbsolutePath());
	application.output('content type: ' + f.getContentType());
	application.output('size: ' + f.size());
}
else {
	application.output('File/folder not found.');
}
```
### createNewFile()

Creates the file on disk if needed. Returns true if the file (name) did not already exists and had to be created - for remote, use the streamFilesToServer to stream a file.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('story.txt');
if (!f.exists())
	f.createNewFile();
```
### deleteFile()

Deletes the file from the disk if possible. Returns true if the file could be deleted. If the file is a directory, then it must be empty in order to be deleted - works on remote files too.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('story.txt');
// or for a remote file:
// var f = plugins.convertToRemoteJSFile('/story.txt');
if (f && f.exists())
	f.deleteFile();
```
### exists()

Returns true if the file/directory exists on the filesystem - works on remote files too.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('./big.jpg');
// or for a remote file:
// var f = plugins.convertToRemoteJSFile('/images/big.jpg');
if (f && f.exists()) {
	application.output('is absolute: ' + f.isAbsolute());
	application.output('is dir: ' + f.isDirectory());
	application.output('is file: ' + f.isFile());
	application.output('is hidden: ' + f.isHidden());
	application.output('can read: ' + f.canRead());
	application.output('can write: ' + f.canWrite());
	application.output('last modified: ' + f.lastModified());
	application.output('name: ' + f.getName());
	application.output('path: ' + f.getPath());
	application.output('absolute path: ' + f.getAbsolutePath());
	application.output('content type: ' + f.getContentType());
	application.output('size: ' + f.size());
}
else {
	application.output('File/folder not found.');
}
```
### getAbsoluteFile()

Returns a JSFile instance that corresponds to the absolute form of this pathname - works on remote files too.


**Returns**\
[JSFile](./JSFile.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('story.txt');
// or for a remote file:
// var f = plugins.file.convertToRemoteJSFile('/story.txt');
application.output('parent folder: ' + f.getAbsoluteFile().getParent());
application.output('parent folder has ' + f.getAbsoluteFile().getParentFile().listFiles().length + ' entries');
```
### getAbsolutePath()

Returns a String representation of the absolute form of this pathname - works on remote files too.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('./big.jpg');
// or for a remote file:
// var f = plugins.convertToRemoteJSFile('/images/big.jpg');
if (f && f.exists()) {
	application.output('is absolute: ' + f.isAbsolute());
	application.output('is dir: ' + f.isDirectory());
	application.output('is file: ' + f.isFile());
	application.output('is hidden: ' + f.isHidden());
	application.output('can read: ' + f.canRead());
	application.output('can write: ' + f.canWrite());
	application.output('last modified: ' + f.lastModified());
	application.output('name: ' + f.getName());
	application.output('path: ' + f.getPath());
	application.output('absolute path: ' + f.getAbsolutePath());
	application.output('content type: ' + f.getContentType());
	application.output('size: ' + f.size());
}
else {
	application.output('File/folder not found.');
}
```
### getBytes()

Gets the contents (bytes) for the file data.


**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
var theFile = plugins.file.showFileOpenDialog();
application.output('The file size in bytes: ' + theFile.getBytes());
```
### getContentType()

Returns the contenttype of this file, like for example 'application/pdf' - works on remote files too.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('./big.jpg');
// or for a remote file:
// var f = plugins.convertToRemoteJSFile('/images/big.jpg');
if (f && f.exists()) {
	application.output('is absolute: ' + f.isAbsolute());
	application.output('is dir: ' + f.isDirectory());
	application.output('is file: ' + f.isFile());
	application.output('is hidden: ' + f.isHidden());
	application.output('can read: ' + f.canRead());
	application.output('can write: ' + f.canWrite());
	application.output('last modified: ' + f.lastModified());
	application.output('name: ' + f.getName());
	application.output('path: ' + f.getPath());
	application.output('absolute path: ' + f.getAbsolutePath());
	application.output('content type: ' + f.getContentType());
	application.output('size: ' + f.size());
}
else {
	application.output('File/folder not found.');
}
```
### getName()

Returns the name of the file. The name consists in the last part of the file path - works on remote files too.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('./big.jpg');
// or for a remote file:
// var f = plugins.convertToRemoteJSFile('/images/big.jpg');
if (f && f.exists()) {
	application.output('is absolute: ' + f.isAbsolute());
	application.output('is dir: ' + f.isDirectory());
	application.output('is file: ' + f.isFile());
	application.output('is hidden: ' + f.isHidden());
	application.output('can read: ' + f.canRead());
	application.output('can write: ' + f.canWrite());
	application.output('last modified: ' + f.lastModified());
	application.output('name: ' + f.getName());
	application.output('path: ' + f.getPath());
	application.output('absolute path: ' + f.getAbsolutePath());
	application.output('content type: ' + f.getContentType());
	application.output('size: ' + f.size());
}
else {
	application.output('File/folder not found.');
}
```
### getParent()

Returns the String representation of the path of the parent of this file - works on remote files too.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('story.txt');
// or for a remote file:
// var f = plugins.file.convertToRemoteJSFile('/story.txt');
application.output('parent folder: ' + f.getAbsoluteFile().getParent());
application.output('parent folder has ' + f.getAbsoluteFile().getParentFile().listFiles().length + ' entries');
```
### getParentFile()

Returns a JSFile instance that corresponds to the parent of this file - works on remote files too.


**Returns**\
[JSFile](./JSFile.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('story.txt');
// or for a remote file:
// var f = plugins.file.convertToRemoteJSFile('/story.txt');
application.output('parent folder: ' + f.getAbsoluteFile().getParent());
application.output('parent folder has ' + f.getAbsoluteFile().getParentFile().listFiles().length + ' entries');
```
### getPath()

Returns a String holding the path to the file - works on remote files too.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('./big.jpg');
// or for a remote file:
// var f = plugins.convertToRemoteJSFile('/images/big.jpg');
if (f && f.exists()) {
	application.output('is absolute: ' + f.isAbsolute());
	application.output('is dir: ' + f.isDirectory());
	application.output('is file: ' + f.isFile());
	application.output('is hidden: ' + f.isHidden());
	application.output('can read: ' + f.canRead());
	application.output('can write: ' + f.canWrite());
	application.output('last modified: ' + f.lastModified());
	application.output('name: ' + f.getName());
	application.output('path: ' + f.getPath());
	application.output('absolute path: ' + f.getAbsolutePath());
	application.output('content type: ' + f.getContentType());
	application.output('size: ' + f.size());
}
else {
	application.output('File/folder not found.');
}
```
### isAbsolute()

Returns true if the path is absolute. The path is absolute if it starts with '/' on Unix/Linux/MacOS or has a driver letter on Windows - works on remote files too.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('./big.jpg');
// or for a remote file:
// var f = plugins.convertToRemoteJSFile('/images/big.jpg');
if (f && f.exists()) {
	application.output('is absolute: ' + f.isAbsolute());
	application.output('is dir: ' + f.isDirectory());
	application.output('is file: ' + f.isFile());
	application.output('is hidden: ' + f.isHidden());
	application.output('can read: ' + f.canRead());
	application.output('can write: ' + f.canWrite());
	application.output('last modified: ' + f.lastModified());
	application.output('name: ' + f.getName());
	application.output('path: ' + f.getPath());
	application.output('absolute path: ' + f.getAbsolutePath());
	application.output('content type: ' + f.getContentType());
	application.output('size: ' + f.size());
}
else {
	application.output('File/folder not found.');
}
```
### isDirectory()

Returns true if the file is a directory - works on remote files too.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('./big.jpg');
// or for a remote file:
// var f = plugins.convertToRemoteJSFile('/images/big.jpg');
if (f && f.exists()) {
	application.output('is absolute: ' + f.isAbsolute());
	application.output('is dir: ' + f.isDirectory());
	application.output('is file: ' + f.isFile());
	application.output('is hidden: ' + f.isHidden());
	application.output('can read: ' + f.canRead());
	application.output('can write: ' + f.canWrite());
	application.output('last modified: ' + f.lastModified());
	application.output('name: ' + f.getName());
	application.output('path: ' + f.getPath());
	application.output('absolute path: ' + f.getAbsolutePath());
	application.output('content type: ' + f.getContentType());
	application.output('size: ' + f.size());
}
else {
	application.output('File/folder not found.');
}
```
### isFile()

Returns true if the file is a file and not a regular file - works on remote files too.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('./big.jpg');
// or for a remote file:
// var f = plugins.convertToRemoteJSFile('/images/big.jpg');
if (f && f.exists()) {
	application.output('is absolute: ' + f.isAbsolute());
	application.output('is dir: ' + f.isDirectory());
	application.output('is file: ' + f.isFile());
	application.output('is hidden: ' + f.isHidden());
	application.output('can read: ' + f.canRead());
	application.output('can write: ' + f.canWrite());
	application.output('last modified: ' + f.lastModified());
	application.output('name: ' + f.getName());
	application.output('path: ' + f.getPath());
	application.output('absolute path: ' + f.getAbsolutePath());
	application.output('content type: ' + f.getContentType());
	application.output('size: ' + f.size());
}
else {
	application.output('File/folder not found.');
}
```
### isHidden()

Returns true if the file is hidden (a file system attribute) - works on remote files too.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('./big.jpg');
// or for a remote file:
// var f = plugins.convertToRemoteJSFile('/images/big.jpg');
if (f && f.exists()) {
	application.output('is absolute: ' + f.isAbsolute());
	application.output('is dir: ' + f.isDirectory());
	application.output('is file: ' + f.isFile());
	application.output('is hidden: ' + f.isHidden());
	application.output('can read: ' + f.canRead());
	application.output('can write: ' + f.canWrite());
	application.output('last modified: ' + f.lastModified());
	application.output('name: ' + f.getName());
	application.output('path: ' + f.getPath());
	application.output('absolute path: ' + f.getAbsolutePath());
	application.output('content type: ' + f.getContentType());
	application.output('size: ' + f.size());
}
else {
	application.output('File/folder not found.');
}
```
### lastModified()

Returns the time/date of the last modification on the file - works on remote files too.


**Returns**\
[Date](../../JSLib/Date.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('./big.jpg');
// or for a remote file:
// var f = plugins.convertToRemoteJSFile('/images/big.jpg');
if (f && f.exists()) {
	application.output('is absolute: ' + f.isAbsolute());
	application.output('is dir: ' + f.isDirectory());
	application.output('is file: ' + f.isFile());
	application.output('is hidden: ' + f.isHidden());
	application.output('can read: ' + f.canRead());
	application.output('can write: ' + f.canWrite());
	application.output('last modified: ' + f.lastModified());
	application.output('name: ' + f.getName());
	application.output('path: ' + f.getPath());
	application.output('absolute path: ' + f.getAbsolutePath());
	application.output('content type: ' + f.getContentType());
	application.output('size: ' + f.size());
}
else {
	application.output('File/folder not found.');
}
```
### list()

Returns an array of strings naming the files and directories located inside the file, if the file is a directory - works on remote files too.


**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
var d = plugins.file.convertToJSFile('plugins');
// or for a remote file:
// var d = plugins.convertToRemoteJSFile('/plugins');
var names = d.list();
application.output('Names:');
for (var i=0; i<names.length; i++)
	application.output(names[i]);
var files = d.listFiles();
application.output('Absolute paths:');
for (var i=0; i<files.length; i++)
	application.output(files[i].getAbsolutePath());
```
### listFiles()

Returns an array of JSFiles naming the files and directories located inside the file, if the file is a directory - works on remote files too.


**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
var d = plugins.file.convertToJSFile('plugins');
// or for a remote file:
// var d = plugins.convertToRemoteJSFile('/plugins');
var names = d.list();
application.output('Names:');
for (var i=0; i<names.length; i++)
	application.output(names[i]);
var files = d.listFiles();
application.output('Absolute paths:');
for (var i=0; i<files.length; i++)
	application.output(files[i].getAbsolutePath());
```
### mkdir()

Creates a directory on disk if possible. Returns true if a new directory was created - for remote, use the streamFilesToServer to create the directory instead.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('one/two/three/four');
f.mkdirs(); // Create all four levels of folders in one step.
var g = plugins.file.convertToJSFile('one/two/three/four/five');
g.mkdir(); // This will work because all parent folders are already created.
```
### mkdirs()

Creates a directory on disk, together with all its parent directories, if possible. Returns true if the hierarchy of directories is created - for remote, use the streamFilesToServer to create the directories instead.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('one/two/three/four');
f.mkdirs(); // Create all four levels of folders in one step.
var g = plugins.file.convertToJSFile('one/two/three/four/five');
g.mkdir(); // This will work because all parent folders are already created.
```
### renameTo(destination)

Renames the file to a different name. Returns true if the file could be renamed - works on remote files too.

**Parameters**\
[Object](../../JSLib/Object.md) destination  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('story.txt');
f.renameTo('otherstory.txt');
// or for a remote file:
// var f = plugins.convertToRemoteJSFile('/story.txt');
// f.renameTo('/otherstory.txt');
```
### setBytes(bytes)

Set the content of the file (local or remote) to the bytes provided
Will not create a new file if one doesn't exist

**Parameters**\
[Array](../../JSLib/Array.md) bytes the data

**Returns**\
[Boolean](../../JSLib/Boolean.md) true if the operation worked


**Sample**

```javascript
var file = plugins.file.convertToJSFile('/pathTo/file.jpg');
// or for a remote file:
// var file = plugins.file.convertToRemoteJSFile('/remotePathTo/file.jpg');
var success = file.setBytes(blobDataProvider, true);
```
### setBytes(bytes, createFile)

Set the content of the file (local or remote) to the bytes provided

**Parameters**\
[Array](../../JSLib/Array.md) bytes the data\
[Boolean](../../JSLib/Boolean.md) createFile true to create a file if it doesn't exist

**Returns**\
[Boolean](../../JSLib/Boolean.md) true if the operation worked


**Sample**

```javascript
var file = plugins.file.convertToJSFile('/pathTo/file.jpg');
// or for a remote file:
// var file = plugins.file.convertToRemoteJSFile('/remotePathTo/file.jpg');
var success = file.setBytes(blobDataProvider, true);
```
### setLastModified(date)

Sets the date/time of the last modification on the file.

**Parameters**\
[Object](../../JSLib/Object.md) date  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('story.txt');
f.createNewFile();
// Make the file look old.
f.setLastModified(new Date(1999, 5, 21));
```
### setReadOnly()

Sets the readonly attribute of the file/directory. Returns true on success.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('invoice.txt');
plugins.file.writeTXTFile(f, 'important data that should not be changed');
f.setReadOnly();
```
### size()

Returns the size in bytes of the file. Returns 0 if the file does not exist on disk - works on remote files too.


**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var f = plugins.file.convertToJSFile('./big.jpg');
// or for a remote file:
// var f = plugins.convertToRemoteJSFile('/images/big.jpg');
if (f && f.exists()) {
	application.output('is absolute: ' + f.isAbsolute());
	application.output('is dir: ' + f.isDirectory());
	application.output('is file: ' + f.isFile());
	application.output('is hidden: ' + f.isHidden());
	application.output('can read: ' + f.canRead());
	application.output('can write: ' + f.canWrite());
	application.output('last modified: ' + f.lastModified());
	application.output('name: ' + f.getName());
	application.output('path: ' + f.getPath());
	application.output('absolute path: ' + f.getAbsolutePath());
	application.output('content type: ' + f.getContentType());
	application.output('size: ' + f.size());
}
else {
	application.output('File/folder not found.');
}
```

