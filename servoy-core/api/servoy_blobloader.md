#  servoy_blobloader

The Servoy Blobloader provides a convenient way to access files stored in a database column or a global variable and use it as if it were part of the Servoy Media library.

The Servoy Blobloader is a media URL, with arguments indicating where to retrieve the file from:

**Blobloader syntax to retrieve from the database**

```javascript
var tableName = 'filestoragetable';
var columnName = 'thefile';
var id = 1;
var mimeType = 'application/pdf';
var fileName = 'myFileName';
var URL = 'media:///servoy_blobloader?servername=' + currentcontroller.getServerName()
URL += '&tablename=' + tableName;
URL += '&dataprovider=' + columnName;
URL += '&rowid1=' + id;
URL += '&mimetype=' + mimeType;
URL += '&filename=' + fileName;
return '<html><body><a target="_blank" href="'+URL+'">test</a></body></html>';
```


**Combined primary key**

In case of a PK buildup out of multiple columns, add &rowid2=value ... &rowidXX=value. The PK values should be ordered by their name ascending.


**Blobloader syntax to retrieve from a global variable**

```javascript
var globalName = 'myGlobal';
var mimeType = 'application/pdf';
var fileName = 'myFileName';
var URL = 'media:///servoy_blobloader?global=' + globalName;
URL += '&mimetype=' + mimeType;
URL += '&filename=' + fileName;
return '<html><body><a target="_blank" href="'+URL+'">test</a></body></html>';
```

The Blobloader url can, for example be used in HTMl Area's to display images stored in the database or to provide a clickable downloadlink for the file in the Web Client.  

In the other situation, the mimetype indicates the browser what the type of file is. The browser might use it to open the file in the appropriate application. The filename is suggested to the user when saving the file from the browser.

For more information about mime types, see [w3schools.com on mimetypes](https://www.w3schools.com/jsref/prop_script_type.asp)