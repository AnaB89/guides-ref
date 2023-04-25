Welcome to the **ngdesktoputils** wiki! This wiki provides comprehensive documentation to using the **ngdesktoputils** web service. This service works with the NGDesktop Client as a bridge to execute client side calls from Servoy.


# Getting Started
First import the service using one of the release [binaries](https://github.com/Servoy/ngdesktoputils/releases) or via Servoy's Web Package Manager.

# Example Usage

`        //print a pdf document to default system's printer `
	`plugins.ngdesktoputils.printPDF("/Users/admin/Documents/myZebraFile.pdf");`

	`//print a pdf document to the specified printer`
	`const options = {`
	    `printer: "Zebra"`
	`}`
	`plugins.ngdesktoputils.printPDF("/Users/admin/Documents/myZebraFile.pdf", options);`

	`//print a pdf document with options: second page only on windows, and 2 page on one side for Unix like system`
	`const options = {`
	    `printer: "Zebra",`
	    `unix: ["-o number-up=2"], `
	    `win32: ['-print-settings "2"']`
	`};`

	`//For available options on Unix like systems check you system's lp manual (man lp)`
	`//For available Windows options check the "Printing options" of the command-line arguments for SumatraPDF: https://www.sumatrapdfreader.org/docs/Command-line-arguments`

# API Documentation 

## Method Summary
### exit
This will close the NGDesktop main application. Make sure to application.exit() first to also close the client before closing the desktop application.

### executeCommand
Executes a command async, the server side call will not block on this call.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
program | string | Name of program to execute (i.e "cmd.exe") | Required
args | array | Array of arguments to pass to program | Optional

### executeCommandSync
This executes a command and returns the result of the stdout. This will also call reject when a error happens so the call will error out. (will not return correct). Try to use the async executeCommand if you do not want blocking io.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
program | string | Name of program to execute (i.e "cmd.exe") | Required
args | array | Array of arguments to pass to program | Optional

### setClipboardContent
Write the specified text to the system's clipboard.

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
text | string | Text to be written in the clipboard | Required

### getClipboardContent
Return the system's clipboard as string.

### isNGDesktop
Return whether application is running as NGDesktop or not.

### printPDF
Prints a pdf document specified by path. Optionally, specify printer or unix print options (lp command) or windows print options(SumatraPDF).
Options are fully depending on operating system.

For available options on Unix like systems check you system's lp manual (man lp)
For available Windows options check the "Printing options" of the command-line arguments for SumatraPDF: [https://www.sumatrapdfreader.org/docs/Command-line-arguments](https://www.sumatrapdfreader.org/docs/Command-line-arguments)

**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
path | string | PDF to be printed | Required
options | string | Printer name or Unix options (lp command) or windows options (SumatraPDF) | Optional

### getPrinters
Returns installed printers on local machine.

### getDefaultPrinter
Returns default printer on local machine.






