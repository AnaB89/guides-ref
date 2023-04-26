# Security

## Constants Summary

| Type                       | Name                                           | Summary                                                                                        |
| -------------------------- | ---------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| [Number](js-lib/number.md) | [ACCESSIBLE](security.md#ACCESSIBLE)           | Constant representing the accessible flag for form security..                                  |
| [Number](js-lib/number.md) | [DELETE](security.md#DELETE)                   | Constant representing the delete flag for table security..                                     |
| [Number](js-lib/number.md) | [INSERT](security.md#INSERT)                   | Constant representing the insert flag for table security..                                     |
| [Number](js-lib/number.md) | [READ](security.md#READ)                       | Constant representing the read flag for table security..                                       |
| [Number](js-lib/number.md) | [TRACKING](security.md#TRACKING)               | Constant representing the tracking flag for table security (tracks sql insert/update/delete).. |
| [Number](js-lib/number.md) | [TRACKING\_VIEWS](security.md#TRACKING\_VIEWS) | Constant representing the tracking flag for table security (tracks sql select)..               |
| [Number](js-lib/number.md) | [UPDATE](security.md#UPDATE)                   | Constant representing the update flag for table security..                                     |
| [Number](js-lib/number.md) | [VIEWABLE](security.md#VIEWABLE)               | Constant representing the viewable flag for form security..                                    |

## Methods Summary

| Type                                       | Name                                                                                                                              | Summary                                                                                                                                       |
| ------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| [Boolean](js-lib/boolean.md)               | [addUserToGroup(a\_userUID, groupName)](security.md#addusertogroup-a\_useruid-groupname)                                          | Adds an user to a named group..                                                                                                               |
| [Object](js-lib/object.md)                 | [authenticate(authenticator\_solution, method)](security.md#authenticate-authenticator\_solution-method)                          | Authenticate to the Servoy Server using one of the installed authenticators or the Servoy default authenticator..                             |
| [Object](js-lib/object.md)                 | [authenticate(authenticator\_solution, method, credentials)](security.md#authenticate-authenticator\_solution-method-credentials) | Authenticate to the Servoy Server using one of the installed authenticators or the Servoy default authenticator..                             |
| [Boolean](js-lib/boolean.md)               | [canAccess(formName)](security.md#canaccess-formname)                                                                             | Returns whether form is accessible..                                                                                                          |
| [Boolean](js-lib/boolean.md)               | [canAccess(formName, elementName)](security.md#canaccess-formname-elementname)                                                    | Returns whether element from form is accessible..                                                                                             |
| [Boolean](js-lib/boolean.md)               | [canDelete(dataSource)](security.md#candelete-datasource)                                                                         | Returns a boolean value for security rights..                                                                                                 |
| [Boolean](js-lib/boolean.md)               | [canInsert(dataSource)](security.md#caninsert-datasource)                                                                         | Returns a boolean value for security rights..                                                                                                 |
| [Boolean](js-lib/boolean.md)               | [canRead(dataSource)](security.md#canread-datasource)                                                                             | Returns a boolean value for security rights..                                                                                                 |
| [Boolean](js-lib/boolean.md)               | [canUpdate(dataSource)](security.md#canupdate-datasource)                                                                         | Returns a boolean value for security rights..                                                                                                 |
| [Boolean](js-lib/boolean.md)               | [canView(formName)](security.md#canview-formname)                                                                                 | Returns whether form is viewable..                                                                                                            |
| [Boolean](js-lib/boolean.md)               | [canView(formName, elementName)](security.md#canview-formname-elementname)                                                        | Returns whether element from form is viewable..                                                                                               |
| [Boolean](js-lib/boolean.md)               | [changeGroupName(oldGroupName, newGroupName)](security.md#changegroupname-oldgroupname-newgroupname)                              | Changes the groupname of a group..                                                                                                            |
| [Boolean](js-lib/boolean.md)               | [changeUserName(a\_userUID, username)](security.md#changeusername-a\_useruid-username)                                            | Changes the username of the specified userUID..                                                                                               |
| [Boolean](js-lib/boolean.md)               | [checkPassword(a\_userUID, password)](security.md#checkpassword-a\_useruid-password)                                              | Returns true if the password for that userUID is correct, else false..                                                                        |
| [String](js-lib/string.md)                 | [createGroup(groupName)](security.md#creategroup-groupname)                                                                       | Creates a group, returns the groupname (or null when group couldn't be created)..                                                             |
| [Object](js-lib/object.md)                 | [createUser(username, password)](security.md#createuser-username-password)                                                        | Creates a new user, returns new uid (or null when group couldn't be created or user alreay exist)..                                           |
| [Object](js-lib/object.md)                 | [createUser(username, password, userUID)](security.md#createuser-username-password-useruid)                                       | Creates a new user, returns new uid (or null when group couldn't be created or user alreay exist)..                                           |
| [Boolean](js-lib/boolean.md)               | [deleteGroup(groupName)](security.md#deletegroup-groupname)                                                                       | Deletes a group, returns true if no error was reported..                                                                                      |
| [Boolean](js-lib/boolean.md)               | [deleteUser(userUID)](security.md#deleteuser-useruid)                                                                             | Deletes an user..                                                                                                                             |
| [String](js-lib/string.md)                 | [getClientID()](security.md#getclientid)                                                                                          | Returns the client ID..                                                                                                                       |
| [JSDataSet](database-manager/jsdataset.md) | [getElementUUIDs(formname)](security.md#getelementuuids-formname)                                                                 | Returns the form elements UUID's as dataset, the one with no name is the form itself..                                                        |
| [JSDataSet](database-manager/jsdataset.md) | [getGroups()](security.md#getgroups)                                                                                              | Get all the groups (returns a dataset)..                                                                                                      |
| [String](js-lib/string.md)                 | [getSystemUserName()](security.md#getsystemusername)                                                                              | Retrieves the username of the currently logged in user on operating system level..                                                            |
| [Array](js-lib/array.md)                   | [getTenantValue()](security.md#gettenantvalue)                                                                                    | Retrieve the tenant value for this Client, this value will be used as the value for all tables that have a column marked as a tenant column.. |
| [JSDataSet](database-manager/jsdataset.md) | [getUserGroups()](security.md#getusergroups)                                                                                      | Get all the groups of the current user..                                                                                                      |
| [JSDataSet](database-manager/jsdataset.md) | [getUserGroups(userUID)](security.md#getusergroups-useruid)                                                                       | Get all the groups for given user UID..                                                                                                       |
| [String](js-lib/string.md)                 | [getUserName()](security.md#getusername)                                                                                          | Get the current user name (null if not logged in), finds the user name for given user UID if passed as parameter..                            |
| [String](js-lib/string.md)                 | [getUserName(userUID)](security.md#getusername-useruid)                                                                           | Get the current user name (null if not logged in), finds the user name for given user UID if passed as parameter..                            |
| [String](js-lib/string.md)                 | [getUserUID()](security.md#getuseruid)                                                                                            | Get the current user UID (null if not logged in); finds the userUID for given user\_name if passed as parameter..                             |
| [String](js-lib/string.md)                 | [getUserUID(username)](security.md#getuseruid-username)                                                                           | Get the current user UID (null if not logged in); finds the userUID for given user\_name if passed as parameter..                             |
| [JSDataSet](database-manager/jsdataset.md) | [getUsers()](security.md#getusers)                                                                                                | Get all the users in the security settings (returns a dataset)..                                                                              |
| [JSDataSet](database-manager/jsdataset.md) | [getUsers(groupName)](security.md#getusers-groupname)                                                                             | Get all the users in the security settings (returns a dataset)..                                                                              |
| [Boolean](js-lib/boolean.md)               | [isUserMemberOfGroup(groupName)](security.md#isusermemberofgroup-groupname)                                                       | Check whatever the current user is part of the specified group.                                                                               |
| [Boolean](js-lib/boolean.md)               | [isUserMemberOfGroup(groupName, userUID)](security.md#isusermemberofgroup-groupname-useruid)                                      | Check whatever the user specified as parameter is part of the specified group..                                                               |
| [Boolean](js-lib/boolean.md)               | [login(username, a\_userUID, groups)](security.md#login-username-a\_useruid-groups)                                               | Login to be able to leave the solution loginForm..                                                                                            |
| void                                       | [logout()](security.md#logout)                                                                                                    | Logout the current user and close the solution, if the solution requires authentication and user is logged in..                               |
| void                                       | [logout(solutionToLoad)](security.md#logout-solutiontoload)                                                                       | Logout the current user and close the solution, if the solution requires authentication and user is logged in..                               |
| void                                       | [logout(solutionToLoad, argument)](security.md#logout-solutiontoload-argument)                                                    | Logout the current user and close the solution, if the solution requires authentication and user is logged in..                               |
| void                                       | [logout(solutionToLoad, method)](security.md#logout-solutiontoload-method)                                                        | Logout the current user and close the solution, if the solution requires authentication and user is logged in..                               |
| void                                       | [logout(solutionToLoad, method, argument)](security.md#logout-solutiontoload-method-argument)                                     | Logout the current user and close the solution, if the solution requires authentication and user is logged in..                               |
| [Boolean](js-lib/boolean.md)               | [removeUserFromGroup(a\_userUID, groupName)](security.md#removeuserfromgroup-a\_useruid-groupname)                                | Removes an user from a group..                                                                                                                |
| [Boolean](js-lib/boolean.md)               | [setPassword(a\_userUID, password)](security.md#setpassword-a\_useruid-password)                                                  | Set a new password for the given userUID..                                                                                                    |
| void                                       | [setSecuritySettings(dataset)](security.md#setsecuritysettings-dataset)                                                           | Sets the security settings; the entries contained in the given dataset will override those contained in the current security settings..       |
| void                                       | [setTenantValue(value)](security.md#settenantvalue-value)                                                                         | Set the tenant value for this Client, this value will be used as the value for all tables that have a column marked as a tenant column..      |
| [Boolean](js-lib/boolean.md)               | [setUserUID(a\_userUID, newUserUID)](security.md#setuseruid-a\_useruid-newuseruid)                                                | Set a new userUID for the given userUID..                                                                                                     |

## Constants Details

### ACCESSIBLE

Constant representing the accessible flag for form security.

**Returns**\
[Number](js-lib/number.md)

**Sample**

```javascript
var colNames = new Array();
colNames[0] = 'uuid';
colNames[1] = 'flags';
var dataset = databaseManager.createEmptyDataSet(0,colNames);

var row = new Array();
row[0] = '413a4d69-becb-4ae4-8fdd-980755d6a7fb';//normally retreived via security.getElementUUIDs(...)
row[1] = JSSecurity.VIEWABLE|JSSecurity.ACCESSIBLE; // use bitwise 'or' for both
dataset.addRow(row);//setting element security

row = new Array();
row[0] = 'example_data.orders';
row[1] = JSSecurity.READ|JSSecurity.INSERT|JSSecurity.UPDATE|JSSecurity.DELETE|JSSecurity.TRACKING; //use bitwise 'or' for multiple flags
dataset.addRow(row);//setting table security

security.setSecuritySettings(dataset);//to be called in solution startup method
```

### DELETE

Constant representing the delete flag for table security.

**Returns**\
[Number](js-lib/number.md)

**Sample**

```javascript
var colNames = new Array();
colNames[0] = 'uuid';
colNames[1] = 'flags';
var dataset = databaseManager.createEmptyDataSet(0,colNames);

var row = new Array();
row[0] = '413a4d69-becb-4ae4-8fdd-980755d6a7fb';//normally retreived via security.getElementUUIDs(...)
row[1] = JSSecurity.VIEWABLE|JSSecurity.ACCESSIBLE; // use bitwise 'or' for both
dataset.addRow(row);//setting element security

row = new Array();
row[0] = 'example_data.orders';
row[1] = JSSecurity.READ|JSSecurity.INSERT|JSSecurity.UPDATE|JSSecurity.DELETE|JSSecurity.TRACKING; //use bitwise 'or' for multiple flags
dataset.addRow(row);//setting table security

security.setSecuritySettings(dataset);//to be called in solution startup method
```

### INSERT

Constant representing the insert flag for table security.

**Returns**\
[Number](js-lib/number.md)

**Sample**

```javascript
var colNames = new Array();
colNames[0] = 'uuid';
colNames[1] = 'flags';
var dataset = databaseManager.createEmptyDataSet(0,colNames);

var row = new Array();
row[0] = '413a4d69-becb-4ae4-8fdd-980755d6a7fb';//normally retreived via security.getElementUUIDs(...)
row[1] = JSSecurity.VIEWABLE|JSSecurity.ACCESSIBLE; // use bitwise 'or' for both
dataset.addRow(row);//setting element security

row = new Array();
row[0] = 'example_data.orders';
row[1] = JSSecurity.READ|JSSecurity.INSERT|JSSecurity.UPDATE|JSSecurity.DELETE|JSSecurity.TRACKING; //use bitwise 'or' for multiple flags
dataset.addRow(row);//setting table security

security.setSecuritySettings(dataset);//to be called in solution startup method
```

### READ

Constant representing the read flag for table security.

**Returns**\
[Number](js-lib/number.md)

**Sample**

```javascript
var colNames = new Array();
colNames[0] = 'uuid';
colNames[1] = 'flags';
var dataset = databaseManager.createEmptyDataSet(0,colNames);

var row = new Array();
row[0] = '413a4d69-becb-4ae4-8fdd-980755d6a7fb';//normally retreived via security.getElementUUIDs(...)
row[1] = JSSecurity.VIEWABLE|JSSecurity.ACCESSIBLE; // use bitwise 'or' for both
dataset.addRow(row);//setting element security

row = new Array();
row[0] = 'example_data.orders';
row[1] = JSSecurity.READ|JSSecurity.INSERT|JSSecurity.UPDATE|JSSecurity.DELETE|JSSecurity.TRACKING; //use bitwise 'or' for multiple flags
dataset.addRow(row);//setting table security

security.setSecuritySettings(dataset);//to be called in solution startup method
```

### TRACKING

Constant representing the tracking flag for table security (tracks sql insert/update/delete).

**Returns**\
[Number](js-lib/number.md)

**Sample**

```javascript
var colNames = new Array();
colNames[0] = 'uuid';
colNames[1] = 'flags';
var dataset = databaseManager.createEmptyDataSet(0,colNames);

var row = new Array();
row[0] = '413a4d69-becb-4ae4-8fdd-980755d6a7fb';//normally retreived via security.getElementUUIDs(...)
row[1] = JSSecurity.VIEWABLE|JSSecurity.ACCESSIBLE; // use bitwise 'or' for both
dataset.addRow(row);//setting element security

row = new Array();
row[0] = 'example_data.orders';
row[1] = JSSecurity.READ|JSSecurity.INSERT|JSSecurity.UPDATE|JSSecurity.DELETE|JSSecurity.TRACKING; //use bitwise 'or' for multiple flags
dataset.addRow(row);//setting table security

security.setSecuritySettings(dataset);//to be called in solution startup method
```

### TRACKING\_VIEWS

Constant representing the tracking flag for table security (tracks sql select).

**Returns**\
[Number](js-lib/number.md)

**Sample**

```javascript
var colNames = new Array();
colNames[0] = 'uuid';
colNames[1] = 'flags';
var dataset = databaseManager.createEmptyDataSet(0,colNames);

var row = new Array();
row[0] = '413a4d69-becb-4ae4-8fdd-980755d6a7fb';//normally retreived via security.getElementUUIDs(...)
row[1] = JSSecurity.VIEWABLE|JSSecurity.ACCESSIBLE; // use bitwise 'or' for both
dataset.addRow(row);//setting element security

row = new Array();
row[0] = 'example_data.orders';
row[1] = JSSecurity.READ|JSSecurity.INSERT|JSSecurity.UPDATE|JSSecurity.DELETE|JSSecurity.TRACKING; //use bitwise 'or' for multiple flags
dataset.addRow(row);//setting table security

security.setSecuritySettings(dataset);//to be called in solution startup method
```

### UPDATE

Constant representing the update flag for table security.

**Returns**\
[Number](js-lib/number.md)

**Sample**

```javascript
var colNames = new Array();
colNames[0] = 'uuid';
colNames[1] = 'flags';
var dataset = databaseManager.createEmptyDataSet(0,colNames);

var row = new Array();
row[0] = '413a4d69-becb-4ae4-8fdd-980755d6a7fb';//normally retreived via security.getElementUUIDs(...)
row[1] = JSSecurity.VIEWABLE|JSSecurity.ACCESSIBLE; // use bitwise 'or' for both
dataset.addRow(row);//setting element security

row = new Array();
row[0] = 'example_data.orders';
row[1] = JSSecurity.READ|JSSecurity.INSERT|JSSecurity.UPDATE|JSSecurity.DELETE|JSSecurity.TRACKING; //use bitwise 'or' for multiple flags
dataset.addRow(row);//setting table security

security.setSecuritySettings(dataset);//to be called in solution startup method
```

### VIEWABLE

Constant representing the viewable flag for form security.

**Returns**\
[Number](js-lib/number.md)

**Sample**

```javascript
var colNames = new Array();
colNames[0] = 'uuid';
colNames[1] = 'flags';
var dataset = databaseManager.createEmptyDataSet(0,colNames);

var row = new Array();
row[0] = '413a4d69-becb-4ae4-8fdd-980755d6a7fb';//normally retreived via security.getElementUUIDs(...)
row[1] = JSSecurity.VIEWABLE|JSSecurity.ACCESSIBLE; // use bitwise 'or' for both
dataset.addRow(row);//setting element security

row = new Array();
row[0] = 'example_data.orders';
row[1] = JSSecurity.READ|JSSecurity.INSERT|JSSecurity.UPDATE|JSSecurity.DELETE|JSSecurity.TRACKING; //use bitwise 'or' for multiple flags
dataset.addRow(row);//setting table security

security.setSecuritySettings(dataset);//to be called in solution startup method
```

## Methods Details

### addUserToGroup(a\_userUID, groupName)

Adds an user to a named group. Note: this method can only be called by an admin.

**Parameters**\
[Object](js-lib/object.md) a\_userUID the user UID to be added\
[Object](js-lib/object.md) groupName the group to add to

**Returns**\
[Boolean](js-lib/boolean.md) true if added

**Sample**

```javascript
var userUID = security.getUserUID();
security.addUserToGroup(userUID, 'groupname');
```

### authenticate(authenticator\_solution, method)

Authenticate to the Servoy Server using one of the installed authenticators or the Servoy default authenticator.

Note: this method should be called from a login solution.

**Parameters**\
[String](js-lib/string.md) authenticator\_solution authenticator solution installed on the Servoy Server, null for servoy built-in authentication\
[String](js-lib/string.md) method authenticator method, null for servoy built-in authentication

**Returns**\
[Object](js-lib/object.md) authentication result from authenticator solution or boolean in case of servoy built-in authentication

**Sample**

```javascript
// create the credentials object as expected by the authenticator solution
var ok =  security.authenticate('myldap_authenticator', 'login', [scopes.globals.userName, scopes.globals.passWord])
if (!ok)
{
	plugins.dialogs.showErrorDialog('Login failed', 'OK')
}

// if no authenticator name is used, the credentials are checked using the Servoy built-in user management
ok = security.authenticate(null, null, [scopes.globals.userName, scopes.globals.passWord])
```

### authenticate(authenticator\_solution, method, credentials)

Authenticate to the Servoy Server using one of the installed authenticators or the Servoy default authenticator.

Note: this method should be called from a login solution, once logged in, the authenticate method has no effect.

**Parameters**\
[String](js-lib/string.md) authenticator\_solution authenticator solution installed on the Servoy Server, null for servoy built-in authentication\
[String](js-lib/string.md) method authenticator method, null for servoy built-in authentication\
[Array](js-lib/array.md) credentials array whose elements are passed as arguments to the authenticator method, in case of servoy built-in authentication this should be \[username, password]

**Returns**\
[Object](js-lib/object.md) authentication result from authenticator solution or boolean in case of servoy built-in authentication

**Sample**

```javascript
// create the credentials object as expected by the authenticator solution
var ok =  security.authenticate('myldap_authenticator', 'login', [scopes.globals.userName, scopes.globals.passWord])
if (!ok)
{
	plugins.dialogs.showErrorDialog('Login failed', 'OK')
}

// if no authenticator name is used, the credentials are checked using the Servoy built-in user management
ok = security.authenticate(null, null, [scopes.globals.userName, scopes.globals.passWord])
```

### canAccess(formName)

Returns whether form is accessible.

security.canAccess(formName)

**Parameters**\
[String](js-lib/string.md) formName form name

**Returns**\
[Boolean](js-lib/boolean.md) true if accessible

**Sample**

```javascript
```

### canAccess(formName, elementName)

Returns whether element from form is accessible.

security.canAccess(formName,elementName)

**Parameters**\
[String](js-lib/string.md) formName form name\
[String](js-lib/string.md) elementName element name from specified form

**Returns**\
[Boolean](js-lib/boolean.md) true if accessible

**Sample**

```javascript
```

### canDelete(dataSource)

Returns a boolean value for security rights.

**Parameters**\
[String](js-lib/string.md) dataSource the datasource

**Returns**\
[Boolean](js-lib/boolean.md) true if allowed

**Sample**

```javascript
var dataSource = controller.getDataSource();
var canDelete = security.canDelete(dataSource);
var canInsert = security.canInsert(dataSource);
var canUpdate = security.canUpdate(dataSource);
var canRead = security.canRead(dataSource);
application.output("Can delete? " + canDelete);
application.output("Can insert? " + canInsert);
application.output("Can update? " + canUpdate);
application.output("Can read? " + canRead);
```

### canInsert(dataSource)

Returns a boolean value for security rights.

**Parameters**\
[String](js-lib/string.md) dataSource the datasource

**Returns**\
[Boolean](js-lib/boolean.md) true if allowed

**Sample**

```javascript
var dataSource = controller.getDataSource();
var canDelete = security.canDelete(dataSource);
var canInsert = security.canInsert(dataSource);
var canUpdate = security.canUpdate(dataSource);
var canRead = security.canRead(dataSource);
application.output("Can delete? " + canDelete);
application.output("Can insert? " + canInsert);
application.output("Can update? " + canUpdate);
application.output("Can read? " + canRead);
```

### canRead(dataSource)

Returns a boolean value for security rights.

**Parameters**\
[String](js-lib/string.md) dataSource the datasource

**Returns**\
[Boolean](js-lib/boolean.md) true if allowed

**Sample**

```javascript
var dataSource = controller.getDataSource();
var canDelete = security.canDelete(dataSource);
var canInsert = security.canInsert(dataSource);
var canUpdate = security.canUpdate(dataSource);
var canRead = security.canRead(dataSource);
application.output("Can delete? " + canDelete);
application.output("Can insert? " + canInsert);
application.output("Can update? " + canUpdate);
application.output("Can read? " + canRead);
```

### canUpdate(dataSource)

Returns a boolean value for security rights.

**Parameters**\
[String](js-lib/string.md) dataSource the datasource

**Returns**\
[Boolean](js-lib/boolean.md) true if allowed

**Sample**

```javascript
var dataSource = controller.getDataSource();
var canDelete = security.canDelete(dataSource);
var canInsert = security.canInsert(dataSource);
var canUpdate = security.canUpdate(dataSource);
var canRead = security.canRead(dataSource);
application.output("Can delete? " + canDelete);
application.output("Can insert? " + canInsert);
application.output("Can update? " + canUpdate);
application.output("Can read? " + canRead);
```

### canView(formName)

Returns whether form is viewable.

security.canView(formName)

**Parameters**\
[String](js-lib/string.md) formName form name

**Returns**\
[Boolean](js-lib/boolean.md) true if viewable

**Sample**

```javascript
```

### canView(formName, elementName)

Returns whether element from form is viewable.

security.canView(formName,elementName)

**Parameters**\
[String](js-lib/string.md) formName form name\
[String](js-lib/string.md) elementName element name from specified form

**Returns**\
[Boolean](js-lib/boolean.md) true if viewable

**Sample**

```javascript
```

### changeGroupName(oldGroupName, newGroupName)

Changes the groupname of a group. Note: this method can only be called by an admin.

**Parameters**\
[Object](js-lib/object.md) oldGroupName the old name\
[String](js-lib/string.md) newGroupName the new name

**Returns**\
[Boolean](js-lib/boolean.md) true if changed

**Sample**

```javascript
security.changeGroupName('oldGroup', 'newGroup');
```

### changeUserName(a\_userUID, username)

Changes the username of the specified userUID. Note: this method can only be called by an admin user or a normal logged in user changing its own userName.

**Parameters**\
[Object](js-lib/object.md) a\_userUID the userUID to work on\
[String](js-lib/string.md) username the new username

**Returns**\
[Boolean](js-lib/boolean.md) true if changed

**Sample**

```javascript
if(security.changeUserName(security.getUserUID('name1'), 'name2'))
{
	application.output('Username changed');
}
```

### checkPassword(a\_userUID, password)

Returns true if the password for that userUID is correct, else false.

**Parameters**\
[Object](js-lib/object.md) a\_userUID the userUID to check the password for\
[String](js-lib/string.md) password the new password

**Returns**\
[Boolean](js-lib/boolean.md) true if password oke

**Sample**

```javascript
if(security.checkPassword(security.getUserUID(), 'password1'))
{
	security.setPassword(security.getUserUID(), 'password2')
}
else
{
	application.output('wrong password')
}
```

### createGroup(groupName)

Creates a group, returns the groupname (or null when group couldn't be created). Note: this method can only be called by an admin.

**Parameters**\
[String](js-lib/string.md) groupName the group name to create

**Returns**\
[String](js-lib/string.md) the created groupname

**Sample**

```javascript
var deleteGroup = true;
//ceate a group
var groupName = security.createGroup('myGroup');
if (groupName)
{
	//create a user
	var uid = security.createUser('myusername', 'mypassword');
	if (uid) //test if user was created
	{
		//set a newUID for the user
		var isChanged = security.setUserUID(uid,'myUserUID')
		// add user to group
		security.addUserToGroup(uid, groupName);
		// if not delete group, do delete group
		if (deleteGroup)
		{
			security.deleteGroup(groupName);
		}
	}
}
```

### createUser(username, password)

Creates a new user, returns new uid (or null when group couldn't be created or user alreay exist). Note: this method can only be called by an admin.

**Parameters**\
[String](js-lib/string.md) username the username\
[String](js-lib/string.md) password the user password

**Returns**\
[Object](js-lib/object.md) the userUID the created userUID, will be same if provided

**Sample**

```javascript
var removeUser = true;
//create a user
var uid = security.createUser('myusername', 'mypassword');
if (uid) //test if user was created
{
	// Get all the groups
	var set = security.getGroups();
	for(var p = 1 ; p <= set.getMaxRowIndex() ; p++)
	{
		// output name of the group
		application.output(set.getValue(p, 2));
		// add user to group
		security.addUserToGroup(uid, set.getValue(p,2));
	}
	// if not remove user, remove user from all the groups
	if(!removeUser)
	{
		// get now all the groups that that users has (all if above did go well)
		var set =security.getUserGroups(uid);
		for(var p = 1;p<=set.getMaxRowIndex();p++)
		{
			// output name of the group
			application.output(set.getValue(p, 2));
			// remove the user from the group
			security.removeUserFromGroup(uid, set.getValue(p,2));
		}
	}
	else
	{
		// delete the user (the user will be removed from the groups)
		security.deleteUser(uid);
	}
}
```

### createUser(username, password, userUID)

Creates a new user, returns new uid (or null when group couldn't be created or user alreay exist). Note: this method can only be called by an admin.

**Parameters**\
[String](js-lib/string.md) username the username\
[String](js-lib/string.md) password the user password\
[Object](js-lib/object.md) userUID the user UID to use

**Returns**\
[Object](js-lib/object.md) the userUID the created userUID, will be same if provided

**Sample**

```javascript
var removeUser = true;
//create a user
var uid = security.createUser('myusername', 'mypassword');
if (uid) //test if user was created
{
	// Get all the groups
	var set = security.getGroups();
	for(var p = 1 ; p <= set.getMaxRowIndex() ; p++)
	{
		// output name of the group
		application.output(set.getValue(p, 2));
		// add user to group
		security.addUserToGroup(uid, set.getValue(p,2));
	}
	// if not remove user, remove user from all the groups
	if(!removeUser)
	{
		// get now all the groups that that users has (all if above did go well)
		var set =security.getUserGroups(uid);
		for(var p = 1;p<=set.getMaxRowIndex();p++)
		{
			// output name of the group
			application.output(set.getValue(p, 2));
			// remove the user from the group
			security.removeUserFromGroup(uid, set.getValue(p,2));
		}
	}
	else
	{
		// delete the user (the user will be removed from the groups)
		security.deleteUser(uid);
	}
}
```

### deleteGroup(groupName)

Deletes a group, returns true if no error was reported. Note: this method can only be called by an admin.

**Parameters**\
[Object](js-lib/object.md) groupName the name of the group to delete

**Returns**\
[Boolean](js-lib/boolean.md) true if deleted

**Sample**

```javascript
var deleteGroup = true;
//ceate a group
var groupName = security.createGroup('myGroup');
if (groupName)
{
	//create a user
	var uid = security.createUser('myusername', 'mypassword');
	if (uid) //test if user was created
	{
		//set a newUID for the user
		var isChanged = security.setUserUID(uid,'myUserUID')
		// add user to group
		security.addUserToGroup(uid, groupName);
		// if not delete group, do delete group
		if (deleteGroup)
		{
			security.deleteGroup(groupName);
		}
	}
}
```

### deleteUser(userUID)

Deletes an user. returns true if no error was reported. Note: this method can only be called by an admin.

**Parameters**\
[Object](js-lib/object.md) userUID The UID of the user to be deleted.

**Returns**\
[Boolean](js-lib/boolean.md) true if the user is successfully deleted.

**Sample**

```javascript
var removeUser = true;
//create a user
var uid = security.createUser('myusername', 'mypassword');
if (uid) //test if user was created
{
	// Get all the groups
	var set = security.getGroups();
	for(var p = 1 ; p <= set.getMaxRowIndex() ; p++)
	{
		// output name of the group
		application.output(set.getValue(p, 2));
		// add user to group
		security.addUserToGroup(uid, set.getValue(p,2));
	}
	// if not remove user, remove user from all the groups
	if(!removeUser)
	{
		// get now all the groups that that users has (all if above did go well)
		var set =security.getUserGroups(uid);
		for(var p = 1;p<=set.getMaxRowIndex();p++)
		{
			// output name of the group
			application.output(set.getValue(p, 2));
			// remove the user from the group
			security.removeUserFromGroup(uid, set.getValue(p,2));
		}
	}
	else
	{
		// delete the user (the user will be removed from the groups)
		security.deleteUser(uid);
	}
}
```

### getClientID()

Returns the client ID.

**Returns**\
[String](js-lib/string.md) the clientId as seen on the server admin page

**Sample**

```javascript
var clientId = security.getClientID()
```

### getElementUUIDs(formname)

Returns the form elements UUID's as dataset, the one with no name is the form itself.

**Parameters**\
[String](js-lib/string.md) formname the formname to retieve the dataset for

**Returns**\
[JSDataSet](database-manager/jsdataset.md) dataset with element info

**Sample**

```javascript
var formElementsUUIDDataSet = security.getElementUUIDs('orders_form');
```

### getGroups()

Get all the groups (returns a dataset). first id column is deprecated!, use only the group name column.

**Returns**\
[JSDataSet](database-manager/jsdataset.md) dataset with all the groups

**Sample**

```javascript
var removeUser = true;
//create a user
var uid = security.createUser('myusername', 'mypassword');
if (uid) //test if user was created
{
	// Get all the groups
	var set = security.getGroups();
	for(var p = 1 ; p <= set.getMaxRowIndex() ; p++)
	{
		// output name of the group
		application.output(set.getValue(p, 2));
		// add user to group
		security.addUserToGroup(uid, set.getValue(p,2));
	}
	// if not remove user, remove user from all the groups
	if(!removeUser)
	{
		// get now all the groups that that users has (all if above did go well)
		var set =security.getUserGroups(uid);
		for(var p = 1;p<=set.getMaxRowIndex();p++)
		{
			// output name of the group
			application.output(set.getValue(p, 2));
			// remove the user from the group
			security.removeUserFromGroup(uid, set.getValue(p,2));
		}
	}
	else
	{
		// delete the user (the user will be removed from the groups)
		security.deleteUser(uid);
	}
}
```

### getSystemUserName()

Retrieves the username of the currently logged in user on operating system level.

**Returns**\
[String](js-lib/string.md) the os user name

**Sample**

```javascript
//gets the current os username
var osUserName = security.getSystemUserName();
```

### getTenantValue()

Retrieve the tenant value for this Client, this value will be used as the value for all tables that have a column marked as a tenant column. This results in adding a table filter for that table based on that column and the this value.

A client with tenant value will only receive databroadcasts from other clients that have no or a common tenant value set Be sure to not access or depend on records having different tenant values, as no databroadcasts will be received for those

**Returns**\
[Array](js-lib/array.md) An array of tenant values for this client.

**Sample**

```javascript
```

### getUserGroups()

Get all the groups of the current user.

**Returns**\
[JSDataSet](database-manager/jsdataset.md) dataset with groupnames

**Sample**

```javascript
//get all the users in the security settings (Returns a JSDataset)
var dsUsers = security.getUsers()

//loop through each user to get their group
//The getValue call is (row,column) where column 1 == id and 2 == name
for(var i=1 ; i<=dsUsers.getMaxRowIndex() ; i++)
{
	//print to the output debugger tab: "user: " and the username
	application.output("user:" + dsUsers.getValue(i,2));

	//set p to the user group for the current user
	/** @type {JSDataSet} */
	var p = security.getUserGroups(dsUsers.getValue(i,1));

	for(k=1;k<=p.getMaxRowIndex();k++)
	{
		//print to the output debugger tab: "group" and the group(s)
		//the user belongs to
		application.output("group: " + p.getValue(k,2));
	}
}
```

### getUserGroups(userUID)

Get all the groups for given user UID.

**Parameters**\
[Object](js-lib/object.md) userUID to retrieve the user groups

**Returns**\
[JSDataSet](database-manager/jsdataset.md) dataset with groupnames

**Sample**

```javascript
//get all the users in the security settings (Returns a JSDataset)
var dsUsers = security.getUsers()

//loop through each user to get their group
//The getValue call is (row,column) where column 1 == id and 2 == name
for(var i=1 ; i<=dsUsers.getMaxRowIndex() ; i++)
{
	//print to the output debugger tab: "user: " and the username
	application.output("user:" + dsUsers.getValue(i,2));

	//set p to the user group for the current user
	/** @type {JSDataSet} */
	var p = security.getUserGroups(dsUsers.getValue(i,1));

	for(k=1;k<=p.getMaxRowIndex();k++)
	{
		//print to the output debugger tab: "group" and the group(s)
		//the user belongs to
		application.output("group: " + p.getValue(k,2));
	}
}
```

### getUserName()

Get the current user name (null if not logged in), finds the user name for given user UID if passed as parameter.

**Returns**\
[String](js-lib/string.md) the user name

**Sample**

```javascript
//gets the current loggedIn username
var userName = security.getUserName();
```

### getUserName(userUID)

Get the current user name (null if not logged in), finds the user name for given user UID if passed as parameter.

**Parameters**\
[Object](js-lib/object.md) userUID the user UID used to retrieve the name

**Returns**\
[String](js-lib/string.md) the user name

**Sample**

```javascript
//gets the current loggedIn username
var userName = security.getUserName();
```

### getUserUID()

Get the current user UID (null if not logged in); finds the userUID for given user\_name if passed as parameter.

**Returns**\
[String](js-lib/string.md) the userUID

**Sample**

```javascript
//gets the current loggedIn username
var userName = security.getUserName();
//gets the uid of the given username
var userUID = security.getUserUID(userName);
//is the same as above
//var my_userUID = security.getUserUID();
```

### getUserUID(username)

Get the current user UID (null if not logged in); finds the userUID for given user\_name if passed as parameter.

**Parameters**\
[String](js-lib/string.md) username the username to find the userUID for

**Returns**\
[String](js-lib/string.md) the userUID

**Sample**

```javascript
//gets the current loggedIn username
var userName = security.getUserName();
//gets the uid of the given username
var userUID = security.getUserUID(userName);
//is the same as above
//var my_userUID = security.getUserUID();
```

### getUsers()

Get all the users in the security settings (returns a dataset).

**Returns**\
[JSDataSet](database-manager/jsdataset.md) dataset with all the users

**Sample**

```javascript
//get all the users in the security settings (Returns a JSDataset)
var dsUsers = security.getUsers()

//loop through each user to get their group
//The getValue call is (row,column) where column 1 == id and 2 == name
for(var i=1 ; i<=dsUsers.getMaxRowIndex() ; i++)
{
	//print to the output debugger tab: "user: " and the username
	application.output("user:" + dsUsers.getValue(i,2));

	//set p to the user group for the current user
	/** @type {JSDataSet} */
	var p = security.getUserGroups(dsUsers.getValue(i,1));

	for(k=1;k<=p.getMaxRowIndex();k++)
	{
		//print to the output debugger tab: "group" and the group(s)
		//the user belongs to
		application.output("group: " + p.getValue(k,2));
	}
}
```

### getUsers(groupName)

Get all the users in the security settings (returns a dataset).

**Parameters**\
[String](js-lib/string.md) groupName the group to filter on

**Returns**\
[JSDataSet](database-manager/jsdataset.md) dataset with all the users

**Sample**

```javascript
//get all the users in the security settings (Returns a JSDataset)
var dsUsers = security.getUsers()

//loop through each user to get their group
//The getValue call is (row,column) where column 1 == id and 2 == name
for(var i=1 ; i<=dsUsers.getMaxRowIndex() ; i++)
{
	//print to the output debugger tab: "user: " and the username
	application.output("user:" + dsUsers.getValue(i,2));

	//set p to the user group for the current user
	/** @type {JSDataSet} */
	var p = security.getUserGroups(dsUsers.getValue(i,1));

	for(k=1;k<=p.getMaxRowIndex();k++)
	{
		//print to the output debugger tab: "group" and the group(s)
		//the user belongs to
		application.output("group: " + p.getValue(k,2));
	}
}
```

### isUserMemberOfGroup(groupName)

Check whatever the current user is part of the specified group

**Parameters**\
[String](js-lib/string.md) groupName name of the group to check

**Returns**\
[Boolean](js-lib/boolean.md) dataset with groupnames

**Sample**

```javascript
//check whatever user is part of the Administrators group
if(security.isUserMemberOfGroup('Administrators', security.getUserUID('admin')))
{
	// do administration stuff
}
```

### isUserMemberOfGroup(groupName, userUID)

Check whatever the user specified as parameter is part of the specified group.

**Parameters**\
[String](js-lib/string.md) groupName name of the group to check\
[Object](js-lib/object.md) userUID UID of the user to check

**Returns**\
[Boolean](js-lib/boolean.md) dataset with groupnames

**Sample**

```javascript
//check whatever user is part of the Administrators group
if(security.isUserMemberOfGroup('Administrators', security.getUserUID('admin')))
{
	// do administration stuff
}
```

### login(username, a\_userUID, groups)

Login to be able to leave the solution loginForm.

Example: Group names may be received from LDAP (Lightweight Directory Access Protocol) - a standard protocol used in web browsers and email applications to enable lookup queries that access a directory listing.

**Parameters**\
[String](js-lib/string.md) username the username, like 'JamesWebb'\
[Object](js-lib/object.md) a\_userUID the user UID to process login for\
[Array](js-lib/array.md) groups the groups array

**Returns**\
[Boolean](js-lib/boolean.md) true if loggedin

**Sample**

```javascript
var groups = ['Administrators']; //normally these groups are for example received from LDAP
var user_uid = scopes.globals.email; //also this uid might be received from external authentication method
var ok =  security.login(scopes.globals.username, user_uid , groups)
if (!ok)
{
	plugins.dialogs.showErrorDialog('Login failure',  'Already logged in? or no user_uid/groups specified?', 'OK')
}
```

### logout()

Logout the current user and close the solution, if the solution requires authentication and user is logged in. You can redirect to another solution if needed; if you want to go to a different url, you need to call application.showURL(url) before calling security.logout() (this is only applicable for Web Client). An alternative option to close a solution and to open another solution, while keeping the user logged in, is application.closeSolution().

**Returns**\
void

**Sample**

```javascript
//Set the url to go to after logout.
//application.showURL('http://www.servoy.com', '_self');  //Web Client only
security.logout();
//security.logout('solution_name');//log out and close current solution and open solution 'solution_name'
//security.logout('solution_name','global_method_name');//log out, close current solution, open solution 'solution_name' and call global method 'global_method_name' of the newly opened solution
//security.logout('solution_name','global_method_name','my_string_argument');//log out, close current solution, open solution 'solution_name', call global method 'global_method_name' with argument 'my_argument'
//security.logout('solution_name','global_second_method_name',2);
//security.logout('solution_name', {a: 'my_string_argument', p1: 'param1', p2: 'param2'});//log out, close current solution, open solution 'solution_name', call (login) solution's onOpen with argument 'my_argument' and queryParams p1,p2
//Note: specifying a solution will not work in the Developer due to debugger dependencies
//specified solution should be of compatible type with client (normal type or client specific(Smart client only/Web client only) type )
```

### logout(solutionToLoad)

Logout the current user and close the solution, if the solution requires authentication and user is logged in. You can redirect to another solution if needed; if you want to go to a different url, you need to call application.showURL(url) before calling security.logout() (this is only applicable for Web Client). An alternative option to close a solution and to open another solution, while keeping the user logged in, is application.closeSolution().

**Parameters**\
[String](js-lib/string.md) solutionToLoad the solution to load after logout

**Returns**\
void

**Sample**

```javascript
//Set the url to go to after logout.
//application.showURL('http://www.servoy.com', '_self');  //Web Client only
security.logout();
//security.logout('solution_name');//log out and close current solution and open solution 'solution_name'
//security.logout('solution_name','global_method_name');//log out, close current solution, open solution 'solution_name' and call global method 'global_method_name' of the newly opened solution
//security.logout('solution_name','global_method_name','my_string_argument');//log out, close current solution, open solution 'solution_name', call global method 'global_method_name' with argument 'my_argument'
//security.logout('solution_name','global_second_method_name',2);
//security.logout('solution_name', {a: 'my_string_argument', p1: 'param1', p2: 'param2'});//log out, close current solution, open solution 'solution_name', call (login) solution's onOpen with argument 'my_argument' and queryParams p1,p2
//Note: specifying a solution will not work in the Developer due to debugger dependencies
//specified solution should be of compatible type with client (normal type or client specific(Smart client only/Web client only) type )
```

### logout(solutionToLoad, argument)

Logout the current user and close the solution, if the solution requires authentication and user is logged in. You can redirect to another solution if needed; if you want to go to a different url, you need to call application.showURL(url) before calling security.logout() (this is only applicable for Web Client). An alternative option to close a solution and to open another solution, while keeping the user logged in, is application.closeSolution().

**Parameters**\
[String](js-lib/string.md) solutionToLoad the solution to load after logout\
[Object](js-lib/object.md) argument the argument to pass to the (login) solution onOpen

**Returns**\
void

**Sample**

```javascript
//Set the url to go to after logout.
//application.showURL('http://www.servoy.com', '_self');  //Web Client only
security.logout();
//security.logout('solution_name');//log out and close current solution and open solution 'solution_name'
//security.logout('solution_name','global_method_name');//log out, close current solution, open solution 'solution_name' and call global method 'global_method_name' of the newly opened solution
//security.logout('solution_name','global_method_name','my_string_argument');//log out, close current solution, open solution 'solution_name', call global method 'global_method_name' with argument 'my_argument'
//security.logout('solution_name','global_second_method_name',2);
//security.logout('solution_name', {a: 'my_string_argument', p1: 'param1', p2: 'param2'});//log out, close current solution, open solution 'solution_name', call (login) solution's onOpen with argument 'my_argument' and queryParams p1,p2
//Note: specifying a solution will not work in the Developer due to debugger dependencies
//specified solution should be of compatible type with client (normal type or client specific(Smart client only/Web client only) type )
```

### logout(solutionToLoad, method)

Logout the current user and close the solution, if the solution requires authentication and user is logged in. You can redirect to another solution if needed; if you want to go to a different url, you need to call application.showURL(url) before calling security.logout() (this is only applicable for Web Client). An alternative option to close a solution and to open another solution, while keeping the user logged in, is application.closeSolution().

**Parameters**\
[String](js-lib/string.md) solutionToLoad the solution to load after logout\
[String](js-lib/string.md) method the method to run in the solution to load

**Returns**\
void

**Sample**

```javascript
//Set the url to go to after logout.
//application.showURL('http://www.servoy.com', '_self');  //Web Client only
security.logout();
//security.logout('solution_name');//log out and close current solution and open solution 'solution_name'
//security.logout('solution_name','global_method_name');//log out, close current solution, open solution 'solution_name' and call global method 'global_method_name' of the newly opened solution
//security.logout('solution_name','global_method_name','my_string_argument');//log out, close current solution, open solution 'solution_name', call global method 'global_method_name' with argument 'my_argument'
//security.logout('solution_name','global_second_method_name',2);
//security.logout('solution_name', {a: 'my_string_argument', p1: 'param1', p2: 'param2'});//log out, close current solution, open solution 'solution_name', call (login) solution's onOpen with argument 'my_argument' and queryParams p1,p2
//Note: specifying a solution will not work in the Developer due to debugger dependencies
//specified solution should be of compatible type with client (normal type or client specific(Smart client only/Web client only) type )
```

### logout(solutionToLoad, method, argument)

Logout the current user and close the solution, if the solution requires authentication and user is logged in. You can redirect to another solution if needed; if you want to go to a different url, you need to call application.showURL(url) before calling security.logout() (this is only applicable for Web Client). An alternative option to close a solution and to open another solution, while keeping the user logged in, is application.closeSolution().

**Parameters**\
[String](js-lib/string.md) solutionToLoad the solution to load after logout\
[String](js-lib/string.md) method the method to run in the solution to load\
[Object](js-lib/object.md) argument the argument to pass to the method to run

**Returns**\
void

**Sample**

```javascript
//Set the url to go to after logout.
//application.showURL('http://www.servoy.com', '_self');  //Web Client only
security.logout();
//security.logout('solution_name');//log out and close current solution and open solution 'solution_name'
//security.logout('solution_name','global_method_name');//log out, close current solution, open solution 'solution_name' and call global method 'global_method_name' of the newly opened solution
//security.logout('solution_name','global_method_name','my_string_argument');//log out, close current solution, open solution 'solution_name', call global method 'global_method_name' with argument 'my_argument'
//security.logout('solution_name','global_second_method_name',2);
//security.logout('solution_name', {a: 'my_string_argument', p1: 'param1', p2: 'param2'});//log out, close current solution, open solution 'solution_name', call (login) solution's onOpen with argument 'my_argument' and queryParams p1,p2
//Note: specifying a solution will not work in the Developer due to debugger dependencies
//specified solution should be of compatible type with client (normal type or client specific(Smart client only/Web client only) type )
```

### removeUserFromGroup(a\_userUID, groupName)

Removes an user from a group. Note: this method can only be called by an admin.

**Parameters**\
[Object](js-lib/object.md) a\_userUID the user UID to be removed\
[Object](js-lib/object.md) groupName the group to remove from

**Returns**\
[Boolean](js-lib/boolean.md) true if removed

**Sample**

```javascript
var removeUser = true;
//create a user
var uid = security.createUser('myusername', 'mypassword');
if (uid) //test if user was created
{
	// Get all the groups
	var set = security.getGroups();
	for(var p = 1 ; p <= set.getMaxRowIndex() ; p++)
	{
		// output name of the group
		application.output(set.getValue(p, 2));
		// add user to group
		security.addUserToGroup(uid, set.getValue(p,2));
	}
	// if not remove user, remove user from all the groups
	if(!removeUser)
	{
		// get now all the groups that that users has (all if above did go well)
		var set =security.getUserGroups(uid);
		for(var p = 1;p<=set.getMaxRowIndex();p++)
		{
			// output name of the group
			application.output(set.getValue(p, 2));
			// remove the user from the group
			security.removeUserFromGroup(uid, set.getValue(p,2));
		}
	}
	else
	{
		// delete the user (the user will be removed from the groups)
		security.deleteUser(uid);
	}
}
```

### setPassword(a\_userUID, password)

Set a new password for the given userUID. Note: this method can only be called by an admin user or a normal logged in user changing its own password.

**Parameters**\
[Object](js-lib/object.md) a\_userUID the userUID to set the new password for\
[String](js-lib/string.md) password the new password

**Returns**\
[Boolean](js-lib/boolean.md) true if changed

**Sample**

```javascript
if(security.checkPassword(security.getUserUID(), 'password1'))
{
	security.setPassword(security.getUserUID(), 'password2')
}
else
{
	application.output('wrong password')
}
```

### setSecuritySettings(dataset)

Sets the security settings; the entries contained in the given dataset will override those contained in the current security settings.

NOTE: The security.getElementUUIDs and security.setSecuritySettings functions can be used to define custom security that overrides Servoy security. For additional information see the function security.getElementUUIDs.

**Parameters**\
[Object](js-lib/object.md) dataset the dataset with security settings

**Returns**\
void

**Sample**

```javascript
var colNames = new Array();
colNames[0] = 'uuid';
colNames[1] = 'flags';
var dataset = databaseManager.createEmptyDataSet(0,colNames);

var row = new Array();
row[0] = '413a4d69-becb-4ae4-8fdd-980755d6a7fb';//normally retreived via security.getElementUUIDs(...)
row[1] = JSSecurity.VIEWABLE|JSSecurity.ACCESSIBLE; // use bitwise 'or' for both
dataset.addRow(row);//setting element security

row = new Array();
row[0] = 'example_data.orders';
row[1] = JSSecurity.READ|JSSecurity.INSERT|JSSecurity.UPDATE|JSSecurity.DELETE|JSSecurity.TRACKING; //use bitwise 'or' for multiple flags
dataset.addRow(row);//setting table security

security.setSecuritySettings(dataset);//to be called in solution startup method
```

### setTenantValue(value)

Set the tenant value for this Client, this value will be used as the value for all tables that have a column marked as a tenant column. This results in adding a table filter for that table based on that column and the this value.

This value will be auto filled in for all the columns that are marked as a tenant column. If you give an array of values then the first array value is used for this.

When a tenant value is set the client will only receive databroadcasts from other clients that have no or a common tenant value set Be sure to not access or depend on records having different tenant values, as no databroadcasts will be received for those

**Parameters**\
[Object](js-lib/object.md) value a single tenant value or an array of tenant values to filter tables having a column flagged as Tenant column by.

**Returns**\
void

**Sample**

```javascript
```

### setUserUID(a\_userUID, newUserUID)

Set a new userUID for the given userUID. Note: this method can only be called by an admin.

**Parameters**\
[Object](js-lib/object.md) a\_userUID the userUID to set the new user UID for\
[String](js-lib/string.md) newUserUID the new user UID

**Returns**\
[Boolean](js-lib/boolean.md) true if changed

**Sample**

```javascript
var deleteGroup = true;
//ceate a group
var groupName = security.createGroup('myGroup');
if (groupName)
{
	//create a user
	var uid = security.createUser('myusername', 'mypassword');
	if (uid) //test if user was created
	{
		//set a newUID for the user
		var isChanged = security.setUserUID(uid,'myUserUID')
		// add user to group
		security.addUserToGroup(uid, groupName);
		// if not delete group, do delete group
		if (deleteGroup)
		{
			security.deleteGroup(groupName);
		}
	}
}
```
