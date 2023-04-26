Required Phonegap plugins
------------------
phonegap-plugin-barcodescanner

# API Documentation 

## Method Summary
### scan
Scan a barcode using phone camera

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
Function | callbackSuccess | on success callback | Optional
Function | callbackError | on error callback | Optional


# Example Usage
```javascript
plugins.svyphonegapBarcode.scan(scanSuccess,scanFail)

function scanSuccess(result){
	application.output(
	"We got a barcode\n" +
    "Result: " + result.text + "\n" +
    "Format: " + result.format + "\n" +
    "Cancelled: " + result.cancelled)
}

function scanFail(err){
	application.output('error : ' + err)
}
```
