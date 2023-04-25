# Full API Reference

### Classes

[DataSetExcelWorkbook](API-svyExcelUtils.md#datasetexcelworkbook-servoyexcelworkbook) ⇐ [`ServoyExcelWorkbook`](API-svyExcelUtils.md#new\_ServoyExcelWorkbook\_new)

[ExcelWorkbook](API-svyExcelUtils.md#excelworkbook)

[FoundSetExcelWorkbook](API-svyExcelUtils.md#foundsetexcelworkbook-servoyexcelworkbook) ⇐ [`ServoyExcelWorkbook`](API-svyExcelUtils.md#new\_ServoyExcelWorkbook\_new)

### Members

[copies](API-svyExcelUtils.md#copies-number) : `Number`

The number of copies

[draft](API-svyExcelUtils.md#draft-boolean) : `Boolean`

Whether it is in draft mode

[fitHeight](API-svyExcelUtils.md#fitheight-number) : `Number`

The number of pages high to fit the sheet in

[fitWidth](API-svyExcelUtils.md#fitwidth-number) : `Number`

The number of pages high to fit the sheet in

[landscape](API-svyExcelUtils.md#landscape-boolean) : `Boolean`

Whether to print in landscape

[mergedRegionType](API-svyExcelUtils.md#mergedregiontype-object) : `Object`

[noColor](API-svyExcelUtils.md#nocolor-boolean) : `Boolean`

Whether it is black and white

[paperSize](API-svyExcelUtils.md#papersize-number) : `Number`

The paper size

### Functions

[createPrintSetup()](API-svyExcelUtils.md#createprintsetup-printsetup) ⇒ `PrintSetup`

Creates a PrintSetup object that can be used in ExcelSheet.setPrintSetup() or to set the default print setup used when workbooks are created from FoundSet or DataSet

[createWorkbook(\[templateOrFileType\])](API-svyExcelUtils.md#createworkbook-templateorfiletype-excelworkbook) ⇒ [`ExcelWorkbook`](API-svyExcelUtils.md#ExcelWorkbook)

Returns an empty ExcelWorkbook

[createWorkbookFromDataSet(dataset, \[columns\], \[headers\], \[templateOrFileType\], \[sheetNameToUse\])](API-svyExcelUtils.md#createworkbookfromdataset-dataset-columns-headers-templateorfiletype-sheetnametouse-datasetexcelwork) ⇒ [`DataSetExcelWorkbook`](API-svyExcelUtils.md#datasetexcelworkbook-servoyexcelworkbook)

Creates an ExcelWorkbook from the given dataset

If a template is provided, the dataset will be inserted in the given sheet

[createWorkbookFromFoundSet(foundset, dataproviders, \[headers\], \[templateOrFileType\], \[sheetNameToUse\])](API-svyExcelUtils.md#createworkbookfromfoundset-foundset-dataproviders-headers-templateorfiletype-sheetnametouse-foundset) ⇒ [`FoundSetExcelWorkbook`](API-svyExcelUtils.md#foundsetexcelworkbook-servoyexcelworkbook)

Creates an ExcelWorkbook from the given foundset

If a templateOrFileType is provided, the foundset will be inserted in the given sheet

[getCellReferenceFromRange(firstRow, lastRow, firstColumn, lastColumn)](API-svyExcelUtils.md#getcellreferencefromrange-firstrow-lastrow-firstcolumn-lastcolumn-string) ⇒ `String`

Creates a cell reference (e.g. "A4:C92") from the given range

[getRangeFromCellReference(cellReference)](API-svyExcelUtils.md#getrangefromcellreference-cellreference-object) ⇒ `Object`

Converts a cell reference (e.g. "B4:AK234" or "C6") to an object holding first and last row and column

[getWorkbook(original)](API-svyExcelUtils.md#getworkbook-original-excelworkbook) ⇒ [`ExcelWorkbook`](API-svyExcelUtils.md#ExcelWorkbook)

Returns an ExcelWorkbook from the given file or media URL

[isLoaded()](API-svyExcelUtils.md#isloaded-boolean) ⇒ `Boolean`

If true, all required libraries are present and the scope can be used

[set()](API-svyExcelUtils.md#set)

[setDefaultPrintSetup(setup)](API-svyExcelUtils.md#setdefaultprintsetup-setup)

Sets the default print setup used when workbooks are created from FoundSet or DataSet

### DataSetExcelWorkbook ⇐ [`ServoyExcelWorkbook`](API-svyExcelUtils.md#new\_ServoyExcelWorkbook\_new)

**Extends**: [`ServoyExcelWorkbook`](API-svyExcelUtils.md#new\_ServoyExcelWorkbook\_new)

* [DataSetExcelWorkbook](API-svyExcelUtils.md#datasetexcelworkbook-servoyexcelworkbook) ⇐ [`ServoyExcelWorkbook`](API-svyExcelUtils.md#new\_ServoyExcelWorkbook\_new)
  * _inner_
    * [\~dataFilled](API-svyExcelUtils.md#datasetexcelworkbook-datafilled-boolean) : `Boolean`
  * _instance_
    * [.cloneCellStyle(cellStyle)](API-svyExcelUtils.md#datasetexcelworkbook.clonecellstyle-cellstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
    * [.cloneFont(font)](API-svyExcelUtils.md#datasetexcelworkbook.clonefont-font-excelfont) ⇒ [`ExcelFont`](API-svyExcelUtils.md#new\_ExcelFont\_new)
    * [.cloneSheet(indexToClone)](API-svyExcelUtils.md#datasetexcelworkbook.clonesheet-indextoclone-excelsheet) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)
    * [.close()](API-svyExcelUtils.md#datasetexcelworkbook.close)
    * [.createCellStyle()](API-svyExcelUtils.md#datasetexcelworkbook.createcellstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
    * [.createColumnStyle(columnIndex)](API-svyExcelUtils.md#datasetexcelworkbook.createcolumnstyle-columnindex-excelcellstyle) ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
    * [.createFont()](API-svyExcelUtils.md#datasetexcelworkbook.createfont-excelfont) ⇒ [`ExcelFont`](API-svyExcelUtils.md#new\_ExcelFont\_new)
    * [.createHeaderStyle()](API-svyExcelUtils.md#datasetexcelworkbook.createheaderstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
    * [.createRowStyle()](API-svyExcelUtils.md#datasetexcelworkbook.createrowstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
    * [.createSheet(sheetName)](API-svyExcelUtils.md#datasetexcelworkbook.createsheet-sheetname-excelsheet) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)
    * [.fillData()](API-svyExcelUtils.md#datasetexcelworkbook.filldata)
    * [.getBytes()](API-svyExcelUtils.md#datasetexcelworkbook.getbytes-array-.less-than-byte-greater-than) ⇒ `[ 'Array' ].<byte>`
    * [.getDataSet()](API-svyExcelUtils.md#datasetexcelworkbook.getdataset-jsdataset) ⇒ `JSDataSet`
    * [.getNumberOfSheets()](API-svyExcelUtils.md#datasetexcelworkbook.getnumberofsheets-number) ⇒ `Number`
    * [.getSheet(sheetName)](API-svyExcelUtils.md#datasetexcelworkbook.getsheet-sheetname-excelsheet) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)
    * [.getSheetAt(index)](API-svyExcelUtils.md#datasetexcelworkbook.getsheetat-index-excelsheet) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)
    * [.getSheetNameAt(index)](API-svyExcelUtils.md#datasetexcelworkbook.getsheetnameat-index-string) ⇒ `String`
    * [.getSheetNames()](API-svyExcelUtils.md#datasetexcelworkbook.getsheetnames-array-.less-than-string-greater-than) ⇒ `[ 'Array' ].<String>`
    * [.removeSheetAt(index)](API-svyExcelUtils.md#datasetexcelworkbook.removesheetat-index)
    * [.setFormatForColumn(columnIndex, format)](API-svyExcelUtils.md#datasetexcelworkbook.setformatforcolumn-columnindex-format)
    * [.setSheetNameAt(index, name)](API-svyExcelUtils.md#datasetexcelworkbook.setsheetnameat-index-name)
    * [.writeToFile(targetFile)](API-svyExcelUtils.md#datasetexcelworkbook.writetofile-targetfile-boolean) ⇒ `Boolean`
    * [.autoSizeColumns](API-svyExcelUtils.md#datasetexcelworkbook.autosizecolumns-boolean) : `Boolean`
    * [.columnFormats](API-svyExcelUtils.md#datasetexcelworkbook.columnformats-array-.less-than-string-greater-than) : `[ 'Array' ].<String>`
    * [.columnStyles](API-svyExcelUtils.md#datasetexcelworkbook.columnstyles-array-.less-than-excelcellstyle-greater-than) : [`[ 'Array' ].<ExcelCellStyle>`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
    * [.dataset](API-svyExcelUtils.md#datasetexcelworkbook.dataset-jsdataset) : `JSDataSet`
    * [.defaultDateFormat](API-svyExcelUtils.md#datasetexcelworkbook.defaultdateformat-string) : `String`
    * [.defaultNumberFormat](API-svyExcelUtils.md#datasetexcelworkbook.defaultnumberformat-string) : `String`
    * [.freezeFirstRow](API-svyExcelUtils.md#datasetexcelworkbook.freezefirstrow-boolean) : `Boolean`
    * [.headerStyle](API-svyExcelUtils.md#datasetexcelworkbook.headerstyle-excelcellstyle) : [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
    * [.rowStyle](API-svyExcelUtils.md#datasetexcelworkbook.rowstyle-excelcellstyle) : [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
    * [.setAutoFilter](API-svyExcelUtils.md#datasetexcelworkbook.setautofilter-boolean) : `Boolean`
    * [.sheet](API-svyExcelUtils.md#datasetexcelworkbook.sheet-excelsheet) : [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)
    * [.sheetName](API-svyExcelUtils.md#datasetexcelworkbook.sheetname-string) : `String`
    * [.startColumn](API-svyExcelUtils.md#datasetexcelworkbook.startcolumn-number) : `Number`
    * [.startRow](API-svyExcelUtils.md#datasetexcelworkbook.startrow-number) : `Number`
    * [.wb](API-svyExcelUtils.md#datasetexcelworkbook.wb-packages.org.apache.poi.ss.usermodel.workbook) : `Packages.org.apache.poi.ss.usermodel.Workbook`
    * [.workbook](API-svyExcelUtils.md#datasetexcelworkbook.workbook-excelworkbook) : [`ExcelWorkbook`](API-svyExcelUtils.md#ExcelWorkbook)
  * [new DataSetExcelWorkbook(dataset, \[columns\], \[headers\], \[templateOrFileType\], \[sheetNameToUse\])](API-svyExcelUtils.md#new-datasetexcelworkbook-dataset-columns-headers-templateorfiletype-sheetnametouse)

#### DataSetExcelWorkbook\~dataFilled : `Boolean`

#### dataSetExcelWorkbook.cloneCellStyle(cellStyle) ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

Clones the given ExcelCellStyle

| Param     | Type                                                              |
| --------- | ----------------------------------------------------------------- |
| cellStyle | [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new) |

#### dataSetExcelWorkbook.cloneFont(font) ⇒ [`ExcelFont`](API-svyExcelUtils.md#new\_ExcelFont\_new)

Clones the given font and returns a new ExcelFont

| Param | Type                                                    |
| ----- | ------------------------------------------------------- |
| font  | [`ExcelFont`](API-svyExcelUtils.md#new\_ExcelFont\_new) |

#### dataSetExcelWorkbook.cloneSheet(indexToClone) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)

Creates an ExcelSheet from an existing sheet in the Workbook

**Returns**: [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new) - clone

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| indexToClone | `Number` | one based   |

#### dataSetExcelWorkbook.close()

Closes this workbook

#### dataSetExcelWorkbook.createCellStyle() ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

Creates an empty ExcelCellStyle

#### dataSetExcelWorkbook.createColumnStyle(columnIndex) ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

Creates and returns an ExcelCellStyle used for a specific column

| Param       | Type     |
| ----------- | -------- |
| columnIndex | `Number` |

#### dataSetExcelWorkbook.createFont() ⇒ [`ExcelFont`](API-svyExcelUtils.md#new\_ExcelFont\_new)

Creates a font

#### dataSetExcelWorkbook.createHeaderStyle() ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

Creates and returns an ExcelCellStyle used for the header row

#### dataSetExcelWorkbook.createRowStyle() ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

Creates and returns an ExcelCellStyle used for a data row

#### dataSetExcelWorkbook.createSheet(sheetName) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)

Creates a sheet with the given name

This method makes sure that no illegal names are provided and might change the name if needed

| Param     | Type     |
| --------- | -------- |
| sheetName | `String` |

#### dataSetExcelWorkbook.fillData()

Fills the sheet with the data of the foundset

This is automatically done when `writeToFile()` or `getBytes()` is called

**Overrides**: [`fillData`](API-svyExcelUtils.md#ServoyExcelWorkbook+fillData)

#### dataSetExcelWorkbook.getBytes() ⇒ `[ 'Array' ].<byte>`

Returns the data of this workbook as a byte\[]

**Returns**: `[ 'Array' ].<byte>` - bytes

#### dataSetExcelWorkbook.getDataSet() ⇒ `JSDataSet`

Returns the dataset used to create this workbook

#### dataSetExcelWorkbook.getNumberOfSheets() ⇒ `Number`

Returns the number of spreadsheets in the workbook

#### dataSetExcelWorkbook.getSheet(sheetName) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)

Returns the sheet with the given name (case insensitive match)

| Param     | Type     |
| --------- | -------- |
| sheetName | `String` |

#### dataSetExcelWorkbook.getSheetAt(index) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)

Returns the ExcelSheet object at the given index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### dataSetExcelWorkbook.getSheetNameAt(index) ⇒ `String`

Returns the name of the sheet at the given index

**Returns**: `String` - sheetName

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### dataSetExcelWorkbook.getSheetNames() ⇒ `[ 'Array' ].<String>`

Returns all sheet names

#### dataSetExcelWorkbook.removeSheetAt(index)

Removes the sheet at the given index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### dataSetExcelWorkbook.setFormatForColumn(columnIndex, format)

Sets a date or number format used for the given column

| Param       | Type     |
| ----------- | -------- |
| columnIndex | `Number` |
| format      | `String` |

#### dataSetExcelWorkbook.setSheetNameAt(index, name)

Sets the sheet name

| Param | Type     |
| ----- | -------- |
| index | `Number` |
| name  | `String` |

#### dataSetExcelWorkbook.writeToFile(targetFile) ⇒ `Boolean`

Writes this workbook to the given file

**Returns**: `Boolean` - success

| Param      | Type                              |
| ---------- | --------------------------------- |
| targetFile | `String` \| `plugins.file.JSFile` |

#### dataSetExcelWorkbook.autoSizeColumns : `Boolean`

Whether or not all data columns should be auto sized

#### dataSetExcelWorkbook.columnFormats : `[ 'Array' ].<String>`

#### dataSetExcelWorkbook.columnStyles : [`[ 'Array' ].<ExcelCellStyle>`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

#### dataSetExcelWorkbook.dataset : `JSDataSet`

The dataset used to create this workbook

#### dataSetExcelWorkbook.defaultDateFormat : `String`

The default format used to format date values

This can be overriden for specific columns by calling `setFormatForColumn()`

#### dataSetExcelWorkbook.defaultNumberFormat : `String`

The default format used to format number values

This can be overriden for specific columns by calling `setFormatForColumn()`

#### dataSetExcelWorkbook.freezeFirstRow : `Boolean`

Whether the header row is frozen or not

**Overrides**: [`freezeFirstRow`](API-svyExcelUtils.md#ServoyExcelWorkbook+freezeFirstRow)

#### dataSetExcelWorkbook.headerStyle : [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

The style used for the header of the data

**Overrides**: [`headerStyle`](API-svyExcelUtils.md#ServoyExcelWorkbook+headerStyle)

#### dataSetExcelWorkbook.rowStyle : [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

The style used for a data cell

**Overrides**: [`rowStyle`](API-svyExcelUtils.md#ServoyExcelWorkbook+rowStyle)

#### dataSetExcelWorkbook.setAutoFilter : `Boolean`

Whether or not the data columns should be auto filtered or not

**Overrides**: [`setAutoFilter`](API-svyExcelUtils.md#ServoyExcelWorkbook+setAutoFilter)

#### dataSetExcelWorkbook.sheet : [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)

The ExcelSheet used or created

#### dataSetExcelWorkbook.sheetName : `String`

The name of the sheet to be used

When a template is used, data will be inserted in the sheet with this name or the first best if not found

#### dataSetExcelWorkbook.startColumn : `Number`

The first column where data will be inserted (one based)

#### dataSetExcelWorkbook.startRow : `Number`

The first row where data will be inserted (one based)

#### dataSetExcelWorkbook.wb : `Packages.org.apache.poi.ss.usermodel.Workbook`

The internal workbook object

#### dataSetExcelWorkbook.workbook : [`ExcelWorkbook`](API-svyExcelUtils.md#excelworkbook)

The ExcelWorkbook created

#### new DataSetExcelWorkbook(dataset, \[columns], \[headers], \[templateOrFileType], \[sheetNameToUse])

A DataSet based Excel workbook

| Param                 | Type                                          | Description                                                                                                                                      |
| --------------------- | --------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| dataset               | `JSDataSet`                                   | the dataset                                                                                                                                      |
| \[columns]            | `[ 'Array' ].<Number>`                        | the column numbers to be included in the sheet                                                                                                   |
| \[headers]            | `[ 'Array' ].<String>`                        | the text to be used as column headers                                                                                                            |
| \[templateOrFileType] | `String` \| `plugins.file.JSFile` \| `Number` | either file or media URL pointing to an existing Excel to be used as template or one of the FILE\_FORMAT constants when creating empty workbooks |
| \[sheetNameToUse]     | `String`                                      | when a template is used, this is the name of the sheet to be filled                                                                              |

**Example**

```js
var query = datasources.db.example_data.orders.createSelect();
query.result.add(query.columns.customerid);	
query.result.add(query.columns.shipname);
query.result.add(query.columns.shipaddress);
query.result.add(query.columns.shipcity);
query.result.add(query.columns.shipcountry);
query.result.add(query.columns.shippeddate);
query.result.add(query.columns.freight);	
var dataset = databaseManager.getDataSetByQuery(query, -1);

var wb = scopes.svyExcelUtils.createWorkbookFromDataSet(dataset, [2,3,4,5,6,7], ["Company", "Address", "City", "Country", "Order date", "Freight"]);

wb.setFormatForColumn(5, "yyyy-MM-dd");
wb.setFormatForColumn(6, "#,##0.00");
wb.sheetName = "Dataset export";
wb.autoSizeColumns = true;
wb.freezeFirstRow = true;
wb.setAutoFilter = true;

var headerStyle = wb.createHeaderStyle();
headerStyle.setFont("Calibri,1,12");
headerStyle.setFillForegroundColor(scopes.svyExcelUtils.INDEXED_COLOR.LIGHT_CORNFLOWER_BLUE);
headerStyle.setFillPattern(scopes.svyExcelUtils.FILL_PATTERN.SOLID_FOREGROUND);

wb.writeToFile("d:\\dataset.xls");
```

***

### ExcelWorkbook

**Suppresswarnings(deprecated)**: needs to be added to prevent warnings from deprecated WorkbookFactory.create(Object)

* [ExcelWorkbook](API-svyExcelUtils.md#excelworkbook)
  * [.cloneCellStyle(cellStyle)](API-svyExcelUtils.md#excelworkbook.clonecellstyle-cellstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
  * [.cloneFont(font)](API-svyExcelUtils.md#excelworkbook.clonefont-font-excelfont) ⇒ [`ExcelFont`](API-svyExcelUtils.md#new\_ExcelFont\_new)
  * [.cloneSheet(indexToClone)](API-svyExcelUtils.md#excelworkbook.clonesheet-indextoclone-excelsheet) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)
  * [.close()](API-svyExcelUtils.md#excelworkbook.close)
  * [.createCellStyle()](API-svyExcelUtils.md#excelworkbook.createcellstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
  * [.createFont()](API-svyExcelUtils.md#excelworkbook.createfont-excelfont) ⇒ [`ExcelFont`](API-svyExcelUtils.md#new\_ExcelFont\_new)
  * [.createSheet(sheetName)](API-svyExcelUtils.md#excelworkbook.createsheet-sheetname-excelsheet) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)
  * [.getBytes()](API-svyExcelUtils.md#excelworkbook.getbytes-array-.less-than-byte-greater-than) ⇒ `[ 'Array' ].<byte>`
  * [.getNumberOfSheets()](API-svyExcelUtils.md#excelworkbook.getnumberofsheets-number) ⇒ `Number`
  * [.getSheet(sheetName)](API-svyExcelUtils.md#excelworkbook.getsheet-sheetname-excelsheet) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)
  * [.getSheetAt(index)](API-svyExcelUtils.md#excelworkbook.getsheetat-index-excelsheet) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)
  * [.getSheetNameAt(index)](API-svyExcelUtils.md#excelworkbook.getsheetnameat-index-string) ⇒ `String`
  * [.getSheetNames()](API-svyExcelUtils.md#excelworkbook.getsheetnames-array-.less-than-string-greater-than) ⇒ `[ 'Array' ].<String>`
  * [.removeSheetAt(index)](API-svyExcelUtils.md#excelworkbook.removesheetat-index)
  * [.setSheetNameAt(index, name)](API-svyExcelUtils.md#excelworkbook.setsheetnameat-index-name)
  * [.writeToFile(targetFile)](API-svyExcelUtils.md#excelworkbook.writetofile-targetfile-boolean) ⇒ `Boolean`
  * [.wb](API-svyExcelUtils.md#excelworkbook.wb-packages.org.apache.poi.ss.usermodel.workbook) : `Packages.org.apache.poi.ss.usermodel.Workbook`
  * [new ExcelWorkbook(\[templateOrFileType\])](API-svyExcelUtils.md#new-excelworkbook-templateorfiletype)

#### excelWorkbook.cloneCellStyle(cellStyle) ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

Clones the given ExcelCellStyle

| Param     | Type                                                              |
| --------- | ----------------------------------------------------------------- |
| cellStyle | [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new) |

#### excelWorkbook.cloneFont(font) ⇒ [`ExcelFont`](API-svyExcelUtils.md#new\_ExcelFont\_new)

Clones the given font and returns a new ExcelFont

| Param | Type                                                    |
| ----- | ------------------------------------------------------- |
| font  | [`ExcelFont`](API-svyExcelUtils.md#new\_ExcelFont\_new) |

#### excelWorkbook.cloneSheet(indexToClone) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)

Creates an ExcelSheet from an existing sheet in the Workbook

**Returns**: [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new) - clone

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| indexToClone | `Number` | one based   |

#### excelWorkbook.close()

Closes this workbook

#### excelWorkbook.createCellStyle() ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

Creates an empty ExcelCellStyle

#### excelWorkbook.createFont() ⇒ [`ExcelFont`](API-svyExcelUtils.md#new\_ExcelFont\_new)

Creates a font

#### excelWorkbook.createSheet(sheetName) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)

Creates a sheet with the given name

This method makes sure that no illegal names are provided and might change the name if needed

| Param     | Type     |
| --------- | -------- |
| sheetName | `String` |

#### excelWorkbook.getBytes() ⇒ `[ 'Array' ].<byte>`

Returns this workbook as a byte\[] array

#### excelWorkbook.getNumberOfSheets() ⇒ `Number`

Returns the number of spreadsheets in the workbook

#### excelWorkbook.getSheet(sheetName) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)

Returns the sheet with the given name (case insensitive match)

| Param     | Type     |
| --------- | -------- |
| sheetName | `String` |

#### excelWorkbook.getSheetAt(index) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)

Returns the ExcelSheet object at the given index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### excelWorkbook.getSheetNameAt(index) ⇒ `String`

Returns the name of the sheet at the given index

**Returns**: `String` - sheetName

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### excelWorkbook.getSheetNames() ⇒ `[ 'Array' ].<String>`

Returns all sheet names

#### excelWorkbook.removeSheetAt(index)

Removes the sheet at the given index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

***

#### excelWorkbook.setSheetNameAt(index, name)

Sets the sheet name

| Param | Type     |
| ----- | -------- |
| index | `Number` |
| name  | `String` |

***

#### excelWorkbook.writeToFile(targetFile) ⇒ `Boolean`

Writes this workbook to the given targetFile

**Returns**: `Boolean` - success

| Param      | Type                              |
| ---------- | --------------------------------- |
| targetFile | `plugins.file.JSFile` \| `String` |

***

#### excelWorkbook.wb : `Packages.org.apache.poi.ss.usermodel.Workbook`

The internal workbook object

***

#### new ExcelWorkbook(\[templateOrFileType])

Creates an empty Excel workbook or reads the one provided

| Param                 | Type                                                            | Description                                                                                                                                     |
| --------------------- | --------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| \[templateOrFileType] | `String` \| `plugins.file.JSFile` \| `Number` \| `Array.<byte>` | either a path, mediaUrl, JSFile or byte\[] when reading an existing workbook or one of the FILE\_FORMAT constants when creating empty workbooks |

**Example**

```js
// Create workbook and sheet
var workbook = new scopes.svyExcelUtils.Workbook(scopes.svyExcelUtils.FILE_FORMAT.XLSX);
var sheet = workbook.createSheet("Test");

// Create style for the header
var headerStyle = workbook.createCellStyle();
headerStyle
   .setFont("Arial,1,12")
   .setFillPattern(scopes.svyExcelUtils.FILL_PATTERN.SOLID_FOREGROUND)
   .setFillForegroundColor(scopes.svyExcelUtils.INDEXED_COLOR.LIGHT_ORANGE)
   .setAlignment(scopes.svyExcelUtils.ALIGNMENT.CENTER);

var rowNum = 1;

// Create header row and cells
var row = sheet.createRow(rowNum ++);
var cell = row.createCell(1);
cell.setCellValue("Test 1", headerStyle);

cell = row.createCell(2);
cell.setCellValue("Test 2", headerStyle);

// Create some data and write to the sheet
var data = [[10, 35], [15, 47], [9, 22], [10, 33]];
for (var i = 0; i < data.length; i++) {
   row = sheet.createRow(rowNum ++);
   row.createCell(1).setCellValue(data[i][0]);
   row.createCell(2).setCellValue(data[i][1]);
}

// Create a style for the sum
var sumStyle = workbook.createCellStyle();
// Clone the default font, so we won't be changing the default
var font = sumStyle.cloneFont();
font.underline = scopes.svyExcelUtils.FONT_UNDERLINE.DOUBLE_ACCOUNTING;
font.isBold = true;

// Create formula cells at the bottom
row = sheet.createRow(rowNum ++);
cell = row.createCell(1);
cell.setCellStyle(sumStyle);
cell.setCellFormula("SUM(" + scopes.svyExcelUtils.getCellReferenceFromRange(2, 1 + data.length, 1, 1) + ")");

cell = row.createCell(2);
cell.setCellStyle(sumStyle);
cell.setCellFormula("SUM(" + scopes.svyExcelUtils.getCellReferenceFromRange(2, 1 + data.length, 2, 2) + ")");

// Write to file
var success = workbook.writeToFile("d:\\test.xls");
```

***

### FoundSetExcelWorkbook ⇐ [`ServoyExcelWorkbook`](API-svyExcelUtils.md#new\_ServoyExcelWorkbook\_new)

**Extends**: [`ServoyExcelWorkbook`](API-svyExcelUtils.md#new\_ServoyExcelWorkbook\_new)

* [FoundSetExcelWorkbook](API-svyExcelUtils.md#foundsetexcelworkbook-servoyexcelworkbook) ⇐ [`ServoyExcelWorkbook`](API-svyExcelUtils.md#new\_ServoyExcelWorkbook\_new)
  * _inner_
    * [\~dataFilled](API-svyExcelUtils.md#foundsetexcelworkbook-datafilled-boolean) : `Boolean`
  * _instance_
    * [.cloneCellStyle(cellStyle)](API-svyExcelUtils.md#foundsetexcelworkbook.clonecellstyle-cellstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
    * [.cloneFont(font)](API-svyExcelUtils.md#foundsetexcelworkbook.clonefont-font-excelfont) ⇒ [`ExcelFont`](API-svyExcelUtils.md#new\_ExcelFont\_new)
    * [.cloneSheet(indexToClone)](API-svyExcelUtils.md#foundsetexcelworkbook.clonesheet-indextoclone-excelsheet) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)
    * [.close()](API-svyExcelUtils.md#foundsetexcelworkbook.close)
    * [.createCellStyle()](API-svyExcelUtils.md#foundsetexcelworkbook.createcellstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
    * [.createColumnStyle(columnIndex)](API-svyExcelUtils.md#foundsetexcelworkbook.createcolumnstyle-columnindex-excelcellstyle) ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
    * [.createFont()](API-svyExcelUtils.md#foundsetexcelworkbook.createfont-excelfont) ⇒ [`ExcelFont`](API-svyExcelUtils.md#new\_ExcelFont\_new)
    * [.createHeaderStyle()](API-svyExcelUtils.md#foundsetexcelworkbook.createheaderstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
    * [.createRowStyle()](API-svyExcelUtils.md#foundsetexcelworkbook.createrowstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
    * [.createSheet(sheetName)](API-svyExcelUtils.md#foundsetexcelworkbook.createsheet-sheetname-excelsheet) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)
    * [.fillData()](API-svyExcelUtils.md#foundsetexcelworkbook.filldata)
    * [.getBytes()](API-svyExcelUtils.md#foundsetexcelworkbook.getbytes-array-.less-than-byte-greater-than) ⇒ `[ 'Array' ].<byte>`
    * [.getFoundSet()](API-svyExcelUtils.md#foundsetexcelworkbook.getfoundset-jsfoundset) ⇒ `JSFoundSet`
    * [.getNumberOfSheets()](API-svyExcelUtils.md#foundsetexcelworkbook.getnumberofsheets-number) ⇒ `Number`
    * [.getSheet(sheetName)](API-svyExcelUtils.md#foundsetexcelworkbook.getsheet-sheetname-excelsheet) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)
    * [.getSheetAt(index)](API-svyExcelUtils.md#foundsetexcelworkbook.getsheetat-index-excelsheet) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)
    * [.getSheetNameAt(index)](API-svyExcelUtils.md#foundsetexcelworkbook.getsheetnameat-index-string) ⇒ `String`
    * [.getSheetNames()](API-svyExcelUtils.md#foundsetexcelworkbook.getsheetnames-array-.less-than-string-greater-than) ⇒ `[ 'Array' ].<String>`
    * [.removeSheetAt(index)](API-svyExcelUtils.md#foundsetexcelworkbook.removesheetat-index)
    * [.setFormatForColumn(columnIndex, format)](API-svyExcelUtils.md#foundsetexcelworkbook.setformatforcolumn-columnindex-format)
    * [.setSheetNameAt(index, name)](API-svyExcelUtils.md#foundsetexcelworkbook.setsheetnameat-index-name)
    * [.writeToFile(targetFile)](API-svyExcelUtils.md#foundsetexcelworkbook.writetofile-targetfile-boolean) ⇒ `Boolean`
    * [.autoSizeColumns](API-svyExcelUtils.md#foundsetexcelworkbook.autosizecolumns-boolean) : `Boolean`
    * [.columnFormats](API-svyExcelUtils.md#foundsetexcelworkbook.columnformats-array-.less-than-string-greater-than) : `[ 'Array' ].<String>`
    * [.columnStyles](API-svyExcelUtils.md#foundsetexcelworkbook.columnstyles-array-.less-than-excelcellstyle-greater-than) : [`[ 'Array' ].<ExcelCellStyle>`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
    * [.defaultDateFormat](API-svyExcelUtils.md#foundsetexcelworkbook.defaultdateformat-string) : `String`
    * [.defaultNumberFormat](API-svyExcelUtils.md#foundsetexcelworkbook.defaultnumberformat-string) : `String`
    * [.foundset](API-svyExcelUtils.md#foundsetexcelworkbook.foundset-jsfoundset) : `JSFoundSet`
    * [.freezeFirstRow](API-svyExcelUtils.md#foundsetexcelworkbook.freezefirstrow-boolean) : `Boolean`
    * [.headerStyle](API-svyExcelUtils.md#foundsetexcelworkbook.headerstyle-excelcellstyle) : [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
    * [.rowStyle](API-svyExcelUtils.md#foundsetexcelworkbook.rowstyle-excelcellstyle) : [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)
    * [.setAutoFilter](API-svyExcelUtils.md#foundsetexcelworkbook.setautofilter-boolean) : `Boolean`
    * [.sheet](API-svyExcelUtils.md#foundsetexcelworkbook.sheet-excelsheet) : [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)
    * [.sheetName](API-svyExcelUtils.md#foundsetexcelworkbook.sheetname-string) : `String`
    * [.startColumn](API-svyExcelUtils.md#foundsetexcelworkbook.startcolumn-number) : `Number`
    * [.startRow](API-svyExcelUtils.md#foundsetexcelworkbook.startrow-number) : `Number`
    * [.wb](API-svyExcelUtils.md#foundsetexcelworkbook.wb-packages.org.apache.poi.ss.usermodel.workbook) : `Packages.org.apache.poi.ss.usermodel.Workbook`
    * [.workbook](API-svyExcelUtils.md#foundsetexcelworkbook.workbook-excelworkbook) : [`ExcelWorkbook`](API-svyExcelUtils.md#excelworkbook)
  * [new FoundSetExcelWorkbook(foundset, dataproviders, \[headers\], \[templateOrFileType\], \[sheetNameToUse\]](API-svyExcelUtils.md#new-foundsetexcelworkbook-foundset-dataproviders-headers-templateorfiletype-sheetnametouse)

#### FoundSetExcelWorkbook\~dataFilled : `Boolean`

#### foundSetExcelWorkbook.cloneCellStyle(cellStyle) ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

Clones the given ExcelCellStyle

| Param     | Type                                                              |
| --------- | ----------------------------------------------------------------- |
| cellStyle | [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new) |

#### foundSetExcelWorkbook.cloneFont(font) ⇒ [`ExcelFont`](API-svyExcelUtils.md#new\_ExcelFont\_new)

Clones the given font and returns a new ExcelFont

| Param | Type                                                    |
| ----- | ------------------------------------------------------- |
| font  | [`ExcelFont`](API-svyExcelUtils.md#new\_ExcelFont\_new) |

#### foundSetExcelWorkbook.cloneSheet(indexToClone) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)

Creates an ExcelSheet from an existing sheet in the Workbook

**Returns**: [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new) - clone

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| indexToClone | `Number` | one based   |

#### foundSetExcelWorkbook.close()

Closes this workbook

#### foundSetExcelWorkbook.createCellStyle() ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

Creates an empty ExcelCellStyle

#### foundSetExcelWorkbook.createColumnStyle(columnIndex) ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

Creates and returns an ExcelCellStyle used for a specific column

| Param       | Type     |
| ----------- | -------- |
| columnIndex | `Number` |

#### foundSetExcelWorkbook.createFont() ⇒ [`ExcelFont`](API-svyExcelUtils.md#new\_ExcelFont\_new)

Creates a font

#### foundSetExcelWorkbook.createHeaderStyle() ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

Creates and returns an ExcelCellStyle used for the header row

#### foundSetExcelWorkbook.createRowStyle() ⇒ [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

Creates and returns an ExcelCellStyle used for a data row

#### foundSetExcelWorkbook.createSheet(sheetName) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)

Creates a sheet with the given name

This method makes sure that no illegal names are provided and might change the name if needed

| Param     | Type     |
| --------- | -------- |
| sheetName | `String` |

#### foundSetExcelWorkbook.fillData()

Fills the sheet with the data of the foundset

This is automatically done when `writeToFile()` or `getBytes()` is called

**Overrides**: [`fillData`](API-svyExcelUtils.md#ServoyExcelWorkbook+fillData)

#### foundSetExcelWorkbook.getBytes() ⇒ `[ 'Array' ].<byte>`

Returns the data of this workbook as a byte\[]

**Returns**: `[ 'Array' ].<byte>` - bytes

#### foundSetExcelWorkbook.getFoundSet() ⇒ `JSFoundSet`

Returns the foundset used to create this workbook

#### foundSetExcelWorkbook.getNumberOfSheets() ⇒ `Number`

Returns the number of spreadsheets in the workbook

#### foundSetExcelWorkbook.getSheet(sheetName) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)

Returns the sheet with the given name (case insensitive match)

| Param     | Type     |
| --------- | -------- |
| sheetName | `String` |

#### foundSetExcelWorkbook.getSheetAt(index) ⇒ [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)

Returns the ExcelSheet object at the given index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### foundSetExcelWorkbook.getSheetNameAt(index) ⇒ `String`

Returns the name of the sheet at the given index

**Returns**: `String` - sheetName

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### foundSetExcelWorkbook.getSheetNames() ⇒ `[ 'Array' ].<String>`

Returns all sheet names

#### foundSetExcelWorkbook.removeSheetAt(index)

Removes the sheet at the given index

| Param | Type     |
| ----- | -------- |
| index | `Number` |

#### foundSetExcelWorkbook.setFormatForColumn(columnIndex, format)

Sets a date or number format used for the given column

| Param       | Type     |
| ----------- | -------- |
| columnIndex | `Number` |
| format      | `String` |

#### foundSetExcelWorkbook.setSheetNameAt(index, name)

Sets the sheet name

| Param | Type     |
| ----- | -------- |
| index | `Number` |
| name  | `String` |

#### foundSetExcelWorkbook.writeToFile(targetFile) ⇒ `Boolean`

Writes this workbook to the given file

**Returns**: `Boolean` - success

| Param      | Type                              |
| ---------- | --------------------------------- |
| targetFile | `String` \| `plugins.file.JSFile` |

#### foundSetExcelWorkbook.autoSizeColumns : `Boolean`

Whether or not all data columns should be auto sized

#### foundSetExcelWorkbook.columnFormats : `[ 'Array' ].<String>`

#### foundSetExcelWorkbook.columnStyles : [`[ 'Array' ].<ExcelCellStyle>`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

#### foundSetExcelWorkbook.defaultDateFormat : `String`

The default format used to format date values

This can be overriden for specific columns by calling `setFormatForColumn()`

#### foundSetExcelWorkbook.defaultNumberFormat : `String`

The default format used to format number values

This can be overriden for specific columns by calling `setFormatForColumn()`

#### foundSetExcelWorkbook.foundset : `JSFoundSet`

The foundset used to create this workbook

#### foundSetExcelWorkbook.freezeFirstRow : `Boolean`

Whether the header row is frozen or not

**Overrides**: [`freezeFirstRow`](API-svyExcelUtils.md#ServoyExcelWorkbook+freezeFirstRow)

#### foundSetExcelWorkbook.headerStyle : [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

The style used for the header of the data

**Overrides**: [`headerStyle`](API-svyExcelUtils.md#ServoyExcelWorkbook+headerStyle)

#### foundSetExcelWorkbook.rowStyle : [`ExcelCellStyle`](API-svyExcelUtils.md#new\_ExcelCellStyle\_new)

The style used for a data cell

**Overrides**: [`rowStyle`](API-svyExcelUtils.md#ServoyExcelWorkbook+rowStyle)

#### foundSetExcelWorkbook.setAutoFilter : `Boolean`

Whether or not the data columns should be auto filtered or not

**Overrides**: [`setAutoFilter`](API-svyExcelUtils.md#ServoyExcelWorkbook+setAutoFilter)

#### foundSetExcelWorkbook.sheet : [`ExcelSheet`](API-svyExcelUtils.md#new\_ExcelSheet\_new)

The ExcelSheet used or created

#### foundSetExcelWorkbook.sheetName : `String`

The name of the sheet to be used

When a template is used, data will be inserted in the\
sheet with this name or the first best if not found

#### foundSetExcelWorkbook.startColumn : `Number`

The first column where data will be inserted (one based)

#### foundSetExcelWorkbook.startRow : `Number`

The first row where data will be inserted (one based)

#### foundSetExcelWorkbook.wb : `Packages.org.apache.poi.ss.usermodel.Workbook`

The internal workbook object

#### foundSetExcelWorkbook.workbook : [`ExcelWorkbook`](API-svyExcelUtils.md#excelworkbook)

The ExcelWorkbook created

#### new FoundSetExcelWorkbook(foundset, dataproviders, \[headers], \[templateOrFileType], \[sheetNameToUse])

A FoundSet based Excel workbook

| Param                 | Type                                          | Description                                                                                                                                      |
| --------------------- | --------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| foundset              | `JSFoundSet`                                  | the foundset                                                                                                                                     |
| dataproviders         | `[ 'Array' ].<String>`                        | the dataproviders to be used for the excel sheet                                                                                                 |
| \[headers]            | `[ 'Array' ].<String>`                        | the text to be used as column headers                                                                                                            |
| \[templateOrFileType] | `String` \| `plugins.file.JSFile` \| `Number` | either file or media URL pointing to an existing Excel to be used as template or one of the FILE\_FORMAT constants when creating empty workbooks |
| \[sheetNameToUse]     | `String`                                      | when a template is used, this is the name of the sheet to be filled                                                                              |

***

### ALIGNMENT : `enum`

Horizontal alignments used in ExcelCellStyle

**Properties**

| Name              | Type                                                       | Default                                                                     |
| ----------------- | ---------------------------------------------------------- | --------------------------------------------------------------------------- |
| CENTER            | `Packages.org.apache.poi.ss.usermodel.HorizontalAlignment` | `Packages.org.apache.poi.ss.usermodel.HorizontalAlignment.CENTER`           |
| CENTER\_SELECTION | `Packages.org.apache.poi.ss.usermodel.HorizontalAlignment` | `Packages.org.apache.poi.ss.usermodel.HorizontalAlignment.CENTER_SELECTION` |
| FILL              | `Packages.org.apache.poi.ss.usermodel.HorizontalAlignment` | `Packages.org.apache.poi.ss.usermodel.HorizontalAlignment.FILL`             |
| GENERAL           | `Packages.org.apache.poi.ss.usermodel.HorizontalAlignment` | `Packages.org.apache.poi.ss.usermodel.HorizontalAlignment.GENERAL`          |
| JUSTIFY           | `Packages.org.apache.poi.ss.usermodel.HorizontalAlignment` | `Packages.org.apache.poi.ss.usermodel.HorizontalAlignment.JUSTIFY`          |
| LEFT              | `Packages.org.apache.poi.ss.usermodel.HorizontalAlignment` | `Packages.org.apache.poi.ss.usermodel.HorizontalAlignment.LEFT`             |
| RIGHT             | `Packages.org.apache.poi.ss.usermodel.HorizontalAlignment` | `Packages.org.apache.poi.ss.usermodel.HorizontalAlignment.RIGHT`            |
| DISTRIBUTED       | `Packages.org.apache.poi.ss.usermodel.HorizontalAlignment` | `Packages.org.apache.poi.ss.usermodel.HorizontalAlignment.DISTRIBUTED`      |

***

### BORDER : `enum`

Borders used in ExcelCellStyle

**Properties**

| Name                   | Type                                               | Default                                                                |
| ---------------------- | -------------------------------------------------- | ---------------------------------------------------------------------- |
| DASH\_DOT              | `Packages.org.apache.poi.ss.usermodel.BorderStyle` | `Packages.org.apache.poi.ss.usermodel.BorderStyle.DASH_DOT`            |
| DASH\_DOT\_DOT         | `Packages.org.apache.poi.ss.usermodel.BorderStyle` | `Packages.org.apache.poi.ss.usermodel.BorderStyle.DASH_DOT_DOT`        |
| DASHED                 | `Packages.org.apache.poi.ss.usermodel.BorderStyle` | `Packages.org.apache.poi.ss.usermodel.BorderStyle.DASHED`              |
| DOTTED                 | `Packages.org.apache.poi.ss.usermodel.BorderStyle` | `Packages.org.apache.poi.ss.usermodel.BorderStyle.DOTTED`              |
| DOUBLE                 | `Packages.org.apache.poi.ss.usermodel.BorderStyle` | `Packages.org.apache.poi.ss.usermodel.BorderStyle.DOUBLE`              |
| HAIR                   | `Packages.org.apache.poi.ss.usermodel.BorderStyle` | `Packages.org.apache.poi.ss.usermodel.BorderStyle.HAIR`                |
| MEDIUM                 | `Packages.org.apache.poi.ss.usermodel.BorderStyle` | `Packages.org.apache.poi.ss.usermodel.BorderStyle.MEDIUM`              |
| MEDIUM\_DASH\_DOT      | `Packages.org.apache.poi.ss.usermodel.BorderStyle` | `Packages.org.apache.poi.ss.usermodel.BorderStyle.MEDIUM_DASH_DOT`     |
| MEDIUM\_DASH\_DOT\_DOT | `Packages.org.apache.poi.ss.usermodel.BorderStyle` | `Packages.org.apache.poi.ss.usermodel.BorderStyle.MEDIUM_DASH_DOT_DOT` |
| MEDIUM\_DASHED         | `Packages.org.apache.poi.ss.usermodel.BorderStyle` | `Packages.org.apache.poi.ss.usermodel.BorderStyle.MEDIUM_DASHED`       |
| NONE                   | `Packages.org.apache.poi.ss.usermodel.BorderStyle` | `Packages.org.apache.poi.ss.usermodel.BorderStyle.NONE`                |
| SLANTED\_DASH\_DOT     | `Packages.org.apache.poi.ss.usermodel.BorderStyle` | `Packages.org.apache.poi.ss.usermodel.BorderStyle.SLANTED_DASH_DOT`    |
| THICK                  | `Packages.org.apache.poi.ss.usermodel.BorderStyle` | `Packages.org.apache.poi.ss.usermodel.BorderStyle.THICK`               |
| THIN                   | `Packages.org.apache.poi.ss.usermodel.BorderStyle` | `Packages.org.apache.poi.ss.usermodel.BorderStyle.THIN`                |

***

### CELL\_TYPE

Possible cell types

**Properties**

| Name    | Default                                                 |
| ------- | ------------------------------------------------------- |
| BLANK   | `Packages.org.apache.poi.ss.usermodel.CellType.BLANK`   |
| BOOLEAN | `Packages.org.apache.poi.ss.usermodel.CellType.BOOLEAN` |
| ERROR   | `Packages.org.apache.poi.ss.usermodel.CellType.ERROR`   |
| FORMULA | `Packages.org.apache.poi.ss.usermodel.CellType.FORMULA` |
| NUMERIC | `Packages.org.apache.poi.ss.usermodel.CellType.NUMERIC` |
| STRING  | `Packages.org.apache.poi.ss.usermodel.CellType.STRING`  |

***

### FILE\_FORMAT

Possible file formats used instead of templates when creating empty workbooks

**Properties**

| Name  | Default | Description                                                                              |
| ----- | ------- | ---------------------------------------------------------------------------------------- |
| XLS   | `1`     | XLS format                                                                               |
| XLSX  | `2`     | XLSX format, requires additional libraries @see [ExcelUtils.md](ExcelUtils.md "mention") |
| SXLSX | `4`     | Streaming version of the XLSX format to avoid out of memory errors                       |



***

### FILL\_PATTERN : `enum`

Fill patterns used in ExcelCellStyle

**Properties**

| Name                  | Type                                                   | Default                                                                    |
| --------------------- | ------------------------------------------------------ | -------------------------------------------------------------------------- |
| NO\_FILL              | `Packages.org.apache.poi.ss.usermodel.FillPatternType` | `Packages.org.apache.poi.ss.usermodel.FillPatternType.NO_FILL`             |
| SOLID\_FOREGROUND     | `Packages.org.apache.poi.ss.usermodel.FillPatternType` | `Packages.org.apache.poi.ss.usermodel.FillPatternType.SOLID_FOREGROUND`    |
| FINE\_DOTS            | `Packages.org.apache.poi.ss.usermodel.FillPatternType` | `Packages.org.apache.poi.ss.usermodel.FillPatternType.FINE_DOTS`           |
| ALT\_BARS             | `Packages.org.apache.poi.ss.usermodel.FillPatternType` | `Packages.org.apache.poi.ss.usermodel.FillPatternType.ALT_BARS`            |
| SPARSE\_DOTS          | `Packages.org.apache.poi.ss.usermodel.FillPatternType` | `Packages.org.apache.poi.ss.usermodel.FillPatternType.SPARSE_DOTS`         |
| THICK\_HORZ\_BANDS    | `Packages.org.apache.poi.ss.usermodel.FillPatternType` | `Packages.org.apache.poi.ss.usermodel.FillPatternType.THICK_HORZ_BANDS`    |
| THICK\_VERT\_BANDS    | `Packages.org.apache.poi.ss.usermodel.FillPatternType` | `Packages.org.apache.poi.ss.usermodel.FillPatternType.THICK_VERT_BANDS`    |
| THICK\_BACKWARD\_DIAG | `Packages.org.apache.poi.ss.usermodel.FillPatternType` | `Packages.org.apache.poi.ss.usermodel.FillPatternType.THICK_BACKWARD_DIAG` |
| THICK\_FORWARD\_DIAG  | `Packages.org.apache.poi.ss.usermodel.FillPatternType` | `Packages.org.apache.poi.ss.usermodel.FillPatternType.THICK_FORWARD_DIAG`  |
| BIG\_SPOTS            | `Packages.org.apache.poi.ss.usermodel.FillPatternType` | `Packages.org.apache.poi.ss.usermodel.FillPatternType.BIG_SPOTS`           |
| BRICKS                | `Packages.org.apache.poi.ss.usermodel.FillPatternType` | `Packages.org.apache.poi.ss.usermodel.FillPatternType.BRICKS`              |
| THIN\_HORZ\_BANDS     | `Packages.org.apache.poi.ss.usermodel.FillPatternType` | `Packages.org.apache.poi.ss.usermodel.FillPatternType.THICK_HORZ_BANDS`    |
| THIN\_VERT\_BANDS     | `Packages.org.apache.poi.ss.usermodel.FillPatternType` | `Packages.org.apache.poi.ss.usermodel.FillPatternType.THICK_VERT_BANDS`    |
| THIN\_BACKWARD\_DIAG  | `Packages.org.apache.poi.ss.usermodel.FillPatternType` | `Packages.org.apache.poi.ss.usermodel.FillPatternType.THICK_FORWARD_DIAG`  |
| THIN\_FORWARD\_DIAG   | `Packages.org.apache.poi.ss.usermodel.FillPatternType` | `Packages.org.apache.poi.ss.usermodel.FillPatternType.THICK_FORWARD_DIAG`  |
| SQUARES               | `Packages.org.apache.poi.ss.usermodel.FillPatternType` | `Packages.org.apache.poi.ss.usermodel.FillPatternType.SQUARES`             |
| DIAMONDS              | `Packages.org.apache.poi.ss.usermodel.FillPatternType` | `Packages.org.apache.poi.ss.usermodel.FillPatternType.DIAMONDS`            |

***

### FONT\_UNDERLINE

Underline patterns used in ExcelFont

**Properties**

| Name               | Default                                                               |
| ------------------ | --------------------------------------------------------------------- |
| DOUBLE             | `Packages.org.apache.poi.hssf.usermodel.HSSFFont.U_DOUBLE`            |
| DOUBLE\_ACCOUNTING | `Packages.org.apache.poi.hssf.usermodel.HSSFFont.U_DOUBLE_ACCOUNTING` |
| NONE               | `Packages.org.apache.poi.hssf.usermodel.HSSFFont.U_NONE`              |
| SINGLE             | `Packages.org.apache.poi.hssf.usermodel.HSSFFont.U_SINGLE`            |
| SINGLE\_ACCOUNTING | `Packages.org.apache.poi.hssf.usermodel.HSSFFont.U_SINGLE_ACCOUNTING` |

***

### INDEXED\_COLOR : `enum`

Colors from the Excel color palette

**Properties**

| Name                    | Type                                                 | Default                                                                    |
| ----------------------- | ---------------------------------------------------- | -------------------------------------------------------------------------- |
| AQUA                    | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.AQUA`                  |
| BLACK                   | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.BLACK`                 |
| BLUE                    | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.BLUE`                  |
| BLUE\_GREY              | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.BLUE_GREY`             |
| BRIGHT\_GREEN           | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.BRIGHT_GREEN`          |
| BROWN                   | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.BROWN`                 |
| CORAL                   | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.CORAL`                 |
| CORNFLOWER\_BLUE        | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.CORNFLOWER_BLUE`       |
| DARK\_BLUE              | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.DARK_BLUE`             |
| DARK\_GREEN             | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.DARK_GREEN`            |
| DARK\_RED               | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.DARK_RED`              |
| DARK\_TEAL              | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.DARK_TEAL`             |
| DARK\_YELLOW            | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.DARK_YELLOW`           |
| GOLD                    | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.GOLD`                  |
| GREEN                   | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.GREEN`                 |
| GREY\_25\_PERCENT       | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.GREY_25_PERCENT`       |
| GREY\_40\_PERCENT       | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.GREY_40_PERCENT`       |
| GREY\_50\_PERCENT       | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.GREY_50_PERCENT`       |
| GREY\_80\_PERCENT       | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.GREY_80_PERCENT`       |
| INDIGO                  | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.INDIGO`                |
| LAVENDER                | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.LAVENDER`              |
| LEMON\_CHIFFON          | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.LEMON_CHIFFON`         |
| LIGHT\_BLUE             | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.LIGHT_BLUE`            |
| LIGHT\_CORNFLOWER\_BLUE | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.LIGHT_CORNFLOWER_BLUE` |
| LIGHT\_GREEN            | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.LIGHT_GREEN`           |
| LIGHT\_ORANGE           | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.LIGHT_ORANGE`          |
| LIGHT\_TURQUOISE        | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.LIGHT_TURQUOISE`       |
| LIGHT\_YELLOW           | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.LIGHT_YELLOW`          |
| LIME                    | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.LIME`                  |
| MAROON                  | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.MAROON`                |
| OLIVE\_GREEN            | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.OLIVE_GREEN`           |
| ORANGE                  | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.ORANGE`                |
| ORCHID                  | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.ORCHID`                |
| PALE\_BLUE              | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.PALE_BLUE`             |
| PINK                    | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.PINK`                  |
| PLUM                    | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.PLUM`                  |
| RED                     | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.RED`                   |
| ROSE                    | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.ROSE`                  |
| ROYAL\_BLUE             | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.ROYAL_BLUE`            |
| SEA\_GREEN              | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.SEA_GREEN`             |
| SKY\_BLUE               | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.SKY_BLUE`              |
| TAN                     | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.TAN`                   |
| TEAL                    | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.TEAL`                  |
| TURQUOISE               | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.TURQUOISE`             |
| VIOLET                  | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.VIOLET`                |
| WHITE                   | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.WHITE`                 |
| YELLOW                  | `Packages.org.apache.poi.ss.usermodel.IndexedColors` | `Packages.org.apache.poi.ss.usermodel.IndexedColors.YELLOW`                |

***

### PAPER\_SIZE

Possible paper sizes for a PrintSetup

**Properties**

| Name                             | Default                                                                         |
| -------------------------------- | ------------------------------------------------------------------------------- |
| A3\_PAPERSIZE                    | `Packages.org.apache.poi.ss.usermodel.PrintSetup.A3_PAPERSIZE`                  |
| A4\_EXTRA\_PAPERSIZE             | `Packages.org.apache.poi.ss.usermodel.PrintSetup.A4_EXTRA_PAPERSIZE`            |
| A4\_PAPERSIZE                    | `Packages.org.apache.poi.ss.usermodel.PrintSetup.A4_PAPERSIZE`                  |
| A4\_PLUS\_PAPERSIZE              | `Packages.org.apache.poi.ss.usermodel.PrintSetup.A4_PLUS_PAPERSIZE`             |
| A4\_ROTATED\_PAPERSIZE           | `Packages.org.apache.poi.ss.usermodel.PrintSetup.A4_ROTATED_PAPERSIZE`          |
| A4\_SMALL\_PAPERSIZE             | `Packages.org.apache.poi.ss.usermodel.PrintSetup.A4_SMALL_PAPERSIZE`            |
| A4\_TRANSVERSE\_PAPERSIZE        | `Packages.org.apache.poi.ss.usermodel.PrintSetup.A4_TRANSVERSE_PAPERSIZE`       |
| A5\_PAPERSIZE                    | `Packages.org.apache.poi.ss.usermodel.PrintSetup.A5_PAPERSIZE`                  |
| B4\_PAPERSIZE                    | `Packages.org.apache.poi.ss.usermodel.PrintSetup.B4_PAPERSIZE`                  |
| B5\_PAPERSIZE                    | `Packages.org.apache.poi.ss.usermodel.PrintSetup.B5_PAPERSIZE`                  |
| ELEVEN\_BY\_SEVENTEEN\_PAPERSIZE | `Packages.org.apache.poi.ss.usermodel.PrintSetup.ELEVEN_BY_SEVENTEEN_PAPERSIZE` |
| ENVELOPE\_10\_PAPERSIZE          | `Packages.org.apache.poi.ss.usermodel.PrintSetup.ENVELOPE_10_PAPERSIZE`         |
| ENVELOPE\_9\_PAPERSIZE           | `Packages.org.apache.poi.ss.usermodel.PrintSetup.ENVELOPE_9_PAPERSIZE`          |
| ENVELOPE\_C3\_PAPERSIZE          | `Packages.org.apache.poi.ss.usermodel.PrintSetup.ENVELOPE_C3_PAPERSIZE`         |
| ENVELOPE\_C4\_PAPERSIZE          | `Packages.org.apache.poi.ss.usermodel.PrintSetup.ENVELOPE_C4_PAPERSIZE`         |
| ENVELOPE\_C5\_PAPERSIZE          | `Packages.org.apache.poi.ss.usermodel.PrintSetup.ENVELOPE_C5_PAPERSIZE`         |
| ENVELOPE\_C6\_PAPERSIZE          | `Packages.org.apache.poi.ss.usermodel.PrintSetup.ENVELOPE_C6_PAPERSIZE`         |
| ENVELOPE\_CS\_PAPERSIZE          | `Packages.org.apache.poi.ss.usermodel.PrintSetup.ENVELOPE_CS_PAPERSIZE`         |
| ENVELOPE\_DL\_PAPERSIZE          | `Packages.org.apache.poi.ss.usermodel.PrintSetup.ENVELOPE_DL_PAPERSIZE`         |
| ENVELOPE\_MONARCH\_PAPERSIZE     | `Packages.org.apache.poi.ss.usermodel.PrintSetup.ENVELOPE_MONARCH_PAPERSIZE`    |
| EXECUTIVE\_PAPERSIZE             | `Packages.org.apache.poi.ss.usermodel.PrintSetup.EXECUTIVE_PAPERSIZE`           |
| FOLIO8\_PAPERSIZE                | `Packages.org.apache.poi.ss.usermodel.PrintSetup.FOLIO8_PAPERSIZE`              |
| LEDGER\_PAPERSIZE                | `Packages.org.apache.poi.ss.usermodel.PrintSetup.LEDGER_PAPERSIZE`              |
| LEGAL\_PAPERSIZE                 | `Packages.org.apache.poi.ss.usermodel.PrintSetup.LEGAL_PAPERSIZE`               |
| LETTER\_PAPERSIZE                | `Packages.org.apache.poi.ss.usermodel.PrintSetup.LETTER_PAPERSIZE`              |
| LETTER\_ROTATED\_PAPERSIZE       | `Packages.org.apache.poi.ss.usermodel.PrintSetup.LETTER_ROTATED_PAPERSIZE`      |
| LETTER\_SMALL\_PAGESIZE          | `Packages.org.apache.poi.ss.usermodel.PrintSetup.LETTER_SMALL_PAGESIZE`         |
| NOTE8\_PAPERSIZE                 | `Packages.org.apache.poi.ss.usermodel.PrintSetup.NOTE8_PAPERSIZE`               |
| PRINTER\_DEFAULT\_PAPERSIZE      | `Packages.org.apache.poi.ss.usermodel.PrintSetup.PRINTER_DEFAULT_PAPERSIZE`     |
| QUARTO\_PAPERSIZE                | `Packages.org.apache.poi.ss.usermodel.PrintSetup.QUARTO_PAPERSIZE`              |
| STATEMENT\_PAPERSIZE             | `Packages.org.apache.poi.ss.usermodel.PrintSetup.STATEMENT_PAPERSIZE`           |
| TABLOID\_PAPERSIZE               | `Packages.org.apache.poi.ss.usermodel.PrintSetup.TABLOID_PAPERSIZE`             |
| TEN\_BY\_FOURTEEN\_PAPERSIZE     | `Packages.org.apache.poi.ss.usermodel.PrintSetup.TEN_BY_FOURTEEN_PAPERSIZE`     |

***

### SHEET\_PANE : `enum`

Panes of a sheet used in split panes

**Properties**

| Name         | Type   | Default                                                       |
| ------------ | ------ | ------------------------------------------------------------- |
| LOWER\_RIGHT | `byte` | `Packages.org.apache.poi.ss.usermodel.Sheet.PANE_LOWER_RIGHT` |
| LOWER\_LEFT  | `byte` | `Packages.org.apache.poi.ss.usermodel.Sheet.PANE_LOWER_LEFT`  |
| UPPER\_LEFT  | `byte` | `Packages.org.apache.poi.ss.usermodel.Sheet.PANE_UPPER_LEFT`  |
| UPPER\_RIGHT | `byte` | `Packages.org.apache.poi.ss.usermodel.Sheet.PANE_UPPER_RIGHT` |

***

### VERTICAL\_ALIGNMENT : `enum`

Vertical alignments used in ExcelCellStyle

**Properties**

| Name        | Type                                                     | Default                                                              |
| ----------- | -------------------------------------------------------- | -------------------------------------------------------------------- |
| BOTTOM      | `Packages.org.apache.poi.ss.usermodel.VerticalAlignment` | `Packages.org.apache.poi.ss.usermodel.VerticalAlignment.BOTTOM`      |
| CENTER      | `Packages.org.apache.poi.ss.usermodel.VerticalAlignment` | `Packages.org.apache.poi.ss.usermodel.VerticalAlignment.CENTER`      |
| JUSTIFY     | `Packages.org.apache.poi.ss.usermodel.VerticalAlignment` | `Packages.org.apache.poi.ss.usermodel.VerticalAlignment.JUSTIFY`     |
| TOP         | `Packages.org.apache.poi.ss.usermodel.VerticalAlignment` | `Packages.org.apache.poi.ss.usermodel.VerticalAlignment.TOP`         |
| DISTRIBUTED | `Packages.org.apache.poi.ss.usermodel.VerticalAlignment` | `Packages.org.apache.poi.ss.usermodel.VerticalAlignment.DISTRIBUTED` |



### createPrintSetup() ⇒ `PrintSetup`

Creates a PrintSetup object that can be used in ExcelSheet.setPrintSetup() or to set the default print setup used when workbooks are created from FoundSet or DataSet

### createWorkbook(\[templateOrFileType]) ⇒ [`ExcelWorkbook`](API-svyExcelUtils.md#excelworkbook)

Returns an empty ExcelWorkbook

| Param                 | Type                                                            | Description                                                                                                  |
| --------------------- | --------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| \[templateOrFileType] | `String` \| `plugins.file.JSFile` \| `Number` \| `Array.<byte>` | either an existing Excel file as template or one of the FILE\_FORMAT constants when creating empty workbooks |

**Example**

```js
// Create workbook and sheet
var workbook = scopes.svyExcelUtils.createWorkbook(scopes.svyExcelUtils.FILE_FORMAT.XLSX);
var sheet = workbook.createSheet("Test");

// Create style for the header
var headerStyle = workbook.createCellStyle();
headerStyle
   .setFont("Arial,1,12")
   .setFillPattern(scopes.svyExcelUtils.FILL_PATTERN.SOLID_FOREGROUND)
   .setFillForegroundColor(scopes.svyExcelUtils.INDEXED_COLOR.LIGHT_ORANGE)
   .setAlignment(scopes.svyExcelUtils.ALIGNMENT.CENTER);

var rowNum = 1;

// Create header row and cells
var row = sheet.createRow(rowNum ++);
var cell = row.createCell(1);
cell.setCellValue("Test 1", headerStyle);

cell = row.createCell(2);
cell.setCellValue("Test 2", headerStyle);

// Create some data and write to the sheet
var data = [[10, 35], [15, 47], [9, 22], [10, 33]];
for (var i = 0; i < data.length; i++) {
   row = sheet.createRow(rowNum ++);
   row.createCell(1).setCellValue(data[i][0]);
   row.createCell(2).setCellValue(data[i][1]);
}

// Create a style for the sum
var sumStyle = workbook.createCellStyle();
// Clone the default font, so we won't be changing the default
var font = sumStyle.cloneFont();
font.underline = scopes.svyExcelUtils.FONT_UNDERLINE.DOUBLE_ACCOUNTING;
font.isBold = true;

// Create formula cells at the bottom
row = sheet.createRow(rowNum ++);
cell = row.createCell(1);
cell.setCellStyle(sumStyle);
cell.setCellFormula("SUM(" + scopes.svyExcelUtils.getCellReferenceFromRange(2, 1 + data.length, 1, 1) + ")");

cell = row.createCell(2);
cell.setCellStyle(sumStyle);
cell.setCellFormula("SUM(" + scopes.svyExcelUtils.getCellReferenceFromRange(2, 1 + data.length, 2, 2) + ")");

// Write to file
var success = workbook.writeToFile("d:\\test.xls");
```

### createWorkbookFromDataSet(dataset, \[columns], \[headers], \[templateOrFileType], \[sheetNameToUse]) ⇒ [`DataSetExcelWorkbook`](API-svyExcelUtils.md#datasetexcelworkbook-servoyexcelworkbook)

Creates an ExcelWorkbook from the given dataset

If a template is provided, the dataset will be inserted in the given sheet

| Param                 | Type                                          | Description                                                                                                                                      |
| --------------------- | --------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| dataset               | `JSDataSet`                                   | the dataset                                                                                                                                      |
| \[columns]            | `[ 'Array' ].<Number>`                        | the column numbers to be included in the sheet                                                                                                   |
| \[headers]            | `[ 'Array' ].<String>`                        | the text to be used as column headers                                                                                                            |
| \[templateOrFileType] | `String` \| `plugins.file.JSFile` \| `Number` | either file or media URL pointing to an existing Excel to be used as template or one of the FILE\_FORMAT constants when creating empty workbooks |
| \[sheetNameToUse]     | `String`                                      | when a template is used, this is the name of the sheet to be filled                                                                              |

### createWorkbookFromFoundSet(foundset, dataproviders, \[headers], \[templateOrFileType], \[sheetNameToUse]) ⇒ [`FoundSetExcelWorkbook`](API-svyExcelUtils.md#foundsetexcelworkbook-servoyexcelworkbook)

Creates an ExcelWorkbook from the given foundset

If a templateOrFileType is provided, the foundset will be inserted in the given sheet

| Param                 | Type                                          | Description                                                                                                                                                |
| --------------------- | --------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| foundset              | `JSFoundSet`                                  | the foundset                                                                                                                                               |
| dataproviders         | `[ 'Array' ].<String>`                        | the dataproviders to be used for the excel sheet                                                                                                           |
| \[headers]            | `[ 'Array' ].<String>`                        | the text to be used as column headers                                                                                                                      |
| \[templateOrFileType] | `String` \| `plugins.file.JSFile` \| `Number` | either file or media URL pointing to an existing Excel to be used as templateOrFileType or one of the FILE\_FORMAT constants when creating empty workbooks |
| \[sheetNameToUse]     | `String`                                      | when a template is used, this is the name of the sheet to be filled                                                                                        |

### getCellReferenceFromRange(firstRow, lastRow, firstColumn, lastColumn) ⇒ `String`

Creates a cell reference (e.g. "A4:C92") from the given range

**Returns**: `String` - cellReference

| Param       | Type     |
| ----------- | -------- |
| firstRow    | `Number` |
| lastRow     | `Number` |
| firstColumn | `Number` |
| lastColumn  | `Number` |

### getRangeFromCellReference(cellReference) ⇒ `Object`

Converts a cell reference (e.g. "B4:AK234" or "C6") to an object holding first and last row and column

| Param         | Type     |
| ------------- | -------- |
| cellReference | `String` |

### getWorkbook(original) ⇒ [`ExcelWorkbook`](API-svyExcelUtils.md#excelworkbook)

Returns an ExcelWorkbook from the given file or media URL

| Param    | Type                                                | Description                         |
| -------- | --------------------------------------------------- | ----------------------------------- |
| original | `String` \| `plugins.file.JSFile` \| `Array.<byte>` | path to the file, file or media URL |

### isLoaded() ⇒ `Boolean`

If true, all required libraries are present and the scope can be used

### set()

### setDefaultPrintSetup(setup)

Sets the default print setup used when workbooks are created from FoundSet or DataSet

| Param | Type         |
| ----- | ------------ |
| setup | `PrintSetup` |

### copies : `Number`

The number of copies

### draft : `Boolean`

Whether it is in draft mode

### fitHeight : `Number`

The number of pages high to fit the sheet in

### fitWidth : `Number`

The number of pages high to fit the sheet in

### landscape : `Boolean`

Whether to print in landscape

### mergedRegionType : `Object`

### noColor : `Boolean`

Whether it is black and white

### paperSize : `Number`

The paper size

***
