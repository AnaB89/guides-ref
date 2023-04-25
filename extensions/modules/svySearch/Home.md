# svySearch

Welcome to the **svySearch** wiki! This wiki provides comprehensive documentation to using the **svySearch** module. This module is designed to parse natural-language text input and apply it to developer-specified patterns for searching.

**Table of Contents**

* [Parsing Rules](Home.md#parsing-rules)
* [API Documentation](Home.md#api-documentation)
  * [svySearch Scope](Home.md#svysearch)
  * [SimpleSearch Class](Home.md#simplesearch)
  * [SearchProvider Class](Home.md#searchprovider)

### Parsing Rules

Text is parsed according to some general patterns. String fragments are matched against developer-specified [SearchProvider](Home.md#searchprovider), which map some rules to how certain columns are searched.

**Patterns**

* [Tokens](Home.md#tokens): Parsing input for individual words
* [Quoted Strings](Home.md#quoted-strings): Used to escape token separators
* [Aliases](Home.md#aliases): Used to explicitly referenes a single [SearchProvider](Home.md#searchprovider)
* [Operators](Home.md#operators): For comparisons other than the default LIKE/Contains
* [Substitutions](Home.md#substitutions): Dynamically match and replace input text, ideal for converting value list values into stored values

#### Tokens

Words separated by white space will be treated as separate tokens. ALL tokens must match ANY [SearchProvider](Home.md#searchprovider).

**Example**

```
John Smith // matches "John Smith", "Smithers Johnson", "John Doe" at "Smithefield Road", etc
```

**NOTE**: _Multiple tokens that match on the same **related** SearchProvider are not currently supported and may result in no records. This cannot be easily supported, because when a SearchProvider is compared to multiple tokens, we cannot know which token(s) matched, and therefore, cannot guarantee the contract for matching ALL tokens._

#### Quoted Strings

Use double quotes to escape tokenization

**Example**

```
"John Smith" // matches only "John Smith" and not "Smithers Johnson", "John Doe" at "Smithefield Road", etc
```

#### Aliases

Any [SearchProvider](Home.md#searchprovider) can be explicitly searched using the data provider name or alias. Aliases are specified left or a ':' character. Additionally, some [SearchProvider](Home.md#searchprovider) can be specified as explicit-only, meaning the field is not searched unless the user performs an alias-based search. This can be useful for date fields

**Example**

```
last-name:smith // matches "John Smith", but not John Doe at "Smithefield Road", etc.
```

#### Operators

By default, all searches are LIKE/Contains for Strings and strict "=" for Numbers and Dates. However, additional operators may be specified at the beginning of a token (except for the BETWEEN operator)

| Operator | Name                  | Summary                                                                                             |
| -------- | --------------------- | --------------------------------------------------------------------------------------------------- |
| -        | Exclude               | Excludes the token from the search using a NOT LIKE for Strings and NOT EQUAL for Numbers and Dates |
| +        | Exact                 | Performs an exact match in lieu of a LIKE                                                           |
| >        | Greater-Than          | Matches all values greater than the specified token                                                 |
| >=       | Greater-Than-Or-Equal | Matches all values greater than or equal to the specified token                                     |
| <        | Less-Than             | Matches all values less than the specified token                                                    |
| <=       | Less-Than-Or-Equal    | Matches all values less than or equal to the specified token                                        |
| ...      | Between               | Matches all values between the two operands                                                         |

**Example**

```
john -smith   // matches "John Doe" and "Suxy Johnson" but not "John Smith"
+john         // matches "John Doe", but not "Suzy Johnson"
freight:>100  // matches any freight greater than $100
freight:>=100 // matches any freight greater or equal to $100
order-date:<01-01-1997  // matches any date less than 01-01-1997
order-date:<=01-01-1997  // matches any date less than or equal to 01-01-1997
order-date:01-01-1997...12-31-1997  // matches any date during the year of 1997
```

#### Substitutions

Substitutions can be applied dynamically to match and replace string fragments within user input. This is ideal for allowing users to express custom ValueList display values in their searches, and have those values resolved to the actual stored/DB value

**Example**

```
user-type:admin // where "admin" is substituted to some stored value, for example "1"
```

## API Documentation

**svySearch** is an object-oriented API for parsing user input and applying searches against the data model.

The API consists of the primary class [SimpleSearch](Home.md#simplesearch), which models a search on a particular data source and its supporting class, [SearchProvider](Home.md#searchprovider), which models th ecomponent of the search that maps to a single data provider.

**Example**

```
//	create the search object
var search = scopes.svySearch.createSimpleSearch(foundset);

//	add some data providers
search.addSearchProvider('shipcity');

//	add related data providers
search.addSearchProvider('orders_to_customers.companyname');
search.addSearchProvider('orders_to_order_details.order_details_to_products.productname');

//	add an explicit search provider
search.addSearchProvider('orderdate')
	.setAlias('date')
	.setImpliedSearch(false);
	
//	set user input
search.setSearchText('germany ordered:01/01/1996');

//	execute search in existing foundset
search.loadRecords(foundset);
```

## svySearch

A single scope that contains the classes

### Method Summary

#### createSimpleSearch

***

**Params**

| Type   | Name           | Summary              | Required |
| ------ | -------------- | -------------------- | -------- |
| Number | **dataSource** | The data source used | Required |

**returns**

[SimpleSearch](Home.md#simplesearch)

**example**

```
scopes.svySearch.createSimpleSearch(foundset);
scopes.svySearch.createSimpleSearch(record);
scopes.svySearch.createSimpleSearch('db:/example_data/orders');
```

## SimpleSearch

A class which models a search on a particular data source and its supporting class

### Method Summary

| Return Type                                                                                   | Method                                                             | Description                                                                                                                |
| --------------------------------------------------------------------------------------------- | ------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------- |
| [SimpleSearch](Home.md#simplesearch)                                                          | [**addAlternateDateFormat**](Home.md#addalternatedateformat)       | Add alternative date format which is used to parse user input for searching dates in addition to the default format.       |
| [SearchProvider](Home.md#searchprovider)                                                      | [**addSearchProvider**](Home.md#addsearchprovider)                 | Adds a dataprovider to the search object.                                                                                  |
| [Array](https://wiki.servoy.com/display/DOCS/Array)<[SearchProvider](Home.md#searchprovider)> | [**getAllSearchProviders**](Home.md#getallsearchproviders)         | Get all search providers for this search object                                                                            |
| [Array](https://wiki.servoy.com/display/DOCS/Array)\<String>                                  | [**getAlternateDateFormats**](Home.md#getalternatedateformats)     | Returns the alternate date format which is used to parse user input for searching dates in addition to the default format. |
| [JSDataSet](https://wiki.servoy.com/display/DOCS/JSDataSet)                                   | [**getDataSet**](Home.md#getdataset)                               | Executes the search and returns the results as a [JSDataSet](https://wiki.servoy.com/display/DOCS/JSDataSet)               |
| [String](https://wiki.servoy.com/display/DOCS/String)                                         | [**getDataSource**](Home.md#getdatasource)                         | Returns the data source used by the search object                                                                          |
| [String](https://wiki.servoy.com/display/DOCS/String)                                         | [**getDateFormat**](Home.md#getdateformat)                         | Returns the date format which is used to parse user input for searching dates                                              |
| [JSFoundSet](https://wiki.servoy.com/display/DOCS/JSFoundSet)                                 | [**getFoundSet**](Home.md#getfoundset)                             | Creates a factory foundset, runs the search and returns it                                                                 |
| [QBSelect](https://wiki.servoy.com/display/DOCS/QBSelect)                                     | [**getQuery**](Home.md#getquery)                                   | Creates and returns a query object parsed from the user input                                                              |
| [SearchProvider](Home.md#searchprovider)                                                      | [**getSearchProvider**](Home.md#getsearchprovider)                 | Gets a [SearchProvider](Home.md#searchprovider) by specified name (alias)                                                  |
| [String](https://wiki.servoy.com/display/DOCS/String)                                         | [**getSearchText**](Home.md#getsearchtext)                         | Gets the raw, unparsed input text                                                                                          |
| [Boolean](https://wiki.servoy.com/display/DOCS/Boolean)                                       | [**loadRecords**](Home.md#loadrecords)                             | Loads records on the specified foundset.                                                                                   |
| [SimpleSearch](Home.md#simplesearch)                                                          | [**removeAlternateDateFormat**](Home.md#removealternatedateformat) | Remove alternative date format which is used to parse user input for searching dates in addition to the default format.    |
| [SimpleSearch](Home.md#simplesearch)                                                          | [**setDateFormat**](Home.md#setdateformat)                         | Sets the date formatting which will be used to parse user input                                                            |
| [SimpleSearch](Home.md#simplesearch)                                                          | [**setSearchAllColumns**](Home.md#setsearchallcolumns)             | Sets that all columns are to be searchable                                                                                 |
| [SimpleSearch](Home.md#simplesearch)                                                          | [**setSearchText**](Home.md#setsearchtext)                         | Set the raw, user input to be parsed                                                                                       |

### Method Details

#### addAlternateDateFormat

Add alternative date format which is used to parse user input for searching dates in addition to the default format.

**Params**

| Type                                                  | Name       | Summary                                                                                                                                                | Required     |
| ----------------------------------------------------- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------ |
| [String](https://wiki.servoy.com/display/DOCS/String) | **format** | any date format pattern that will result in a well defined time interval to search for (e.g. MM-yyyy will look for beginning of month to end of month) | **Required** |

**Returns** [SimpleSearch](Home.md#simplesearch)

**Example**

```
 simpleSearch.addAlternateDateFormat("dd/MM/yyyy");
 simpleSearch.addAlternateDateFormat("MM-yyyy");
 simpleSearch.addAlternateDateFormat("MM/yyyy");
 simpleSearch.addAlternateDateFormat("MMM yyyy");
 simpleSearch.addAlternateDateFormat("MMMM yyyy");
 simpleSearch.addAlternateDateFormat("yyyy");
 ...
 
 //The following are invalid formats
 // simpleSearch.addAlternateDateFormat("dd/yyyy"); will throw an exception
 // simpleSearch.addAlternateDateFormat("MM"); will throw an exception
```

#### addSearchProvider

Adds a search provider to the search object.

**Params**

| Type                                                    | Name               | Summary                                                                                   | Required                                   |
| ------------------------------------------------------- | ------------------ | ----------------------------------------------------------------------------------------- | ------------------------------------------ |
| [String](https://wiki.servoy.com/display/DOCS/String)   | **dataProviderID** | The data provider that will be searched. Can be columns, related columns                  | **Required**                               |
| [String](https://wiki.servoy.com/display/DOCS/String)   | **alias**          | The natural language name of the search provider. Used in explicit searches.              | Optional. Default is same as data provider |
| [Boolean](https://wiki.servoy.com/display/DOCS/Boolean) | **impliedSearch**  | Set this false to indicate that a provider is not searchable unless explicitly referenced | Optional. Default is True                  |
| [Boolean](https://wiki.servoy.com/display/DOCS/Boolean) | **caseSensitive**  | Set this to be true to force case-sensitive search on this search provider                | Optional. Default is False                 |

**Returns** [SearchProvider](Home.md#searchprovider)

#### getAllSearchProviders

Get all search providers for this search object

**Returns** [Array](https://wiki.servoy.com/display/DOCS/Array)<[SearchProvider](Home.md#searchprovider)>

#### getAlternateDateFormats

Returns the alternate date format which is used to parse user input for searching dates in addition to the default format.

**Returns** [Array](https://wiki.servoy.com/display/DOCS/Array)\<String>

#### getDataSet

Executes the search and returns the results as a [JSDataSet](https://wiki.servoy.com/display/DOCS/JSDataSet)

**Params**

| Type   | Name        | Summary                  | Required                            |
| ------ | ----------- | ------------------------ | ----------------------------------- |
| Number | **maxRows** | The max rows to retrieve | Optional. Default is -1 (unlimited) |

**Returns** [JSDataSet](https://wiki.servoy.com/display/DOCS/JSDataSet)

#### getDataSource

Returns the data source used by the search object

**Returns** [String](https://wiki.servoy.com/display/DOCS/String)

#### getDateFormat

Returns the date format which is used to parse user input for searching dates

**Returns** [String](https://wiki.servoy.com/display/DOCS/String)

#### getFoundSet

Creates a factory foundset, runs the search and returns it

**Returns** [JSFoundSet](https://wiki.servoy.com/display/DOCS/JSFoundSet)

#### getQuery

Creates and returns a query object parsed from the user input

**Returns** [QBSelect](https://wiki.servoy.com/display/DOCS/QBSelect)

#### getSearchProvider

Gets the specified [SearchProvider](Home.md#searchprovider)

**Params**

| Type                                                  | Name                    | Summary                                | Required |
| ----------------------------------------------------- | ----------------------- | -------------------------------------- | -------- |
| [String](https://wiki.servoy.com/display/DOCS/String) | **aliasOrDataProvider** | The name or alias of the data provider | Required |

**Returns** [SearchProvider](Home.md#searchprovider) or null if named [SearchProvider](Home.md#searchprovider) is not found

#### getSearchText

Gets the raw, unparsed input text

**Returns** [String](https://wiki.servoy.com/display/DOCS/String)

#### loadRecords

Loads records in the specified foundset

**Params**

| Type                                                          | Name         | Summary                                                                                             | Required |
| ------------------------------------------------------------- | ------------ | --------------------------------------------------------------------------------------------------- | -------- |
| [JSFoundSet](https://wiki.servoy.com/display/DOCS/JSFoundSet) | **foundSet** | The [JSFoundSet](https://wiki.servoy.com/display/DOCS/JSFoundSet) object upon which to load records | Required |

**Returns** [Boolean](https://wiki.servoy.com/display/DOCS/Boolean) True indicates query was successful, although may have loaded zero records

#### removeAlternateDateFormat

Remove alternative date format which is used to parse user input for searching dates in addition to the default format.

**Params**

| Type                                                  | Name       | Summary                                 | Required     |
| ----------------------------------------------------- | ---------- | --------------------------------------- | ------------ |
| [String](https://wiki.servoy.com/display/DOCS/String) | **format** | the alternate date format to be removed | **Required** |

**Returns** [SimpleSearch](Home.md#simplesearch)

#### setDateFormat

Sets the date formatting which will be used to parse user input

**Params**

| Type                                                  | Name       | Summary                             | Required |
| ----------------------------------------------------- | ---------- | ----------------------------------- | -------- |
| [String](https://wiki.servoy.com/display/DOCS/String) | **format** | The format to use for date searches | Required |

**Returns** [SimpleSearch](Home.md#simplesearch) Returns this [SimpleSearch](Home.md#simplesearch) for convenience, method chaining

#### setSearchAllColumns

Sets that all columns are to be searchable

This should be called **before** adding any additional, related search providers

**Returns** [SimpleSearch](Home.md#simplesearch) Returns this [SimpleSearch](Home.md#simplesearch) for convenience, method chaining

#### setSearchText

Set the raw, user input to be parsed

**Params**

| Type                                                  | Name           | Summary                   | Required |
| ----------------------------------------------------- | -------------- | ------------------------- | -------- |
| [String](https://wiki.servoy.com/display/DOCS/String) | **searchText** | The raw text to be parsed | Required |

**Returns** [SimpleSearch](Home.md#simplesearch) Returns this [SimpleSearch](Home.md#simplesearch) for convenience, method chaining

## [SearchProvider](Home.md#searchprovider)

A class which models the component of the search that maps to a single data provider.

### Method Summary

| Return Type                                                                                                | Method                                                   | Description                                                                                     |
| ---------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| [SearchProvider](Home.md#searchprovider)                                                                   | [**addSubstitution**](Home.md#addsubstitution)           | Add a substitution kev-value pair to this search provider                                       |
| [String](https://wiki.servoy.com/display/DOCS/String)                                                      | [**getAlias**](Home.md#getAlias)                         | Gets the alias of this search provider.                                                         |
| [String](https://wiki.servoy.com/display/DOCS/String)                                                      | [**getDataProviderID**](Home.md#getdataproviderid)       | Gets the data provider ID                                                                       |
| JSColumn                                                                                                   | [**getJSColumn**](Home.md#getjscolumn)                   | Get the JSColumn object that corresponds to this search provider                                |
| JSTable                                                                                                    | [**getJSTable**](Home.md#getjstable)                     | Get the JSTable object that corresponds to this search provider                                 |
| [String](https://wiki.servoy.com/display/DOCS/String)                                                      | [**getStringMatching**](Home.md#getstringmatching)       | gets the String matching mode for this [SearchProvider](Home.md#searchprovider)                 |
| [Array](https://wiki.servoy.com/display/DOCS/Array)<[String](https://wiki.servoy.com/display/DOCS/String)> | [**getSubstitutionsKeys**](Home.md#getsubstitutionskeys) | Get all the keys for substitutions                                                              |
| [String](https://wiki.servoy.com/display/DOCS/String)                                                      | [**getSubstitutionValue**](Home.md#getsubstitutionvalue) | Get the substitution value for a given key                                                      |
| [Boolean](https://wiki.servoy.com/display/DOCS/Boolean)                                                    | [**isCaseSensitive**](Home.md#iscasesensitive)           | Indicates if this [SearchProvider](Home.md#searchprovider) is case-sensitive                    |
| [Boolean](https://wiki.servoy.com/display/DOCS/Boolean)                                                    | [**isCastInteger**](Home.md#iscastinteger)               | Indicates if this [SearchProvider](Home.md#searchprovider) will cast INTEGER to TEXT            |
| [Boolean](https://wiki.servoy.com/display/DOCS/Boolean)                                                    | [**isImpliedSearch**](Home.md#isimpliedsearch)           | Indicates if this [SearchProvider](Home.md#searchprovider) is an implied search                 |
| [SearchProvider](Home.md#searchprovider)                                                                   | [**setAlias**](Home.md#setalias)                         | Sets the natural language name for this [SearchProvider](Home.md#searchprovider)                |
| [SearchProvider](Home.md#searchprovider)                                                                   | [**setCaseSensitive**](Home.md#setcasesensitive)         | Specifies if this [SearchProvider](Home.md#searchprovider) will perform case-sensitive searches |
| [SearchProvider](Home.md#searchprovider)                                                                   | [**setCastInteger**](Home.md#setcastinteger)             | Specifies if this [SearchProvider](Home.md#searchprovider) will cast INTEGER to TEXT            |
| [SearchProvider](Home.md#searchprovider)                                                                   | [**setImpliedSearch**](Home.md#setimpliedsearch)         | Specifies if this search provider is included in implied search                                 |
| [SearchProvider](Home.md#searchprovider)                                                                   | [**setStringMatching**](Home.md#setstringmatching)       | Sets the String matching mode for this [SearchProvider](Home.md#searchprovider)                 |

### Method Details

#### addSubstitution

Add a substitution kev-value pair to this search provider

Substitutions provide replacement capability for user input.

A typical use case involves parsing a value list display value

**Params**

| Type                                                  | Name      | Summary                      | Required |
| ----------------------------------------------------- | --------- | ---------------------------- | -------- |
| [String](https://wiki.servoy.com/display/DOCS/String) | **key**   | A string to be replaced      | Required |
| [String](https://wiki.servoy.com/display/DOCS/String) | **value** | The value to replace it with | Required |

**Returns** [SearchProvider](Home.md#searchprovider) this [SearchProvider](Home.md#searchprovider) for convenience, method chaining

#### getAlias

Gets the alias of this search provider.

**Returns** [String](https://wiki.servoy.com/display/DOCS/String) The alias, or null if none was specified

#### getDataProviderID

Gets the data provider ID

**Returns** [String](https://wiki.servoy.com/display/DOCS/String) The data provider which will be searched

#### getJSColumn

Get the JSColumn object that corresponds to this search provider

**Returns** JSColumn

#### getJSTable

Get the JSTable object that corresponds to this search provider

**Returns** JSTable

#### getStringMatching

Get the matching mode for this search provider.

**Returns** [String](https://wiki.servoy.com/display/DOCS/String)

#### getSubstitutionsKeys

Get all the keys for substitutions

**Returns** [Array](https://wiki.servoy.com/display/DOCS/Array)<[String](https://wiki.servoy.com/display/DOCS/String)>

#### getSubstitutionValue

Get the substitution value for a given key

**Params**

| Type                                                  | Name    | Summary              | Required |
| ----------------------------------------------------- | ------- | -------------------- | -------- |
| [String](https://wiki.servoy.com/display/DOCS/String) | **key** | The substitution key | Required |

**Returns** [String](https://wiki.servoy.com/display/DOCS/String)

#### isCaseSensitive

Indicates if this [SearchProvider](Home.md#searchprovider) is case-sensitive

**Returns** [Boolean](https://wiki.servoy.com/display/DOCS/Boolean)

#### isCastInteger

Indicates if this [SearchProvider](Home.md#searchprovider) will cast INTEGER values to TEXT in the query

**Returns** \[Boolean]

#### isImpliedSearch

Indicates if this [SearchProvider](Home.md#searchprovider) is an implied search

**Returns** [Boolean](https://wiki.servoy.com/display/DOCS/Boolean)

#### setAlias

Sets the natural language name for this [SearchProvider](Home.md#searchprovider)

The alias can be used in explicit searches

**Params**

| Type                                                  | Name      | Summary   | Required |
| ----------------------------------------------------- | --------- | --------- | -------- |
| [String](https://wiki.servoy.com/display/DOCS/String) | **alias** | The alias | Required |

**Returns** [SearchProvider](Home.md#searchprovider) this [SearchProvider](Home.md#searchprovider) for convenience, method chaining

#### setCaseSensitive

Specifies if this [SearchProvider](Home.md#searchprovider) will perform case-sensitive searches

**Params**

| Type                                                    | Name              | Summary                      | Required |
| ------------------------------------------------------- | ----------------- | ---------------------------- | -------- |
| [Boolean](https://wiki.servoy.com/display/DOCS/Boolean) | **caseSensitive** | The value for case-sensitive | Required |

**Returns** [SearchProvider](Home.md#searchprovider) this [SearchProvider](Home.md#searchprovider) for convenience, method chaining

#### setCastInteger

Specifies if this [SearchProvider](Home.md#searchprovider) will cast INTEGER values to TEXT in the query. For example, a search term `"1025"` would match on `10250`, `10251`, `91025`, etc.

**Params**

| Type                                                    | Name            | Summary                                        | Required |
| ------------------------------------------------------- | --------------- | ---------------------------------------------- | -------- |
| [Boolean](https://wiki.servoy.com/display/DOCS/Boolean) | **castInteger** | True if the INTEGER values should cast to TEXT | Required |

**Returns** [SearchProvider](Home.md#searchprovider) this [SearchProvider](Home.md#searchprovider) for convenience, method chaining

#### setImpliedSearch

Specifies if this search provider is included in implied search

A value of **true** indicates that the provider will always be searched

A value of **false** indicates that provider will ONLY be searched when used in explicit field matching

**Params**

| Type                                                    | Name              | Summary                      | Required |
| ------------------------------------------------------- | ----------------- | ---------------------------- | -------- |
| [Boolean](https://wiki.servoy.com/display/DOCS/Boolean) | **impliedSearch** | The value for implied search | Required |

**Returns** [SearchProvider](Home.md#searchprovider) this [SearchProvider](Home.md#searchprovider) for convenience, method chaining

#### setStringMatching

Sets the string matching mode for this SearchProvider

**Params**

| Type                                                  | Name               | Summary                   | Required |
| ----------------------------------------------------- | ------------------ | ------------------------- | -------- |
| [String](https://wiki.servoy.com/display/DOCS/String) | **stringMatching** | The desired matching mode | Required |

**Returns** [SearchProvider](Home.md#searchprovider) this [SearchProvider](Home.md#searchprovider) for convenience, method chaining
