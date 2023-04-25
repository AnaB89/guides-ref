#  Application

## **Return Types**
[APPLICATION_TYPES](Application/APPLICATION_TYPES.md),[CLIENTDESIGN](Application/CLIENTDESIGN.md),[DRAGNDROP](Application/DRAGNDROP.md),[ELEMENT_TYPES](Application/ELEMENT_TYPES.md),[CSSPosition](Application/CSSPosition.md),[Renderable](Application/Renderable.md),[JSDNDEvent](Application/JSDNDEvent.md),[JSEvent](Application/JSEvent.md),[JSRenderEvent](Application/JSRenderEvent.md),[JSUpload](Application/JSUpload.md),[JSWindow](Application/JSWindow.md),[JSLogger](Application/JSLogger.md),[JSLogBuilder](Application/JSLogBuilder.md),[LOGGINGLEVEL](Application/LOGGINGLEVEL.md),[UICONSTANTS](Application/UICONSTANTS.md),[UUID](Application/UUID.md),[WEBCONSTANTS](Application/WEBCONSTANTS.md),[NGCONSTANTS](Application/NGCONSTANTS.md),
## **Supported Clients**

    SmartClient
    WebClient
    NGClient
    MobileClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [addClientInfo(info)](Application.md#addclientinfo-info)                   | Adds a string of client information which gets stored on the server, and can be viewed on the Clients page of Servoy Server Administration Console..                                    |
|void | [beep()](Application.md#beep)                   | Produces a "beep" sound; commonly used to indicate an error or warning dialog..                                    |
| [Boolean](JSLib/Boolean.md) | [closeAllWindows()](Application.md#closeallwindows)                   | Close all visible windows (except main application window)..                                    |
|void | [closeSolution()](Application.md#closesolution)                   | Closes the currently open solution and optionally opens another solution, calling a specified global method with the specified arguments..                                    |
|void | [closeSolution(solutionToLoad)](Application.md#closesolution-solutiontoload)                   | Closes the currently open solution and optionally opens another solution, calling a specified global method with the specified arguments..                                    |
|void | [closeSolution(solutionToLoad, methodArgument)](Application.md#closesolution-solutiontoload-methodargument)                   | Closes the currently open solution and optionally opens another solution, calling a specified global method with the specified arguments..                                    |
|void | [closeSolution(solutionToLoad, methodName)](Application.md#closesolution-solutiontoload-methodname)                   | Closes the currently open solution and optionally opens another solution, calling a specified global method with the specified arguments..                                    |
|void | [closeSolution(solutionToLoad, methodName, methodArgument)](Application.md#closesolution-solutiontoload-methodname-methodargument)                   | Closes the currently open solution and optionally opens another solution, calling a specified global method with the specified arguments..                                    |
| [Boolean](JSLib/Boolean.md) | [createNewFormInstance(designFormName, newInstanceScriptName)](Application.md#createnewforminstance-designformname-newinstancescriptname)                   | Create a new form instance..                                    |
| [JSWindow](Application/JSWindow.md) | [createWindow(windowName, type)](Application.md#createwindow-windowname-type)                   | Creates a new window that can be used for displaying forms..                                    |
| [JSWindow](Application/JSWindow.md) | [createWindow(windowName, type, parentWindow)](Application.md#createwindow-windowname-type-parentwindow)                   | Creates a new window that can be used for displaying forms..                                    |
|void | [executeLater(function, delay)](Application.md#executelater-function-delay)                   | Runs at method at the given delay in milliseconds..                                    |
|void | [executeLater(function, delay, arguments)](Application.md#executelater-function-delay-arguments)                   | Runs at method at the given delay in milliseconds with the arguments given to the method..                                    |
| [String](JSLib/String.md) | [executeProgram(program)](Application.md#executeprogram-program)                   | Execute a program and returns output..                                    |
| [String](JSLib/String.md) | [executeProgram(program, params)](Application.md#executeprogram-program-params)                   | Execute a program and returns output..                                    |
| [String](JSLib/String.md) | [executeProgram(program, params, environmentVars)](Application.md#executeprogram-program-params-environmentvars)                   | Execute a program and returns output..                                    |
| [String](JSLib/String.md) | [executeProgram(program, params, environmentVars, startDir)](Application.md#executeprogram-program-params-environmentvars-startdir)                   | Execute a program and returns output..                                    |
|void | [executeProgramInBackground(program)](Application.md#executeprograminbackground-program)                   | Execute a program in the background..                                    |
|void | [executeProgramInBackground(program, params)](Application.md#executeprograminbackground-program-params)                   | Execute a program in the background..                                    |
|void | [executeProgramInBackground(program, params, environmentVars)](Application.md#executeprograminbackground-program-params-environmentvars)                   | Execute a program in the background..                                    |
|void | [executeProgramInBackground(program, params, environmentVars, startDir)](Application.md#executeprograminbackground-program-params-environmentvars-startdir)                   | Execute a program in the background..                                    |
|void | [exit()](Application.md#exit)                   | Stop and exit application..                                    |
| [Object](JSLib/Object.md) | [generateBrowserFunction(functionString)](Application.md#generatebrowserfunction-functionstring)                   | This generates a browser function for the given function string that can be executed in the browser The resulting object can be assigned into a config/property object that is then assigned to a component The component will receive this function as a real function object..                                    |
| [Number](JSLib/Number.md) | [getActiveClientCount(currentSolutionOnly)](Application.md#getactiveclientcount-currentsolutiononly)                   | Get the active user count on the server (can be limited to current solution)..                                    |
| [JSWindow](Application/JSWindow.md) | [getActiveWindow()](Application.md#getactivewindow)                   | This gets the currently focused active window; this can be the main application window or a modal dialog..                                    |
| [Number](JSLib/Number.md) | [getApplicationType()](Application.md#getapplicationtype)                   | Get the application type..                                    |
| [Number](JSLib/Number.md) | [getClientCountForInfo(info)](Application.md#getclientcountforinfo-info)                   | Gets the count for all clients displaying the same additional information in the Clients page of Servoy Server Administration Console..                                    |
| [Object](JSLib/Object.md) | [getClientProperty(name)](Application.md#getclientproperty-name)                   | Sets a UI property..                                    |
| [String](JSLib/String.md) | [getClipboardString()](Application.md#getclipboardstring)                   | Gets a string from the clipboard, null if not a string or empty..                                    |
| [String](JSLib/String.md) | [getCurrentLookAndFeelName()](Application.md#getcurrentlookandfeelname)                   | Gets the name of the current Look And Feel specified in Application Preferences..                                    |
| [String](JSLib/String.md) | [getHostName()](Application.md#gethostname)                   | Get the name of the localhost..                                    |
| [String](JSLib/String.md) | [getIPAddress()](Application.md#getipaddress)                   | Get the clients' IP address..                                    |
| [Array](JSLib/Array.md) | [getLicenseNames()](Application.md#getlicensenames)                   | Get the names of the used client licenses (as strings in array)..                                    |
| [JSLogger](Application/JSLogger.md) | [getLogger()](Application.md#getlogger)                   | Get a JSLogger instance which offers an API for logging with arguments..                                    |
| [JSLogger](Application/JSLogger.md) | [getLogger(loggerName)](Application.md#getlogger-loggername)                   | Get a JSLogger instance which offers an API for logging with arguments..                                    |
| [String](JSLib/String.md) | [getMediaURL(mediaName)](Application.md#getmediaurl-medianame)                   | Get the media url that can be used to server a media in NGClient..                                    |
| [String](JSLib/String.md) | [getOSName()](Application.md#getosname)                   | Returns the name of the operating system of the client..                                    |
| [Array](JSLib/Array.md) | [getPrinters()](Application.md#getprinters)                   | Get all the printer names in an array..                                    |
| [Number](JSLib/Number.md) | [getScreenHeight()](Application.md#getscreenheight)                   | Get the screen height in pixels..                                    |
| [Number](JSLib/Number.md) | [getScreenWidth()](Application.md#getscreenwidth)                   | Get the screen width in pixels..                                    |
| [Date](JSLib/Date.md) | [getServerTimeStamp()](Application.md#getservertimestamp)                   | Returns a date object initialized on server with current date and time..                                    |
| [String](JSLib/String.md) | [getServerURL()](Application.md#getserverurl)                   | Gets the HTTP server url..                                    |
| [String](JSLib/String.md) | [getServerUUID()](Application.md#getserveruuid)                   | Get the uuid from this server instance (the same value that is shown on the admin page).                                    |
| [String](JSLib/String.md) | [getSolutionName()](Application.md#getsolutionname)                   | Returns the name of the current solution..                                    |
| [Number](JSLib/Number.md) | [getSolutionRelease()](Application.md#getsolutionrelease)                   | Get the solution release number..                                    |
| [Array](JSLib/Array.md) | [getStartupArguments()](Application.md#getstartuparguments)                   | Get the parameters which are provided by startup..                                    |
| [Date](JSLib/Date.md) | [getTimeStamp()](Application.md#gettimestamp)                   | Returns a date object initialized in client with current date and time..                                    |
| [UUID](Application/UUID.md) | [getUUID()](Application.md#getuuid)                   | Get a new UUID object (also known as GUID) or convert the parameter (that can be string or byte array) to an UUID object..                                    |
| [UUID](Application/UUID.md) | [getUUID(byteArray)](Application.md#getuuid-bytearray)                   | Get a new UUID object (also known as GUID) or convert the parameter (that can be string or byte array) to an UUID object..                                    |
| [UUID](Application/UUID.md) | [getUUID(uuidString)](Application.md#getuuid-uuidstring)                   | Get a new UUID object (also known as GUID) or convert the parameter (that can be string or byte array) to an UUID object..                                    |
| [String](JSLib/String.md) | [getUserProperty(name)](Application.md#getuserproperty-name)                   | Get a persistent user property..                                    |
| [Array](JSLib/Array.md) | [getUserPropertyNames()](Application.md#getuserpropertynames)                   | Get all persistent user property names..                                    |
| [Array](JSLib/Array.md) | [getValueListArray(name)](Application.md#getvaluelistarray-name)                   | Retrieve a valuelist as array, to get real-values for display-values..                                    |
| [Object](JSLib/Object.md) | [getValueListDisplayValue(name, realValue)](Application.md#getvaluelistdisplayvalue-name-realvalue)                   | Retrieve a valuelist display-value for a real-value..                                    |
| [JSDataSet](Database%20Manager/JSDataSet.md) | [getValueListItems(name)](Application.md#getvaluelistitems-name)                   | Get all values from a custom or database type value list as dataset (with columns displayValue,realValue)..                                    |
| [Array](JSLib/Array.md) | [getValueListNames()](Application.md#getvaluelistnames)                   | Get all the valuelist names as array..                                    |
| [String](JSLib/String.md) | [getVersion()](Application.md#getversion)                   | Returns the application version..                                    |
| [Object](JSLib/Object.md) | [getVersionInfo()](Application.md#getversioninfo)                   | Get the full version information of this solution and all its modules..                                    |
| [JSWindow](Application/JSWindow.md) | [getWindow()](Application.md#getwindow)                   | Get the main application window..                                    |
| [JSWindow](Application/JSWindow.md) | [getWindow(name)](Application.md#getwindow-name)                   | Get a window by window name..                                    |
| [Boolean](JSLib/Boolean.md) | [isInDeveloper()](Application.md#isindeveloper)                   | Returns true if the solution is running in the developer..                                    |
| [Boolean](JSLib/Boolean.md) | [isLastPrintPreviewPrinted()](Application.md#islastprintpreviewprinted)                   | Check if the last printpreview did print..                                    |
|void | [output(msg)](Application.md#output-msg)                   | Output something on the out stream..                                    |
|void | [output(msg, level)](Application.md#output-msg-level)                   | Output something on the out stream..                                    |
|void | [overrideStyle(originalStyleName, newStyleName)](Application.md#overridestyle-originalstylename-newstylename)                   | Overrides one style with another..                                    |
|void | [playSound(url)](Application.md#playsound-url)                   | Play a sound (AU file, an AIFF file, a WAV file, and a MIDI file)..                                    |
| [Boolean](JSLib/Boolean.md) | [putClientProperty(name, value)](Application.md#putclientproperty-name-value)                   | Sets a UI property..                                    |
|void | [redo()](Application.md#redo)                   | Redo last action (if possible)..                                    |
| [Boolean](JSLib/Boolean.md) | [refreshGlobalMethodValueList(element)](Application.md#refreshglobalmethodvaluelist-element)                   | Refresh a global method valuelist by forcing it to call the global method..                                    |
| [Boolean](JSLib/Boolean.md) | [refreshGlobalMethodValueList(element, propertyName)](Application.md#refreshglobalmethodvaluelist-element-propertyname)                   | Refresh a global method valuelist by forcing it to call the global method..                                    |
|void | [removeAllClientInfo()](Application.md#removeallclientinfo)                   | Removes all names given to the client via the admin page..                                    |
|void | [removeAllUserProperties()](Application.md#removealluserproperties)                   | Removes all user properties..                                    |
| [Boolean](JSLib/Boolean.md) | [removeClientInfo(info)](Application.md#removeclientinfo-info)                   | Removes a string of client information which is stored on the server and previously was added using the application..                                    |
|void | [removeUserProperty(name)](Application.md#removeuserproperty-name)                   | Removes a user property..                                    |
|void | [setClipboardContent(string)](Application.md#setclipboardcontent-string)                   | Sets a string object in the clipboard..                                    |
|void | [setNumpadEnterAsFocusNextEnabled(enabled)](Application.md#setnumpadenterasfocusnextenabled-enabled)                   | Set if numpad enter should behave like focus next..                                    |
|void | [setStatusText(text)](Application.md#setstatustext-text)                   | Set the status area value..                                    |
|void | [setStatusText(text, tooltip)](Application.md#setstatustext-text-tooltip)                   | Set the status area value..                                    |
|void | [setToolbarVisible(name, visible)](Application.md#settoolbarvisible-name-visible)                   | Make a toolbar visible or invisible..                                    |
|void | [setUserProperty(name, value)](Application.md#setuserproperty-name-value)                   | Sets a user property for this client: <br> In NGClient this is stored in the locale storage of the browser, so it will be persisted over restarts as long as the user didn't clear the data..                                    |
|void | [setValueListItems(name, dataset)](Application.md#setvaluelistitems-name-dataset)                   | Fill a custom type valuelist with values from array(s) or dataset..                                    |
|void | [setValueListItems(name, dataset, autoconvert)](Application.md#setvaluelistitems-name-dataset-autoconvert)                   | Fill a custom type valuelist with values from array(s) or dataset..                                    |
|void | [setValueListItems(name, displayValues)](Application.md#setvaluelistitems-name-displayvalues)                   | Fill a custom type valuelist with values from array(s) or dataset..                                    |
|void | [setValueListItems(name, displayValues, autoconvert)](Application.md#setvaluelistitems-name-displayvalues-autoconvert)                   | Fill a custom type valuelist with values from array(s) or dataset..                                    |
|void | [setValueListItems(name, displayValues, realValues)](Application.md#setvaluelistitems-name-displayvalues-realvalues)                   | Fill a custom type valuelist with values from array(s) or dataset..                                    |
|void | [setValueListItems(name, displayValues, realValues, autoconvert)](Application.md#setvaluelistitems-name-displayvalues-realvalues-autoconvert)                   | Fill a custom type valuelist with values from array(s) or dataset..                                    |
| [Date](JSLib/Date.md) | [showCalendar()](Application.md#showcalendar)                   | Show the calendar, returns selected date or null if canceled..                                    |
| [Date](JSLib/Date.md) | [showCalendar(dateFormat)](Application.md#showcalendar-dateformat)                   | Show the calendar, returns selected date or null if canceled..                                    |
| [Date](JSLib/Date.md) | [showCalendar(selectedDate)](Application.md#showcalendar-selecteddate)                   | Show the calendar, returns selected date or null if canceled..                                    |
| [Date](JSLib/Date.md) | [showCalendar(selectedDate, dateFormat)](Application.md#showcalendar-selecteddate-dateformat)                   | Show the calendar, returns selected date or null if canceled..                                    |
| [String](JSLib/String.md) | [showColorChooser()](Application.md#showcolorchooser)                   | Show the colorChooser..                                    |
| [String](JSLib/String.md) | [showColorChooser(colorString)](Application.md#showcolorchooser-colorstring)                   | Show the colorChooser..                                    |
| [String](JSLib/String.md) | [showFontChooser()](Application.md#showfontchooser)                   | Show the font chooser dialog..                                    |
| [String](JSLib/String.md) | [showFontChooser(defaultFont)](Application.md#showfontchooser-defaultfont)                   | Show the font chooser dialog..                                    |
|void | [showForm(form)](Application.md#showform-form)                   | Show the form specified by the parameter, that can be a name (is case sensitive!) or a form object..                                    |
| [String](JSLib/String.md) | [showI18NDialog()](Application.md#showi18ndialog)                   | Opens the i18n dialog so users can change translations..                                    |
| [String](JSLib/String.md) | [showI18NDialog(keyToSelect)](Application.md#showi18ndialog-keytoselect)                   | Opens the i18n dialog so users can change translations..                                    |
| [String](JSLib/String.md) | [showI18NDialog(keyToSelect, languageToSelect)](Application.md#showi18ndialog-keytoselect-languagetoselect)                   | Opens the i18n dialog so users can change translations..                                    |
| [Boolean](JSLib/Boolean.md) | [showURL(url)](Application.md#showurl-url)                   | Shows an URL in a browser..                                    |
| [Boolean](JSLib/Boolean.md) | [showURL(url, browserTarget)](Application.md#showurl-url-browsertarget)                   | Shows an URL in a browser..                                    |
| [Boolean](JSLib/Boolean.md) | [showURL(url, browserTarget, timeout)](Application.md#showurl-url-browsertarget-timeout)                   | Shows an URL in a browser..                                    |
| [Boolean](JSLib/Boolean.md) | [showURL(url, browserTarget, browserTargetOptions)](Application.md#showurl-url-browsertarget-browsertargetoptions)                   | Shows an URL in a browser..                                    |
| [Boolean](JSLib/Boolean.md) | [showURL(url, browserTarget, browserTargetOptions, timeout)](Application.md#showurl-url-browsertarget-browsertargetoptions-timeout)                   | Shows an URL in a browser..                                    |
|void | [sleep(ms)](Application.md#sleep-ms)                   | Sleep for specified time (in milliseconds)..                                    |
|void | [undo()](Application.md#undo)                   | Undo last action (if possible)..                                    |
|void | [updateUI()](Application.md#updateui)                   | Updates the UI (painting)..                                    |
|void | [updateUI(milliseconds)](Application.md#updateui-milliseconds)                   | Updates the UI (painting)..                                    |

## Methods Details

### addClientInfo(info)

Adds a string of client information which gets stored on the server,
and can be viewed on the Clients page of Servoy Server Administration Console.

The new piece of client information is added on behalf of the running
Servoy client.

This function can be called more than once, if you want to add multiple
lines of client information.

NOTE:
This function can also be used with the function <em>getClientCountForInfo</em>
to count the number of clients with matching addditional client information.

**Parameters**\
[String](JSLib/String.md) info A line of text to be added as additional client information
            on behalf of the running Servoy client.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.addClientInfo('SaaS company name');
application.addClientInfo('For any issues call +31-SA-AS');
```
### beep()

Produces a "beep" sound; commonly used to indicate an error or warning dialog.


**Returns**\
void 

**Supported Clients**\
SmartClient

**Sample**

```javascript
application.beep();
```
### closeAllWindows()

Close all visible windows (except main application window). Returns true if operation was successful.


**Returns**\
[Boolean](JSLib/Boolean.md) Boolean true if all windows were closed and false otherwise.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var win = application.createWindow("aWindowName", JSWindow.WINDOW, null);
win.setInitialBounds(10, 10, 300, 300);
win.title = "This is a window";
controller.show(win);

var win2 = application.createWindow("anotherWindowName", JSWindow.WINDOW, null);
win2.setInitialBounds(100, 100, 300, 300);
win2.title = "This is another window";
controller.show(win2);

var qdialog = plugins.dialogs.showQuestionDialog("QuestionDialog","Do you want to close the windows?","Yes","No");
if (qdialog == "Yes") {
	application.closeAllWindows();
	controller.show(null);
}
```
### closeSolution()

Closes the currently open solution and optionally opens another solution, calling a specified global method with the specified arguments.
If the user has been logged in, this function keeps the user logged in and in the newly open solution, the login is skipped and the solution goes straight to the first form.
If you want to go to a different url, you need to call application.showURL(url) before calling application.closeSolution() (this is only applicable for Web Client).
An alternative option is security.logout() which also does a log out for the user (for solutions that require authentication).


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//application.showURL('http://www.servoy.com', '_self');  //Web Client only
application.closeSolution();
//close current solution, open solution 'solution_name', call global method 'global_method_name' with argument 'my_argument'.
//if the user has been logged in, he will stay logged in
//application.closeSolution('solution_name','global_method_name','my_argument');
//application.closeSolution('solution_name', {a: 'my_string_argument', p1: 'param1', p2: 'param2'});//close current solution, open solution 'solution_name', call solution's onOpen with argument 'my_argument' and queryParams p1,p2
//Note: specifying a solution will not work in the Developer due to debugger dependencies
//specified solution should be of compatible type with client (normal type or client specific(Smart client only/Web client only) type )
```
### closeSolution(solutionToLoad)

Closes the currently open solution and optionally opens another solution, calling a specified global method with the specified arguments.
If the user has been logged in, this function keeps the user logged in and in the newly open solution, the login is skipped and the solution goes straight to the first form.
If you want to go to a different url, you need to call application.showURL(url) before calling application.closeSolution() (this is only applicable for Web Client).
An alternative option is security.logout() which also does a log out for the user (for solutions that require authentication).

**Parameters**\
[String](JSLib/String.md) solutionToLoad Name of the solution to load

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//application.showURL('http://www.servoy.com', '_self');  //Web Client only
application.closeSolution();
//close current solution, open solution 'solution_name', call global method 'global_method_name' with argument 'my_argument'.
//if the user has been logged in, he will stay logged in
//application.closeSolution('solution_name','global_method_name','my_argument');
//application.closeSolution('solution_name', {a: 'my_string_argument', p1: 'param1', p2: 'param2'});//close current solution, open solution 'solution_name', call solution's onOpen with argument 'my_argument' and queryParams p1,p2
//Note: specifying a solution will not work in the Developer due to debugger dependencies
//specified solution should be of compatible type with client (normal type or client specific(Smart client only/Web client only) type )
```
### closeSolution(solutionToLoad, methodArgument)

Closes the currently open solution and optionally opens another solution, calling a specified global method with the specified arguments.
If the user has been logged in, this function keeps the user logged in and in the newly open solution, the login is skipped and the solution goes straight to the first form.
If you want to go to a different url, you need to call application.showURL(url) before calling application.closeSolution() (this is only applicable for Web Client).
An alternative option is security.logout() which also does a log out for the user (for solutions that require authentication).

**Parameters**\
[String](JSLib/String.md) solutionToLoad Name of the solution to load\
[Object](JSLib/Object.md) methodArgument Argument passed to the solution onOpen

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//application.showURL('http://www.servoy.com', '_self');  //Web Client only
application.closeSolution();
//close current solution, open solution 'solution_name', call global method 'global_method_name' with argument 'my_argument'.
//if the user has been logged in, he will stay logged in
//application.closeSolution('solution_name','global_method_name','my_argument');
//application.closeSolution('solution_name', {a: 'my_string_argument', p1: 'param1', p2: 'param2'});//close current solution, open solution 'solution_name', call solution's onOpen with argument 'my_argument' and queryParams p1,p2
//Note: specifying a solution will not work in the Developer due to debugger dependencies
//specified solution should be of compatible type with client (normal type or client specific(Smart client only/Web client only) type )
```
### closeSolution(solutionToLoad, methodName)

Closes the currently open solution and optionally opens another solution, calling a specified global method with the specified arguments.
If the user has been logged in, this function keeps the user logged in and in the newly open solution, the login is skipped and the solution goes straight to the first form.
If you want to go to a different url, you need to call application.showURL(url) before calling application.closeSolution() (this is only applicable for Web Client).
An alternative option is security.logout() which also does a log out for the user (for solutions that require authentication).

**Parameters**\
[String](JSLib/String.md) solutionToLoad Name of the solution to load\
[String](JSLib/String.md) methodName Name of the global method to call

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//application.showURL('http://www.servoy.com', '_self');  //Web Client only
application.closeSolution();
//close current solution, open solution 'solution_name', call global method 'global_method_name' with argument 'my_argument'.
//if the user has been logged in, he will stay logged in
//application.closeSolution('solution_name','global_method_name','my_argument');
//application.closeSolution('solution_name', {a: 'my_string_argument', p1: 'param1', p2: 'param2'});//close current solution, open solution 'solution_name', call solution's onOpen with argument 'my_argument' and queryParams p1,p2
//Note: specifying a solution will not work in the Developer due to debugger dependencies
//specified solution should be of compatible type with client (normal type or client specific(Smart client only/Web client only) type )
```
### closeSolution(solutionToLoad, methodName, methodArgument)

Closes the currently open solution and optionally opens another solution, calling a specified global method with the specified arguments.
If the user has been logged in, this function keeps the user logged in and in the newly open solution, the login is skipped and the solution goes straight to the first form.
If you want to go to a different url, you need to call application.showURL(url) before calling application.closeSolution() (this is only applicable for Web Client).
An alternative option is security.logout() which also does a log out for the user (for solutions that require authentication).

**Parameters**\
[String](JSLib/String.md) solutionToLoad Name of the solution to load\
[String](JSLib/String.md) methodName Name of the global method to call\
[Object](JSLib/Object.md) methodArgument Argument passed to the global method

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//application.showURL('http://www.servoy.com', '_self');  //Web Client only
application.closeSolution();
//close current solution, open solution 'solution_name', call global method 'global_method_name' with argument 'my_argument'.
//if the user has been logged in, he will stay logged in
//application.closeSolution('solution_name','global_method_name','my_argument');
//application.closeSolution('solution_name', {a: 'my_string_argument', p1: 'param1', p2: 'param2'});//close current solution, open solution 'solution_name', call solution's onOpen with argument 'my_argument' and queryParams p1,p2
//Note: specifying a solution will not work in the Developer due to debugger dependencies
//specified solution should be of compatible type with client (normal type or client specific(Smart client only/Web client only) type )
```
### createNewFormInstance(designFormName, newInstanceScriptName)

Create a new form instance.

**Parameters**\
[String](JSLib/String.md) designFormName Name of the design form\
[String](JSLib/String.md) newInstanceScriptName Name of the new form instance

**Returns**\
[Boolean](JSLib/Boolean.md) Boolean (true) if the instance was created succesfully, (false) otherwise

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var ok = application.createNewFormInstance('orders','orders_view');
if (ok)
{
	var dialog = application.createWindow("myDialog", JSWindow.DIALOG);
 dialog.show('orders_view')
	//forms['orders_view'].controller.show()
	//forms.xyz.elements.myTabPanel.addTab(forms['orders_view'])
	//forms['orders_view'].elements.mylabel.setLocation(10,20)
}
```
### createWindow(windowName, type)

Creates a new window that can be used for displaying forms. Initially the window is not visible.
If there is already a window with the given name, it will be closed and destroyed prior to creating the new window.
Use the form controller show() and showRecords() methods in order to show a form in this window.

**Parameters**\
[String](JSLib/String.md) windowName the name of the window. Should not be null.\
[Number](JSLib/Number.md) type the type of the window. Can be one of JSWindow.DIALOG, JSWindow.MODAL_DIALOG, JSWindow.WINDOW. (WINDOW does not work for NGClient)

**Returns**\
[JSWindow](Application/JSWindow.md) the newly created window.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// create and show a window, with specified title, initial location and size
// type of the window can be one of JSWindow.DIALOG, JSWindow.MODAL_DIALOG, JSWindow.WINDOW (WINDOW does not work for NGClient)
// If parentWindow is not specified, the current window will be used as parent; parentWindow parameter is only used by dialogs
var win = application.createWindow("windowName", JSWindow.WINDOW);
win.setInitialBounds(10, 10, 300, 300);
win.title = "This is a window";
controller.show(win);
// create and show a non-modal dialog with default initial bounds/title
var nmd = application.createWindow("nonModalDialogName", JSWindow.DIALOG);
controller.showRecords(15, nmd); // 15 is a single-number pk in this case
```
### createWindow(windowName, type, parentWindow)

Creates a new window that can be used for displaying forms. Initially the window is not visible.
If there is already a window with the given name, it will be closed and destroyed prior to creating the new window.
Use the form controller show() and showRecords() methods in order to show a form in this window.

**Parameters**\
[String](JSLib/String.md) windowName the name of the window. Should not be null.\
[Number](JSLib/Number.md) type the type of the window. Can be one of JSWindow.DIALOG, JSWindow.MODAL_DIALOG, JSWindow.WINDOW (WINDOW  doesn't work in NGClient).\
[JSWindow](Application/JSWindow.md) parentWindow the parent JSWindow object. If it is not specified, the current window will be used as parent. This parameter is only used by dialogs.

**Returns**\
[JSWindow](Application/JSWindow.md) the newly created window.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// create and show a window, with specified title, initial location and size (WINDOW does not work for NGClient)
var win = application.createWindow("windowName", JSWindow.WINDOW);
win.setInitialBounds(10, 10, 300, 300);
win.title = "This is a window";
controller.show(win);
// create and show a non-modal dialog with default initial bounds/title
var nmd = application.createWindow("nonModalDialogName", JSWindow.DIALOG);
controller.showRecords(15, nmd); // 15 is a single-number pk in this case
```
### executeLater(function, delay)

Runs at method at the given delay in milliseconds.

This is like a simple scheduler to quickly run something after a bit of delay

**Parameters**\
[Function](JSLib/Function.md) function The function to call\
[Number](JSLib/Number.md) delay The millis that has to elapse before the function is called.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### executeLater(function, delay, arguments)

Runs at method at the given delay in milliseconds with the arguments given to the method.

This is like a simple scheduler to quickly run something after a bit of delay

**Parameters**\
[Function](JSLib/Function.md) function The function to call\
[Number](JSLib/Number.md) delay The millis that has to elapse before the function is called.\
[Array](JSLib/Array.md) arguments The arguments that are given to the function when called.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### executeProgram(program)

Execute a program and returns output. Specify the cmd as you would do in a console.

**Parameters**\
[String](JSLib/String.md) program (fullpath) of the program to execute

**Returns**\
[String](JSLib/String.md) The output generated by the program execution.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// For Windows systems:
// Runs a binary located in the user's home directory. The application will run in the current working
// directory, which in general is the one where Servoy was started from.
application.executeProgram("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"]);
// The same as above, but run the application in the user's home directory.
application.executeProgram("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"], null, "c:\\Users\\myself\\");
// The same as above, but also set an environment variable for the called program.
application.executeProgram("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"], ["MY_ENV_VAR=something"], "c:\\Users\\myself\\");
// For non-Windows systems:
application.executeProgram("/home/myself/myapp", ["arg1", "arg2", "arg3"]);
application.executeProgram("/home/myself/myapp", ["arg1", "arg2", "arg3"], null, "/home/myself/");
application.executeProgram("/home/myself/myapp", ["arg1", "arg2", "arg3"], ["MY_ENV_VAR=something"], "/home/myself/");
// Open a file with the default application associated with it. (on Windows)
application.executeProgram("rundll32.exe", ["url.dll,FileProtocolHandler", "filename"]);
// Open a file with the default application associated with it. (on Linux)
application.executeProgram("xdg-open", ["filename"]);
// Open a file with the default application associated with it. (on MacOS)
application.executeProgram("open", ["filename"]);
// Open a file with a specific application (on MacOS).
application.executeProgram("open", ["-a", "OpenOffice.org.app", "filename.doc"]);
```
### executeProgram(program, params)

Execute a program and returns output. Specify the cmd as you would do in a console.

**Parameters**\
[String](JSLib/String.md) program (fullpath) of the program to execute\
[Array](JSLib/Array.md) params an array of strings as program arguments

**Returns**\
[String](JSLib/String.md) The output generated by the program execution.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// For Windows systems:
// Runs a binary located in the user's home directory. The application will run in the current working
// directory, which in general is the one where Servoy was started from.
application.executeProgram("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"]);
// The same as above, but run the application in the user's home directory.
application.executeProgram("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"], null, "c:\\Users\\myself\\");
// The same as above, but also set an environment variable for the called program.
application.executeProgram("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"], ["MY_ENV_VAR=something"], "c:\\Users\\myself\\");
// For non-Windows systems:
application.executeProgram("/home/myself/myapp", ["arg1", "arg2", "arg3"]);
application.executeProgram("/home/myself/myapp", ["arg1", "arg2", "arg3"], null, "/home/myself/");
application.executeProgram("/home/myself/myapp", ["arg1", "arg2", "arg3"], ["MY_ENV_VAR=something"], "/home/myself/");
// Open a file with the default application associated with it. (on Windows)
application.executeProgram("rundll32.exe", ["url.dll,FileProtocolHandler", "filename"]);
// Open a file with the default application associated with it. (on Linux)
application.executeProgram("xdg-open", ["filename"]);
// Open a file with the default application associated with it. (on MacOS)
application.executeProgram("open", ["filename"]);
// Open a file with a specific application (on MacOS).
application.executeProgram("open", ["-a", "OpenOffice.org.app", "filename.doc"]);
```
### executeProgram(program, params, environmentVars)

Execute a program and returns output. Specify the cmd as you would do in a console.

**Parameters**\
[String](JSLib/String.md) program (fullpath) of the program to execute\
[Array](JSLib/Array.md) params an array of strings as program arguments\
[Array](JSLib/Array.md) environmentVars array of strings, each element of which has environment variable settings in the format name=value, or null if the subprocess should inherit the environment of the current process.

**Returns**\
[String](JSLib/String.md) The output generated by the program execution.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// For Windows systems:
// Runs a binary located in the user's home directory. The application will run in the current working
// directory, which in general is the one where Servoy was started from.
application.executeProgram("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"]);
// The same as above, but run the application in the user's home directory.
application.executeProgram("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"], null, "c:\\Users\\myself\\");
// The same as above, but also set an environment variable for the called program.
application.executeProgram("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"], ["MY_ENV_VAR=something"], "c:\\Users\\myself\\");
// For non-Windows systems:
application.executeProgram("/home/myself/myapp", ["arg1", "arg2", "arg3"]);
application.executeProgram("/home/myself/myapp", ["arg1", "arg2", "arg3"], null, "/home/myself/");
application.executeProgram("/home/myself/myapp", ["arg1", "arg2", "arg3"], ["MY_ENV_VAR=something"], "/home/myself/");
// Open a file with the default application associated with it. (on Windows)
application.executeProgram("rundll32.exe", ["url.dll,FileProtocolHandler", "filename"]);
// Open a file with the default application associated with it. (on Linux)
application.executeProgram("xdg-open", ["filename"]);
// Open a file with the default application associated with it. (on MacOS)
application.executeProgram("open", ["filename"]);
// Open a file with a specific application (on MacOS).
application.executeProgram("open", ["-a", "OpenOffice.org.app", "filename.doc"]);
```
### executeProgram(program, params, environmentVars, startDir)

Execute a program and returns output. Specify the cmd as you would do in a console.

**Parameters**\
[String](JSLib/String.md) program (fullpath) of the program to execute\
[Array](JSLib/Array.md) params an array of strings as program arguments\
[Array](JSLib/Array.md) environmentVars array of strings, each element of which has environment variable settings in the format name=value, or null if the subprocess should inherit the environment of the current process.\
[String](JSLib/String.md) startDir the working directory of the subprocess, or null if the subprocess should inherit the working directory of the current process.

**Returns**\
[String](JSLib/String.md) The output generated by the program execution.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// For Windows systems:
// Runs a binary located in the user's home directory. The application will run in the current working
// directory, which in general is the one where Servoy was started from.
application.executeProgram("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"]);
// The same as above, but run the application in the user's home directory.
application.executeProgram("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"], null, "c:\\Users\\myself\\");
// The same as above, but also set an environment variable for the called program.
application.executeProgram("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"], ["MY_ENV_VAR=something"], "c:\\Users\\myself\\");
// For non-Windows systems:
application.executeProgram("/home/myself/myapp", ["arg1", "arg2", "arg3"]);
application.executeProgram("/home/myself/myapp", ["arg1", "arg2", "arg3"], null, "/home/myself/");
application.executeProgram("/home/myself/myapp", ["arg1", "arg2", "arg3"], ["MY_ENV_VAR=something"], "/home/myself/");
// Open a file with the default application associated with it. (on Windows)
application.executeProgram("rundll32.exe", ["url.dll,FileProtocolHandler", "filename"]);
// Open a file with the default application associated with it. (on Linux)
application.executeProgram("xdg-open", ["filename"]);
// Open a file with the default application associated with it. (on MacOS)
application.executeProgram("open", ["filename"]);
// Open a file with a specific application (on MacOS).
application.executeProgram("open", ["-a", "OpenOffice.org.app", "filename.doc"]);
```
### executeProgramInBackground(program)

Execute a program in the background. Specify the cmd as you would do in a console.

**Parameters**\
[String](JSLib/String.md) program (fullpath) of the program to execute

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// For Windows systems:
// Runs a binary located in the user's home directory. The application will run in the current working
// directory, which in general is the one where Servoy was started from.
application.executeProgramInBackground("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"]);
// The same as above, but run the application in the user's home directory.
application.executeProgramInBackground("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"], null, "c:\\Users\\myself\\");
// The same as above, but also set an environment variable for the called program.
application.executeProgramInBackground("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"], ["MY_ENV_VAR=something"], "c:\\Users\\myself\\");
// For non-Windows systems:
application.executeProgramInBackground("/home/myself/myapp", ["arg1", "arg2", "arg3"]);
application.executeProgramInBackground("/home/myself/myapp", ["arg1", "arg2", "arg3"], null, "/home/myself/");
application.executeProgramInBackground("/home/myself/myapp", ["arg1", "arg2", "arg3"], ["MY_ENV_VAR=something"], "/home/myself/");
// Open a file with the default application associated with it. (on Windows)
application.executeProgramInBackground("rundll32.exe", ["url.dll,FileProtocolHandler", "filename"]);
// Open a file with the default application associated with it. (on Linux)
application.executeProgramInBackground("xdg-open", ["filename"]);
// Open a file with the default application associated with it. (on MacOS)
application.executeProgramInBackground("open", ["filename"]);
// Open a file with a specific application (on MacOS).
application.executeProgram("open", ["-a", "OpenOffice.org.app", "filename.doc"]);
```
### executeProgramInBackground(program, params)

Execute a program in the background. Specify the cmd as you would do in a console.

**Parameters**\
[String](JSLib/String.md) program (fullpath) of the program to execute\
[Array](JSLib/Array.md) params an array of strings as program arguments

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// For Windows systems:
// Runs a binary located in the user's home directory. The application will run in the current working
// directory, which in general is the one where Servoy was started from.
application.executeProgramInBackground("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"]);
// The same as above, but run the application in the user's home directory.
application.executeProgramInBackground("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"], null, "c:\\Users\\myself\\");
// The same as above, but also set an environment variable for the called program.
application.executeProgramInBackground("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"], ["MY_ENV_VAR=something"], "c:\\Users\\myself\\");
// For non-Windows systems:
application.executeProgramInBackground("/home/myself/myapp", ["arg1", "arg2", "arg3"]);
application.executeProgramInBackground("/home/myself/myapp", ["arg1", "arg2", "arg3"], null, "/home/myself/");
application.executeProgramInBackground("/home/myself/myapp", ["arg1", "arg2", "arg3"], ["MY_ENV_VAR=something"], "/home/myself/");
// Open a file with the default application associated with it. (on Windows)
application.executeProgramInBackground("rundll32.exe", ["url.dll,FileProtocolHandler", "filename"]);
// Open a file with the default application associated with it. (on Linux)
application.executeProgramInBackground("xdg-open", ["filename"]);
// Open a file with the default application associated with it. (on MacOS)
application.executeProgramInBackground("open", ["filename"]);
// Open a file with a specific application (on MacOS).
application.executeProgram("open", ["-a", "OpenOffice.org.app", "filename.doc"]);
```
### executeProgramInBackground(program, params, environmentVars)

Execute a program in the background. Specify the cmd as you would do in a console.

**Parameters**\
[String](JSLib/String.md) program (fullpath) of the program to execute\
[Array](JSLib/Array.md) params an array of strings as program arguments\
[Array](JSLib/Array.md) environmentVars array of strings, each element of which has environment variable settings in the format name=value, or null if the subprocess should inherit the environment of the current process.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// For Windows systems:
// Runs a binary located in the user's home directory. The application will run in the current working
// directory, which in general is the one where Servoy was started from.
application.executeProgramInBackground("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"]);
// The same as above, but run the application in the user's home directory.
application.executeProgramInBackground("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"], null, "c:\\Users\\myself\\");
// The same as above, but also set an environment variable for the called program.
application.executeProgramInBackground("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"], ["MY_ENV_VAR=something"], "c:\\Users\\myself\\");
// For non-Windows systems:
application.executeProgramInBackground("/home/myself/myapp", ["arg1", "arg2", "arg3"]);
application.executeProgramInBackground("/home/myself/myapp", ["arg1", "arg2", "arg3"], null, "/home/myself/");
application.executeProgramInBackground("/home/myself/myapp", ["arg1", "arg2", "arg3"], ["MY_ENV_VAR=something"], "/home/myself/");
// Open a file with the default application associated with it. (on Windows)
application.executeProgramInBackground("rundll32.exe", ["url.dll,FileProtocolHandler", "filename"]);
// Open a file with the default application associated with it. (on Linux)
application.executeProgramInBackground("xdg-open", ["filename"]);
// Open a file with the default application associated with it. (on MacOS)
application.executeProgramInBackground("open", ["filename"]);
// Open a file with a specific application (on MacOS).
application.executeProgram("open", ["-a", "OpenOffice.org.app", "filename.doc"]);
```
### executeProgramInBackground(program, params, environmentVars, startDir)

Execute a program in the background. Specify the cmd as you would do in a console.

**Parameters**\
[String](JSLib/String.md) program (fullpath) of the program to execute\
[Array](JSLib/Array.md) params an array of strings as program arguments\
[Array](JSLib/Array.md) environmentVars array of strings, each element of which has environment variable settings in the format name=value, or null if the subprocess should inherit the environment of the current process.\
[String](JSLib/String.md) startDir the working directory of the subprocess, or null if the subprocess should inherit the working directory of the current process.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// For Windows systems:
// Runs a binary located in the user's home directory. The application will run in the current working
// directory, which in general is the one where Servoy was started from.
application.executeProgramInBackground("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"]);
// The same as above, but run the application in the user's home directory.
application.executeProgramInBackground("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"], null, "c:\\Users\\myself\\");
// The same as above, but also set an environment variable for the called program.
application.executeProgramInBackground("c:\\Users\\myself\\myapp.exe", ["arg1", "arg2", "arg3"], ["MY_ENV_VAR=something"], "c:\\Users\\myself\\");
// For non-Windows systems:
application.executeProgramInBackground("/home/myself/myapp", ["arg1", "arg2", "arg3"]);
application.executeProgramInBackground("/home/myself/myapp", ["arg1", "arg2", "arg3"], null, "/home/myself/");
application.executeProgramInBackground("/home/myself/myapp", ["arg1", "arg2", "arg3"], ["MY_ENV_VAR=something"], "/home/myself/");
// Open a file with the default application associated with it. (on Windows)
application.executeProgramInBackground("rundll32.exe", ["url.dll,FileProtocolHandler", "filename"]);
// Open a file with the default application associated with it. (on Linux)
application.executeProgramInBackground("xdg-open", ["filename"]);
// Open a file with the default application associated with it. (on MacOS)
application.executeProgramInBackground("open", ["filename"]);
// Open a file with a specific application (on MacOS).
application.executeProgram("open", ["-a", "OpenOffice.org.app", "filename.doc"]);
```
### exit()

Stop and exit application.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// exit application
application.exit();
```
### generateBrowserFunction(functionString)

This generates a browser function for the given function string that can be executed in the browser
The resulting object can be assigned into a config/property object that is then assigned to a component
The component will receive this function as a real function object.

This is a more dynamic variant of the spec property "clientfunction" https://wiki.servoy.com/display/DOCS/Property+Types

**Parameters**\
[String](JSLib/String.md) functionString The function string of a js function that should be running in the clients browser.

**Returns**\
[Object](JSLib/Object.md) An object that can be assignd to a javascript/json object that is send to the client

**Supported Clients**\
NGClient

**Sample**

```javascript
var options = { myfunction: application.generateBrowserFunction("function(param) { return param + 1 }") };
elements.component.setOptions(options);
```
### getActiveClientCount(currentSolutionOnly)

Get the active user count on the server (can be limited to current solution).

**Parameters**\
[Boolean](JSLib/Boolean.md) currentSolutionOnly Boolean (true) to get the active user count on server only to the current solution

**Returns**\
[Number](JSLib/Number.md) Active user count on the server

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var count = application.getActiveClientCount(true);
```
### getActiveWindow()

This gets the currently focused active window; this can be the main application window or a modal dialog.
For a webclient getWindow() can return the main window that is not really the main for the current tab in the browser
that can return the previous tab that a user could have opened. For this method is better suited because this
will give you the actual tab in the browser. Another call would be form.controller.getWindow() of a form that you know in which window it resides.


**Returns**\
[JSWindow](Application/JSWindow.md) the current active/focussed window.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// get the currently active/focused window or dialog
var activeWindow = application.getActiveWindow();
```
### getApplicationType()

Get the application type.


**Returns**\
[Number](JSLib/Number.md) Constant application type

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var type = application.getApplicationType();
//see application type contstant
```
### getClientCountForInfo(info)

Gets the count for all clients displaying the same additional information
in the Clients page of Servoy Server Administration Console.

**Parameters**\
[String](JSLib/String.md) info The additional client info string to search for.

**Returns**\
[Number](JSLib/Number.md) Number of clients

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var count = application.getClientCountForInfo('SaaS company name');
application.output('Including yourself, there are ' + count + ' client(s) running on behalf of the company.');
```
### getClientProperty(name)

Sets a UI property.

**Parameters**\
[Object](JSLib/Object.md) name Name of the client property

**Returns**\
[Object](JSLib/Object.md) the property value for the given name/key, null of nothing was found

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//Only use this function from the solution on open method!
//In smart client, use this to set javax.swing.UIDefaults properties.
application.putClientProperty('ToolTip.hideAccelerator', true)
//To change the comboboxes selection background color, do this:
application.putClientProperty('ComboBox.selectionBackground', new Packages.javax.swing.plaf.ColorUIResource(java.awt.Color.RED))

//In web client, use this to change the template directory.
//To change the default dir of templates/default to templates/green_skin, do this:
application.putClientProperty('templates.dir','green_skin');
```
### getClipboardString()

Gets a string from the clipboard, null if not a string or empty.


**Returns**\
[String](JSLib/String.md) The string from the clipboard

**Supported Clients**\
SmartClient,NGClient

**Sample**

```javascript
var fromClipboard = application.getClipboardString();
```
### getCurrentLookAndFeelName()

Gets the name of the current Look And Feel specified in Application Preferences.


**Returns**\
[String](JSLib/String.md) Current Look And Feel

**Supported Clients**\
SmartClient

**Sample**

```javascript
var laf = application.getCurrentLookAndFeelName();
```
### getHostName()

Get the name of the localhost.


**Returns**\
[String](JSLib/String.md) Name of the localhost

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var hostName = application.getHostName();
```
### getIPAddress()

Get the clients' IP address.


**Returns**\
[String](JSLib/String.md) IP address of the client

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var ip = application.getIPAddress();
```
### getLicenseNames()

Get the names of the used client licenses (as strings in array).


**Returns**\
[Array](JSLib/Array.md) Client licenses names

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var array = application.getLicenseNames();
```
### getLogger()

Get a JSLogger instance which offers an API for logging with arguments.
Available logging levels are (in order): fatal, error, warn, info, debug and trace.
If no loggerName is given to this method, it returns the default logger (LoggerFactory.getLogger(Debug.class))
NOTE: the default logging level of the the default logger is 'warn', so info, debug and trace events are not logged.


**Returns**\
[JSLogger](Application/JSLogger.md) a new JSLogger instance

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var log = application.getLogger(); // returns the default logger.
application.output("is logging level 'warn' enabled? " + log.isWarnEnabled); // if false, next line won't log
log.warn.log("this logger logs {} {} {}", "all", "my", "arguments");
```
### getLogger(loggerName)

Get a JSLogger instance which offers an API for logging with arguments.
Available logging levels are (in order): fatal, error, warn, info, debug and trace.
The argument should be the name of a logger that is configured in myServoyInstallationDir/application_server/log4j.xml.
A new logger can be configured in log4j.xml by adding the following line:
<Logger name="myLogger" level="INFO"/>

**Parameters**\
[String](JSLib/String.md) loggerName the name of the logger, as configured in log4j.xml

**Returns**\
[JSLogger](Application/JSLogger.md) a new JSLogger instance

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var log = application.getLogger("myLogger");
application.output("is logging level 'warn' enabled? " + log.isWarnEnabled); // if false, next line won't log
log.warn.log("this logger logs {} {} {}", "all", "my", "arguments");
```
### getMediaURL(mediaName)

Get the media url that can be used to server a media in NGClient.

**Parameters**\
[String](JSLib/String.md) mediaName Name of the media

**Returns**\
[String](JSLib/String.md) 

**Supported Clients**\
NGClient

**Sample**

```javascript
application.getMediaURL('solution.css');
```
### getOSName()

Returns the name of the operating system of the client.
In Smart Client this will return os.name system property. In Web/NG Client will return "OSFamily majorVersion.minorVersion".


**Returns**\
[String](JSLib/String.md) Name of the operating system of the client

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var osname = application.getOSName();
```
### getPrinters()

Get all the printer names in an array.


**Returns**\
[Array](JSLib/Array.md) All printer names

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
var printersArray = application.getPrinters();
```
### getScreenHeight()

Get the screen height in pixels.


**Returns**\
[Number](JSLib/Number.md) Screen height

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var height = application.getScreenHeight();
```
### getScreenWidth()

Get the screen width in pixels.


**Returns**\
[Number](JSLib/Number.md) Screen width

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var width = application.getScreenWidth();
```
### getServerTimeStamp()

Returns a date object initialized on server with current date and time.
For NG and web clients this is the same as new Date() in scripting.


**Returns**\
[Date](JSLib/Date.md) Server time

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var servertime = application.getServerTimeStamp();
```
### getServerURL()

Gets the HTTP server url.

This url will end with a / so don't append to this server url something that starts with a / again
because RFC 3986 says that the path of a url (the part after the domain[:poort]) can not start with 2 slashes.


**Returns**\
[String](JSLib/String.md) HTTP server URL

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var url = application.getServerURL();
```
### getServerUUID()

Get the uuid from this server instance (the same value that is shown on the admin page)


**Returns**\
[String](JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var uuid = application.getServerUUID();
```
### getSolutionName()

Returns the name of the current solution.


**Returns**\
[String](JSLib/String.md) Current solution name

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var solutionName = application.getSolutionName();
```
### getSolutionRelease()

Get the solution release number.


**Returns**\
[Number](JSLib/Number.md) Current solution release number

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var release = application.getSolutionRelease();
```
### getStartupArguments()

Get the parameters which are provided by startup.
It returns an array with 2 elements, a string that is the startup argument and a map containing all named startup arguments, or
null if there is no argument passed


**Returns**\
[Array](JSLib/Array.md) Array with 2 elements, a string that is the startup argument and a map containing all named startup arguments,
or null if there is no argument passed

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var args_array = application.getStartupArguments();
// the first element in the array is the 'argument' value from the startup
var argument = args_array[0];
// the second element is a map  containing all the named startup arguments
var startupArgumentObj = args_array[1];
var arg1 = startupArgumentObj['arg1_name'];
var arg2 = startupArgumentObj['arg2_name'];
```
### getTimeStamp()

Returns a date object initialized in client with current date and time.
This should be used instead of new Date() for webclients when the clients are in different times zones then the server.
Then this call will really return a time that is the locals webclients time.
For NG clients this is only useful when displaying on the client using format property (Use local time), and then
this is equivalent to new Date() on the client side, so basically this can be used to pre-fill with 'now' such a display.


**Returns**\
[Date](JSLib/Date.md) Current time at the client

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var clienttime = application.getTimeStamp();
```
### getUUID()

Get a new UUID object (also known as GUID) or convert the parameter (that can be string or byte array) to an UUID object. A table column marked as UUID will work with such objects.


**Returns**\
[UUID](Application/UUID.md) The new UUID object

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var new_uuid_object = application.getUUID(); // generate new uuid object
var uuid_object1 = application.getUUID(new_uuid_object.toString()); // convert a string representing an uuid to an uuid object
var uuid_object2 = application.getUUID(new_uuid_object.toBytes());  // convert a byte array representing an uuid to an uuid object
```
### getUUID(byteArray)

Get a new UUID object (also known as GUID) or convert the parameter (that can be string or byte array) to an UUID object. A table column marked as UUID will work with such objects.

**Parameters**\
[Array](JSLib/Array.md) byteArray Byte array representing an uuid

**Returns**\
[UUID](Application/UUID.md) The new UUID object

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var new_uuid_object = application.getUUID(); // generate new uuid object
var uuid_object1 = application.getUUID(new_uuid_object.toString()); // convert a string representing an uuid to an uuid object
var uuid_object2 = application.getUUID(new_uuid_object.toBytes());  // convert a byte array representing an uuid to an uuid object
```
### getUUID(uuidString)

Get a new UUID object (also known as GUID) or convert the parameter (that can be string or byte array) to an UUID object. A table column marked as UUID will work with such objects.

**Parameters**\
[String](JSLib/String.md) uuidString String representing an uuid

**Returns**\
[UUID](Application/UUID.md) The new UUID object

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var new_uuid_object = application.getUUID(); // generate new uuid object
var uuid_object1 = application.getUUID(new_uuid_object.toString()); // convert a string representing an uuid to an uuid object
var uuid_object2 = application.getUUID(new_uuid_object.toBytes());  // convert a byte array representing an uuid to an uuid object
```
### getUserProperty(name)

Get a persistent user property.

In NGClient this is stored in the locale storage of the browser, so it will be persisted over restarts as long as the user didn't clear the data.

**Parameters**\
[String](JSLib/String.md) name Name of the property

**Returns**\
[String](JSLib/String.md) Property value

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var value = application.getUserProperty('showOrders');
```
### getUserPropertyNames()

Get all persistent user property names.


**Returns**\
[Array](JSLib/Array.md) Array of all user property names

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// display all user properties
allPropertyNames = application.getUserPropertyNames();
for(var i = 0; i < allPropertyNames.length; i++)
{
	application.output(allPropertyNames[i] + " = " + application.getUserProperty(allPropertyNames[i]));
}
```
### getValueListArray(name)

Retrieve a valuelist as array, to get real-values for display-values.
NOTE: this doesn't return a value for a valuelist that depends on a database relation or is a global method valuelist.

**Parameters**\
[String](JSLib/String.md) name The name of the valuelist

**Returns**\
[Array](JSLib/Array.md) Named array for the valuelist

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var packet_types = application.getValueListArray('packet_types');
if (a_realValue == packet_types['displayValue'])
{
}
```
### getValueListDisplayValue(name, realValue)

Retrieve a valuelist display-value for a real-value.
NOTE: this doesn't return a value for a valuelist that depends on a database relation or is a global method valuelist.

**Parameters**\
[String](JSLib/String.md) name Name of the valuelist\
[Object](JSLib/Object.md) realValue Real value of the valuelist

**Returns**\
[Object](JSLib/Object.md) Display value of the real value from the valuelist

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var displayable_status = application.getValueListDisplayValue('case_status',status);
```
### getValueListItems(name)

Get all values from a custom or database type value list as dataset (with columns displayValue,realValue).
NOTE: this doesn't return a value for a valuelist that depends on a database relation or is a global method valuelist.

**Parameters**\
[String](JSLib/String.md) name Name of the valuelist

**Returns**\
[JSDataSet](Database%20Manager/JSDataSet.md) DataSet with valuelist's display values and real values

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//Note:see databaseManager.JSDataSet for full details of dataset
var dataset = application.getValueListItems('my_en_types');
//example to calc a strange total
global_total = 0;
for( var i = 1 ; i <= dataset.getMaxRowIndex() ; i++ )
{
	global_total = global_total + dataset.getValue(i,1);
}
//example to assign to dataprovider
//employee_salary = dataset.getValue(1,1)
```
### getValueListNames()

Get all the valuelist names as array.


**Returns**\
[Array](JSLib/Array.md) Array with all valuelist names

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var array = application.getValueListNames();
```
### getVersion()

Returns the application version.


**Returns**\
[String](JSLib/String.md) Application version

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.getVersion();
```
### getVersionInfo()

Get the full version information of this solution and all its modules.
This will return an object that is a map of Name(Sting)->Version(String) of the solution and all its modules.


**Returns**\
[Object](JSLib/Object.md) Name->Version map object.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### getWindow()

Get the main application window. This is the window that is created first for this client.

In a smart client this is always just the first started window where the solution is loaded in.
In a webclient the user may open the same solution in a new tab in the same browser. In that case the main solution
window will always be the first opened tab, even if that one was already closed.
application.getActiveWindow() will always return the currently active/focused window or dialog.
If you need the window of the current top-level form, controller.getWindow() of that form will
always return the correct window.


**Returns**\
[JSWindow](Application/JSWindow.md) the main application JSWindow.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// close and dispose window resources
var mainAppWindow = application.getWindow();
```
### getWindow(name)

Get a window by window name. When not supplying a name, the main application window is grabbed.

**Parameters**\
[String](JSLib/String.md) name the name of the window. If not specified, the main application JSWindow will be returned.

**Returns**\
[JSWindow](Application/JSWindow.md) the JSWindow with the specified name, or null if no such window exists.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// close and dispose window resources
var win = application.getWindow("someWindowName");
if (win != null) {
	win.destroy();
}
```
### isInDeveloper()

Returns true if the solution is running in the developer.


**Returns**\
[Boolean](JSLib/Boolean.md) Boolean (true) if the solution is running in the developer, (false) otherwise

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var flag = application.isInDeveloper();
```
### isLastPrintPreviewPrinted()

Check if the last printpreview did print.


**Returns**\
[Boolean](JSLib/Boolean.md) Boolean (true) is the last print preview did print, (false) otherwise

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
//attached this method to onShow on the form being shown after printpreview
//set a global called scopes.globals.showPrintPreview to 1 in the onPrintPreview method
if (scopes.globals.showPrintPreview == 1)
{
	scopes.globals.showPrintPreview = 0;//clear for next time
	if (application.isLastPrintPreviewPrinted())
	{
		plugins.dialogs.showInfoDialog('Alert',  'There is printed in printpreview',  'OK')
	}
}
```
### output(msg)

Output something on the out stream. (if running in debugger view output console tab)

**Parameters**\
[Object](JSLib/Object.md) msg Object to send to output stream

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
// log level is used to determine how/if to log in servoy_log.txt; for smart client java out and err streams are used
application.output('my very important trace msg');// default log level: info
```
### output(msg, level)

Output something on the out stream. (if running in debugger view output console tab)

**Parameters**\
[Object](JSLib/Object.md) msg Object to send to output stream\
[Number](JSLib/Number.md) level the log level where it should log to.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// log level is used to determine how/if to log in servoy_log.txt; for smart client java out and err streams are used
application.output('my very important msg',LOGGINGLEVEL.ERROR);// log level: error
```
### overrideStyle(originalStyleName, newStyleName)

Overrides one style with another. In NGClient, it overrides the original stylesheet media defined on a solution with another media.

**Parameters**\
[String](JSLib/String.md) originalStyleName Name of the style to override\
[String](JSLib/String.md) newStyleName Name of the new style

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
// Smart Client/Web Client usage
//This function will only have effect on  forms not yet created, so solution onLoad is the best place to override'
//For example overriding the use of default/designed style anywhere in the solution from 'mystyle' to 'mystyle_mac'
application.overrideStyle('mystyle','mystyle_mace')//in this case both styles should have about the same classes

//NGClient usage
application.overrideStyle('oldstylesheet.css','mystylesheets/newstylesheet.css');
//Also less is supported also with compiling it at runtime
applicaiton.overrideStyle('solution.less', 'tenant.less'); // tenant.less can be a solution model changed or generated file, then it will be recompiled at runtime.
```
### playSound(url)

Play a sound (AU file, an AIFF file, a WAV file, and a MIDI file).

**Parameters**\
[String](JSLib/String.md) url URL of the sound file

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
application.playSound('media:///click.wav');
```
### putClientProperty(name, value)

Sets a UI property.

**Parameters**\
[Object](JSLib/Object.md) name Name of the client property\
[Object](JSLib/Object.md) value New value of the client property

**Returns**\
[Boolean](JSLib/Boolean.md) Boolean (true) if the client property was set with the new value

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//Only use this function from the solution on open method!
//In smart client, use this to set javax.swing.UIDefaults properties.
application.putClientProperty('ToolTip.hideAccelerator', true)
//To change the comboboxes selection background color, do this:
application.putClientProperty('ComboBox.selectionBackground', new Packages.javax.swing.plaf.ColorUIResource(java.awt.Color.RED))

//In web client, use this to change the template directory.
//To change the default dir of templates/default to templates/green_skin, do this:
application.putClientProperty('templates.dir','green_skin');
```
### redo()

Redo last action (if possible).


**Returns**\
void 

**Supported Clients**\
SmartClient

**Sample**

```javascript
application.redo();
```
### refreshGlobalMethodValueList(element)

Refresh a global method valuelist by forcing it to call the global method. The element which has the valuelist must be provided.
If there is no propertyName specified, the element must have only one valuelist property.

**Parameters**\
[Object](JSLib/Object.md) element form element

**Returns**\
[Boolean](JSLib/Boolean.md) boolean indicating if valuelist was refreshed

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.refreshGlobalMethodValueList(elements.mytypeahead);
```
### refreshGlobalMethodValueList(element, propertyName)

Refresh a global method valuelist by forcing it to call the global method. The element which has the valuelist must be provided.
The valuelist is searched under provided property from the spec - for usage in NGClient custom components.

**Parameters**\
[Object](JSLib/Object.md) element form element\
[String](JSLib/String.md) propertyName name of property from the spec

**Returns**\
[Boolean](JSLib/Boolean.md) boolean indicating if valuelist was refreshed

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.refreshGlobalMethodValueList(elements.mycustomcomponent,'myvaluelistProperty');
```
### removeAllClientInfo()

Removes all names given to the client via the admin page.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.removeAllClientInfo();
```
### removeAllUserProperties()

Removes all user properties.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### removeClientInfo(info)

Removes a string of client information which is stored on the server and
previously was added using the application.addClientInfo('client info')

This function can be called more than once, if you want to delete multiple
lines of client information.

**Parameters**\
[String](JSLib/String.md) info A line of text to be removed from the client information
            on behalf of the running Servoy client.

**Returns**\
[Boolean](JSLib/Boolean.md) boolean indicator if info was removed successfully

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var removed = application.removeClientInfo('SaaS company name');
```
### removeUserProperty(name)

Removes a user property.

**Parameters**\
[String](JSLib/String.md) name Name of the user property

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### setClipboardContent(string)

Sets a string object in the clipboard.

**Parameters**\
[Object](JSLib/Object.md) string New content of the clipboard

**Returns**\
void 

**Supported Clients**\
SmartClient,NGClient

**Sample**

```javascript
application.setClipboardContent('test');
```
### setNumpadEnterAsFocusNextEnabled(enabled)

Set if numpad enter should behave like focus next.

**Parameters**\
[Boolean](JSLib/Boolean.md) enabled Boolean (true) if numpad enter should behave like focus next

**Returns**\
void 

**Supported Clients**\
SmartClient

**Sample**

```javascript
application.setNumpadEnterAsFocusNextEnabled(true);
```
### setStatusText(text)

Set the status area value.

**Parameters**\
[String](JSLib/String.md) text New status text

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
application.setStatusText('Your status text');
```
### setStatusText(text, tooltip)

Set the status area value.

NOTE: Most modern browsers do not support status bar and status text anymore. This method sets status property of the window using javascript.

**Parameters**\
[String](JSLib/String.md) text New status text\
[String](JSLib/String.md) tooltip Status tooltip text

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient

**Sample**

```javascript
application.setStatusText('Your status text','Your status tooltip text');
```
### setToolbarVisible(name, visible)

Make a toolbar visible or invisible.

**Parameters**\
[String](JSLib/String.md) name Name of the toolbar\
[Boolean](JSLib/Boolean.md) visible Visibility of the toolbar

**Returns**\
void 

**Supported Clients**\
SmartClient

**Sample**

```javascript
//example: hide the text toolbar
application.setToolbarVisible('text',false);
```
### setUserProperty(name, value)

Sets a user property for this client: 
In NGClient this is stored in the locale storage of the browser, so it will be persisted over restarts as long as the user didn't clear the data.

For headless clients(including Batch Processors and Authentication clients) the user property is stored in memory and will be lost upon client restart.

For Web Client the user property will be stored in a persistent cookie

For Smart Client it will be stored in a properties file on the client machine.

**Parameters**\
[String](JSLib/String.md) name Name of the user property\
[String](JSLib/String.md) value New value of the user property

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
application.setUserProperty('showOrders','1');
```
### setValueListItems(name, dataset)

Fill a custom type valuelist with values from array(s) or dataset.

NOTE: if you modify values for checkbox/radio field, note that having one value in valuelist is a special case, so switching between one value and 0/multiple values may have side effects
NOTE: This is expensive operation, which triggers refresh of all visible forms. Over usage of this method may inflict performance issues.

**Parameters**\
[String](JSLib/String.md) name Name of the valuelist\
[JSDataSet](Database%20Manager/JSDataSet.md) dataset Dataset with display/real values

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//set display values (return values will be same as display values)
application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'));
//set display values and return values (which are stored in dataprovider)
//application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'),new Array(10000,10010,10456));
//set display values and return values converted to numbers
//application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'),new Array('10000','10010', '10456'), true);
//do query and fill valuelist (see databaseManager for full details of queries/dataset)
//var query = 'select display_value,optional_real_value from test_table';
//var dataset = databaseManager.getDataSetByQuery(databaseManager.getDataSourceServerName(controller.getDataSource()), query, null, 25);

//application.setValueListItems('my_en_types',dataset);
```
### setValueListItems(name, dataset, autoconvert)

Fill a custom type valuelist with values from array(s) or dataset.

NOTE: if you modify values for checkbox/radio field, note that having one value in valuelist is a special case, so switching between one value and 0/multiple values may have side effects
NOTE: This is expensive operation, which triggers refresh of all visible forms. Over usage of this method may inflict performance issues.

**Parameters**\
[String](JSLib/String.md) name Name of the valuelist\
[JSDataSet](Database%20Manager/JSDataSet.md) dataset Dataset with display/real values\
[Boolean](JSLib/Boolean.md) autoconvert Boolean (true) if display values and return values should be converted to numbers

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//set display values (return values will be same as display values)
application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'));
//set display values and return values (which are stored in dataprovider)
//application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'),new Array(10000,10010,10456));
//set display values and return values converted to numbers
//application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'),new Array('10000','10010', '10456'), true);
//do query and fill valuelist (see databaseManager for full details of queries/dataset)
//var query = 'select display_value,optional_real_value from test_table';
//var dataset = databaseManager.getDataSetByQuery(databaseManager.getDataSourceServerName(controller.getDataSource()), query, null, 25);

//application.setValueListItems('my_en_types',dataset);
```
### setValueListItems(name, displayValues)

Fill a custom type valuelist with values from array(s) or dataset.

NOTE: if you modify values for checkbox/radio field, note that having one value in valuelist is a special case, so switching between one value and 0/multiple values may have side effects
NOTE: This is expensive operation, which triggers refresh of all visible forms. Over usage of this method may inflict performance issues.

**Parameters**\
[String](JSLib/String.md) name Name of the valuelist\
[Array](JSLib/Array.md) displayValues Display values array

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
//set display values (return values will be same as display values)
application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'));
//set display values and return values (which are stored in dataprovider)
//application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'),new Array(10000,10010,10456));
//set display values and return values converted to numbers
//application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'),new Array('10000','10010', '10456'), true);
//do query and fill valuelist (see databaseManager for full details of queries/dataset)
//var query = 'select display_value,optional_real_value from test_table';
//var dataset = databaseManager.getDataSetByQuery(databaseManager.getDataSourceServerName(controller.getDataSource()), query, null, 25);

//application.setValueListItems('my_en_types',dataset);
```
### setValueListItems(name, displayValues, autoconvert)

Fill a custom type valuelist with values from array(s) or dataset.

NOTE: if you modify values for checkbox/radio field, note that having one value in valuelist is a special case, so switching between one value and 0/multiple values may have side effects
NOTE: This is expensive operation, which triggers refresh of all visible forms. Over usage of this method may inflict performance issues.

**Parameters**\
[String](JSLib/String.md) name Name of the valuelist\
[Array](JSLib/Array.md) displayValues Display values array\
[Boolean](JSLib/Boolean.md) autoconvert Boolean (true) if display values and return values should be converted to numbers

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//set display values (return values will be same as display values)
application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'));
//set display values and return values (which are stored in dataprovider)
//application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'),new Array(10000,10010,10456));
//set display values and return values converted to numbers
//application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'),new Array('10000','10010', '10456'), true);
//do query and fill valuelist (see databaseManager for full details of queries/dataset)
//var query = 'select display_value,optional_real_value from test_table';
//var dataset = databaseManager.getDataSetByQuery(databaseManager.getDataSourceServerName(controller.getDataSource()), query, null, 25);

//application.setValueListItems('my_en_types',dataset);
```
### setValueListItems(name, displayValues, realValues)

Fill a custom type valuelist with values from array(s) or dataset.

NOTE: if you modify values for checkbox/radio field, note that having one value in valuelist is a special case, so switching between one value and 0/multiple values may have side effects
NOTE: This is expensive operation, which triggers refresh of all visible forms. Over usage of this method may inflict performance issues.

**Parameters**\
[String](JSLib/String.md) name Name of the valuelist\
[Array](JSLib/Array.md) displayValues Display values array\
[Array](JSLib/Array.md) realValues Real values array

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
//set display values (return values will be same as display values)
application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'));
//set display values and return values (which are stored in dataprovider)
//application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'),new Array(10000,10010,10456));
//set display values and return values converted to numbers
//application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'),new Array('10000','10010', '10456'), true);
//do query and fill valuelist (see databaseManager for full details of queries/dataset)
//var query = 'select display_value,optional_real_value from test_table';
//var dataset = databaseManager.getDataSetByQuery(databaseManager.getDataSourceServerName(controller.getDataSource()), query, null, 25);

//application.setValueListItems('my_en_types',dataset);
```
### setValueListItems(name, displayValues, realValues, autoconvert)

Fill a custom type valuelist with values from array(s) or dataset.

NOTE: if you modify values for checkbox/radio field, note that having one value in valuelist is a special case, so switching between one value and 0/multiple values may have side effects
NOTE: This is expensive operation, which triggers refresh of all visible forms. Over usage of this method may inflict performance issues.

**Parameters**\
[String](JSLib/String.md) name  ;\
[Array](JSLib/Array.md) displayValues Display values array\
[Array](JSLib/Array.md) realValues Real values array\
[Boolean](JSLib/Boolean.md) autoconvert Boolean (true) if display values and return values should be converted to numbers

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//set display values (return values will be same as display values)
application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'));
//set display values and return values (which are stored in dataprovider)
//application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'),new Array(10000,10010,10456));
//set display values and return values converted to numbers
//application.setValueListItems('my_en_types',new Array('Item 1', 'Item 2', 'Item 3'),new Array('10000','10010', '10456'), true);
//do query and fill valuelist (see databaseManager for full details of queries/dataset)
//var query = 'select display_value,optional_real_value from test_table';
//var dataset = databaseManager.getDataSetByQuery(databaseManager.getDataSourceServerName(controller.getDataSource()), query, null, 25);

//application.setValueListItems('my_en_types',dataset);
```
### showCalendar()

Show the calendar, returns selected date or null if canceled. Initial value and date format can be also specified.


**Returns**\
[Date](JSLib/Date.md) Selected date or null if canceled

**Supported Clients**\
SmartClient

**Sample**

```javascript
var selectedDate = application.showCalendar();
```
### showCalendar(dateFormat)

Show the calendar, returns selected date or null if canceled. Initial value and date format can be also specified.

**Parameters**\
[String](JSLib/String.md) dateFormat Date format

**Returns**\
[Date](JSLib/Date.md) Selected date or null if canceled

**Supported Clients**\
SmartClient

**Sample**

```javascript
var selectedDate = application.showCalendar();
```
### showCalendar(selectedDate)

Show the calendar, returns selected date or null if canceled. Initial value and date format can be also specified.

**Parameters**\
[Date](JSLib/Date.md) selectedDate Default selected date

**Returns**\
[Date](JSLib/Date.md) Selected date or null if canceled

**Supported Clients**\
SmartClient

**Sample**

```javascript
var selectedDate = application.showCalendar();
```
### showCalendar(selectedDate, dateFormat)

Show the calendar, returns selected date or null if canceled. Initial value and date format can be also specified.

**Parameters**\
[Date](JSLib/Date.md) selectedDate Default selected date\
[String](JSLib/String.md) dateFormat Date format

**Returns**\
[Date](JSLib/Date.md) Selected date or null if canceled

**Supported Clients**\
SmartClient

**Sample**

```javascript
var selectedDate = application.showCalendar();
```
### showColorChooser()

Show the colorChooser. Returned value is in format #RRGGBB or null if canceled.


**Returns**\
[String](JSLib/String.md) selected color or null if canceled

**Supported Clients**\
SmartClient

**Sample**

```javascript
var selectedColor = application.showColorChooser();
```
### showColorChooser(colorString)

Show the colorChooser. Returned value is in format #RRGGBB or null if canceled.

**Parameters**\
[String](JSLib/String.md) colorString Default color

**Returns**\
[String](JSLib/String.md) selected color or null if canceled

**Supported Clients**\
SmartClient

**Sample**

```javascript
var selectedColor = application.showColorChooser();
```
### showFontChooser()

Show the font chooser dialog. Returns the selected font. Can specify a default font.


**Returns**\
[String](JSLib/String.md) selected font

**Supported Clients**\
SmartClient

**Sample**

```javascript
var selectedFont = application.showFontChooser();
elements.myfield.font = selectedFont
```
### showFontChooser(defaultFont)

Show the font chooser dialog. Returns the selected font. Can specify a default font.

**Parameters**\
[String](JSLib/String.md) defaultFont Default font

**Returns**\
[String](JSLib/String.md) selected font

**Supported Clients**\
SmartClient

**Sample**

```javascript
var selectedFont = application.showFontChooser();
elements.myfield.font = selectedFont
```
### showForm(form)

Show the form specified by the parameter, that can be a name (is case sensitive!) or a form object.
This will show the form in the active/currently focused window. So when called from a form in a dialog the dialog will show the form.

**Parameters**\
[Object](JSLib/Object.md) form Form object or name

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.showForm('MyForm');
```
### showI18NDialog()

Opens the i18n dialog so users can change translations. Returns the key selected by the user (not it's translation)  or null if cancel is pressed. Optional parameters specify the initial selections in the dialog.


**Returns**\
[String](JSLib/String.md) selected I18N key or null if cancel is pressed

**Supported Clients**\
SmartClient

**Sample**

```javascript
application.showI18NDialog("servoy.button.close", "en");
```
### showI18NDialog(keyToSelect)

Opens the i18n dialog so users can change translations. Returns the key selected by the user (not it's translation)  or null if cancel is pressed. Optional parameters specify the initial selections in the dialog.

**Parameters**\
[String](JSLib/String.md) keyToSelect Default selected key

**Returns**\
[String](JSLib/String.md) selected I18N key or null if cancel is pressed

**Supported Clients**\
SmartClient

**Sample**

```javascript
application.showI18NDialog("servoy.button.close", "en");
```
### showI18NDialog(keyToSelect, languageToSelect)

Opens the i18n dialog so users can change translations. Returns the key selected by the user (not it's translation)  or null if cancel is pressed. Optional parameters specify the initial selections in the dialog.

**Parameters**\
[String](JSLib/String.md) keyToSelect Default selected key\
[String](JSLib/String.md) languageToSelect Default selected language

**Returns**\
[String](JSLib/String.md) selected I18N key or null if cancel is pressed

**Supported Clients**\
SmartClient

**Sample**

```javascript
application.showI18NDialog("servoy.button.close", "en");
```
### showURL(url)

Shows an URL in a browser.

**Parameters**\
[String](JSLib/String.md) url URL to show

**Returns**\
[Boolean](JSLib/Boolean.md) Boolean (true) if URL was shown

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.showURL('http://www.example.com');

//NGClient and webclient specific additional parameters...
//2nd parameter: target frame or named dialog/window, so its possible to control in which (internal) frame or dialog the url is loaded, '_self' is current window,'_blank' is new dialog, '_top' is main window; default is '_blank'
//3rd parameter: dialog options used when a dialog is specified, example: 'height=200,width=400,status=yes,toolbar=no,menubar=no,location=no'
//3rd or 4th parameter: a timeout in seconds when the url should be shown, immediately/0 is default'
```
### showURL(url, browserTarget)

Shows an URL in a browser.

**Parameters**\
[String](JSLib/String.md) url URL to show\
[String](JSLib/String.md) browserTarget Target frame or named dialog/window

**Returns**\
[Boolean](JSLib/Boolean.md) Boolean (true) if URL was shown

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.showURL('http://www.example.com');

//NGClient and webclient specific additional parameters...
//2nd parameter: target frame or named dialog/window, so its possible to control in which (internal) frame or dialog the url is loaded, '_self' is current window,'_blank' is new dialog, '_top' is main window; default is '_blank'
//3rd parameter: dialog options used when a dialog is specified, example: 'height=200,width=400,status=yes,toolbar=no,menubar=no,location=no'
//3rd or 4th parameter: a timeout in seconds when the url should be shown, immediately/0 is default'
```
### showURL(url, browserTarget, timeout)

Shows an URL in a browser.

**Parameters**\
[String](JSLib/String.md) url URL to show\
[String](JSLib/String.md) browserTarget Target frame or named dialog/window\
[Number](JSLib/Number.md) timeout A timeout in seconds when the url should be shown

**Returns**\
[Boolean](JSLib/Boolean.md) Boolean (true) if URL was shown

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.showURL('http://www.example.com');

//NGClient and webclient specific additional parameters...
//2nd parameter: target frame or named dialog/window, so its possible to control in which (internal) frame or dialog the url is loaded, '_self' is current window,'_blank' is new dialog, '_top' is main window; default is '_blank'
//3rd parameter: dialog options used when a dialog is specified, example: 'height=200,width=400,status=yes,toolbar=no,menubar=no,location=no'
//3rd or 4th parameter: a timeout in seconds when the url should be shown, immediately/0 is default'
```
### showURL(url, browserTarget, browserTargetOptions)

Shows an URL in a browser.

**Parameters**\
[String](JSLib/String.md) url URL to show\
[String](JSLib/String.md) browserTarget Target frame or named dialog/window\
[String](JSLib/String.md) browserTargetOptions Dialog options used when a dialog is specified / a timeout in seconds when the url should be shown

**Returns**\
[Boolean](JSLib/Boolean.md) Boolean (true) if URL was shown

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.showURL('http://www.example.com');

//NGClient and webclient specific additional parameters...
//2nd parameter: target frame or named dialog/window, so its possible to control in which (internal) frame or dialog the url is loaded, '_self' is current window,'_blank' is new dialog, '_top' is main window; default is '_blank'
//3rd parameter: dialog options used when a dialog is specified, example: 'height=200,width=400,status=yes,toolbar=no,menubar=no,location=no'
//3rd or 4th parameter: a timeout in seconds when the url should be shown, immediately/0 is default'
```
### showURL(url, browserTarget, browserTargetOptions, timeout)

Shows an URL in a browser.

**Parameters**\
[String](JSLib/String.md) url URL to show\
[String](JSLib/String.md) browserTarget Target frame or named dialog/window\
[String](JSLib/String.md) browserTargetOptions Dialog options used when a dialog is specified / a timeout in seconds when the url should be shown\
[Number](JSLib/Number.md) timeout A timeout in seconds when the url should be shown

**Returns**\
[Boolean](JSLib/Boolean.md) Boolean (true) if URL was shown

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
application.showURL('http://www.example.com');

//NGClient and webclient specific additional parameters...
//2nd parameter: target frame or named dialog/window, so its possible to control in which (internal) frame or dialog the url is loaded, '_self' is current window,'_blank' is new dialog, '_top' is main window; default is '_blank'
//3rd parameter: dialog options used when a dialog is specified, example: 'height=200,width=400,status=yes,toolbar=no,menubar=no,location=no'
//3rd or 4th parameter: a timeout in seconds when the url should be shown, immediately/0 is default'
```
### sleep(ms)

Sleep for specified time (in milliseconds).

**Parameters**\
[Number](JSLib/Number.md) ms Sleep time in milliseconds

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//Sleep for 3 seconds
application.sleep(3000);
```
### undo()

Undo last action (if possible).


**Returns**\
void 

**Supported Clients**\
SmartClient

**Sample**

```javascript
application.undo();
```
### updateUI()

Updates the UI (painting). If in a script an element changed and the script continues doing
things, you can give an number in ms how long this can take.
Warning: this gives the UI time to paint, but this also means that it will give the ui time to respond to all other events,
so if a user keeps clicking on other stuff this will also be handled right away inside this call.

NOTE:In NGClient, this method will send to browser all outstanding changes. If called too often (with many changes), can cause performance issues.


**Returns**\
void 

**Supported Clients**\
SmartClient,NGClient

**Sample**

```javascript
application.updateUI(500);
//continue doing things
```
### updateUI(milliseconds)

Updates the UI (painting). If in a script an element changed and the script continues doing
things, you can give an number in ms how long this can take.
Warning: this gives the UI time to paint, but this also means that it will give the ui time to respond to all other events,
so if a user keeps clicking on other stuff this will also be handled right away inside this call.

NOTE:In NGClient, this method will send to browser all outstanding changes. If called too often (with many changes), can cause performance issues.

**Parameters**\
[Number](JSLib/Number.md) milliseconds How long the update should take in milliseconds

**Returns**\
void 

**Supported Clients**\
SmartClient,NGClient

**Sample**

```javascript
application.updateUI(500);
//continue doing things
```

