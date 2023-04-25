#  JSProgressMonitor

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../../JSLib/Boolean.md) | [cancel()](JSProgressMonitor.md#cancel)                   | Cancels the transfer process..                                    |
| [Number](../../JSLib/Number.md) | [getCurrentBytesToTransfer()](JSProgressMonitor.md#getcurrentbytestotransfer)                   | Returns the number of bytes to transfer for the current file..                                    |
| [Number](../../JSLib/Number.md) | [getCurrentFileIndex()](JSProgressMonitor.md#getcurrentfileindex)                   | Returns the index of the current file being transferred..                                    |
| [Number](../../JSLib/Number.md) | [getCurrentTransferredBytes()](JSProgressMonitor.md#getcurrenttransferredbytes)                   | Returns the number of bytes already transferred for the current file..                                    |
| [String](../../JSLib/String.md) | [getCurrentTransferredFileName()](JSProgressMonitor.md#getcurrenttransferredfilename)                   | Returns the name of the current file being transferred..                                    |
| [Number](../../JSLib/Number.md) | [getTotalBytesToTransfer()](JSProgressMonitor.md#gettotalbytestotransfer)                   | Returns the total bytes to transfer to or from the server (sum of all the files size).                                    |
| [Number](../../JSLib/Number.md) | [getTotalFilesToTransfer()](JSProgressMonitor.md#gettotalfilestotransfer)                   | Returns the total number of files to transfer..                                    |
| [Number](../../JSLib/Number.md) | [getTotalTransferredBytes()](JSProgressMonitor.md#gettotaltransferredbytes)                   | Returns the total bytes already transferred (for all files).                                    |
| [Boolean](../../JSLib/Boolean.md) | [isCanceled()](JSProgressMonitor.md#iscanceled)                   | Returns true if the process was canceled..                                    |
| [Boolean](../../JSLib/Boolean.md) | [isFinished()](JSProgressMonitor.md#isfinished)                   | Returns true if the process is finished..                                    |
| [JSProgressMonitor](./JSProgressMonitor.md) | [setProgressCallBack(function, interval)](JSProgressMonitor.md#setprogresscallback-function-interval)                   | Sets a method to be called repeatedly at the given interval (in seconds), the method will receive an instance of this JSProgressMonitor updated with the latest values..                                    |
| [JSProgressMonitor](./JSProgressMonitor.md) | [setProgressCallBack(function, interval, delay)](JSProgressMonitor.md#setprogresscallback-function-interval-delay)                   | Sets a method to be called repeatedly at the given interval (in seconds), the method will receive an instance of this JSProgressMonitor updated with the latest values..                                    |

## Methods Details

### cancel()

Cancels the transfer process.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
monitor.cancel();
```
### getCurrentBytesToTransfer()

Returns the number of bytes to transfer for the current file.


**Returns**\
[Number](../../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.output('total transferred: ' + monitor.getTotalTransferredBytes() + ' / ' + monitor.getTotalBytesToTransfer());
application.output('current file: ' + monitor.getCurrentTransferredFileName() + ' ( ' + monitor.getCurrentFileIndex() + ' / ' + monitor.getTotalFilesToTransfer() + ' )');
application.output('current bytes transferred: '+monitor.getCurrentTransferredBytes() + ' / ' + monitor.getCurrentBytesToTransfer());
if (monitor.isCanceled()) {
	application.output('canceled!')
}
if (monitor.isFinished()) {
	application.output('finished!')
}
```
### getCurrentFileIndex()

Returns the index of the current file being transferred.


**Returns**\
[Number](../../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.output('total transferred: ' + monitor.getTotalTransferredBytes() + ' / ' + monitor.getTotalBytesToTransfer());
application.output('current file: ' + monitor.getCurrentTransferredFileName() + ' ( ' + monitor.getCurrentFileIndex() + ' / ' + monitor.getTotalFilesToTransfer() + ' )');
application.output('current bytes transferred: '+monitor.getCurrentTransferredBytes() + ' / ' + monitor.getCurrentBytesToTransfer());
if (monitor.isCanceled()) {
	application.output('canceled!')
}
if (monitor.isFinished()) {
	application.output('finished!')
}
```
### getCurrentTransferredBytes()

Returns the number of bytes already transferred for the current file.


**Returns**\
[Number](../../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.output('total transferred: ' + monitor.getTotalTransferredBytes() + ' / ' + monitor.getTotalBytesToTransfer());
application.output('current file: ' + monitor.getCurrentTransferredFileName() + ' ( ' + monitor.getCurrentFileIndex() + ' / ' + monitor.getTotalFilesToTransfer() + ' )');
application.output('current bytes transferred: '+monitor.getCurrentTransferredBytes() + ' / ' + monitor.getCurrentBytesToTransfer());
if (monitor.isCanceled()) {
	application.output('canceled!')
}
if (monitor.isFinished()) {
	application.output('finished!')
}
```
### getCurrentTransferredFileName()

Returns the name of the current file being transferred.


**Returns**\
[String](../../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.output('total transferred: ' + monitor.getTotalTransferredBytes() + ' / ' + monitor.getTotalBytesToTransfer());
application.output('current file: ' + monitor.getCurrentTransferredFileName() + ' ( ' + monitor.getCurrentFileIndex() + ' / ' + monitor.getTotalFilesToTransfer() + ' )');
application.output('current bytes transferred: '+monitor.getCurrentTransferredBytes() + ' / ' + monitor.getCurrentBytesToTransfer());
if (monitor.isCanceled()) {
	application.output('canceled!')
}
if (monitor.isFinished()) {
	application.output('finished!')
}
```
### getTotalBytesToTransfer()

Returns the total bytes to transfer to or from the server (sum of all the files size)


**Returns**\
[Number](../../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.output('total transferred: ' + monitor.getTotalTransferredBytes() + ' / ' + monitor.getTotalBytesToTransfer());
application.output('current file: ' + monitor.getCurrentTransferredFileName() + ' ( ' + monitor.getCurrentFileIndex() + ' / ' + monitor.getTotalFilesToTransfer() + ' )');
application.output('current bytes transferred: '+monitor.getCurrentTransferredBytes() + ' / ' + monitor.getCurrentBytesToTransfer());
if (monitor.isCanceled()) {
	application.output('canceled!')
}
if (monitor.isFinished()) {
	application.output('finished!')
}
```
### getTotalFilesToTransfer()

Returns the total number of files to transfer.


**Returns**\
[Number](../../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.output('total transferred: ' + monitor.getTotalTransferredBytes() + ' / ' + monitor.getTotalBytesToTransfer());
application.output('current file: ' + monitor.getCurrentTransferredFileName() + ' ( ' + monitor.getCurrentFileIndex() + ' / ' + monitor.getTotalFilesToTransfer() + ' )');
application.output('current bytes transferred: '+monitor.getCurrentTransferredBytes() + ' / ' + monitor.getCurrentBytesToTransfer());
if (monitor.isCanceled()) {
	application.output('canceled!')
}
if (monitor.isFinished()) {
	application.output('finished!')
}
```
### getTotalTransferredBytes()

Returns the total bytes already transferred (for all files)


**Returns**\
[Number](../../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.output('total transferred: ' + monitor.getTotalTransferredBytes() + ' / ' + monitor.getTotalBytesToTransfer());
application.output('current file: ' + monitor.getCurrentTransferredFileName() + ' ( ' + monitor.getCurrentFileIndex() + ' / ' + monitor.getTotalFilesToTransfer() + ' )');
application.output('current bytes transferred: '+monitor.getCurrentTransferredBytes() + ' / ' + monitor.getCurrentBytesToTransfer());
if (monitor.isCanceled()) {
	application.output('canceled!')
}
if (monitor.isFinished()) {
	application.output('finished!')
}
```
### isCanceled()

Returns true if the process was canceled.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.output('total transferred: ' + monitor.getTotalTransferredBytes() + ' / ' + monitor.getTotalBytesToTransfer());
application.output('current file: ' + monitor.getCurrentTransferredFileName() + ' ( ' + monitor.getCurrentFileIndex() + ' / ' + monitor.getTotalFilesToTransfer() + ' )');
application.output('current bytes transferred: '+monitor.getCurrentTransferredBytes() + ' / ' + monitor.getCurrentBytesToTransfer());
if (monitor.isCanceled()) {
	application.output('canceled!')
}
if (monitor.isFinished()) {
	application.output('finished!')
}
```
### isFinished()

Returns true if the process is finished.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.output('total transferred: ' + monitor.getTotalTransferredBytes() + ' / ' + monitor.getTotalBytesToTransfer());
application.output('current file: ' + monitor.getCurrentTransferredFileName() + ' ( ' + monitor.getCurrentFileIndex() + ' / ' + monitor.getTotalFilesToTransfer() + ' )');
application.output('current bytes transferred: '+monitor.getCurrentTransferredBytes() + ' / ' + monitor.getCurrentBytesToTransfer());
if (monitor.isCanceled()) {
	application.output('canceled!')
}
if (monitor.isFinished()) {
	application.output('finished!')
}
```
### setProgressCallBack(function, interval)

Sets a method to be called repeatedly at the given interval (in seconds), the method will receive an instance of this JSProgressMonitor updated with the latest values. Can use an optional delay (for testing purpose in developer).

**Parameters**\
[Function](../../JSLib/Function.md) function the Function to call back at the specified interval\
[Number](../../JSLib/Number.md) interval the interval (in seconds) to use

**Returns**\
[JSProgressMonitor](./JSProgressMonitor.md) this for chaining

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// call the progressCallbackFuntion every 2 and a half seconds (with a delay of 200ms in developer):
monitor.setProgressCallBack(progressCallbackFunction, 2.5, (application.isInDeveloper() ? 200 : 0));
```
### setProgressCallBack(function, interval, delay)

Sets a method to be called repeatedly at the given interval (in seconds), the method will receive an instance of this JSProgressMonitor updated with the latest values. Can use an optional delay (for testing purpose in developer).

**Parameters**\
[Function](../../JSLib/Function.md) function the Function to call back at the specified interval\
[Number](../../JSLib/Number.md) interval the interval (in seconds) to use\
[Number](../../JSLib/Number.md) delay adds a delay for testing purpose in Developer

**Returns**\
[JSProgressMonitor](./JSProgressMonitor.md) this for chaining

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// call the progressCallbackFuntion every 2 and a half seconds (with a delay of 200ms in developer):
monitor.setProgressCallBack(progressCallbackFunction, 2.5, (application.isInDeveloper() ? 200 : 0));
```

