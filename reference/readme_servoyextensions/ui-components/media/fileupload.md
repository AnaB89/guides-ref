# File upload

Single file upload component. File content will be saved in the dataprovider.

## Table of contents

* [Getting uploaded file name and mime type](fileupload.md#getting-uploaded-file-name-and-mime-type)
* [File upload properties](fileupload.md#file-upload-properties)
* [File upload events](fileupload.md#file-upload-events)

## Getting uploaded file name and mime type

To get the name and mime type of the uploaded file, you need to create form variables, on the component's parent form, with the following names, 'dataprovider\_filename' and 'dataprovider\_mimetype', where 'dataprovider' is the dataprovider name of the component. These form variables will be filled with the right values after the file is uploaded. Ex.: you have a fileupload component, with dataprovider : 'picture', after the upload, if the form variables 'picture\_filename' and 'picture\_mimetype' exits, they will have the uploaded file name and mime type.

## File upload properties

The component has the following properties:

| Property               | Type         | Default                                            | Description                                                                                                                                                                          |
| ---------------------- | ------------ | -------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| accept                 | tagstring    | \*/\*                                              | Valid file types (could be comma separated file extensions ".csv, .txt" or valid mime types "text/\*" or "text/css"). Drop zone validation styles work just with explicit filetypes. |
| dataProviderID         | dataprovider | null                                               | Dataprovider where file is saved                                                                                                                                                     |
| displayTags            | boolean      | true                                               | The mesages displayed should resolve tags                                                                                                                                            |
| enabled                | enabled      | true                                               | When false upload has disabled appearance and actions do not work                                                                                                                    |
| location               | point        | null                                               | Label location                                                                                                                                                                       |
| size                   | dimension    | null                                               | Label size                                                                                                                                                                           |
| styleClass             | styleclass   | null                                               | Additional style class(es) of the component                                                                                                                                          |
| styleClassExpression   | dataprovider | null                                               | Additional style class(es) of the component provided using a dataprovider                                                                                                            |
| toolTipText            | tagstring    | null                                               | File upload tooltip                                                                                                                                                                  |
| uploadText             | tagstring    | "Drop a file here or click to upload"              | File upload message                                                                                                                                                                  |
| uploadProgressText     | tagstring    | "Uploading click to cancel"                        | File uploading message                                                                                                                                                               |
| uploadSuccessText      | tagstring    | "Successfully uploaded"                            | File uploaded successfully message                                                                                                                                                   |
| uploadCancelText       | tagstring    | "Upload canceled"                                  | File upload cancel message                                                                                                                                                           |
| uploadNotSupportedText | tagstring    | "File Drag/Drop is not supported for this browser" | Drag and drop not supported                                                                                                                                                          |
| resultDisplayTimeout   | int          | 2000                                               | Time in milliseconds while upload result will be displayed. After timeout component will revert to initial display                                                                   |
| visible                | visible      | true                                               | When false component is not visible                                                                                                                                                  |

## File upload events

| Event                | Params                                                               | Return  | Description                      |
| -------------------- | -------------------------------------------------------------------- | ------- | -------------------------------- |
| onDataChangeMethodID | oldValue:dataprovider type, newValue:dataprovider type event:JSEvent | boolean | Fired when textbox value changes |
