Welcome to the office365 wiki!

This plugin enables the [Javascript API for Office](https://dev.office.com/reference/add-ins/javascript-api-for-office) into a Servoy solution which can run as a Microsoft Office [Add-In](https://dev.office.com/docs/add-ins/overview/office-add-ins).

Microsoft Office Add-in runs interactive HTML5 Web Application, as the Servoy NGClient, allowing you to write/read rich text from/to the document using the Office Javascript API. 

All the API implemented in the office365 plugin are synchronous, execution is resumed only once the task is completed making the programming much easier compared to the asynchronous implementation of the standard Javascript API for Office.
Each API can invoke an optional onError handler, containing the error message, in case of failed operation. 

**Table of contents**
* [Word](Word.md)

# Getting Started

To run as a Microsoft Office Add-in the NGClient solution should be embedded into a HTML5 iframe. This documentation provide the guidelines and the resources necessary to setup the sample solution office365$demo.servoy as an Office Add-in.

These are the steps you should follow to run the sample solution as add-in.
* Import the sample solution [office365$demo.servoy](https://github.com/Servoy/office365/releases/download/v1.0.0-b1/office365.demo.servoy)
* Import into the sample solution the [angularmaterial](https://github.com/Servoy/angularmaterial) web components; download the angularmaterial.zip, right click on the Web Packages node in solution explorer -> import zip web package. 
* Download office365 service
* Extract [officeFiles.zip](https://github.com/Servoy/office365/releases/download/v1.0.0-b1/officeFiles.zip) into webapps ROOT (you can find it at SERVOY_INSTALL_FOLDER\application_server\server\webapps\ROOT).
* [Enable HTTPS](https://wiki.servoy.com/display/DOCS/Enabling+HTTPS) in your Servoy environment at port 8443
* Insert the Add-in using the manifest-office365.xml from [officeFiles.zip](https://github.com/Servoy/office365/releases/download/v1.0.0-b1/officeFiles.zip)

# Run your own solution as Add-in

You can use the resouces provided to run the sample solution as Add-in and modify them to point at your own NG Servoy Solution.

### Embedding the Servoy solution in the HTML5 iframe

The office.html page available in the from [officeFiles.zip](https://github.com/Servoy/office365/releases/download/v1.0.0-b1/officeFiles.zip) embed the NG Servoy solution.

The Servoy solution to be run in the Add-in is defined in the office.html at 

```html
<iframe id="iservoy" style="border:0px; width:100%; height:98%;"src="https://localhost:8443/solutions/office365$demo/index.html">
</iframe>
```

Change the src location to your own solution location to embed it into the Add-in. Note that solution should be reached over https.
You should be now able to see your solution loading into the iframe at https://localhost:8443/office/office.html.

### Make your own manifest.xml

To use your Web Application. You should create a manifest.xml file which describe your Add-in application, the permissions granted and the URL to reach your Web Application.
The manifest.xml is defined as below:

```html
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<OfficeApp xmlns="http://schemas.microsoft.com/office/appforoffice/1.1" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:type="TaskPaneApp">
  <Id>b16d4eb7-6848-4e92-b448-11c0fa77ad66</Id>
  <Version>1.0.0.0</Version>
  <ProviderName>[Provider name]</ProviderName>
  <DefaultLocale>en-US</DefaultLocale>
  <DisplayName DefaultValue="myTitle"/>
  <Description DefaultValue="[Task pane Add-in description]"/>
  <Hosts>
    <Host Name="Document"/>
    <Host Name="Workbook"/>
    <Host Name="Presentation"/>
    <Host Name="Project"/>
  </Hosts>
  <DefaultSettings>
    <SourceLocation DefaultValue="https://localhost:8443/office/office.html"/>
  </DefaultSettings>
  <Permissions>ReadWriteDocument</Permissions>
</OfficeApp>
```

The source location defines the URL to the Web Application embedded in the Add-in. Note that the default value is set to https://localhost:8443/office/office.html which is the URL of the Web App embedding the Servoy solution into the iframe.

For development and test you can load the Add-in into Office using the Online version of Office.
* Open a document online, for instance a blank document at Word Online.
* Go to Insert > Office Add-ins
* Choose Manage My Add-ins in the upper-right corner of the dialog box, and select Upload My Add-in.
* Select the manifest.xml file and choose OK.
Read more about how to get started with Office Add-in at http://dev.office.com/getting-started/addins.

To test your Add-in using the Offline version of office Microsoft Visual Studio is required.

## Enable Servoy HTTPS
Office requires to load the solution over https. The Office Add-in won't work if the solution is not exposed over https; for more details on how to enable https in Servoy see the wiki page Network Related Settings [Enabling HTTPS](https://wiki.servoy.com/display/DOCS/Enabling+HTTPS).