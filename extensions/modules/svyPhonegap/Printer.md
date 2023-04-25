Required Phonegap plugins
------------------
cordova-plugin-printer

# API Documentation 

## Method Summary
### print
Print content. Shows a dialog to print content from local or network printer via the Android Print or Apple AirPrint Interfaces.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
String | content | content | Required
Object | options | options | Optional
Function | callback | on success callback | Optional

### printPDF
Print a base64 encoded PDF file. Shows a dialog to print content from local or network printer via the Android Print or Apple AirPrint Interfaces.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
String | content | Base64 encoded PDF string | Required
Function | callback | on success callback | Optional



# Example Usage
```javascript
//Printing some text
content = '<h1>Lorem Ipsum</h1> <h4>"Neque porro quisquam est qui dolorem';
content += 'ipsum quia dolor sit amet, consectetur, adipisci velit..."</h4>'; 
content += 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque id sagittis orci.';
plugins.svyphonegapPrinter.print(content)
```

For more examples of usage check out the svyMobile project.