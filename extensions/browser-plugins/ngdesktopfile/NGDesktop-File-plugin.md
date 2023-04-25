Welcome to the **ngdesktopfile** wiki! This wiki provides comprehensive documentation to using the **ngdesktopfile** web service. This service works with the NGDesktop Client as a bridge to execute client side calls dealing with filesystem from Servoy.


# Getting Started
First import the service using one of the release [binaries](https://github.com/Servoy/ngdesktopfile/releases) or via Servoy's Web Package Manager.

# Example Usage

# API Documentation 

## Method Summary

### homeDir
Returns the home dir of the user like c:/users/[username] under windows. Will return always a both with forward slashes.

### tmpDir
Returns the tmp directory of the client machine. Will return always a both with forward slashes.

### listDir
returns an array of filenames that are in the given path. Please use forward slashes (/) instead of backward slashes.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
path | string | Path to lookup | Required

### watchDir
Watch a directory for changes at the given path.
The following events will be generated:
 - add is for adding file
 - addDir is for adding folders
 - unlink is for deleting files
 - unlinkDir is for delete folders
 - change is for changing files

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
path | string | Path to directory | Required
callback | string | callback for events | Required

### unwatchDir
Stop watching a directory found at the given path.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
path | string | Path to directory | Required

### watchFile
Watches a give path, that should represent a file, for modifications. Please use forward slashes (/) instead of backward slashes in the path/filename.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
path | string | Path to file | Required
callback | function | callback for events | Required

### unwatchFile
Removes the watch to the file that was added by the watchFile() function. Please use forward slashes (/) instead of backward slashes in the path/filename.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
path | string | Path to file | Required

### writeFile
Writes the given bytes to the path, if the path has sub directories that are not there then those are made. If the path is missing or contain only the file name then the native system dialog for saving files it is called. Please use forward slashes (/) instead of backward slashes in the path/filename.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
path | string | Path to file | Required
bytes | byte array | File bytes | Required

### readFile
Reads the given bytes of a path, the callback is a function that will get as parameters the 'path' as a String and the 'file' as a JSUpload object. If the path is missing or contain only the file name then the native system dialog for opening files it is called. Please use forward slashes (/) instead of backward slashes in the path/filename

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
callback | function | callback for events | Optional
path | string | Path to file | Required

### setReadOnly
Set permissions to the specified file. If readOnly parameter is false, the file permisions flags will be set to read/write mode.
Return a boolean indicating success or failure

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
path | string | Path to file | Required
flag | boolean | Path to file | Required

### getReadOnly
Verify readonly status on the specified file. 
Returns true for readonly status otherwise false

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
path | string | Path to file | Required

### deletFileSync
Delete the given file, returning a boolean indicating success or failure.
Return boolean indicating success or failure

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
path | string | Path to file | Required

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
callback | string | callback for selected folder | Required

### deleteFile
Delete a files at given path. Please use forward slashes (/) instead of backward slashes in the path/filename.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
path | string | Path to file | Required
errorCallback | function | callback for events | Optional

### selectDirectory
Select a folder and pass its path to the callback

### showSaveDialog
Shows a file save dialog and calls the callback method with the file path.
For the options object see https://www.electronjs.org/docs/api/dialog#dialogshowsavedialogsyncbrowserwindow-options

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
callback | function | Callback to be called | Required
options | object | Dialog's options | Optional

Core options are:

 - title: String the dialog title.
 - defaultPath: String - absolute directory path, absolute file path, or file name to use by default.
 - buttonLabel: String - custom label for the confirmation button, when left empty the default label will be used.
 - filters: Array<{name: String, extensions: Array<String>}> - an array of file filters (e.g. [{ name: 'Images', extensions: ['jpg', 'png', 'gif'] }])

### showSaveDialogSync
To not block any process, showSaveDialog with a callback method is preferred over this method
For the options object see https://www.electronjs.org/docs/api/dialog#dialogshowsavedialogsyncbrowserwindow-options

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
options | object | Dialog's options | Optional

Core options are:

 - title: String the dialog title.
 - defaultPath: String - absolute directory path, absolute file path, or file name to use by default.
 - buttonLabel: String - custom label for the confirmation button, when left empty the default label will be used.
 - filters: Array<{name: String, extensions: Array<String>}> - an array of file filters (e.g. [{ name: 'Images', extensions: ['jpg', 'png', 'gif'] }])

### showOpenDialog
Shows a file open dialog and calls the callback with the selected file path(s)
For the options object see https://www.electronjs.org/docs/api/dialog#dialogshowopendialogbrowserwindow-options

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
callback | function | Callback to be called | Required
options | object | Dialog's options | Optional

Core options are:
 
 - title: String the dialog title.
 - defaultPath: String the default (starting) path.
 - buttonLabel: String custom label for the confirmation button, when left empty the default label will be used.
 - filters: Array<{name: String, extensions: Array<String>}> an array of file filters (e.g. [{ name: 'Images', extensions: ['jpg', 'png', 'gif'] }]).

properties: an Array of property keywords such as

 - openFile: Allow files to be selected.
 - openDirectory: Allow directories to be selected.
 - multiSelections: Allow multiple paths to be selected.

### showOpenDialogSync
Shows a file open dialog and calls the callback with the selected file path(s)
To not block any process, showOpenDialog with a callback method is preferred over this method
For the options object see https://www.electronjs.org/docs/api/dialog#dialogshowopendialogbrowserwindow-options

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
options | object | Dialog's options | Optional

Core options are:
 
 - title: String the dialog title.
 - defaultPath: String the default (starting) path.
 - buttonLabel: String custom label for the confirmation button, when left empty the default label will be used.
 - filters: Array<{name: String, extensions: Array<String>}> an array of file filters (e.g. [{ name: 'Images', extensions: ['jpg', 'png', 'gif'] }])

properties: an Array of property keywords such as 

 - openFile: Allow files to be selected.
 - openDirectory: Allow directories to be selected.
 - multiSelections: Allow multiple paths to be selected.

### openFile
Opens a file specified at the given path on the client. This path must exist on the client's machine, you can't open a file with a path pointing to a file on the server, use writeFile() first to write it to the clients machine. It returns a string value. If the value is empty, then the file has been successfully opened, otherwise the string contains the error message.
			 
**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
path | string | Path to the file | Required

### exists
Test whether or not the given path exists by checking with the file system. It returns true if the path exists, false otherwise.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
path | string | Path to the file | Required

### appendToTXTFile
Synchronously append data to a file, creating the file if it does not yet exist. Return a boolean indicating success or failure

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
path | string | Path to the file | Required
text | string | Text to be added | Required
encoding | string | encoding text (defaults to utf8)

The supportd encoding is mapping to the list provided by nodejs (https://nodejs.org/api/buffer.html#buffers-and-character-encodings) 

### copyFile
Synchronously copies src to dest. By default, dest is overwritten if it already exists. Return boolean to indicate success or failure

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
src | string | Source filepath | Required
dest | string | Destination filepath | Required
overwrite | boolean | Default to true | Optional

### createFolder
Synchronously creates a folder, including any necessary but nonexistent parent folders. Return boolean to indicate success or failure

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
path | string | Folder's path | Required

### deleteFolder
Synchronously deletes a folder, fails when folder is not empty. Return boolean to indicate success or failure

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
path | string | Folder's path | Required

### renameFile
Synchronously rename file at oldPath to the pathname provided as newPath. In the case that newPath already exists, it will be overwritten. Return boolean to indicate success or failure

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
oldPath | string | Current file's path | Required
newPath | string | new file's path | Required

### writeTXTFileSync
Synchronously writes text to the given file

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
path | string | Path to the file | Required
text | string | Text to be added | Required
encoding | string | encoding text (defaults to utf8)

The supportd encoding is mapping to the list provided by nodejs (https://nodejs.org/api/buffer.html#buffers-and-character-encodings) 


### readTXTFileSync
Reads and returns the text of the given file.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
path | string | Path to the file | Required
encoding | string | encoding text (defaults to utf8)

The supportd encoding is mapping to the list provided by nodejs (https://nodejs.org/api/buffer.html#buffers-and-character-encodings) 

### getFileStats
Return a 'stats' object containing related file's information's. Please use forward slashes (/) instead of backward slashes in the path

**Stats Object**

isBlockDevice: Returns true if the Stats object describes a block device.

isCharacterDevice: Returns true if the Stats object describes a character device.

isDirectory: Returns true if the Stats object describes a file system directory.

isFIFO: Returns true if the Stats object describes a first-in-first-out (FIFO) pipe.

isFile: Returns true if the Stats object describes a regular file.

isSocket: Returns true if the Stats object describes a socket.

isSymbolicLink: Returns true if the Stats object describes a symbolic link. This method is only valid when using lstat().

dev: The numeric identifier of the device containing the file.

ino: The file system specific "Inode" number for the file.

mode: A bit-field describing the file type and mode.

nlink: The number of hard-links that exist for the file.

uid: The numeric user identifier of the user that owns the file (POSIX).

gid: The numeric group identifier of the group that owns the file (POSIX).

rdev: A numeric device identifier if the file is considered "special".

size: The size of the file in bytes.

blksize: The file system block size for i/o operations.

blocks: The number of blocks allocated for this file.

atimeMs: The timestamp indicating the last time this file was accessed expressed in milliseconds since the POSIX Epoch.

mtimeMs: The timestamp indicating the last time this file was modified expressed in milliseconds since the POSIX Epoch.

ctimeMs: The timestamp indicating the last time the file status was changed expressed in milliseconds since the POSIX Epoch.

birthtimeMs: The timestamp indicating the creation time of this file expressed in milliseconds since the POSIX Epoch.

atimeNs: Only present when bigint: true is passed into the method that generates the object. The timestamp indicating the last time this file was accessed expressed in nanoseconds since the POSIX Epoch.

mtimeNs: Only present when bigint: true is passed into the method that generates the object. The timestamp indicating the last time this file was modified expressed in nanoseconds since the POSIX Epoch.

ctimeNs: Only present when bigint: true is passed into the method that generates the object. The timestamp indicating the last time the file status was changed expressed in nanoseconds since the POSIX Epoch.

birthtimeNs: Only present when bigint: true is passed into the method that generates the object. The timestamp indicating the creation time of this file expressed in nanoseconds since the POSIX Epoch.

atime: The timestamp indicating the last time this file was accessed.

mtime: The timestamp indicating the last time this file was modified.

ctime: The timestamp indicating the last time the file status was changed.

birthtime: The timestamp indicating the creation time of this file.