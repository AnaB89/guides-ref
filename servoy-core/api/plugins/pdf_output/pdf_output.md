#  pdf_output


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Array](../../JSLib/Array.md) | [combinePDFDocuments(pdf_docs_bytearrays)](pdf_output.md#combinepdfdocuments-pdf_docs_bytearrays)                   | Combine multiple PDF docs into one..                                    |
| [Array](../../JSLib/Array.md) | [combineProtectedPDFDocuments(pdf_docs_bytearrays, pdf_docs_passwords)](pdf_output.md#combineprotectedpdfdocuments-pdf_docs_bytearrays-pdf_docs_passwords)                   | Combine multiple protected PDF docs into one..                                    |
| [Array](../../JSLib/Array.md) | [convertPDFFormToPDFDocument(pdf_form, field_values)](pdf_output.md#convertpdfformtopdfdocument-pdf_form-field_values)                   | Convert a PDF form to a PDF document..                                    |
| [Array](../../JSLib/Array.md) | [convertProtectedPDFFormToPDFDocument(pdf_form, pdf_password, field_values)](pdf_output.md#convertprotectedpdfformtopdfdocument-pdf_form-pdf_password-field_values)                   | Convert a protected PDF form to a PDF document..                                    |
| [Array](../../JSLib/Array.md) | [encrypt(data, ownerPassword)](pdf_output.md#encrypt-data-ownerpassword)                   | Add password protection and security options to the PDF.                                    |
| [Array](../../JSLib/Array.md) | [encrypt(data, ownerPassword, userPassword)](pdf_output.md#encrypt-data-ownerpassword-userpassword)                   | Add password protection and security options to the PDF.                                    |
| [Array](../../JSLib/Array.md) | [encrypt(data, ownerPassword, userPassword, allowAssembly, allowCopy, allowDegradedPrinting, allowFillIn, allowModifyAnnotations, allowModifyContents, allowPrinting, allowScreenreaders)](pdf_output.md#encrypt-data-ownerpassword-userpassword-allowassembly-allowcopy-allowdegradedprinting-allowfillin-allowmodifyannotations-allowmodifycontents-allowprinting-allowscreenreaders)                   | Add password protection and security options to the PDF.                                    |
| [Array](../../JSLib/Array.md) | [encrypt(data, ownerPassword, userPassword, allowAssembly, allowCopy, allowDegradedPrinting, allowFillIn, allowModifyAnnotations, allowModifyContents, allowPrinting, allowScreenreaders, is128bit)](pdf_output.md#encrypt-data-ownerpassword-userpassword-allowassembly-allowcopy-allowdegradedprinting-allowfillin-allowmodifyannotations-allowmodifycontents-allowprinting-allowscreenreaders-is128bit)                   | Add password protection and security options to the PDF.                                    |
| [Array](../../JSLib/Array.md) | [encrypt(data, ownerPassword, userPassword, allowAssembly, allowCopy, allowDegradedPrinting, allowFillIn, allowModifyAnnotations, allowModifyContents, allowPrinting, allowScreenreaders, is128bit, metaData)](pdf_output.md#encrypt-data-ownerpassword-userpassword-allowassembly-allowcopy-allowdegradedprinting-allowfillin-allowmodifyannotations-allowmodifycontents-allowprinting-allowscreenreaders-is128bit-metadata)                   | Add password protection and security options to the PDF.                                    |
| [Number](../../JSLib/Number.md) | [getNumberOfPages(data)](pdf_output.md#getnumberofpages-data)                   | Returns the number of pages for pdf document..                                    |
| [Array](../../JSLib/Array.md) | [getThumbnailImage(data)](pdf_output.md#getthumbnailimage-data)                   | Create a thumbnail from the provided PDF.                                    |
| [Array](../../JSLib/Array.md) | [getThumbnailImage(data, pageNumber)](pdf_output.md#getthumbnailimage-data-pagenumber)                   | Create a thumbnail from the provided PDF.                                    |
| [Array](../../JSLib/Array.md) | [getThumbnailImage(data, pageNumber, dpi)](pdf_output.md#getthumbnailimage-data-pagenumber-dpi)                   | Create a thumbnail from the provided PDF.                                    |
| [Array](../../JSLib/Array.md) | [numberPages(data)](pdf_output.md#numberpages-data)                   | Add pages numbers to a PDF.                                    |
| [Array](../../JSLib/Array.md) | [numberPages(data, fontSize, locationX, locationY, font, hexColor)](pdf_output.md#numberpages-data-fontsize-locationx-locationy-font-hexcolor)                   | Add pages numbers to a PDF.                                    |
| [Array](../../JSLib/Array.md) | [overlay(data, forOverlay)](pdf_output.md#overlay-data-foroverlay)                   | Add some PDF based content over a PDF.                                    |
| [Array](../../JSLib/Array.md) | [overlay(data, forOverlay, isOver)](pdf_output.md#overlay-data-foroverlay-isover)                   | Add some PDF based content over a PDF.                                    |
| [Array](../../JSLib/Array.md) | [overlay(data, forOverlay, isOver, pages)](pdf_output.md#overlay-data-foroverlay-isover-pages)                   | Add some PDF based content over a PDF.                                    |
| [Array](../../JSLib/Array.md) | [overlay(data, forOverlay, pages)](pdf_output.md#overlay-data-foroverlay-pages)                   | Add some PDF based content over a PDF.                                    |
| [Array](../../JSLib/Array.md) | [overlayText(data, text)](pdf_output.md#overlaytext-data-text)                   | Add text over every page at a 45 degree angle.                                    |
| [Array](../../JSLib/Array.md) | [overlayText(data, text, locationX, locationY, isOver, fontSize, font, hexColor)](pdf_output.md#overlaytext-data-text-locationx-locationy-isover-fontsize-font-hexcolor)                   | Add text over every page at a 45 degree angle.                                    |
| [Array](../../JSLib/Array.md) | [overlayText(data, text, locationX, locationY, isOver, fontSize, font, hexColor, angle)](pdf_output.md#overlaytext-data-text-locationx-locationy-isover-fontsize-font-hexcolor-angle)                   | Add text over every page at a 45 degree angle.                                    |
| [Array](../../JSLib/Array.md) | [watermark(data, image)](pdf_output.md#watermark-data-image)                   | Add an image as a watermark on every page, or the pages specified as a parameter.                                    |
| [Array](../../JSLib/Array.md) | [watermark(data, image, locationX, locationY, isOver)](pdf_output.md#watermark-data-image-locationx-locationy-isover)                   | Add an image as a watermark on every page, or the pages specified as a parameter.                                    |
| [Array](../../JSLib/Array.md) | [watermark(data, image, locationX, locationY, isOver, pages)](pdf_output.md#watermark-data-image-locationx-locationy-isover-pages)                   | Add an image as a watermark on every page, or the pages specified as a parameter.                                    |

## Methods Details

### combinePDFDocuments(pdf_docs_bytearrays)

Combine multiple PDF docs into one.
Note: this function may fail when creating large PDF files due to lack of available heap memory. To compensate, please configure the application server with more heap memory via -Xmx parameter.

**Parameters**\
[Array](../../JSLib/Array.md) pdf_docs_bytearrays the array of documents to combine

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
pdf_blob_column = combinePDFDocuments(new Array(pdf_blob1,pdf_blob2,pdf_blob3));
```
### combineProtectedPDFDocuments(pdf_docs_bytearrays, pdf_docs_passwords)

Combine multiple protected PDF docs into one.
Note: this function may fail when creating large PDF files due to lack of available heap memory. To compensate, please configure the application server with more heap memory via -Xmx parameter.

**Parameters**\
[Array](../../JSLib/Array.md) pdf_docs_bytearrays the array of documents to combine\
[Array](../../JSLib/Array.md) pdf_docs_passwords an array of passwords to use

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
pdf_blob_column = combineProtectedPDFDocuments(new Array(pdf_blob1,pdf_blob2,pdf_blob3), new Array(pdf_blob1_pass,pdf_blob2_pass,pdf_blob3_pass));
```
### convertPDFFormToPDFDocument(pdf_form, field_values)

Convert a PDF form to a PDF document.

**Parameters**\
[Array](../../JSLib/Array.md) pdf_form the PDF Form to convert\
[Object](../../JSLib/Object.md) field_values the values to use

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
var pdfform = plugins.file.readFile('c:/temp/1040a-form.pdf');
//var field_values = plugins.file.readFile('c:/temp/1040a-data.fdf');//read adobe fdf values or
var field_values = new Array()//construct field values
field_values[0] = 'f1-1=John C.J.'
field_values[1] = 'f1-2=Longlasting'
var result_pdf_doc = plugins.pdf_output.convertPDFFormToPDFDocument(pdfform, field_values)
if (result_pdf_doc != null)
{
	plugins.file.writeFile('c:/temp/1040a-flatten.pdf', result_pdf_doc)
}
```
### convertProtectedPDFFormToPDFDocument(pdf_form, pdf_password, field_values)

Convert a protected PDF form to a PDF document.

**Parameters**\
[Array](../../JSLib/Array.md) pdf_form the PDF Form to convert\
[String](../../JSLib/String.md) pdf_password the password to use\
[Object](../../JSLib/Object.md) field_values the field values to use

**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
var pdfform = plugins.file.readFile('c:/temp/1040a-form.pdf');
//var field_values = plugins.file.readFile('c:/temp/1040a-data.fdf');//read adobe fdf values or
var field_values = new Array()//construct field values
field_values[0] = 'f1-1=John C.J.'
field_values[1] = 'f1-2=Longlasting'
var result_pdf_doc = plugins.pdf_output.convertProtectedPDFFormToPDFDocument(pdfform, 'pdf_password', field_values)
if (result_pdf_doc != null)
{
	plugins.file.writeFile('c:/temp/1040a-flatten.pdf', result_pdf_doc)
}
```
### encrypt(data, ownerPassword)

Add password protection and security options to the PDF

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[String](../../JSLib/String.md) ownerPassword the owner password

**Returns**\
[Array](../../JSLib/Array.md) the encrypted PDF


**Sample**

```javascript
// Add password protection and security options to the PDF
// NOTE: Passwords are case sensitive
var unEncryptedFile = plugins.file.showFileOpenDialog();
if (unEncryptedFile) {
	var data = plugins.file.readFile(unEncryptedFile);
	encryptedResult = %%elementName%%.encrypt(data, 'secretPassword', 'secretUserPassword', false, false, false, false, false, false, false, false, true);
}
```
### encrypt(data, ownerPassword, userPassword)

Add password protection and security options to the PDF

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[String](../../JSLib/String.md) ownerPassword the owner password\
[String](../../JSLib/String.md) userPassword the user password

**Returns**\
[Array](../../JSLib/Array.md) the encrypted PDF


**Sample**

```javascript
// Add password protection and security options to the PDF
// NOTE: Passwords are case sensitive
var unEncryptedFile = plugins.file.showFileOpenDialog();
if (unEncryptedFile) {
	var data = plugins.file.readFile(unEncryptedFile);
	encryptedResult = %%elementName%%.encrypt(data, 'secretPassword', 'secretUserPassword', false, false, false, false, false, false, false, false, true);
}
```
### encrypt(data, ownerPassword, userPassword, allowAssembly, allowCopy, allowDegradedPrinting, allowFillIn, allowModifyAnnotations, allowModifyContents, allowPrinting, allowScreenreaders)

Add password protection and security options to the PDF

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[String](../../JSLib/String.md) ownerPassword the owner password\
[String](../../JSLib/String.md) userPassword the user password\
[Boolean](../../JSLib/Boolean.md) allowAssembly whether to set the allow assembly permission\
[Boolean](../../JSLib/Boolean.md) allowCopy whether to set the allow copy permission\
[Boolean](../../JSLib/Boolean.md) allowDegradedPrinting whether to set the allow degraded printing permission\
[Boolean](../../JSLib/Boolean.md) allowFillIn whether to set the allow fill in permission\
[Boolean](../../JSLib/Boolean.md) allowModifyAnnotations whether to set the allow modify annotations permission\
[Boolean](../../JSLib/Boolean.md) allowModifyContents whether to set the allow modify contents permission\
[Boolean](../../JSLib/Boolean.md) allowPrinting whether to set the allow printing permission\
[Boolean](../../JSLib/Boolean.md) allowScreenreaders whether to set the allow screen readers permission

**Returns**\
[Array](../../JSLib/Array.md) the encrypted PDF


**Sample**

```javascript
// Add password protection and security options to the PDF
// NOTE: Passwords are case sensitive
var unEncryptedFile = plugins.file.showFileOpenDialog();
if (unEncryptedFile) {
	var data = plugins.file.readFile(unEncryptedFile);
	encryptedResult = %%elementName%%.encrypt(data, 'secretPassword', 'secretUserPassword', false, false, false, false, false, false, false, false, true);
}
```
### encrypt(data, ownerPassword, userPassword, allowAssembly, allowCopy, allowDegradedPrinting, allowFillIn, allowModifyAnnotations, allowModifyContents, allowPrinting, allowScreenreaders, is128bit)

Add password protection and security options to the PDF

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[String](../../JSLib/String.md) ownerPassword the owner password\
[String](../../JSLib/String.md) userPassword the user password\
[Boolean](../../JSLib/Boolean.md) allowAssembly whether to set the allow assembly permission\
[Boolean](../../JSLib/Boolean.md) allowCopy whether to set the allow copy permission\
[Boolean](../../JSLib/Boolean.md) allowDegradedPrinting whether to set the allow degraded printing permission\
[Boolean](../../JSLib/Boolean.md) allowFillIn whether to set the allow fill in permission\
[Boolean](../../JSLib/Boolean.md) allowModifyAnnotations whether to set the allow modify annotations permission\
[Boolean](../../JSLib/Boolean.md) allowModifyContents whether to set the allow modify contents permission\
[Boolean](../../JSLib/Boolean.md) allowPrinting whether to set the allow printing permission\
[Boolean](../../JSLib/Boolean.md) allowScreenreaders whether to set the allow screen readers permission\
[Boolean](../../JSLib/Boolean.md) is128bit whether to use 128-bit encryption

**Returns**\
[Array](../../JSLib/Array.md) the encrypted PDF


**Sample**

```javascript
// Add password protection and security options to the PDF
// NOTE: Passwords are case sensitive
var unEncryptedFile = plugins.file.showFileOpenDialog();
if (unEncryptedFile) {
	var data = plugins.file.readFile(unEncryptedFile);
	encryptedResult = %%elementName%%.encrypt(data, 'secretPassword', 'secretUserPassword', false, false, false, false, false, false, false, false, true);
}
```
### encrypt(data, ownerPassword, userPassword, allowAssembly, allowCopy, allowDegradedPrinting, allowFillIn, allowModifyAnnotations, allowModifyContents, allowPrinting, allowScreenreaders, is128bit, metaData)

Add password protection and security options to the PDF

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[String](../../JSLib/String.md) ownerPassword the owner password\
[String](../../JSLib/String.md) userPassword the user password\
[Boolean](../../JSLib/Boolean.md) allowAssembly whether to set the allow assembly permission\
[Boolean](../../JSLib/Boolean.md) allowCopy whether to set the allow copy permission\
[Boolean](../../JSLib/Boolean.md) allowDegradedPrinting whether to set the allow degraded printing permission\
[Boolean](../../JSLib/Boolean.md) allowFillIn whether to set the allow fill in permission\
[Boolean](../../JSLib/Boolean.md) allowModifyAnnotations whether to set the allow modify annotations permission\
[Boolean](../../JSLib/Boolean.md) allowModifyContents whether to set the allow modify contents permission\
[Boolean](../../JSLib/Boolean.md) allowPrinting whether to set the allow printing permission\
[Boolean](../../JSLib/Boolean.md) allowScreenreaders whether to set the allow screen readers permission\
[Boolean](../../JSLib/Boolean.md) is128bit whether to use 128-bit encryption\
[Object](../../JSLib/Object.md) metaData a JavaScript object (Scriptable) that contains the metadata as property/value pairs

**Returns**\
[Array](../../JSLib/Array.md) the encrypted PDF


**Sample**

```javascript
// Add password protection and security options to the PDF
// NOTE: Passwords are case sensitive
var unEncryptedFile = plugins.file.showFileOpenDialog();
if (unEncryptedFile) {
	var data = plugins.file.readFile(unEncryptedFile);
	encryptedResult = %%elementName%%.encrypt(data, 'secretPassword', 'secretUserPassword', false, false, false, false, false, false, false, false, true);
}
```
### getNumberOfPages(data)

Returns the number of pages for pdf document.

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF

**Returns**\
[Number](../../JSLib/Number.md) the number of pages of the PDF document


**Sample**

```javascript
//get the number of pages
var pages = plugins.pdf_output.getNumberOfPages(bytes);
```
### getThumbnailImage(data)

Create a thumbnail from the provided PDF

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF

**Returns**\
[Array](../../JSLib/Array.md) the PDF thumbnail as PNG format


**Sample**

```javascript
//read PDF file data
var pdf = plugins.file.readFile();
//get the thumbnail (default the first page is rendered with 72 dpi resolution)
var pngImg = plugins.pdf_output.getThumbnailImage(pdf);
//save PNG image to file
var thumbnailFile = plugins.file.convertToJSFile()
plugins.file.writeFile(thumbnailFile, pngImg);
```
### getThumbnailImage(data, pageNumber)

Create a thumbnail from the provided PDF

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[Number](../../JSLib/Number.md) pageNumber PDF page to get thumbnail of. This parameter is zero based index.

**Returns**\
[Array](../../JSLib/Array.md) the PDF thumbnail as PNG format


**Sample**

```javascript
//read PDF file data
var pdf = plugins.file.readFile();
//get the thumbnail (default the first page is rendered with 72 dpi resolution)
var pngImg = plugins.pdf_output.getThumbnailImage(pdf);
//save PNG image to file
var thumbnailFile = plugins.file.convertToJSFile()
plugins.file.writeFile(thumbnailFile, pngImg);
```
### getThumbnailImage(data, pageNumber, dpi)

Create a thumbnail from the provided PDF

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[Number](../../JSLib/Number.md) pageNumber PDF page to get thumbnail of. This parameter is zero based index.\
[Number](../../JSLib/Number.md) dpi resolution used to render the thumbnail image

**Returns**\
[Array](../../JSLib/Array.md) the PDF thumbnail as PNG format


**Sample**

```javascript
//read PDF file data
var pdf = plugins.file.readFile();
//get the thumbnail (default the first page is rendered with 72 dpi resolution)
var pngImg = plugins.pdf_output.getThumbnailImage(pdf);
//save PNG image to file
var thumbnailFile = plugins.file.convertToJSFile()
plugins.file.writeFile(thumbnailFile, pngImg);
```
### numberPages(data)

Add pages numbers to a PDF

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF

**Returns**\
[Array](../../JSLib/Array.md) the PDF with numbered pages


**Sample**

```javascript
// Add pages numbers to a PDF
var unNumberedFile = plugins.file.showFileOpenDialog();
if (unNumberedFile) {
	var data = plugins.file.readFile(unNumberedFile);
	pageNumberedPdf = %%elementName%%.numberPages(data, 12, 520, 30, 'Courier', '#ff0033');
}
```
### numberPages(data, fontSize, locationX, locationY, font, hexColor)

Add pages numbers to a PDF

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[Number](../../JSLib/Number.md) fontSize the font size to use\
[Number](../../JSLib/Number.md) locationX the x location of the numbers\
[Number](../../JSLib/Number.md) locationY the y location of the numbers\
[String](../../JSLib/String.md) font the font to use\
[String](../../JSLib/String.md) hexColor the font color to use

**Returns**\
[Array](../../JSLib/Array.md) the PDF with numbered pages


**Sample**

```javascript
// Add pages numbers to a PDF
var unNumberedFile = plugins.file.showFileOpenDialog();
if (unNumberedFile) {
	var data = plugins.file.readFile(unNumberedFile);
	pageNumberedPdf = %%elementName%%.numberPages(data, 12, 520, 30, 'Courier', '#ff0033');
}
```
### overlay(data, forOverlay)

Add some PDF based content over a PDF

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[Array](../../JSLib/Array.md) forOverlay a PDF to use as overlay

**Returns**\
[Array](../../JSLib/Array.md) the PDF with added overlay


**Sample**

```javascript
// Add some PDF based content over a PDF
var pages = new Array();
pages[0] = '1';
pages[1] = '3';
pages[2] = '5';
var input1 = plugins.file.showFileOpenDialog(1,null,false,'pdf',null,'Select source file');
if (input1) {
	var data = plugins.file.readFile(input1);
	var input2 = plugins.file.showFileOpenDialog(1,null,false,'pdf',null,'Select file for overlay');
	if (input2) {
		var data2 = plugins.file.readFile(input2);
		overlayedPdf = %%elementName%%.overlay( data, data2, false, pages );
		//overlayedPdf = %%elementName%%.overlay( data, data2 );
		//overlayedPdf = %%elementName%%.overlay( data, data2, false, null );
		//overlayedPdf = %%elementName%%.overlay( data, data2, pages );
	}
}
```
### overlay(data, forOverlay, isOver)

Add some PDF based content over a PDF

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[Array](../../JSLib/Array.md) forOverlay a PDF to use as overlay\
[Boolean](../../JSLib/Boolean.md) isOver whether the overlay will be put over the content

**Returns**\
[Array](../../JSLib/Array.md) the PDF with added overlay


**Sample**

```javascript
// Add some PDF based content over a PDF
var pages = new Array();
pages[0] = '1';
pages[1] = '3';
pages[2] = '5';
var input1 = plugins.file.showFileOpenDialog(1,null,false,'pdf',null,'Select source file');
if (input1) {
	var data = plugins.file.readFile(input1);
	var input2 = plugins.file.showFileOpenDialog(1,null,false,'pdf',null,'Select file for overlay');
	if (input2) {
		var data2 = plugins.file.readFile(input2);
		overlayedPdf = %%elementName%%.overlay( data, data2, false, pages );
		//overlayedPdf = %%elementName%%.overlay( data, data2 );
		//overlayedPdf = %%elementName%%.overlay( data, data2, false, null );
		//overlayedPdf = %%elementName%%.overlay( data, data2, pages );
	}
}
```
### overlay(data, forOverlay, isOver, pages)

Add some PDF based content over a PDF

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[Array](../../JSLib/Array.md) forOverlay a PDF to use as overlay\
[Boolean](../../JSLib/Boolean.md) isOver whether the overlay will be put over the content\
[Array](../../JSLib/Array.md) pages an array of page numbers to put the overlay on

**Returns**\
[Array](../../JSLib/Array.md) the PDF with added overlay


**Sample**

```javascript
// Add some PDF based content over a PDF
var pages = new Array();
pages[0] = '1';
pages[1] = '3';
pages[2] = '5';
var input1 = plugins.file.showFileOpenDialog(1,null,false,'pdf',null,'Select source file');
if (input1) {
	var data = plugins.file.readFile(input1);
	var input2 = plugins.file.showFileOpenDialog(1,null,false,'pdf',null,'Select file for overlay');
	if (input2) {
		var data2 = plugins.file.readFile(input2);
		overlayedPdf = %%elementName%%.overlay( data, data2, false, pages );
		//overlayedPdf = %%elementName%%.overlay( data, data2 );
		//overlayedPdf = %%elementName%%.overlay( data, data2, false, null );
		//overlayedPdf = %%elementName%%.overlay( data, data2, pages );
	}
}
```
### overlay(data, forOverlay, pages)

Add some PDF based content over a PDF

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[Array](../../JSLib/Array.md) forOverlay a PDF to use as overlay\
[Array](../../JSLib/Array.md) pages an array of page numbers to put the overlay on

**Returns**\
[Array](../../JSLib/Array.md) the PDF with added overlay


**Sample**

```javascript
// Add some PDF based content over a PDF
var pages = new Array();
pages[0] = '1';
pages[1] = '3';
pages[2] = '5';
var input1 = plugins.file.showFileOpenDialog(1,null,false,'pdf',null,'Select source file');
if (input1) {
	var data = plugins.file.readFile(input1);
	var input2 = plugins.file.showFileOpenDialog(1,null,false,'pdf',null,'Select file for overlay');
	if (input2) {
		var data2 = plugins.file.readFile(input2);
		overlayedPdf = %%elementName%%.overlay( data, data2, false, pages );
		//overlayedPdf = %%elementName%%.overlay( data, data2 );
		//overlayedPdf = %%elementName%%.overlay( data, data2, false, null );
		//overlayedPdf = %%elementName%%.overlay( data, data2, pages );
	}
}
```
### overlayText(data, text)

Add text over every page at a 45 degree angle

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[String](../../JSLib/String.md) text the text to use for the overlay

**Returns**\
[Array](../../JSLib/Array.md) the PDF with added overlay


**Sample**

```javascript
// Add text over every page at a 45 degree angle\m
var pdf = plugins.file.showFileOpenDialog();
if (pdf) {
	var data = plugins.file.readFile(pdf);
	modifiedPdf = %%elementName%%.overlayText(data, 'DRAFT', 230, 430, true, 32, 'Helvetica', '#33ff33');
}
```
### overlayText(data, text, locationX, locationY, isOver, fontSize, font, hexColor)

Add text over every page at a 45 degree angle

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[String](../../JSLib/String.md) text the text to use for the overlay\
[Number](../../JSLib/Number.md) locationX the x location of the overlay\
[Number](../../JSLib/Number.md) locationY the y location of the overlay\
[Boolean](../../JSLib/Boolean.md) isOver whether to put the overlay over the content\
[Number](../../JSLib/Number.md) fontSize the font size to use\
[String](../../JSLib/String.md) font the font to use\
[String](../../JSLib/String.md) hexColor the font color to use

**Returns**\
[Array](../../JSLib/Array.md) the PDF with added overlay


**Sample**

```javascript
// Add text over every page at a 45 degree angle\m
var pdf = plugins.file.showFileOpenDialog();
if (pdf) {
	var data = plugins.file.readFile(pdf);
	modifiedPdf = %%elementName%%.overlayText(data, 'DRAFT', 230, 430, true, 32, 'Helvetica', '#33ff33');
}
```
### overlayText(data, text, locationX, locationY, isOver, fontSize, font, hexColor, angle)

Add text over every page at a 45 degree angle

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[String](../../JSLib/String.md) text the text to use for the overlay\
[Number](../../JSLib/Number.md) locationX the x location of the overlay\
[Number](../../JSLib/Number.md) locationY the y location of the overlay\
[Boolean](../../JSLib/Boolean.md) isOver whether to put the overlay over the content\
[Number](../../JSLib/Number.md) fontSize the font size to use\
[String](../../JSLib/String.md) font the font to use\
[String](../../JSLib/String.md) hexColor the font color to use\
[Number](../../JSLib/Number.md) angle the angle of the overlay

**Returns**\
[Array](../../JSLib/Array.md) the PDF with added overlay


**Sample**

```javascript
// Add text over every page at a 45 degree angle\m
var pdf = plugins.file.showFileOpenDialog();
if (pdf) {
	var data = plugins.file.readFile(pdf);
	modifiedPdf = %%elementName%%.overlayText(data, 'DRAFT', 230, 430, true, 32, 'Helvetica', '#33ff33');
}
```
### watermark(data, image)

Add an image as a watermark on every page, or the pages specified as a parameter

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[Object](../../JSLib/Object.md) image the path of an image to use or array of bytes containing actual image

**Returns**\
[Array](../../JSLib/Array.md) the PDF with added watermak


**Sample**

```javascript
// Add an image as a watermark on every page, or the pages specified as a parameter.
var pdf = plugins.file.showFileOpenDialog();
if (pdf) {
	var data = plugins.file.readFile(pdf);
	var image = plugins.file.showFileOpenDialog();
	modifiedPdf = %%elementName%%.watermark(data, image);
}
```
### watermark(data, image, locationX, locationY, isOver)

Add an image as a watermark on every page, or the pages specified as a parameter

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[Object](../../JSLib/Object.md) image the path of an image to use or array of bytes containing actual image\
[Number](../../JSLib/Number.md) locationX the x location of the image\
[Number](../../JSLib/Number.md) locationY the y location of the image\
[Boolean](../../JSLib/Boolean.md) isOver whether to put over the content

**Returns**\
[Array](../../JSLib/Array.md) the PDF with added watermak


**Sample**

```javascript

```
### watermark(data, image, locationX, locationY, isOver, pages)

Add an image as a watermark on every page, or the pages specified as a parameter

**Parameters**\
[Array](../../JSLib/Array.md) data the PDF\
[Object](../../JSLib/Object.md) image the path of an image to use or array of bytes containing actual image\
[Number](../../JSLib/Number.md) locationX the x location of the image\
[Number](../../JSLib/Number.md) locationY the y location of the image\
[Boolean](../../JSLib/Boolean.md) isOver whether to put over the content\
[Array](../../JSLib/Array.md) pages an array of pages where to apply the watermark

**Returns**\
[Array](../../JSLib/Array.md) the PDF with added watermak


**Sample**

```javascript

```

