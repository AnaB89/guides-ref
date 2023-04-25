# svySecurityUX

Welcome to svySecurityUX!

* [**Security UX Templates**](svySecurityUX.md#security-ux-templates)
  * [Login Template](svySecurityUX.md#login-template)
  * [Tenant Template](svySecurityUX.md#tenant-template)
  * [Roles Template](svySecurityUX.md#roles-template)
  * [Users Template](svySecurityUX.md#users-template)
  * [User Template](svySecurityUX.md#user-template)
* [**Getting Started**](svySecurityUX.md#getting-started)
  * [Login Form](svySecurityUX.md#optional-login-form)
  * [SecurityUX and Navigation](svySecurityUX.md#securityux-and-navigation)
  * [Navigation Actions](svySecurityUX.md#navigation-actions)
  * [After User Create Event](svySecurityUX.md#after-user-create-event)

The svySecurityUX module provides out of the box intuitive templates (served as Servoy forms) for the logged tenant's security-related administration tasks, such as managing users and roles, along with some useful summary and usage statistics.

## Security UX Templates

Note that the provided templates (except for the login form) are relative to the logged tenant; therefore can be accessed only once the tenant's user has logged in. Will be up to you to define and implement access permissions to the tenant's administration templates within your solution.

**READ CAREFULLY** if you are using a [master-slave](https://github.com/Servoy/svySecurity/wiki/Master-and-Slave-tenants) tenant setup you should not use these templates to administer the roles and their assigned permissions for master tenants. That's because any change will be applied only to the tenant of the logged user and will not be propagated to the slave tenants.

Below are listed the offered templates of the svySecurityUX module; each template is a Servoy's forms which can be used as-is within your own solution or can be customized by extending the template form or duplicate it. Note once you extend or duplicate the form you will be responsible to update and maintain your own form adjusting it to possible changes of future releases.

**Custom Look & Feel**: the look\&feel of the provided templates can be easily customized using the [Servoy Theme](https://wiki.servoy.com/pages/viewpage.action?pageId=31752222)

#### Login Template

The form **svyLoginUX** can be used as login form for your solution; it offers the essentials login functionalities such as password and error checking.

You may extend the form and set your own logo and your own background image in the extended form.

* Verify Tenant and User combination exists
* Check User's Password
* Report login errors

![Login Template](images/2019-12-30\_1233.png)

#### Tenant Template

The tenant template form offers an overview of the logged tenant with the following functionalities:

* Tenant's summary info
* List all existing Roles
* List all existing Users
* Navigate to the tenant's Roles and Users
* Lock/Unlock the tenant
* Edit tenant's display name

![Tenant Template](images/2019-12-30\_1237.png)

#### Roles Template

The Role template allows to administer all Roles of the logged tenant:

* Create Roles
* Remove Roles
* Assign Permissions to Roles

![Roles Template](images/2019-12-30\_1237\_2.png)

#### Users Template

The Users template allows to administer all Users of the logged tenant:

* Create User
* Remove User
* Assign Roles to Users

![Users Template](images/2019-12-30\_1236.png)

#### User Template

The User template offers an overview for any User of the logged tenant:

* User summary info
* Edit display name
* Edit email
* Lock/Unlock user
* Reset password
* List assigned roles

![User Template](images/2019-12-30\_1236\_2.png)

## Getting Started

Include the module svySecurityUX as module of your solution. Security administration templates are available as Servoy forms within the svySecurityUX module.

Is recommended to use the [Servoy Theme](https://wiki.servoy.com/pages/viewpage.action?pageId=31752222) to obtain a pleasant look\&feel which can be easily customized to suite your own style and colors.

#### (Optional) Login Form

* It is recommended to create your own [Login Module ](https://wiki.servoy.com/display/DOCS/Implementing+Security).
* Within that module, create your own form duplicating the **svyLoginUX** form. Make this the firstForm property of your login module.
* (Optional) change the Servoy logo with your own logo in the newly created form by setting the image media of the _logo_ element (can select any image from the media folder of your solution).
* (Optional) custom messages for login errors

![Create Login Form](images/2019-12-30\_1406.png)

![Set solution's login form](images/2019-12-30\_1412.png)

![Change logo](images/2019-12-30\_1414.png)

You can show custom messages to the user instead of the default login errors by overriding the method _onLoginError_ of your login form

```
function onLoginError(error) {

	var errorTxt;
	switch (error) {
	case ERROR_CODES.INSUFFICIENT_PERMISSIONS:
		errorTxt = "The User does not have any permission; login is denied";
		break;
	case ERROR_CODES.LOCKED_TENANT:
		errorTxt = "The Tenant is locked";
		break;
	case ERROR_CODES.LOCKED_USER:
		errorTxt = "The User is locked";
		break;
	case ERROR_CODES.PASSWORD_MISMATCH:
		errorTxt = "The entered password is not correct";
		break;
	case ERROR_CODES.PASSWORD_NOT_SPECIFIED:
		errorTxt = "Please enter the User's password";
		break;
	case ERROR_CODES.TENANT_NOT_FOUND:
		errorTxt = "Tenant not found";
		break;
	case ERROR_CODES.TENANT_NOT_SPECIFIED:
		errorTxt = "Please enter the Tenant";
		break;
	case ERROR_CODES.USER_NOT_FOUND:
		errorTxt = "User not found";
		break;
	case ERROR_CODES.USER_NOT_SPECIFIED:
		errorTxt = "Please enter the User";
		break;
	default:
		errorTxt = error
		break;
	}

	elements.errorMsg.text = errorTxt;
	elements.errorMsg.visible = true;
}
```

#### SecurityUX and Navigation

Security templates are available as forms within the svySecurityUX module. The available templates are listed in the enum **scopes.svyNavigationUX.SVY\_SECURITY\_UX**

```
var SVY_SECURITY_UX = {
	TENANT: "svySecurityUXTenant",
	TENANT_ROLES: "svySecurityUXTenantRolesContainer",
	TENANT_USERS: "svySecurityUXTenantUsersContainer",
	USER: "svySecurityUXUser"
}
```

To access the security templates within your solution is as simple as showing a Servoy form. They can be used within any navigation system; will be up to you to decide how the user can navigate to the Security templates. You will also be responsible to define access control permission if you want to restrict their access only to certain users.

If you make use of the [svyNavigation](broken-reference) module already the templates can be seamlessly plugged in your navigation menu.

#### Example

Assuming you are using the [sidenav](../../ui-components/navigation/Sidenav.md) menu with [svyNavigation](broken-reference) module you can simply list the security template as menu items of your sidenav.

```
function loadMenuItems() {
 	var menuItems = [];
	
        // your home screen
	/** @type {CustomType<servoyextra-sidenav.MenuItem>} */
	var menuItem = new Object();
	menuItem.id = "yourFormName";
	menuItem.iconStyleClass = "fa fa-home";
	menuItem.text = "Home";
	menuItems.push(menuItem);
	
	// tenant's security menu item
	/** @type {CustomType<servoyextra-sidenav.MenuItem>} */
	var secMenuItem = new Object();
	secMenuItem.id = scopes.svySecurityUX.SVY_SECURITY_UX.TENANT;
	secMenuItem.iconStyleClass = "fas fa-shield-alt";
	secMenuItem.text = "Security";
	menuItems.push(secMenuItem);
	
	// users menu item
	/** @type {CustomType<servoyextra-sidenav.MenuItem>} */
	var secUsersItem = new Object();
	secUsersItem.id = scopes.svySecurityUX.SVY_SECURITY_UX.TENANT_USERS;
	secUsersItem.iconStyleClass = "fas fa-users"
	secUsersItem.text = "Users"
	
	// roles menu item
	/** @type {CustomType<servoyextra-sidenav.MenuItem>} */
	var secRolesItem = new Object();
	secRolesItem.id = scopes.svySecurityUX.SVY_SECURITY_UX.TENANT_ROLES;
	secRolesItem.iconStyleClass = "fas fa-key"
	secRolesItem.text = "Roles"

	// security submenu
	secMenuItem.menuItems = [secUsersItem, secRolesItem];
	
	return menuItems;
}
```

#### Navigation Actions

Within the templates there are pre-defined actions to navigate across the security templates (e.g. "View Roles", "View Users", "Edit User, "Back"..). Each navigation action will trigger a Navigation Event; if you already make use of the [svyNavigation](broken-reference) module, the navigation template will handle the navigation for you.

If you don't use the svyNavigation module but instead you have implemented your custom navigation you can decide either to

* A: subscribe for the Navigation Event and handle it on your own
* B: extend the template form and override the navigation action with your own implementation

**A:** Use the svyNavigation API to subscribe to the Navigation Event triggered by the security templates actions. When a navigation event is triggered handle the navigation by showing the target form and (if any) load in the target form the data to be shown.

```
function onSolutionOpen(arg, queryParams) {
	
	// subscribe for navigation events
	scopes.svyNavigation.addNavigationListener(onNavigation);
}

function onNavigation(event) {
	
	// handle AFTER_OPEN events
	if (event.getEventType() === scopes.svyNavigation.NAVIGATION_EVENT.AFTER_OPEN) {
		
		// get the name of the form to be shown
		var item = event.getNavigationItem();
		var form = forms[item.getFormName()];
		
		// load data to show
		var data = event.getDataToShow();
		if (data && data instanceof JSRecord) {
			// if passed data is a record
			scopes.svyDataUtils.loadRecords(form.foundset, data.getPKs());
		} else if (data) {
			// else default to loadRecords(*)
			form.foundset.loadRecords(data);
		}
			
		// show the form
		application.showForm(form)
	}
}

```

**B:** You can extend the security templates forms and override the action click which trigger the navigation in your extended form. Note when you extend the template forms you will probably navigate to your own forms instead of using the default templates defined in the enum _scopes.svyNavigationUX.SVY\_SECURITY\_UX_.

#### After User Create Event

Anytime a user is created using the templates, you may like to perform some custom actions, for example "Send a registration email to the newly created User" or "Set a default password for the newly created User".

You can subscribe to the User Created Event using the svySecurityUX API addAfterUserCreateListener

```
function onSolutionOpen(arg, queryParams) {
	// run onAfterUserCreate when a user is created from the svySecurityUX templates
	scopes.svySecurityUX.addAfterUserCreateListener(onAfterUserCreate);
}

function onAfterUserCreate(userName, tenantName) {
	var user = scopes.svySecurity.getUser(userName, tenantName);
	user.setPassword("0000");
	if (scopes.myScope.sendRegistrationEmail(user)) {
		plugins.webnotificationsToastr.success("An invitation email has been sent to the new user " + userName, "Invitation sent");
	}
}
```
