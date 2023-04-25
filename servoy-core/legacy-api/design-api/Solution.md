#  Solution

## **Supported Clients**

    SmartClient
    WebClient
    NGClient
    MobileClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [comment](Solution.md#comment)                   | .                                    |
| [Number](../JSLib/Number.md) | [firstForm](Solution.md#firstForm)                   | The first form that loads when a solution is deployed..                                    |
| [String](../JSLib/String.md) | [i18nDataSource](Solution.md#i18nDataSource)                   | The i18n database server connection and database table that stores the i18n keys for a solution..                                    |
| [Number](../JSLib/Number.md) | [loginForm](Solution.md#loginForm)                   | The name of the login form that loads when a solution is deployed..                                    |
| [String](../JSLib/String.md) | [loginSolutionName](Solution.md#loginSolutionName)                   | Get the first module that is also a login solution..                                    |
| [String](../JSLib/String.md) | [modulesNames](Solution.md#modulesNames)                   | The list of modules that have been added to a solution..                                    |
| [Boolean](../JSLib/Boolean.md) | [mustAuthenticate](Solution.md#mustAuthenticate)                   | Flag that tells if authentication is needed in order to access the solution..                                    |
| [Number](../JSLib/Number.md) | [solutionType](Solution.md#solutionType)                   | The type of a solution; can be "Normal" (non-module), "Module", "Web client only", "Smart client only", "Login", "Authenticator", "Pre-import hook module", "Post-import hook module", "Mobile"..                                    |
| [Number](../JSLib/Number.md) | [styleSheet](Solution.md#styleSheet)                   | The custom CSS used by the solution (a MEDIA lib entry)..                                    |
| [Number](../JSLib/Number.md) | [textOrientation](Solution.md#textOrientation)                   | The direction that text is displayed..                                    |
| [String](../JSLib/String.md) | [titleText](Solution.md#titleText)                   | The menu bar title of a solution..                                    |
| [String](../JSLib/String.md) | [version](Solution.md#version)                   | This is the version of the solution, this can be any kind of string but try to follow "Semantic Versioning"..                                    |

## Events Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [void](../void.md) | [onAutoSaveFailed(recordMarkers)](Solution.md#onautosavefailed-recordmarkers)                   | The method that is executed when autosave results in validation or save failures..                                    |
| [void](../void.md) | [onBeforeLogin(queryParams)](Solution.md#onbeforelogin-queryparams)                   | The method that is to onOpen just that it executes before the login on solutions with a login form (not login soliution)..                                    |
| [Boolean](../JSLib/Boolean.md) | [onClose(force)](Solution.md#onclose-force)                   | The method that is executed when a solution closes..                                    |
| [void](../void.md) | [onDataBroadcast(dataSource, action, pks, cached)](Solution.md#ondatabroadcast-datasource-action-pks-cached)                   | Method that is executed when data broadcast occurs..                                    |
| [Boolean](../JSLib/Boolean.md) | [onError(ex)](Solution.md#onerror-ex)                   | The method that is executed when a solution opens and an error occurs..                                    |
| [void](../void.md) | [onOpen(arg, queryParams)](Solution.md#onopen-arg-queryparams)                   | The method that is executed when a solution opens..                                    |

## Properties Details

### comment



**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### firstForm

The first form that loads when a solution is deployed.

NOTE: If the Login form is specified, then the firstForm is the first form that will load next after the loginForm.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### i18nDataSource

The i18n database server connection and database table that stores the i18n keys for a solution.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### loginForm

The name of the login form that loads when a solution is deployed.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### loginSolutionName

Get the first module that is also a login solution.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### modulesNames

The list of modules that have been added to a solution.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### mustAuthenticate

Flag that tells if authentication is needed in order to access the solution.
If unchecked, the Smart Client will always require authentication, regardless of this setting.
If checked, authentication is required, and either a provided loginSolution or otherwise the default Servoy login mechanism will be used.
If default Servoy login mechanism is used, the "servoy.webclient.basic.authentication" setting on the Admin Page can be used to enable the use of the standard browser basic authentication.

**Returns**\
[Boolean](../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### solutionType

The type of a solution; can be "Normal" (non-module), "Module", "Web client only", "Smart client only",
"Login", "Authenticator", "Pre-import hook module", "Post-import hook module", "Mobile".
These constants are defined in SolutionMetaData class.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### styleSheet

The custom CSS used by the solution (a MEDIA lib entry). It can reference other media resources (even additional .css through relative '@import' statements).
For NGClient - this CSS will be available directly in the browser.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
NGClient

**Sample**

```javascript

```
### textOrientation

The direction that text is displayed.

Options include:
DEFAULT
left to right
right to left
locale specific

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### titleText

The menu bar title of a solution.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### version

This is the version of the solution, this can be any kind of string but try to follow "Semantic Versioning".
This version is important when you are making modules that are distributed by the Servoy Package Manager.
Then this version is used to know what the developer has installed. This version should be in sync then with the webpackage.json file.

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```

