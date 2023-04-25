Welcome to **svyPDFViewer**! 

This wiki provides comprehensive documentation for using the **svyPDFViewer** web-component, which makes viewing PDF documents in Servoy's NGClient easy and intuitive.

# Getting Started

It's easy to get started. Simply import the [web package](https://github.com/Servoy/svyPDFViewer/releases/download/v1.1.0/pdfviewer.zip) via Servoy's Web Package Manager.

If you like to see a sample, install the example solution, [**svyPDFViewerExample.servoy**] (https://github.com/Servoy/svyPDFViewer/releases/download/v1.1.0/svyPDFViewerExample.servoy)

## Example Usage

Load document using **absolute** URL
```
elements.pdfViewer.documentURL = 'http://www.cbu.edu.zm/downloads/pdf-sample.pdf';
```


Load document using URL which is **relative** to the web application's root context. For example:
- http://my-host:8080/myApplication/reports/test.pdf - this would be in production server)
- http://localhost:8080/reports/test.pdf - this would be in developer
```
elements.pdfViewer.documentURL = 'reports/test.pdf'; 
```

# API Documentation

## Property Summary
Type | Name| Description
----------- | ------ | -----------
String|[**documentURL**](#documenturl)|The URL of the PDF document
String|[**noCache**](#nocache)|Indicates if caching should be disabled

## Method Summary
Return Type | Method | Description
----------- | ------ | -----------
void|[**reload**](#reload)|ReLoads the document in the viewer.
void|[**~~loadDocument~~**](#loaddocument)|(Re)Loads the document in the viewer. Deprecated. Use [documentURL](#documenturl) instead


## Method Details

### reload
---
Reloads the document. Use in combination with [noCache](#nocache). Call this method when document has changed on the server. 

### ~~loadDocument~~
---
Deprecated. Use [documentURL](#documenturl) instead
	
## Property Details

### documentURL
---
**Type** String
The URL of the PDF document. Can be absolute or relative.

### noCache
---
**Type** Boolean
Indicates if caching should be disabled. Set to true when PDF might change on the server.