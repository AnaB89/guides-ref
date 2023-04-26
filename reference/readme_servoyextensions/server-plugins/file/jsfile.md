# JSFile

## Methods Summary

| Type                                                             | Name                                                               | Summary                                                                                                                                        |
| ---------------------------------------------------------------- | ------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| [Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) | [canRead()](jsfile.md#canread)                                     | Returns true if the file exists and is readable (has access to it) - works on remote files too..                                               |
| [Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) | [canWrite()](jsfile.md#canwrite)                                   | Returns true if the file exists and can be modified - works on remote files too..                                                              |
| [Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) | [createNewFile()](jsfile.md#createnewfile)                         | Creates the file on disk if needed..                                                                                                           |
| [Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) | [deleteFile()](jsfile.md#deletefile)                               | Deletes the file from the disk if possible..                                                                                                   |
| [Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) | [exists()](jsfile.md#exists)                                       | Returns true if the file/directory exists on the filesystem - works on remote files too..                                                      |
| [JSFile](jsfile.md)                                              | [getAbsoluteFile()](jsfile.md#getabsolutefile)                     | Returns a JSFile instance that corresponds to the absolute form of this pathname - works on remote files too..                                 |
| [String](../../../readme\_servoycore/dev-api/js-lib/string.md)   | [getAbsolutePath()](jsfile.md#getabsolutepath)                     | Returns a String representation of the absolute form of this pathname - works on remote files too..                                            |
| [Array](../../../readme\_servoycore/dev-api/js-lib/array.md)     | [getBytes()](jsfile.md#getbytes)                                   | Gets the contents (bytes) for the file data..                                                                                                  |
| [String](../../../readme\_servoycore/dev-api/js-lib/string.md)   | [getContentType()](jsfile.md#getcontenttype)                       | Returns the contenttype of this file, like for example 'application/pdf' - works on remote files too..                                         |
| [String](../../../readme\_servoycore/dev-api/js-lib/string.md)   | [getName()](jsfile.md#getname)                                     | Returns the name of the file..                                                                                                                 |
| [String](../../../readme\_servoycore/dev-api/js-lib/string.md)   | [getParent()](jsfile.md#getparent)                                 | Returns the String representation of the path of the parent of this file - works on remote files too..                                         |
| [JSFile](jsfile.md)                                              | [getParentFile()](jsfile.md#getparentfile)                         | Returns a JSFile instance that corresponds to the parent of this file - works on remote files too..                                            |
| [String](../../../readme\_servoycore/dev-api/js-lib/string.md)   | [getPath()](jsfile.md#getpath)                                     | Returns a String holding the path to the file - works on remote files too..                                                                    |
| [Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) | [isAbsolute()](jsfile.md#isabsolute)                               | Returns true if the path is absolute..                                                                                                         |
| [Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) | [isDirectory()](jsfile.md#isdirectory)                             | Returns true if the file is a directory - works on remote files too..                                                                          |
| [Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) | [isFile()](jsfile.md#isfile)                                       | Returns true if the file is a file and not a regular file - works on remote files too..                                                        |
| [Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) | [isHidden()](jsfile.md#ishidden)                                   | Returns true if the file is hidden (a file system attribute) - works on remote files too..                                                     |
| [Date](../../../readme\_servoycore/dev-api/js-lib/date.md)       | [lastModified()](jsfile.md#lastmodified)                           | Returns the time/date of the last modification on the file - works on remote files too..                                                       |
| [Array](../../../readme\_servoycore/dev-api/js-lib/array.md)     | [list()](jsfile.md#list)                                           | Returns an array of strings naming the files and directories located inside the file, if the file is a directory - works on remote files too.. |
| [Array](../../../readme\_servoycore/dev-api/js-lib/array.md)     | [listFiles()](jsfile.md#listfiles)                                 | Returns an array of JSFiles naming the files and directories located inside the file, if the file is a directory - works on remote files too.. |
| [Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) | [mkdir()](jsfile.md#mkdir)                                         | Creates a directory on disk if possible..                                                                                                      |
| [Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) | [mkdirs()](jsfile.md#mkdirs)                                       | Creates a directory on disk, together with all its parent directories, if possible..                                                           |
| [Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) | [renameTo(destination)](jsfile.md#renameto-destination)            | Renames the file to a different name..                                                                                                         |
| [Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) | [setBytes(bytes)](jsfile.md#setbytes-bytes)                        | <p>Set the content of the file (local or remote) to the bytes provided<br>Will not create a new file if one doesn't exist.</p>                 |
| [Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) | [setBytes(bytes, createFile)](jsfile.md#setbytes-bytes-createfile) | Set the content of the file (local or remote) to the bytes provided.                                                                           |
| [Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) | [setLastModified(date)](jsfile.md#setlastmodified-date)            | Sets the date/time of the last modification on the file..                                                                                      |
| [Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) | [setReadOnly()](jsfile.md#setreadonly)                             | Sets the readonly attribute of the file/directory..                                                                                            |
| [Number](../../../readme\_servoycore/dev-api/js-lib/number.md)   | [size()](jsfile.md#size)                                           | Returns the size in bytes of the file..                                                                                                        |

## Methods Details

### canRead()

Returns true if the file exists and is readable (has access to it) - works on remote files too.

**Returns**\
[Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md)

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
[Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md)

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
[Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md)

**Sample**

```javascript
var f = plugins.file.convertToJSFile('story.txt');
if (!f.exists())
	f.createNewFile();
```

### deleteFile()

Deletes the file from the disk if possible. Returns true if the file could be deleted. If the file is a directory, then it must be empty in order to be deleted - works on remote files too.

**Returns**\
[Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md)

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
[Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md)

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
[JSFile](jsfile.md)

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
[String](../../../readme\_servoycore/dev-api/js-lib/string.md)

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
[Array](../../../readme\_servoycore/dev-api/js-lib/array.md)

**Sample**

```javascript
var theFile = plugins.file.showFileOpenDialog();
application.output('The file size in bytes: ' + theFile.getBytes());
```

### getContentType()

Returns the contenttype of this file, like for example 'application/pdf' - works on remote files too.

**Returns**\
[String](../../../readme\_servoycore/dev-api/js-lib/string.md)

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
[String](../../../readme\_servoycore/dev-api/js-lib/string.md)

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
[String](../../../readme\_servoycore/dev-api/js-lib/string.md)

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
[JSFile](jsfile.md)

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
[String](../../../readme\_servoycore/dev-api/js-lib/string.md)

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
[Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md)

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
[Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md)

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
[Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md)

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
[Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md)

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
[Date](../../../readme\_servoycore/dev-api/js-lib/date.md)

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
[Array](../../../readme\_servoycore/dev-api/js-lib/array.md)

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
[Array](../../../readme\_servoycore/dev-api/js-lib/array.md)

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
[Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md)

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
[Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md)

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
[Object](../../../readme\_servoycore/dev-api/js-lib/object.md) destination ;

**Returns**\
[Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md)

**Sample**

```javascript
var f = plugins.file.convertToJSFile('story.txt');
f.renameTo('otherstory.txt');
// or for a remote file:
// var f = plugins.convertToRemoteJSFile('/story.txt');
// f.renameTo('/otherstory.txt');
```

### setBytes(bytes)

Set the content of the file (local or remote) to the bytes provided Will not create a new file if one doesn't exist

**Parameters**\
[Array](../../../readme\_servoycore/dev-api/js-lib/array.md) bytes the data

**Returns**\
[Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) true if the operation worked

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
[Array](../../../readme\_servoycore/dev-api/js-lib/array.md) bytes the data\
[Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) createFile true to create a file if it doesn't exist

**Returns**\
[Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md) true if the operation worked

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
[Object](../../../readme\_servoycore/dev-api/js-lib/object.md) date ;

**Returns**\
[Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md)

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
[Boolean](../../../readme\_servoycore/dev-api/js-lib/boolean.md)

**Sample**

```javascript
var f = plugins.file.convertToJSFile('invoice.txt');
plugins.file.writeTXTFile(f, 'important data that should not be changed');
f.setReadOnly();
```

### size()

Returns the size in bytes of the file. Returns 0 if the file does not exist on disk - works on remote files too.

**Returns**\
[Number](../../../readme\_servoycore/dev-api/js-lib/number.md)

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
