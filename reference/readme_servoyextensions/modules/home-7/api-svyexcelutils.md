# Full API Reference

### Classes

[DataSetExcelWorkbook](api-svyexcelutils.md#datasetexcelworkbook-servoyexcelworkbook) ⇐ [`ServoyExcelWorkbook`](api-svyexcelutils.md#new\_ServoyExcelWorkbook\_new)

[ExcelWorkbook](api-svyexcelutils.md#excelworkbook)

[FoundSetExcelWorkbook](api-svyexcelutils.md#foundsetexcelworkbook-servoyexcelworkbook) ⇐ [`ServoyExcelWorkbook`](api-svyexcelutils.md#new\_ServoyExcelWorkbook\_new)

### Members

[copies](api-svyexcelutils.md#copies-number) : `Number`

The number of copies

[draft](api-svyexcelutils.md#draft-boolean) : `Boolean`

Whether it is in draft mode

[fitHeight](api-svyexcelutils.md#fitheight-number) : `Number`

The number of pages high to fit the sheet in

[fitWidth](api-svyexcelutils.md#fitwidth-number) : `Number`

The number of pages high to fit the sheet in

[landscape](api-svyexcelutils.md#landscape-boolean) : `Boolean`

Whether to print in landscape

[mergedRegionType](api-svyexcelutils.md#mergedregiontype-object) : `Object`

[noColor](api-svyexcelutils.md#nocolor-boolean) : `Boolean`

Whether it is black and white

[paperSize](api-svyexcelutils.md#papersize-number) : `Number`

The paper size

### Functions

[createPrintSetup()](api-svyexcelutils.md#createprintsetup-printsetup) ⇒ `PrintSetup`

Creates a PrintSetup object that can be used in ExcelSheet.setPrintSetup() or to set the default print setup used when workbooks are created from FoundSet or DataSet

[createWorkbook(\[templateOrFileType\])](api-svyexcelutils.md#createworkbook-templateorfiletype-excelworkbook) ⇒ [`ExcelWorkbook`](api-svyexcelutils.md#ExcelWorkbook)

Returns an empty ExcelWorkbook

[createWorkbookFromDataSet(dataset, \[columns\], \[headers\], \[templateOrFileType\], \[sheetNameToUse\])](api-svyexcelutils.md#createworkbookfromdataset-dataset-columns-headers-templateorfiletype-sheetnametouse-datasetexcelwork) ⇒ [`DataSetExcelWorkbook`](api-svyexcelutils.md#datasetexcelworkbook-servoyexcelworkbook)

Creates an ExcelWorkbook from the given dataset

If a template is provided, the dataset will be inserted in the given sheet

[createWorkbookFromFoundSet(foundset, dataproviders, \[headers\], \[templateOrFileType\], \[sheetNameToUse\])](api-svyexcelutils.md#createworkbookfromfoundset-foundset-dataproviders-headers-templateorfiletype-sheetnametouse-foundset) ⇒ [`FoundSetExcelWorkbook`](api-svyexcelutils.md#foundsetexcelworkbook-servoyexcelworkbook)

Creates an ExcelWorkbook from the given foundset

If a templateOrFileType is provided, the foundset will be inserted in the given sheet

[getCellReferenceFromRange(firstRow, lastRow, firstColumn, lastColumn)](api-svyexcelutils.md#getcellreferencefromrange-firstrow-lastrow-firstcolumn-lastcolumn-string) ⇒ `String`

Creates a cell reference (e.g. "A4:C92") from the given range

[getRangeFromCellReference(cellReference)](api-svyexcelutils.md#getrangefromcellreference-cellreference-object) ⇒ `Object`

Converts a cell reference (e.g. "B4:AK234" or "C6") to an object holding first and last row and column

[getWorkbook(original)](api-svyexcelutils.md#getworkbook-original-excelworkbook) ⇒ [`ExcelWorkbook`](api-svyexcelutils.md#ExcelWorkbook)

Returns an ExcelWorkbook from the given file or media URL

[isLoaded()](api-svyexcelutils.md#isloaded-boolean) ⇒ `Boolean`

If true, all required libraries are present and the scope can be used

[set()](api-svyexcelutils.md#set)

[setDefaultPrintSetup(setup)](api-svyexcelutils.md#setdefaultprintsetup-setup)

Sets the default print setup used when workbooks are created from FoundSet or DataSet

### DataSetExcelWorkbook ⇐ [`ServoyExcelWorkbook`](api-svyexcelutils.md#new\_ServoyExcelWorkbook\_new)

**Extends**: [`ServoyExcelWorkbook`](api-svyexcelutils.md#new\_ServoyExcelWorkbook\_new)

* [DataSetExcelWorkbook](api-svyexcelutils.md#datasetexcelworkbook-servoyexcelworkbook) ⇐ [`ServoyExcelWorkbook`](api-svyexcelutils.md#new\_ServoyExcelWorkbook\_new)
  * _inner_
    * [\~dataFilled](api-svyexcelutils.md#datasetexcelworkbook-datafilled-boolean) : `Boolean`
  * _instance_
    * [.cloneCellStyle(cellStyle)](api-svyexcelutils.md#datasetexcelworkbook.clonecellstyle-cellstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
    * [.cloneFont(font)](api-svyexcelutils.md#datasetexcelworkbook.clonefont-font-excelfont) ⇒ [`ExcelFont`](api-svyexcelutils.md#new\_ExcelFont\_new)
    * [.cloneSheet(indexToClone)](api-svyexcelutils.md#datasetexcelworkbook.clonesheet-indextoclone-excelsheet) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)
    * [.close()](api-svyexcelutils.md#datasetexcelworkbook.close)
    * [.createCellStyle()](api-svyexcelutils.md#datasetexcelworkbook.createcellstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
    * [.createColumnStyle(columnIndex)](api-svyexcelutils.md#datasetexcelworkbook.createcolumnstyle-columnindex-excelcellstyle) ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
    * [.createFont()](api-svyexcelutils.md#datasetexcelworkbook.createfont-excelfont) ⇒ [`ExcelFont`](api-svyexcelutils.md#new\_ExcelFont\_new)
    * [.createHeaderStyle()](api-svyexcelutils.md#datasetexcelworkbook.createheaderstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
    * [.createRowStyle()](api-svyexcelutils.md#datasetexcelworkbook.createrowstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
    * [.createSheet(sheetName)](api-svyexcelutils.md#datasetexcelworkbook.createsheet-sheetname-excelsheet) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)
    * [.fillData()](api-svyexcelutils.md#datasetexcelworkbook.filldata)
    * [.getBytes()](api-svyexcelutils.md#datasetexcelworkbook.getbytes-array-.less-than-byte-greater-than) ⇒ `[ 'Array' ].<byte>`
    * [.getDataSet()](api-svyexcelutils.md#datasetexcelworkbook.getdataset-jsdataset) ⇒ `JSDataSet`
    * [.getNumberOfSheets()](api-svyexcelutils.md#datasetexcelworkbook.getnumberofsheets-number) ⇒ `Number`
    * [.getSheet(sheetName)](api-svyexcelutils.md#datasetexcelworkbook.getsheet-sheetname-excelsheet) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)
    * [.getSheetAt(index)](api-svyexcelutils.md#datasetexcelworkbook.getsheetat-index-excelsheet) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)
    * [.getSheetNameAt(index)](api-svyexcelutils.md#datasetexcelworkbook.getsheetnameat-index-string) ⇒ `String`
    * [.getSheetNames()](api-svyexcelutils.md#datasetexcelworkbook.getsheetnames-array-.less-than-string-greater-than) ⇒ `[ 'Array' ].<String>`
    * [.removeSheetAt(index)](api-svyexcelutils.md#datasetexcelworkbook.removesheetat-index)
    * [.setFormatForColumn(columnIndex, format)](api-svyexcelutils.md#datasetexcelworkbook.setformatforcolumn-columnindex-format)
    * [.setSheetNameAt(index, name)](api-svyexcelutils.md#datasetexcelworkbook.setsheetnameat-index-name)
    * [.writeToFile(targetFile)](api-svyexcelutils.md#datasetexcelworkbook.writetofile-targetfile-boolean) ⇒ `Boolean`
    * [.autoSizeColumns](api-svyexcelutils.md#datasetexcelworkbook.autosizecolumns-boolean) : `Boolean`
    * [.columnFormats](api-svyexcelutils.md#datasetexcelworkbook.columnformats-array-.less-than-string-greater-than) : `[ 'Array' ].<String>`
    * [.columnStyles](api-svyexcelutils.md#datasetexcelworkbook.columnstyles-array-.less-than-excelcellstyle-greater-than) : [`[ 'Array' ].<ExcelCellStyle>`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
    * [.dataset](api-svyexcelutils.md#datasetexcelworkbook.dataset-jsdataset) : `JSDataSet`
    * [.defaultDateFormat](api-svyexcelutils.md#datasetexcelworkbook.defaultdateformat-string) : `String`
    * [.defaultNumberFormat](api-svyexcelutils.md#datasetexcelworkbook.defaultnumberformat-string) : `String`
    * [.freezeFirstRow](api-svyexcelutils.md#datasetexcelworkbook.freezefirstrow-boolean) : `Boolean`
    * [.headerStyle](api-svyexcelutils.md#datasetexcelworkbook.headerstyle-excelcellstyle) : [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
    * [.rowStyle](api-svyexcelutils.md#datasetexcelworkbook.rowstyle-excelcellstyle) : [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
    * [.setAutoFilter](api-svyexcelutils.md#datasetexcelworkbook.setautofilter-boolean) : `Boolean`
    * [.sheet](api-svyexcelutils.md#datasetexcelworkbook.sheet-excelsheet) : [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)
    * [.sheetName](api-svyexcelutils.md#datasetexcelworkbook.sheetname-string) : `String`
    * [.startColumn](api-svyexcelutils.md#datasetexcelworkbook.startcolumn-number) : `Number`
    * [.startRow](api-svyexcelutils.md#datasetexcelworkbook.startrow-number) : `Number`
    * [.wb](api-svyexcelutils.md#datasetexcelworkbook.wb-packages.org.apache.poi.ss.usermodel.workbook) : `Packages.org.apache.poi.ss.usermodel.Workbook`
    * [.workbook](api-svyexcelutils.md#datasetexcelworkbook.workbook-excelworkbook) : [`ExcelWorkbook`](api-svyexcelutils.md#ExcelWorkbook)
  * [new DataSetExcelWorkbook(dataset, \[columns\], \[headers\], \[templateOrFileType\], \[sheetNameToUse\])](api-svyexcelutils.md#new-datasetexcelworkbook-dataset-columns-headers-templateorfiletype-sheetnametouse)

#### DataSetExcelWorkbook\~dataFilled : `Boolean`

#### dataSetExcelWorkbook.cloneCellStyle(cellStyle) ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

Clones the given ExcelCellStyle

| Param     | Type                                                              |
| --------- | ----------------------------------------------------------------- |
| cellStyle | [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new) |

#### dataSetExcelWorkbook.cloneFont(font) ⇒ [`ExcelFont`](api-svyexcelutils.md#new\_ExcelFont\_new)

Clones the given font and returns a new ExcelFont

| Param | Type                                                    |
| ----- | ------------------------------------------------------- |
| font  | [`ExcelFont`](api-svyexcelutils.md#new\_ExcelFont\_new) |

#### dataSetExcelWorkbook.cloneSheet(indexToClone) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)

Creates an ExcelSheet from an existing sheet in the Workbook

**Returns**: [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new) - clone

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| indexToClone | `Number` | one based   |

#### dataSetExcelWorkbook.close()

Closes this workbook

#### dataSetExcelWorkbook.createCellStyle() ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

Creates an empty ExcelCellStyle

#### dataSetExcelWorkbook.createColumnStyle(columnIndex) ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

Creates and returns an ExcelCellStyle used for a specific column

| Param       | Type     |
| ----------- | -------- |
| columnIndex | `Number` |

#### dataSetExcelWorkbook.createFont() ⇒ [`ExcelFont`](api-svyexcelutils.md#new\_ExcelFont\_new)

Creates a font

#### dataSetExcelWorkbook.createHeaderStyle() ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

Creates and returns an ExcelCellStyle used for the header row

#### dataSetExcelWorkbook.createRowStyle() ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

Creates and returns an ExcelCellStyle used for a data row

#### dataSetExcelWorkbook.createSheet(sheetName) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)

Creates a sheet with the given name

This method makes sure that no illegal names are provided and might change the name if needed

| Param     | Type     |
| --------- | -------- |
| sheetName | `String` |

#### dataSetExcelWorkbook.fillData()

Fills the sheet with the data of the foundset

This is automatically done when `writeToFile()` or `getBytes()` is called

**Overrides**: [`fillData`](api-svyexcelutils.md#ServoyExcelWorkbook+fillData)

#### dataSetExcelWorkbook.getBytes() ⇒ `[ 'Array' ].<byte>`

Returns the data of this workbook as a byte\[]

**Returns**: `[ 'Array' ].<byte>` - bytes

#### dataSetExcelWorkbook.getDataSet() ⇒ `JSDataSet`

Returns the dataset used to create this workbook

#### dataSetExcelWorkbook.getNumberOfSheets() ⇒ `Number`

Returns the number of spreadsheets in the workbook

#### dataSetExcelWorkbook.getSheet(sheetName) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)

Returns the sheet with the given name (case insensitive match)

| Param     | Type     |
| --------- | -------- |
| sheetName | `String` |

#### dataSetExcelWorkbook.getSheetAt(index) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)

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

#### dataSetExcelWorkbook.columnStyles : [`[ 'Array' ].<ExcelCellStyle>`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

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

**Overrides**: [`freezeFirstRow`](api-svyexcelutils.md#ServoyExcelWorkbook+freezeFirstRow)

#### dataSetExcelWorkbook.headerStyle : [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

The style used for the header of the data

**Overrides**: [`headerStyle`](api-svyexcelutils.md#ServoyExcelWorkbook+headerStyle)

#### dataSetExcelWorkbook.rowStyle : [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

The style used for a data cell

**Overrides**: [`rowStyle`](api-svyexcelutils.md#ServoyExcelWorkbook+rowStyle)

#### dataSetExcelWorkbook.setAutoFilter : `Boolean`

Whether or not the data columns should be auto filtered or not

**Overrides**: [`setAutoFilter`](api-svyexcelutils.md#ServoyExcelWorkbook+setAutoFilter)

#### dataSetExcelWorkbook.sheet : [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)

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

#### dataSetExcelWorkbook.workbook : [`ExcelWorkbook`](api-svyexcelutils.md#excelworkbook)

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

* [ExcelWorkbook](api-svyexcelutils.md#excelworkbook)
  * [.cloneCellStyle(cellStyle)](api-svyexcelutils.md#excelworkbook.clonecellstyle-cellstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
  * [.cloneFont(font)](api-svyexcelutils.md#excelworkbook.clonefont-font-excelfont) ⇒ [`ExcelFont`](api-svyexcelutils.md#new\_ExcelFont\_new)
  * [.cloneSheet(indexToClone)](api-svyexcelutils.md#excelworkbook.clonesheet-indextoclone-excelsheet) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)
  * [.close()](api-svyexcelutils.md#excelworkbook.close)
  * [.createCellStyle()](api-svyexcelutils.md#excelworkbook.createcellstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
  * [.createFont()](api-svyexcelutils.md#excelworkbook.createfont-excelfont) ⇒ [`ExcelFont`](api-svyexcelutils.md#new\_ExcelFont\_new)
  * [.createSheet(sheetName)](api-svyexcelutils.md#excelworkbook.createsheet-sheetname-excelsheet) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)
  * [.getBytes()](api-svyexcelutils.md#excelworkbook.getbytes-array-.less-than-byte-greater-than) ⇒ `[ 'Array' ].<byte>`
  * [.getNumberOfSheets()](api-svyexcelutils.md#excelworkbook.getnumberofsheets-number) ⇒ `Number`
  * [.getSheet(sheetName)](api-svyexcelutils.md#excelworkbook.getsheet-sheetname-excelsheet) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)
  * [.getSheetAt(index)](api-svyexcelutils.md#excelworkbook.getsheetat-index-excelsheet) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)
  * [.getSheetNameAt(index)](api-svyexcelutils.md#excelworkbook.getsheetnameat-index-string) ⇒ `String`
  * [.getSheetNames()](api-svyexcelutils.md#excelworkbook.getsheetnames-array-.less-than-string-greater-than) ⇒ `[ 'Array' ].<String>`
  * [.removeSheetAt(index)](api-svyexcelutils.md#excelworkbook.removesheetat-index)
  * [.setSheetNameAt(index, name)](api-svyexcelutils.md#excelworkbook.setsheetnameat-index-name)
  * [.writeToFile(targetFile)](api-svyexcelutils.md#excelworkbook.writetofile-targetfile-boolean) ⇒ `Boolean`
  * [.wb](api-svyexcelutils.md#excelworkbook.wb-packages.org.apache.poi.ss.usermodel.workbook) : `Packages.org.apache.poi.ss.usermodel.Workbook`
  * [new ExcelWorkbook(\[templateOrFileType\])](api-svyexcelutils.md#new-excelworkbook-templateorfiletype)

#### excelWorkbook.cloneCellStyle(cellStyle) ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

Clones the given ExcelCellStyle

| Param     | Type                                                              |
| --------- | ----------------------------------------------------------------- |
| cellStyle | [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new) |

#### excelWorkbook.cloneFont(font) ⇒ [`ExcelFont`](api-svyexcelutils.md#new\_ExcelFont\_new)

Clones the given font and returns a new ExcelFont

| Param | Type                                                    |
| ----- | ------------------------------------------------------- |
| font  | [`ExcelFont`](api-svyexcelutils.md#new\_ExcelFont\_new) |

#### excelWorkbook.cloneSheet(indexToClone) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)

Creates an ExcelSheet from an existing sheet in the Workbook

**Returns**: [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new) - clone

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| indexToClone | `Number` | one based   |

#### excelWorkbook.close()

Closes this workbook

#### excelWorkbook.createCellStyle() ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

Creates an empty ExcelCellStyle

#### excelWorkbook.createFont() ⇒ [`ExcelFont`](api-svyexcelutils.md#new\_ExcelFont\_new)

Creates a font

#### excelWorkbook.createSheet(sheetName) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)

Creates a sheet with the given name

This method makes sure that no illegal names are provided and might change the name if needed

| Param     | Type     |
| --------- | -------- |
| sheetName | `String` |

#### excelWorkbook.getBytes() ⇒ `[ 'Array' ].<byte>`

Returns this workbook as a byte\[] array

#### excelWorkbook.getNumberOfSheets() ⇒ `Number`

Returns the number of spreadsheets in the workbook

#### excelWorkbook.getSheet(sheetName) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)

Returns the sheet with the given name (case insensitive match)

| Param     | Type     |
| --------- | -------- |
| sheetName | `String` |

#### excelWorkbook.getSheetAt(index) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)

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

### FoundSetExcelWorkbook ⇐ [`ServoyExcelWorkbook`](api-svyexcelutils.md#new\_ServoyExcelWorkbook\_new)

**Extends**: [`ServoyExcelWorkbook`](api-svyexcelutils.md#new\_ServoyExcelWorkbook\_new)

* [FoundSetExcelWorkbook](api-svyexcelutils.md#foundsetexcelworkbook-servoyexcelworkbook) ⇐ [`ServoyExcelWorkbook`](api-svyexcelutils.md#new\_ServoyExcelWorkbook\_new)
  * _inner_
    * [\~dataFilled](api-svyexcelutils.md#foundsetexcelworkbook-datafilled-boolean) : `Boolean`
  * _instance_
    * [.cloneCellStyle(cellStyle)](api-svyexcelutils.md#foundsetexcelworkbook.clonecellstyle-cellstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
    * [.cloneFont(font)](api-svyexcelutils.md#foundsetexcelworkbook.clonefont-font-excelfont) ⇒ [`ExcelFont`](api-svyexcelutils.md#new\_ExcelFont\_new)
    * [.cloneSheet(indexToClone)](api-svyexcelutils.md#foundsetexcelworkbook.clonesheet-indextoclone-excelsheet) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)
    * [.close()](api-svyexcelutils.md#foundsetexcelworkbook.close)
    * [.createCellStyle()](api-svyexcelutils.md#foundsetexcelworkbook.createcellstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
    * [.createColumnStyle(columnIndex)](api-svyexcelutils.md#foundsetexcelworkbook.createcolumnstyle-columnindex-excelcellstyle) ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
    * [.createFont()](api-svyexcelutils.md#foundsetexcelworkbook.createfont-excelfont) ⇒ [`ExcelFont`](api-svyexcelutils.md#new\_ExcelFont\_new)
    * [.createHeaderStyle()](api-svyexcelutils.md#foundsetexcelworkbook.createheaderstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
    * [.createRowStyle()](api-svyexcelutils.md#foundsetexcelworkbook.createrowstyle-excelcellstyle) ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
    * [.createSheet(sheetName)](api-svyexcelutils.md#foundsetexcelworkbook.createsheet-sheetname-excelsheet) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)
    * [.fillData()](api-svyexcelutils.md#foundsetexcelworkbook.filldata)
    * [.getBytes()](api-svyexcelutils.md#foundsetexcelworkbook.getbytes-array-.less-than-byte-greater-than) ⇒ `[ 'Array' ].<byte>`
    * [.getFoundSet()](api-svyexcelutils.md#foundsetexcelworkbook.getfoundset-jsfoundset) ⇒ `JSFoundSet`
    * [.getNumberOfSheets()](api-svyexcelutils.md#foundsetexcelworkbook.getnumberofsheets-number) ⇒ `Number`
    * [.getSheet(sheetName)](api-svyexcelutils.md#foundsetexcelworkbook.getsheet-sheetname-excelsheet) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)
    * [.getSheetAt(index)](api-svyexcelutils.md#foundsetexcelworkbook.getsheetat-index-excelsheet) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)
    * [.getSheetNameAt(index)](api-svyexcelutils.md#foundsetexcelworkbook.getsheetnameat-index-string) ⇒ `String`
    * [.getSheetNames()](api-svyexcelutils.md#foundsetexcelworkbook.getsheetnames-array-.less-than-string-greater-than) ⇒ `[ 'Array' ].<String>`
    * [.removeSheetAt(index)](api-svyexcelutils.md#foundsetexcelworkbook.removesheetat-index)
    * [.setFormatForColumn(columnIndex, format)](api-svyexcelutils.md#foundsetexcelworkbook.setformatforcolumn-columnindex-format)
    * [.setSheetNameAt(index, name)](api-svyexcelutils.md#foundsetexcelworkbook.setsheetnameat-index-name)
    * [.writeToFile(targetFile)](api-svyexcelutils.md#foundsetexcelworkbook.writetofile-targetfile-boolean) ⇒ `Boolean`
    * [.autoSizeColumns](api-svyexcelutils.md#foundsetexcelworkbook.autosizecolumns-boolean) : `Boolean`
    * [.columnFormats](api-svyexcelutils.md#foundsetexcelworkbook.columnformats-array-.less-than-string-greater-than) : `[ 'Array' ].<String>`
    * [.columnStyles](api-svyexcelutils.md#foundsetexcelworkbook.columnstyles-array-.less-than-excelcellstyle-greater-than) : [`[ 'Array' ].<ExcelCellStyle>`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
    * [.defaultDateFormat](api-svyexcelutils.md#foundsetexcelworkbook.defaultdateformat-string) : `String`
    * [.defaultNumberFormat](api-svyexcelutils.md#foundsetexcelworkbook.defaultnumberformat-string) : `String`
    * [.foundset](api-svyexcelutils.md#foundsetexcelworkbook.foundset-jsfoundset) : `JSFoundSet`
    * [.freezeFirstRow](api-svyexcelutils.md#foundsetexcelworkbook.freezefirstrow-boolean) : `Boolean`
    * [.headerStyle](api-svyexcelutils.md#foundsetexcelworkbook.headerstyle-excelcellstyle) : [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
    * [.rowStyle](api-svyexcelutils.md#foundsetexcelworkbook.rowstyle-excelcellstyle) : [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)
    * [.setAutoFilter](api-svyexcelutils.md#foundsetexcelworkbook.setautofilter-boolean) : `Boolean`
    * [.sheet](api-svyexcelutils.md#foundsetexcelworkbook.sheet-excelsheet) : [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)
    * [.sheetName](api-svyexcelutils.md#foundsetexcelworkbook.sheetname-string) : `String`
    * [.startColumn](api-svyexcelutils.md#foundsetexcelworkbook.startcolumn-number) : `Number`
    * [.startRow](api-svyexcelutils.md#foundsetexcelworkbook.startrow-number) : `Number`
    * [.wb](api-svyexcelutils.md#foundsetexcelworkbook.wb-packages.org.apache.poi.ss.usermodel.workbook) : `Packages.org.apache.poi.ss.usermodel.Workbook`
    * [.workbook](api-svyexcelutils.md#foundsetexcelworkbook.workbook-excelworkbook) : [`ExcelWorkbook`](api-svyexcelutils.md#excelworkbook)
  * [new FoundSetExcelWorkbook(foundset, dataproviders, \[headers\], \[templateOrFileType\], \[sheetNameToUse\]](api-svyexcelutils.md#new-foundsetexcelworkbook-foundset-dataproviders-headers-templateorfiletype-sheetnametouse)

#### FoundSetExcelWorkbook\~dataFilled : `Boolean`

#### foundSetExcelWorkbook.cloneCellStyle(cellStyle) ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

Clones the given ExcelCellStyle

| Param     | Type                                                              |
| --------- | ----------------------------------------------------------------- |
| cellStyle | [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new) |

#### foundSetExcelWorkbook.cloneFont(font) ⇒ [`ExcelFont`](api-svyexcelutils.md#new\_ExcelFont\_new)

Clones the given font and returns a new ExcelFont

| Param | Type                                                    |
| ----- | ------------------------------------------------------- |
| font  | [`ExcelFont`](api-svyexcelutils.md#new\_ExcelFont\_new) |

#### foundSetExcelWorkbook.cloneSheet(indexToClone) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)

Creates an ExcelSheet from an existing sheet in the Workbook

**Returns**: [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new) - clone

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| indexToClone | `Number` | one based   |

#### foundSetExcelWorkbook.close()

Closes this workbook

#### foundSetExcelWorkbook.createCellStyle() ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

Creates an empty ExcelCellStyle

#### foundSetExcelWorkbook.createColumnStyle(columnIndex) ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

Creates and returns an ExcelCellStyle used for a specific column

| Param       | Type     |
| ----------- | -------- |
| columnIndex | `Number` |

#### foundSetExcelWorkbook.createFont() ⇒ [`ExcelFont`](api-svyexcelutils.md#new\_ExcelFont\_new)

Creates a font

#### foundSetExcelWorkbook.createHeaderStyle() ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

Creates and returns an ExcelCellStyle used for the header row

#### foundSetExcelWorkbook.createRowStyle() ⇒ [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

Creates and returns an ExcelCellStyle used for a data row

#### foundSetExcelWorkbook.createSheet(sheetName) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)

Creates a sheet with the given name

This method makes sure that no illegal names are provided and might change the name if needed

| Param     | Type     |
| --------- | -------- |
| sheetName | `String` |

#### foundSetExcelWorkbook.fillData()

Fills the sheet with the data of the foundset

This is automatically done when `writeToFile()` or `getBytes()` is called

**Overrides**: [`fillData`](api-svyexcelutils.md#ServoyExcelWorkbook+fillData)

#### foundSetExcelWorkbook.getBytes() ⇒ `[ 'Array' ].<byte>`

Returns the data of this workbook as a byte\[]

**Returns**: `[ 'Array' ].<byte>` - bytes

#### foundSetExcelWorkbook.getFoundSet() ⇒ `JSFoundSet`

Returns the foundset used to create this workbook

#### foundSetExcelWorkbook.getNumberOfSheets() ⇒ `Number`

Returns the number of spreadsheets in the workbook

#### foundSetExcelWorkbook.getSheet(sheetName) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)

Returns the sheet with the given name (case insensitive match)

| Param     | Type     |
| --------- | -------- |
| sheetName | `String` |

#### foundSetExcelWorkbook.getSheetAt(index) ⇒ [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)

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

#### foundSetExcelWorkbook.columnStyles : [`[ 'Array' ].<ExcelCellStyle>`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

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

**Overrides**: [`freezeFirstRow`](api-svyexcelutils.md#ServoyExcelWorkbook+freezeFirstRow)

#### foundSetExcelWorkbook.headerStyle : [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

The style used for the header of the data

**Overrides**: [`headerStyle`](api-svyexcelutils.md#ServoyExcelWorkbook+headerStyle)

#### foundSetExcelWorkbook.rowStyle : [`ExcelCellStyle`](api-svyexcelutils.md#new\_ExcelCellStyle\_new)

The style used for a data cell

**Overrides**: [`rowStyle`](api-svyexcelutils.md#ServoyExcelWorkbook+rowStyle)

#### foundSetExcelWorkbook.setAutoFilter : `Boolean`

Whether or not the data columns should be auto filtered or not

**Overrides**: [`setAutoFilter`](api-svyexcelutils.md#ServoyExcelWorkbook+setAutoFilter)

#### foundSetExcelWorkbook.sheet : [`ExcelSheet`](api-svyexcelutils.md#new\_ExcelSheet\_new)

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

#### foundSetExcelWorkbook.workbook : [`ExcelWorkbook`](api-svyexcelutils.md#excelworkbook)

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
| XLSX  | `2`     | XLSX format, requires additional libraries @see [excelutils.md](excelutils.md "mention") |
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

### createWorkbook(\[templateOrFileType]) ⇒ [`ExcelWorkbook`](api-svyexcelutils.md#excelworkbook)

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

### createWorkbookFromDataSet(dataset, \[columns], \[headers], \[templateOrFileType], \[sheetNameToUse]) ⇒ [`DataSetExcelWorkbook`](api-svyexcelutils.md#datasetexcelworkbook-servoyexcelworkbook)

Creates an ExcelWorkbook from the given dataset

If a template is provided, the dataset will be inserted in the given sheet

| Param                 | Type                                          | Description                                                                                                                                      |
| --------------------- | --------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| dataset               | `JSDataSet`                                   | the dataset                                                                                                                                      |
| \[columns]            | `[ 'Array' ].<Number>`                        | the column numbers to be included in the sheet                                                                                                   |
| \[headers]            | `[ 'Array' ].<String>`                        | the text to be used as column headers                                                                                                            |
| \[templateOrFileType] | `String` \| `plugins.file.JSFile` \| `Number` | either file or media URL pointing to an existing Excel to be used as template or one of the FILE\_FORMAT constants when creating empty workbooks |
| \[sheetNameToUse]     | `String`                                      | when a template is used, this is the name of the sheet to be filled                                                                              |

### createWorkbookFromFoundSet(foundset, dataproviders, \[headers], \[templateOrFileType], \[sheetNameToUse]) ⇒ [`FoundSetExcelWorkbook`](api-svyexcelutils.md#foundsetexcelworkbook-servoyexcelworkbook)

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

### getWorkbook(original) ⇒ [`ExcelWorkbook`](api-svyexcelutils.md#excelworkbook)

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
