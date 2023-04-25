# MultiFile Upload

Added in version v2.0.0

The MultiFile Upload component is a slick and powerful file uploader. It allows users to drag and drop (or select) a number of files and review them before upload. The component supports several languages, meta fields that allow users to enter additional information for each file, file restrictions and an extensive API and events to interact with the component.

![MultiFile Upload demo](https://github.com/transloadit/uppy/blob/master/assets/uppy-demo.gif)

## Table of contents

* [Getting started](MultiFile-Upload.md#getting-started)
* [MultiFile Upload properties](MultiFile-Upload.md#multifile-upload-properties)
* [Custom types](MultiFile-Upload.md#custom-types)
  * [uploadRestriction type](MultiFile-Upload.md#uploadrestriction-type)
  * [metaField type](MultiFile-Upload.md#metafield-type)
  * [uploadFile type](MultiFile-Upload.md#uploadfile-type)
  * [progress type](MultiFile-Upload.md#progress-type)
* [MultiFile Upload events](MultiFile-Upload.md#multifile-upload-events)
* [MultiFile Upload API](MultiFile-Upload.md#multifile-upload-api)
* [MultiFile Localization](MultiFile-Upload.md#multifile-localization)

## Getting started

To get started with the MultiFile Upload component, drag the component on a form and attach a method to the [onFileUploaded](MultiFile-Upload.md#multifile-upload-events) event. Whenever a file is completely uploaded to the server, this method is fired and receives a [JSUpload](https://wiki.servoy.com/display/DOCS/JSUpload) object as argument. From that you can get the bytes of the file uploaded, its name, content type etc.

The component can either be shown as a "drop zone" on the form or as a modal dialog. This is controlled via the [inline property](MultiFile-Upload.md#multifile-upload-properties). When `true`, the component will render a UI on the form, when `false`, nothing will be rendered on the form and the component needs to be opened as a modal via the [openModal()](MultiFile-Upload.md#multifile-upload-api) API call.

## MultiFile Upload properties

The component offers these properties to control its behaviour:

| Property             | Type                                                                | Default | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| -------------------- | ------------------------------------------------------------------- | ------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| inline               | Boolean                                                             | null    | When `false`, the component does not show on the form, but in a modal that is shown when openModal() is called                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| autoProceed          | Boolean                                                             | false   | By default the component will wait for an upload button to be pressed in the UI, or the upload() method to be called, before starting an upload. Setting this to autoProceed: `true` will start uploading automatically after the first file is selected.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| allowMultipleUploads | Boolean                                                             | true    | <p>Whether to allow multiple upload batches. This means multiple calls to .upload(), or a user adding more files after already uploading some. An upload batch is made up of the files that were added since the previous .upload() call.<br><br>With this option set to <code>true</code>, users can upload some files, and then add more files and upload those as well. A model use case for this is uploading images to a gallery or adding attachments to an email.<br><br>With this option set to <code>false</code>, users can upload some files, and you can listen for the <code>onUploadComplete</code> event to continue to the next step in your app’s upload flow. A typical use case for this is uploading a new profile picture.</p> |
| restrictions         | [uploadRestriction\[\]](MultiFile-Upload.md#uploadrestriction-type) | null    | Optionally, provide rules and conditions to limit the type and/or number of files that can be selected.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| language             | String                                                              | English | <p>One of the language packs shipped (currently English, Spanish, German, French, Dutch, Italian, Chinese, Czech, Danish, Finnish, Greek, Hungarian, Japanese, Persian, Russian, Swedish, Turkish)<br><br>If you need to provide your own translations, use the localeStrings property.</p>                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| localeStrings        | Map                                                                 |         | Any number of key/value pairs to translate single strings in the component, overriding the ones provided by the language pack selected.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| hideUploadButton     | Boolean                                                             | false   | Hide the upload button. Use this if you are providing a custom upload button somewhere, and using the upload() API.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| note                 | String                                                              | null    | Optionally, specify a string of text that explains something about the upload for the user. This is a place to explain any restrictions that are put in place. For example: 'Images and video only, 2–3 files, up to 1 MB'.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| metaFields           | [metaField\[\]](MultiFile-Upload.md#meta-field-type)                | null    | <p>An array of UI field objects that will be shown when a user clicks the “edit” button on that file. Configuring this enables the “edit” button on file cards. Each object requires:<br><br></p><ul><li>id, the name of the meta field. Note: this will also be used in CSS/HTML as part of the id attribute, so it’s better to avoid using characters like periods, semicolons, etc.</li><li>name, the label shown in the interface.</li><li>placeholder, the text shown when no value is set in the field.</li></ul><p><br><br>Note: these fields are currently not available in the onFileUploaded handler and can only be retrieved in the onUploadComplete handler or when the files are fetched via getFiles() or getFile()</p>              |
| closeAfterFinish     | Boolean                                                             | false   | <p>Set to true to automatically close the modal when all current uploads are complete. You can use this together with the allowMultipleUploads: false option to create a smooth experience when uploading a single (batch of) file(s).<br><br>With this option, the modal is only automatically closed when uploads are complete and successful. If some uploads failed, the modal stays open so the user can retry failed uploads or cancel the current batch and upload an entirely different set of files instead.<br><br>Setting allowMultipleUploads: false is strongly recommended when using this option. With multiple upload batches, the auto-closing behavior can be very confusing for users.</p>                                       |
| disableStatusBar     | Boolean                                                             | false   | Dashboard ships with the StatusBar plugin that shows upload progress and pause/resume/cancel buttons. If you want, you can disable the StatusBar to provide your own custom solution.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| sources              | Map                                                                 | null    | Allows to add additional sources of files (other than the user's file system) to the component (currently only Webcam is supported)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |

## Custom types

### uploadRestriction type

Optionally, provide rules and conditions to limit the type and/or number of files that can be selected. It is used on the restrictions property of the component and has the following properties:

| Property         | Type   | Default | Description                                                                                                                       |
| ---------------- | ------ | ------- | --------------------------------------------------------------------------------------------------------------------------------- |
| maxFileSize      | Number | null    | maximum file size in bytes for each individual file                                                                               |
| maxNumberOfFiles | Number | null    | total number of files that can be selected                                                                                        |
| minNumberOfFiles | Number | null    | minimum number of files that must be selected before the upload                                                                   |
| allowedFileTypes | String | null    | array of wildcards image/\*, exact mime types image/jpeg, or file extensions .jpg: \['image/\*', '.jpg', '.jpeg', '.png', '.gif'] |

maxNumberOfFiles also affects the number of files a user is able to select via the system file dialog in UI plugins like DragDrop, FileInput and Dashboard: when set to 1, they will only be able to select a single file. When null or another number is provided, they will be able to select multiple files.

### metaField type

Meta fields can be added to the component and will be shown when a user clicks the “edit” button on a specific file. Adding meta fields enables the “edit” button on file cards.

| Property    | Type   | Default | Description                                                                                                                                                               |
| ----------- | ------ | ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id          | String | null    | the name of the meta field. Note: this will also be used in CSS/HTML as part of the id attribute, so it’s better to avoid using characters like periods, semicolons, etc. |
| name        | String | null    | the label shown in the interface.                                                                                                                                         |
| placeholder | String | null    | the text shown when no value is set in the field.                                                                                                                         |

### uploadFile type

uploadFiles can be retrieved via the getFiles() or getFile(fileID) API calls or will be passed as parameter to some of the handlers of the component.

An uploadFile file has the following properties:

| Property   | Type                                          | Description                                     |
| ---------- | --------------------------------------------- | ----------------------------------------------- |
| id         | String                                        | the ID of the file used in the component.       |
| name       | String                                        | the file's name.                                |
| extension  | String                                        | the file extension (e.g. '.jpg')                |
| type       | String                                        | the file's mime type (e.g. 'image/jpeg').       |
| size       | Integer                                       | the file size in bytes.                         |
| metaFields | Object                                        | a key/value map of all meta fields of the file. |
| progress   | [progress](MultiFile-Upload.md#progress-type) | the file's progress as a progress object.       |
| error      | String                                        | possible error message.                         |

### progress type

An object detailing a file's transfer progress with the following properties:

| Property       | Type    | Description                                      |
| -------------- | ------- | ------------------------------------------------ |
| bytesTotal     | Integer | the total number of bytes to be uploaded.        |
| bytesUploaded  | Integer | the number of bytes uploaded.                    |
| percentage     | Integer | the percentage uploaded                          |
| uploadComplete | Boolean | whether the file has been successfully uploaded. |
| uploadStarted  | Date    | the date on which the upload has been started    |

## MultiFile Upload events

| Event               | Params                                                                                                                                                               | Return  | Description                                                                                                                                                                                                                     |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| onFileUploaded      | fileUploaded:JSUpload                                                                                                                                                |         | Fired when a file is uploaded and receives the file uploaded as a JSUpload object                                                                                                                                               |
| onFileAdded         | fileAdded:[uploadFile](MultiFile-Upload.md#uploadfile-type)                                                                                                          |         | Fired when a file has been added to the list of files                                                                                                                                                                           |
| onBeforeFileAdded   | <p>fileToAdd:<a href="MultiFile-Upload.md#uploadfile-type">uploadFile</a>,<br>files:<a href="MultiFile-Upload.md#uploadfile-type">uploadFile[]</a></p>               | Boolean | Fired when a file is added to the list of files to upload. When `false` is returned, the file will not be added                                                                                                                 |
| onFileRemoved       | fileRemoved:[uploadFile](MultiFile-Upload.md#uploadfile-type)                                                                                                        |         | Fired when a file is removed from the list of files to upload                                                                                                                                                                   |
| onUploadComplete    | <p>successfulFiles:<a href="MultiFile-Upload.md#uploadfile-type">uploadFile[]</a>,<br>failedFiles:<a href="MultiFile-Upload.md#uploadfile-type">uploadFile[]</a></p> |         | Fired when the upload of all files is complete                                                                                                                                                                                  |
| onModalOpened       |                                                                                                                                                                      |         | Fired when the modal is opened                                                                                                                                                                                                  |
| onModalClosed       |                                                                                                                                                                      |         | Fired when the modal is closed                                                                                                                                                                                                  |
| onRestrictionFailed | <p>file:<a href="MultiFile-Upload.md#uploadfile-type">uploadFile</a>,<br>error:String</p>                                                                            |         | Fired when a file violates certain [restrictions](MultiFile-Upload.md#uploadRestriction-type) when added. This event is just providing another choice for those who want to customize the behavior of file upload restrictions. |

## MultiFile Upload API

| Method      | Params                                                                                    | Return                                                | Description                                                                                                                                    |
| ----------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| reset       |                                                                                           |                                                       | Stop all uploads in progress and clear file selection, set progress to 0. Basically, return things to the way they were before any user input. |
| initialize  |                                                                                           |                                                       | Re-initializes the component.                                                                                                                  |
| openModal   |                                                                                           |                                                       | Shows the modal window (only if `inline` property is set to false).                                                                            |
| closeModal  |                                                                                           |                                                       | Hides the modal window.                                                                                                                        |
| upload      |                                                                                           |                                                       | Start uploading selected files.                                                                                                                |
| retryAll    |                                                                                           |                                                       | Retry all uploads (after an error, for example).                                                                                               |
| cancelAll   | fileID:String                                                                             |                                                       | Cancel all uploads, reset progress and remove all files.                                                                                       |
| retryUpload | fileID:String                                                                             |                                                       | Retry an upload (after an error, for example).                                                                                                 |
| info        | <p>message:String|{message:String,details:String},<br>type:String<br>duration:Integer</p> |                                                       | Sets a message in state, with optional details. The types supported are info, warning, success or error.                                       |
| getFiles    |                                                                                           | [uploadFile\[\]](MultiFile-Upload.md#uploadfile-type) | Get an array of all file objects in the component.                                                                                             |
| getFile     | fileID:String                                                                             | [uploadFile](MultiFile-Upload.md#uploadfile-type)     | Get a specific file object by its ID.                                                                                                          |
| removeFile  | fileID:String                                                                             |                                                       | Remove a file from the component.                                                                                                              |

## MultiFile Localization

To localize the component, use the `language` property to choose among any of the shipped languages. If you want to translate single strings differently or provide a full own translation, you can use the localeStrings property to provide those translations.

Below you find all keys and their English translation for reference. Please note that some keys are nested in a complex object, such as

`filesUploadedOfTotal: {`\
`'0': '%{complete} of %{smart_count} file uploaded',`\
`'1': '%{complete} of %{smart_count} files uploaded',`\
`'2': '%{complete} of %{smart_count} files uploaded'`\
`}`

For this to work properly, you have to provide the property of the nested object directly with the key, separated with a dot as in

`filesUploadedOfTotal.0 = '%{complete} of %{smart_count} file uploaded'`\
`filesUploadedOfTotal.1 = '%{complete} of %{smart_count} files uploaded'`\
`filesUploadedOfTotal.2 = '%{complete} of %{smart_count} files uploaded'`

### Localization keys

Here is a list of all keys and their English translation defaults:

| Key                             | English (default) translation                                                                           |
| ------------------------------- | ------------------------------------------------------------------------------------------------------- |
| addMore                         | 'Add more'                                                                                              |
| addMoreFiles                    | 'Add more files'                                                                                        |
| addingMoreFiles                 | 'Adding more files'                                                                                     |
| allowAccessDescription          | 'In order to take pictures or record video with your camera, please allow camera access for this site.' |
| allowAccessTitle                | 'Please allow access to your camera'                                                                    |
| authenticateWith                | 'Connect to %{pluginName}'                                                                              |
| authenticateWithTitle           | 'Please authenticate with %{pluginName} to select files'                                                |
| back                            | 'Back'                                                                                                  |
| browse                          | 'browse'                                                                                                |
| cancel                          | 'Cancel'                                                                                                |
| cancelUpload                    | 'Cancel upload'                                                                                         |
| chooseFiles                     | 'Choose files'                                                                                          |
| closeModal                      | 'Close Modal'                                                                                           |
| companionAuthError              | 'Authorization required'                                                                                |
| companionError                  | 'Connection with Companion failed'                                                                      |
| companionUnauthorizeHint        | 'To unauthorize to your %{provider} account, please go to %{url}'                                       |
| complete                        | 'Complete'                                                                                              |
| connectedToInternet             | 'Connected to the Internet'                                                                             |
| copyLink                        | 'Copy link'                                                                                             |
| copyLinkToClipboardFallback     | 'Copy the URL below'                                                                                    |
| copyLinkToClipboardSuccess      | 'Link copied to clipboard'                                                                              |
| creatingAssembly                | 'Preparing upload...'                                                                                   |
| creatingAssemblyFailed          | 'Transloadit                                                                                            |
| dashboardTitle                  | 'File Uploader'                                                                                         |
| dashboardWindowTitle            | 'File Uploader Window (Press escape to close)'                                                          |
| dataUploadedOfTotal             | '%{complete} of %{total}'                                                                               |
| done                            | 'Done'                                                                                                  |
| dropHereOr                      | 'Drop files here or %{browse}'                                                                          |
| dropHint                        | 'Drop your files here'                                                                                  |
| dropPaste                       | 'Drop files here, paste or %{browse}'                                                                   |
| dropPasteImport                 | 'Drop files here, paste, %{browse} or import from'                                                      |
| edit                            | 'Edit'                                                                                                  |
| editFile                        | 'Edit file'                                                                                             |
| editing                         | 'Editing %{file}'                                                                                       |
| emptyFolderAdded                | 'No files were added from empty folder'                                                                 |
| encoding                        | 'Encoding...'                                                                                           |
| enterCorrectUrl                 | 'Incorrect URL                                                                                          |
| enterUrlToImport                | 'Enter URL to import a file'                                                                            |
| exceedsSize                     | 'This file exceeds maximum allowed size of'                                                             |
| failedToFetch                   | 'Companion failed to fetch this URL, please make sure it’s correct'                                     |
| failedToUpload                  | 'Failed to upload %{file}'                                                                              |
| fileSource                      | 'File source                                                                                            |
| filesUploadedOfTotal.0          | '%{complete} of %{smart\_count} file uploaded'                                                          |
| filesUploadedOfTotal.1          | '%{complete} of %{smart\_count} files uploaded'                                                         |
| filesUploadedOfTotal.2          | '%{complete} of %{smart\_count} files uploaded'                                                         |
| filter                          | 'Filter'                                                                                                |
| finishEditingFile               | 'Finish editing file'                                                                                   |
| folderAdded.0                   | 'Added %{smart\_count} file from %{folder}'                                                             |
| folderAdded.1                   | 'Added %{smart\_count} files from %{folder}'                                                            |
| folderAdded.2                   | 'Added %{smart\_count} files from %{folder}'                                                            |
| generatingThumbnails            | 'Generating thumbnails...'                                                                              |
| import                          | 'Import'                                                                                                |
| importFrom                      | 'Import from %{name}'                                                                                   |
| link                            | 'Link'                                                                                                  |
| loading                         | 'Loading...'                                                                                            |
| logOut                          | 'Log out'                                                                                               |
| myDevice                        | 'My Device'                                                                                             |
| noFilesFound                    | 'You have no files or folders here'                                                                     |
| noInternetConnection            | 'No Internet connection'                                                                                |
| openFolderNamed                 | 'Open folder %{name}'                                                                                   |
| pause                           | 'Pause'                                                                                                 |
| pauseUpload                     | 'Pause upload'                                                                                          |
| paused                          | 'Paused'                                                                                                |
| poweredBy                       | 'Powered by'                                                                                            |
| preparingUpload                 | 'Preparing upload...'                                                                                   |
| processingXFiles.0              | 'Processing %{smart\_count} file'                                                                       |
| processingXFiles.1              | 'Processing %{smart\_count} files'                                                                      |
| processingXFiles.2              | 'Processing %{smart\_count} files'                                                                      |
| removeFile                      | 'Remove file'                                                                                           |
| resetFilter                     | 'Reset filter'                                                                                          |
| resume                          | 'Resume'                                                                                                |
| resumeUpload                    | 'Resume upload'                                                                                         |
| retry                           | 'Retry'                                                                                                 |
| retryUpload                     | 'Retry upload'                                                                                          |
| saveChanges                     | 'Save changes'                                                                                          |
| selectAllFilesFromFolderNamed   | 'Select all files from folder %{name}'                                                                  |
| selectFileNamed                 | 'Select file %{name}'                                                                                   |
| selectX.0                       | 'Select %{smart\_count}'                                                                                |
| selectX.1                       | 'Select %{smart\_count}'                                                                                |
| selectX.2                       | 'Select %{smart\_count}'                                                                                |
| smile                           | 'Smile!'                                                                                                |
| startRecording                  | 'Begin video recording'                                                                                 |
| stopRecording                   | 'Stop video recording'                                                                                  |
| takePicture                     | 'Take a picture'                                                                                        |
| timedOut                        | 'Upload stalled for %{seconds} seconds, aborting.'                                                      |
| unselectAllFilesFromFolderNamed | 'Unselect all files from folder %{name}'                                                                |
| unselectFileNamed               | 'Unselect file %{name}'                                                                                 |
| upload                          | 'Upload'                                                                                                |
| uploadComplete                  | 'Upload complete'                                                                                       |
| uploadFailed                    | 'Upload failed'                                                                                         |
| uploadPaused                    | 'Upload paused'                                                                                         |
| uploadXFiles.0                  | 'Upload %{smart\_count} file'                                                                           |
| uploadXFiles.1                  | 'Upload %{smart\_count} files'                                                                          |
| uploadXFiles.2                  | 'Upload %{smart\_count} files'                                                                          |
| uploadXNewFiles.0               | 'Upload +%{smart\_count} file'                                                                          |
| uploadXNewFiles.1               | 'Upload +%{smart\_count} files'                                                                         |
| uploadXNewFiles.2               | 'Upload +%{smart\_count} files'                                                                         |
| uploading                       | 'Uploading'                                                                                             |
| uploadingXFiles.0               | 'Uploading %{smart\_count} file'                                                                        |
| uploadingXFiles.1               | 'Uploading %{smart\_count} files'                                                                       |
| uploadingXFiles.2               | 'Uploading %{smart\_count} files'                                                                       |
| xFilesSelected.0                | '%{smart\_count} file selected'                                                                         |
| xFilesSelected.1                | '%{smart\_count} files selected'                                                                        |
| xFilesSelected.2                | '%{smart\_count} files selected'                                                                        |
| xMoreFilesAdded.0               | '%{smart\_count} more file added'                                                                       |
| xMoreFilesAdded.1               | '%{smart\_count} more files added'                                                                      |
| xMoreFilesAdded.2               | '%{smart\_count} more files added'                                                                      |
| xTimeLeft                       | '%{time} left'                                                                                          |
| youCanOnlyUploadFileTypes       | 'You can only upload                                                                                    |
| youCanOnlyUploadX.0             | 'You can only upload %{smart\_count} file'                                                              |
| youCanOnlyUploadX.1             | 'You can only upload %{smart\_count} files'                                                             |
| youCanOnlyUploadX.2             | 'You can only upload %{smart\_count} files'                                                             |
| youHaveToAtLeastSelectX.0       | 'You have to select at least %{smart\_count} file'                                                      |
| youHaveToAtLeastSelectX.1       | 'You have to select at least %{smart\_count} files'                                                     |
| youHaveToAtLeastSelectX.2       | 'You have to select at least %{smart\_count} files'                                                     |
