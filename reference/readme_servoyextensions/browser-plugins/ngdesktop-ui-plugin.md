Welcome to the **ngdesktopui** wiki! This wiki provides comprehensive documentation to using the **ngdesktopui** web service. This service works with the NGDesktop Client as a bridge to execute client side calls dealing with UI from Servoy.


# Getting Started
First import the service one of the release [binaries](https://github.com/Servoy/ngdesktopui/releases) or via Servoy's Web Package Manager.

# Example Usage

The following code snippet is create a sample menu for NGDesktop: 

`function createTestMenu(event) {`

	var isMac = application.getOSName().toUpperCase().indexOf('MAC')>=0;
	var menu = plugins.ngdesktopui;
	menu.removeAllMenus();
	var ngdesktopIndex = menu.addMenu("Servoy NGDesktop"); //on MacOS this name is hidden
	menu.addMenuItem(ngdesktopIndex,"About Servoy NGDesktop...",callback);
	menu.addSeparator(ngdesktopIndex);
	menu.addRoleItem(ngdesktopIndex,"services");
	menu.addSeparator(ngdesktopIndex);
	if (isMac) {
		menu.addRoleItem(ngdesktopIndex,"hide", "Hide this application");
		menu.addRoleItem(ngdesktopIndex,"hideOthers");
		menu.addSeparator(ngdesktopIndex);
	}
	menu.addRoleItem(ngdesktopIndex,"quit");
	
	//add file menu
	var fileIndex = menu.addMenu("File");
	menu.addMenuItem(fileIndex,"New",callback);
	menu.addMenuItem(fileIndex,"Open...",callback);
	
	//insert menuitem example
	//since this will be a submenu the callback is set to null
	recentIndex = menu.addMenuItem(fileIndex,"Open recent", null, 1);
	addRecentFiles(fileIndex, recentIndex);
	
	//add edit menu
	var editIndex = menu.addMenu("Edit");
	menu.addRoleItem(editIndex,"undo");
	menu.addRoleItem(editIndex,"redo");
	menu.addSeparator(editIndex);
	menu.addRoleItem(editIndex,"cut");
	menu.addRoleItem(editIndex,"copy");
	menu.addRoleItem(editIndex,"paste");
	
	//add help menu
	var helpIndex = menu.addMenu("Help");
	menu.addMenuItem(helpIndex,"Search...",callback);
	menu.addMenuItem(helpIndex,"Servoy NGDesktop help",callback)
}

`function addRecentFiles(menuIndex, submenuIndex) {`

	var menu = plugins.ngdesktopui;
	var position = menu.addMenuItem(menuIndex,"Bureau.pdf",callback, 0, submenuIndex);
	position = menu.addMenuItem(menuIndex,"Advertising.pdf",callback, position + 1, submenuIndex);
	position = menu.addSeparator(menuIndex,position + 1, submenuIndex);
	position = menu.addRoleItem(menuIndex,"clearRecentDocuments", null, position + 1,submenuIndex);
}

The following issues has been discovered so far:
 - setMenuBarVisibility has no effect on MacOS. You can't hide a MacOS menu
 - removeAllMenus - for MacOS is display a minimal menu having the app name as Menu name and Quit option as menuItem
 - on macOS - the first menuName is always the app name: first addMenu(menuName) will not display the "menuName" but the app name. The name behind (which you will work with), still remain "menuName"
 - on MacOS - the checkboxes and radio buttons in menus are not correctly rendered. This seems to be a Chromium issue. Further investigation needed for this
 - When clicking on a radio button - it will be selected, and the previous radio buttons (from the adiacent radio items) will be deselected. However, calling multiple times addRadioButton(menuName, menuitemName, true) will add multiple selected radio buttons (they will unselect automatically when one radio button is selected). It is your responsability to call addRadioButton() with "selected" parameter set to true - only once. The same issue is true also for insertRadioButton 

The following sample will create a custom tray menu for NG Desktop:

`function createTrayMenu(event) {`

	var trayMenu = plugins.ngdesktopui.createTrayMenu();
	trayMenu.title = NG Desktop'; //optional
	trayMenu.tooltip = 'Testing tray menu'; //optional
	trayMenu.icon = solutionModel.getMedia('tray_close.png').getBytes(); //optional
   	trayMenu.pressedIcon = solutionModel.getMedia('tray_open.png').getBytes();//optional
   	
   	trayMenu.addMenuItem(0, 'Sys info', trayCallback);
   	trayMenu.addMenuItem(1, 'Maximise', trayCallback);
   	trayMenu.addMenuItem(2, 'Unmaximise', trayCallback);
   	trayMenu.addMenuItem(3, 'Home directory', trayCallback);
   	trayMenu.addSeparator(4);
   	trayMenu.addRoleItem(5, 'Quit');
	
   	trayMenu.done();
}

`function trayCallback(itemName, itemType, itemStatus) {`

	switch (itemName ) {
		case 'Sys info':
			var sysInfo = plugins.ngdesktoputils.getSystemInformation();
			plugins.dialogs.showInfoDialog('System', 'Platform: ' + sysInfo.osPlatform + '     Version: ' + sysInfo.osRelease);
			break;
		case 'Maximise':
			plugins.ngdesktopui.maximizeWindow();
			break;
		case 'Unmaximise':
			plugins.ngdesktopui.unmaximizeWindow();
			break;
		case 'Home directory':
			plugins.dialogs.showInfoDialog('Home directory',plugins.ngdesktopfile.homeDir());
			break;
	}
}



# API Documentation 

### Callback function
The callback function is receiving the following parameters:

**Params**
Type | Name | Summary 
--- | --- | --- 
string | text | clicked item name
string | type | clicked item type ("normal", "checkbox", "radio")
boolean | checked | check state (true or false for checkboxes, true for radio buttons and undefined for the other types) 


## Method Summary
### addMenu
Add new menu to existing menubar

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
string | text | Menu label | Required
index | int | Insert position | Optional

### removeMenu
Remove specified menu

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
index | int | Menu index (zero based) | Required

### addDevToolsMenu
Add Developer Tools menu to the menu bar.
Use it just for debugging. Remove any call to this function once you're done.  

### getMenuIndexByText
Return the index order of the menu (zero based index) 

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
string | text | Menu label to query | Required

### getMenuText
Return the menu label

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
int | index | Index to query | Required

### getMenuCount
Count menus from the menubar

### removeAllMenus
Cleanup the menubar. For Mac OS this means to display a minimal menu.

### setMenuBarVisibility
Show/Hide menu bar. On MacOS this method has no effect

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
boolean | visibility | true - show menubar, false - hide menubar | Required

### removeAllMenuItems
Cleanup the specified menu

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
int | index | Menu index to cleanup | Required

### addSeparator
Add a separator line

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
int | index | Menu index | Required
int | position | Insert position | Optional
int | itemIndex | Submenu index | Optional


### addMenuItem
Add an item to the specified menu

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
int | index | Menu index | Required
string | text | Menu label | Required
function | callback | Callback function | Required (may be null)
int | position | Insert position | Optional
int | itemIndex  Submenu index | Optional

### removeMenuItem
Delete an item

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
int | index | Menu index | Required
int | position | Insert position | Required
int | itemIndex  Submenu index | Optional

### getMenuItemsCount
Count items

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
int | index | Menu index | Required
int | itemIndex | Submenu index | Optional

### addCheckBox
Add a checkbox to the specified menu

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
int | index | Menu index | Required
string | text | Menu label | Required
function | callback | Callback function | Required (may be null)
boolean | checked | initial checkbox status (default is false) | Optional
int | position | Insert position | Optional
int | itemIndex  Submenu index | Optional

### addRadioButton
Add a radio button to the specified menu.
Note that the first added radio button in the group is alwasy selected regardless the 'selected' value
There are no group creation method. A group consist from all adiacent radio buttons in a menu

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
int | index | Menu index | Required
string | text | Menu label | Required
function | callback | Callback function | Required (may be null)
boolean | selected | select radio button (default is false) | Optional
int | position | Insert position | Optional
int | itemIndex  Submenu index | Optional

### getMenuItemIndexByText
Get menuitem index from the specified menu

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
int | index | Menu index | Required
string | text | Item label to query for | Required

### getMenuItemText
Get menuitem label

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
int | index | Menu index | Required
int | itemIndex | Menuitem index | Required

### addRoleItem
Roles allow menu items to have predefined behaviors. 

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
int | index | Menu index | Required
string | role | The item role (see below) | Required
string | text | The item label | Optional
int | position | Insert position | Optional
int | itemIndex | Submenu index | Optional



It is best to specify role for any menu item that matches a standard role, rather than trying to manually implement the behavior using a callback function. The built-in role behavior will give the best native experience.

The role property can have following values:

* undo
* about - Trigger a native about panel (custom message box on Window, which does not provide its own).
* redo
* cut
* copy
* paste
* pasteAndMatchStyle
* selectAll
* delete
* minimize - Minimize current window.
* close - Close current window.
* quit - Quit the application.
* reload - Reload the current window.
* forceReload - Reload the current window ignoring the cache.
* toggleDevTools - Toggle developer tools in the current window.
* togglefullscreen - Toggle full screen mode on the current window.
* resetZoom - Reset the focused page's zoom level to the original size.
* zoomIn - Zoom in the focused page by 10%.
* zoomOut - Zoom out the focused page by 10%.
* fileMenu - Whole default "File" menu (Close / Quit)
* editMenu - Whole default "Edit" menu (Undo, Copy, etc.).
* viewMenu - Whole default "View" menu (Reload, Toggle Developer Tools, etc.)
* windowMenu - Whole default "Window" menu (Minimize, Zoom, etc.).

The following additional roles are available on macOS:

* appMenu - Whole default "App" menu (About, Services, etc.)
* hide - Map to the hide action.
* hideOthers - Map to the hideOtherApplications action.
* unhide - Map to the unhideAllApplications action.
* startSpeaking - Map to the startSpeaking action.
* stopSpeaking - Map to the stopSpeaking action.
* front - Map to the arrangeInFront action.
* zoom - Map to the performZoom action.
* toggleTabBar - Map to the toggleTabBar action.
* selectNextTab - Map to the selectNextTab action.
* selectPreviousTab - Map to the selectPreviousTab action.
* mergeAllWindows - Map to the mergeAllWindows action.
* moveTabToNewWindow - Map to the moveTabToNewWindow action.
* window - The submenu is a "Window" menu.
* help - The submenu is a "Help" menu.
* services - The submenu is a "Services" menu. This is only intended for use in the Application Menu and is not the same as the "Services" submenu used in context menus in macOS apps, which is not implemented in Electron.
* recentDocuments - The submenu is an "Open Recent" menu.
* clearRecentDocuments - Map to the clearRecentDocuments action.

### createBrowserView
Creates a BrowserView (looks like an iframe) and adds this to the current window at the given coordinates with the given width and height.
It returns and id that can be used to close/clean up this view later on, or to target that view to inject some javascript.

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
int | x | The X coordinate to position this view | Required
int | y | The Y coordinate to position this view | Required
int | width | The width of this view | Required
int | height | The height of this view | Required
string | url | The url to load into this view | Required

			
### closeBrowserView
Closes a and destroys a previously created BrowserView by the given id.

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
int | id | The id of the view to close | Required

### injectJSIntoBrowserView
Injects the given javascript into the content of the BrowserView of the given id.
The javascript can be a function declaration that is then called later on.
The last statement return value is given back to the callback as a first argument.
If something goes wrong then the callback is called where the first argument is null and a second argument has the message of the exception.

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
int | id | The id of the view to execute javascript in | Required
string | js | The piece of javascript that is injected into this view | Required
function | callback | the callback function that is used to get the results or exception if the call fails | Required

### createTrayMenu
Return a TrayMenu object type.

### TrayMenu properties

Type | Name | Summary | Required
string | title | tray menu title displayed next to the tray icon | Optional
string | tooltip | just a tooptip | Optional
byte[] | icon | icon to be displayed in the tray | Optional 
byte[] | pressedIcon | icon to be displayed when opening the tray (MacOS only) | Optional

### TrayMenu api
This methods are available only through the TrayMenu object - trayMenu.method(params). The autocompletion is not yet available

### Callback function
The callback function is receiving the following parameters:

Type | Name | Summary | Required
--- | --- | --- | ---
string | text | clicked item name | Required
string | type | clicked item type ("normal", "checkbox") | Required
boolean | checked | check state (true or false for checkboxes, false otherwise) | Required

### addMenuItem
Add item to the tray menu

Type | Name | Summary | Required
--- | --- | --- | ---
int | index | zero based index where to add / insert items in tray menu | Required
string | text | menu item text | Required
function | callback | Callback function | Required

### removeMenuItem

Type | Name | Summary | Required
--- | --- | --- | ---
int | index | zero based index of the item to be removed | Required

### addCheckBox

Type | Name | Summary | Required
--- | --- | --- | ---
int | index | zero based index where to add / insert items in tray menu | Required
string | text | menu item text | Required
function | callback | Callback function | Required
boolean | checked | Initial status of the checkbox | Required

### addSeparator

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
int | index | zero based index of the position where to add / insert the separator | Required

### addRoleItem
Add a tray menu item with predefined (system) behavior. For details, check the documentation for the addRoleItem method above (for NG Desktop menu) 

**Params**
Type | Name | Summary | Required
--- | --- | --- | ---
int | index | zero based index of the position where to add / insert role | Required
string | role | The item role (see above ethod with the same name) | Required
string | text | Role label | Optional


### done
When all desired changes to the tray menu are finalized, call this method for the changes to takes effect.
  

### Example Usage
// open google.com<br/>
var id = plugins.ngdesktopui.createBrowserView(100,200,700,500,"https://www.google.com/");<br/>
// get the value of the search field and return this.<br/>
plugins.ngdesktopui.injectJSIntoBrowserView(id, "function test() { return document.getElementsByName('q')[0].value};test();", callback);
