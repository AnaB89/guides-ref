# API Documentation

### Classes

[Permission](api-documentation.md#permission)

Represents a security permission in the system. Mapped internally to a Servoy security group which must be defined.

[Role](api-documentation.md#role)

Security role which can have [user](api-documentation.md#user) members and can be granted [permissions](api-documentation.md#permission).

[Session](api-documentation.md#session)

Security application session created by a [User](api-documentation.md#user) which starts when the user [logs in](api-documentation.md#login-user-useruid-permissionstoapply-boolean) and ends when the user [logs out](api-documentation.md#logout).

[Tenant](api-documentation.md#tenant)

Tenant account which is used to segregate all data. [Users](api-documentation.md#user) and [Roles](api-documentation.md#role) belong to a Tenant.

[User](api-documentation.md#user)

Application user account associated with a [Tenant](api-documentation.md#tenant). Security [Permissions](api-documentation.md#permission) are granted to users through their [Role](api-documentation.md#role) membership.

### Functions

[changeExternalDBTransactionSupportFlag(mustSupportExternalTransactions)](api-documentation.md#changeexternaldbtransactionsupportflag-mustsupportexternaltransactions)

Use this method to change the behavior of the svySecurity module with respect to DB transactions.

If the flag is set to false (default) then when saving or deleting security-related records if an external DB transaction is detected the operation will fail. If the flag is set to true then when saving or deleting security-related records the module will start/commit a DB transaction only if an external DB transaction is not detected. On exceptions any DB transaction will be rolled back regardless if it is started internally or externally (exceptions will be propagated to the external transaction so callers will be able to react on them accordingly)

[cloneTenant(tenantToClone, name, \[makeSlave\])](api-documentation.md#clonetenant-tenanttoclone-name-makeslave-tenant) ⇒ [`Tenant`](api-documentation.md#tenant)

Creates and returns a new tenant with the specified name as a clone of the given tenant. The names of tenants must be unique in the system. The cloned tenant has the same roles and role permissions as the original. When makeSlave is true, the newly created clone will be a slave of the tenant to clone, inheriting all role / permission changes made to the master.\
WARNING: Cannot call this function when logged in as an user.

[consumeAccessToken(token)](api-documentation.md#consumeaccesstoken-token-user) ⇒ [`User`](api-documentation.md#user)

Consumes a secure-access token and returns the user associated with the token if a valid match was found. Tokens may be used only once to identify a user. Subsequent calls to consume the same token will fail. Secure-access tokens are created with [generateAccessToken](api-documentation.md#user.generateaccesstoken-duration-string)

[createTenant(name)](api-documentation.md#createtenant-name-tenant) ⇒ [`Tenant`](api-documentation.md#tenant)

Creates and returns a new tenant with the specified name. The names of tenants must be unique in the system.

[deleteTenant(tenant)](api-documentation.md#deletetenant-tenant-boolean) ⇒ `Boolean`

Immediately and permanently deletes the specified tenant and all records associated with it, including all users and roles. Tenant will not be deleted if it has users with active sessions.\
If the deleted tenant is a Master tenant and is a slave of another master tenant, this operation will replace the master tenant of it's direct slaves with the master of the tenant that is deleted; If the delated tenant is a Master tenant and has no Master tenant, this operation will remove the master from all it's direct slaves.

[getActiveSessions()](api-documentation.md#getactivesessions-array-.less-than-session-greater-than) ⇒ [`[ 'Array' ].<Session>`](api-documentation.md#session)

Gets all active sessions for the application.

[getPermission(name)](api-documentation.md#getpermission-name-permission) ⇒ [`Permission`](api-documentation.md#permission)

Gets a permission by its unique permission name.

[getPermissions()](api-documentation.md#getpermissions-array-.less-than-permission-greater-than) ⇒ [`[ 'Array' ].<Permission>`](api-documentation.md#permission)

Gets all permissions available in this application.

[getRole(roleName, \[tenantName\])](api-documentation.md#getrole-rolename-tenantname-role) ⇒ [`Role`](api-documentation.md#role)

Gets a role by the specified role name and tenant name. If tenant name is not specified will use the tenant of the user currently logged in the application, if available.

[getSession()](api-documentation.md#getsession-session) ⇒ [`Session`](api-documentation.md#session)

Gets the current user session or null if no session initialized (no user is currently [logged in](api-documentation.md#login-user-useruid-permissionstoapply-boolean)).

[getSessionCount()](api-documentation.md#getsessioncount-number) ⇒ `Number`

Gets the number of all unique sessions which have ever been initialized in the application. This includes both active sessions (for users currently logged in the application) and inactive sessions (sessions from the past which have already been closed).

[getTenant(\[name\])](api-documentation.md#gettenant-name-tenant) ⇒ [`Tenant`](api-documentation.md#tenant)

Gets a tenant by its unique tenant name. If tenant name is not specified then will return the tenant of the currently logged in user. If tenant name is not specified and no user is currently logged in then will return null.

[getTenants()](api-documentation.md#gettenants-array-.less-than-tenant-greater-than) ⇒ [`[ 'Array' ].<Tenant>`](api-documentation.md#tenant)

Gets all tenants in the system.

[getUser(\[userName\], \[tenantName\])](api-documentation.md#getuser-username-tenantname-user) ⇒ [`User`](api-documentation.md#user)

Gets a user by the specified username and tenant name. If username is not specified will return the user currently logged in the application, if available.

[getUsers()](api-documentation.md#getusers-array-.less-than-user-greater-than) ⇒ [`[ 'Array' ].<User>`](api-documentation.md#user)

Gets all users in the system.

[getVersion()](api-documentation.md#getversion-string) ⇒ `String`

Gets the version of this module

[login(user, \[userUid\], \[permissionsToApply\])](api-documentation.md#login-user-useruid-permissionstoapply-boolean) ⇒ `Boolean`

Logs in the specified user and initializes a new [Session](api-documentation.md#session) for it. The login request will not be successful if the user account or the parent [tenant](api-documentation.md#user.gettenant-tenant) account [is locked](api-documentation.md#user.islocked-boolean) and the lock has not [expired](api-documentation.md#user.getlockexpiration-date) yet. The login request will not be successful also if no [permissions](api-documentation.md#user.getpermissions-array-.less-than-permission-greater-than) have been granted to the specified user. This method internally calls the standard Servoy security.login().

[logout()](api-documentation.md#logout)

Logs the current user out of the application and closes the associated [Session](api-documentation.md#session). This method internally calls security.logout() to end the Servoy client session.

[syncPermissions(\[forcePermissionRemoval\])](api-documentation.md#syncpermissions-forcepermissionremoval)

Utility to sync permission records to the internal, design-time Servoy Security Groups. This should be called on solution import or on startup This action will create new permission records.

NOTE: This action will not delete permissions which have been removed from internal security. Design-time groups should never be renamed. They will be seen only as an ADD and will lose their tie to roles.

### Permission

Represents a security permission in the system. Mapped internally to a Servoy security group which must be defined.

* [Permission](api-documentation.md#permission)
  * [.addRole(role)](api-documentation.md#permission.addrole-role-permission) ⇒ [`Permission`](api-documentation.md#permission)
  * [.getDisplayName()](api-documentation.md#permission.getdisplayname-string) ⇒ `String`
  * [.getName()](api-documentation.md#permission.getname-string) ⇒ `String`
  * [.getRoles()](api-documentation.md#permission.getroles-array-.less-than-role-greater-than) ⇒ [`[ 'Array' ].<Role>`](api-documentation.md#role)
  * [.getUsers()](api-documentation.md#Permission+getUsers) ⇒ [`[ 'Array' ].<User>`](api-documentation.md#user)
  * [.hasRole(role)](api-documentation.md#permission.hasrole-role-boolean) ⇒ `Boolean`
  * [.removeRole(role)](api-documentation.md#permission.removerole-role-permission) ⇒ [`Permission`](api-documentation.md#permission)
  * [.setDisplayName(\[displayName\])](api-documentation.md#permission.setdisplayname-displayname-permission) ⇒ [`Permission`](api-documentation.md#permission)
  * [new Permission(record)](api-documentation.md#new-permission-record)

***

#### permission.addRole(role) ⇒ [`Permission`](api-documentation.md#permission)

Grants this permission to the specified role. The permission will be granted to all users that are members of the specified role.\
If the tenant of this permission is a master tenant, the role will also be added to the same permission for all the slaves of this permission tenant.\
You cannot grant permission to role of a master tenant when logged in as an user. You cannot grant permission to role of a slave tenant at anytime.

**Returns**: [`Permission`](api-documentation.md#permission) - This permission for call-chaining support. Throws an exception when permission cannot be granted.

| Param | Type                                | Description                                                |
| ----- | ----------------------------------- | ---------------------------------------------------------- |
| role  | [`Role`](api-documentation.md#role) | The role object to which the permission should be granted. |

#### permission.getDisplayName() ⇒ `String`

Gets the display name of this permission. The display name can be set using [setDisplayName](api-documentation.md#permission.setdisplayname-displayname-permission).

**Returns**: `String` - The display name of the permission. Can be null.

#### permission.getName() ⇒ `String`

Gets the name of this permission. The permission name is unique in the system and matches a Servoy security group name.

**Returns**: `String` - The name of the permission.

#### permission.getRoles() ⇒ [`[ 'Array' ].<Role>`](api-documentation.md#role)

Gets all the roles to which this permission is granted.

**Returns**: [`[ 'Array' ].<Role>`](api-documentation.md#role) - An array with all roles to which this permission is granted or an empty array if the permission has not been granted to any role.

#### permission.getUsers() ⇒ [`[ 'Array' ].<User>`](api-documentation.md#user)

Gets all users whom this permission is granted to via the users' role membership.

**Returns**: [`[ 'Array' ].<User>`](api-documentation.md#user) - An array with all users whom this permission is granted to or an empty array if no user has this permission.

#### permission.hasRole(role) ⇒ `Boolean`

Checks if this permission is granted to the specified role.

**Returns**: `Boolean` - True if this permission is granted to the specified role.

| Param | Type                                            | Description                                       |
| ----- | ----------------------------------------------- | ------------------------------------------------- |
| role  | [`Role`](api-documentation.md#role) \| `String` | The role object or the name of the role to check. |

#### permission.removeRole(role) ⇒ [`Permission`](api-documentation.md#permission)

Removes this permission from the specified role. The permission will no longer be granted to all users that are members of the specified role.\
If the tenant of this permission is a master tenant, the role will also be removed from the same permission for all the slaves of this permission tenant.\
You cannot remove permission from role of a master tenant when logged in as an user. You cannot remove permission from role of a slave tenant at anytime.

**Returns**: [`Permission`](api-documentation.md#permission) - This permission for call-chaining support. Throws an exception when permission cannot be removed.

| Param | Type                                            | Description                                        |
| ----- | ----------------------------------------------- | -------------------------------------------------- |
| role  | [`Role`](api-documentation.md#Role) \| `String` | The role object or the name of the role to remove. |

#### permission.setDisplayName(\[displayName]) ⇒ [`Permission`](api-documentation.md#permission)

Sets the display name of this permission.

**Returns**: [`Permission`](api-documentation.md#permission) - This permission for call-chaining support.

| Param          | Type     | Description              |
| -------------- | -------- | ------------------------ |
| \[displayName] | `String` | The display name to use. |

#### new Permission(record)

Permission objects cannot be created through the API. They are created automatically when the scope is loaded. Use [getPermission](api-documentation.md#getpermission-name-permission) or [getPermissions](api-documentation.md#getpermissions-array-.less-than-permission-greater-than) to get permission objects. Creating permission objects with the new operator is reserved for internal use only.

| Param  | Type                           |
| ------ | ------------------------------ |
| record | `[ 'JSRecord' ].<permissions>` |

***

### Role

Security role which can have [user](api-documentation.md#user) members and can be granted [permissions](api-documentation.md#permission).

* [Role](api-documentation.md#role)
  * [.addPermission(permission)](api-documentation.md#role.addpermission-permission-role) ⇒ [`Role`](api-documentation.md#role)
  * [.addUser(user)](api-documentation.md#role.adduser-user-role) ⇒ [`Role`](api-documentation.md#role)
  * [.getDisplayName()](api-documentation.md#role.getdisplayname-string) ⇒ `String`
  * [.getName()](api-documentation.md#role.getname-string) ⇒ `String`
  * [.getPermissions()](api-documentation.md#role.getpermissions-array-.less-than-permission-greater-than) ⇒ [`[ 'Array' ].<Permission>`](api-documentation.md#permission)
  * [.getTenant()](api-documentation.md#role.gettenant-tenant) ⇒ [`Tenant`](api-documentation.md#tenant)
  * [.getUsers()](api-documentation.md#role.getusers-array-.less-than-user-greater-than) ⇒ [`[ 'Array' ].<User>`](api-documentation.md#user)
  * [.hasPermission(permission)](api-documentation.md#role.haspermission-permission-boolean) ⇒ `Boolean`
  * [.hasUser(user)](api-documentation.md#role.hasuser-user-boolean) ⇒ `Boolean`
  * [.removePermission(permission)](api-documentation.md#role.removepermission-permission-role) ⇒ [`Role`](api-documentation.md#role)
  * [.removeUser(user)](api-documentation.md#role.removeuser-user-role) ⇒ [`Role`](api-documentation.md#role)
  * [.setDisplayName(displayName)](api-documentation.md#role.setdisplayname-displayname-role) ⇒ [`Role`](api-documentation.md#role)
  * [new Role(record)](api-documentation.md#new-role-record)

#### role.addPermission(permission) ⇒ [`Role`](api-documentation.md#role)

Grants the specified permission to this role. Any users that are members of this role will be granted the permission.\
\
If the tenant of this role is a master tenant, the permission will also be added to the same role in all slaves of this role tenant.\
You cannot grant permission to role of a master tenant when logged in as an user. You cannot grant permission to role of a slave tenant at anytime.

**Returns**: [`Role`](api-documentation.md#role) - This role for call-chaining support.

| Param      | Type                                                        | Description                                                                                               |
| ---------- | ----------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| permission | [`Permission`](api-documentation.md#permission) \| `String` | The permission object or name of permission to add.\ Throws an exception when permission cannot be grant. |

#### role.addUser(user) ⇒ [`Role`](api-documentation.md#role)

Adds the specified user as member of this role. All permissions granted to this role will be granted to the user.

**Returns**: [`Role`](api-documentation.md#role) - This role for call-chaining support.

| Param | Type                                            | Description                                                                                           |
| ----- | ----------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| user  | [`User`](api-documentation.md#user) \| `String` | The user object or username of user to add. The user must be associated with the tenant of this role. |

#### role.getDisplayName() ⇒ `String`

Gets the display name of this role.

**Returns**: `String` - The display name of this role. Can be null.

#### role.getName() ⇒ `String`

Gets the name of this role. The role name is unique to the associated tenant.

**Returns**: `String` - The role name.

#### role.getPermissions() ⇒ [`[ 'Array' ].<Permission>`](api-documentation.md#permission)

Gets all the permissions granted to this role.

**Returns**: [`[ 'Array' ].<Permission>`](api-documentation.md#permission) - An array with all permissions granted to this role or an empty array if no permissions are granted.

#### role.getTenant() ⇒ [`Tenant`](api-documentation.md#tenant)

Gets the tenant which this role belongs to.

**Returns**: [`Tenant`](api-documentation.md#tenant) - The tenant which this role belongs to.

#### role.getUsers() ⇒ [`[ 'Array' ].<User>`](api-documentation.md#user)

Gets all the users who are members of this role.

**Returns**: [`[ 'Array' ].<User>`](api-documentation.md#user) - An array with all users who are members of this role or an empty array if the role has no members.

#### role.hasPermission(permission) ⇒ `Boolean`

Checks if the specified permission is granted to this role.

**Returns**: `Boolean` - True if the specified permission is granted to this role.

| Param      | Type                                                        | Description                                           |
| ---------- | ----------------------------------------------------------- | ----------------------------------------------------- |
| permission | [`Permission`](api-documentation.md#permission) \| `String` | The permission object or name of permission to check. |

#### role.hasUser(user) ⇒ `Boolean`

Checks if the specified user is a member of this role.

**Returns**: `Boolean` - True if the specified user is a member of this role.

| Param | Type                                            | Description                                                                                             |
| ----- | ----------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| user  | [`User`](api-documentation.md#user) \| `String` | The user object or username of user to check. The user must be associated with the tenant of this role. |

#### role.removePermission(permission) ⇒ [`Role`](api-documentation.md#role)

Removes the specified permission from this role. The permission will no longer be granted to all users that are members of this role.\
If the tenant of this role is a master tenant, the permission will also be removed from the same role in all slaves of this role tenant.\
You cannot remove permission from role of a master tenant when logged in as an user. You cannot remove permission from role of a slave tenant at anytime.

**Returns**: [`Role`](api-documentation.md#role) - This role for call-chaining support. Throws an exception when permission cannot be removed.

| Param      | Type                                                        | Description                                            |
| ---------- | ----------------------------------------------------------- | ------------------------------------------------------ |
| permission | [`Permission`](api-documentation.md#permission) \| `String` | The permission object or name of permission to remove. |

#### role.removeUser(user) ⇒ [`Role`](api-documentation.md#role)

Removes the specified user from the members of this role. All permissions granted to this role will no longer be granted to the user.

**Returns**: [`Role`](api-documentation.md#role) - This role for call-chaining support.

| Param | Type                                            | Description                                    |
| ----- | ----------------------------------------------- | ---------------------------------------------- |
| user  | [`User`](api-documentation.md#user) \| `String` | The user object or username of user to remove. |

#### role.setDisplayName(displayName) ⇒ [`Role`](api-documentation.md#role)

Sets the display name of this role.\
If the tenant of this role is a master tenant, the displayName will be set to the same role in all slaves of this role tenant.\
You cannot set the display name to role of a master tenant when logged in as an user. You cannot set the display name to role of a slave tenant at anytime.

**Returns**: [`Role`](api-documentation.md#role) - This role for call-chaining support. throws an exception if the displayName cannot be changed

| Param       | Type     | Description              |
| ----------- | -------- | ------------------------ |
| displayName | `String` | The display name to use. |

#### new Role(record)

Use [createRole](api-documentation.md#tenant.createrole-name-role) to create role objects. Creating role objects with the new operator is reserved for internal use only.

| Param  | Type                     |
| ------ | ------------------------ |
| record | `[ 'JSRecord' ].<roles>` |

***

### Session

Security application session created by a [User](api-documentation.md#user) which starts when the user [logs in](api-documentation.md#login-user-useruid-permissionstoapply-boolean) and ends when the user [logs out](api-documentation.md#logout).

* [Session](api-documentation.md#session)
  * [.getDuration()](api-documentation.md#session.getduration-number) ⇒ `Number`
  * [.getEnd()](api-documentation.md#session.getend-date) ⇒ `Date`
  * [.getID()](api-documentation.md#session.getid-string) ⇒ `String`
  * [.getIPAddress()](api-documentation.md#session.getipaddress-string) ⇒ `String`
  * [.getServoyClientID()](api-documentation.md#session.getservoyclientid-string) ⇒ `String`
  * [.getSolutionName()](api-documentation.md#session.getsolutionname-string) ⇒ `String`
  * [.getStart()](api-documentation.md#session.getstart-date) ⇒ `Date`
  * [.getTenant()](api-documentation.md#session.gettenant-tenant) ⇒ [`Tenant`](api-documentation.md#tenant)
  * [.getTenantName()](api-documentation.md#session.gettenantname-string) ⇒ `String`
  * [.getUser()](api-documentation.md#session.getuser-user) ⇒ [`User`](api-documentation.md#user)
  * [.getUserAgentString()](api-documentation.md#session.getuseragentstring-string) ⇒ `String`
  * [.getUserName()](api-documentation.md#session.getusername-string) ⇒ `String`
  * [.isAbandoned()](api-documentation.md#session.isabandoned-boolean) ⇒ `Boolean`
  * [.isActive()](api-documentation.md#session.isactive-boolean) ⇒ `Boolean`
  * [.isTerminated()](api-documentation.md#session.isterminated-boolean) ⇒ `Boolean`
  * [new Session(record)](api-documentation.md#new-session-record)

#### session.getDuration() ⇒ `Number`

Gets the session duration in milliseconds (as updated in the database)

**Returns**: `Number` - The Servoy Client ID associated with the session.

**Note**: The session duration is updated on each "client ping" which by default is once per minute

#### session.getEnd() ⇒ `Date`

Gets the end datetime of this session. Can be null if the session is still active or if the session has not been properly closed. The session end date/time is set by [logout](api-documentation.md#logout).

**Returns**: `Date` - The end date/time of this session.

#### session.getID() ⇒ `String`

Gets the internal unique ID of this session. This matches the Servoy Client ID as seen in the Servoy App Server admin page.

**Returns**: `String` - The internal unique ID of this session.

#### session.getIPAddress() ⇒ `String`

Gets the client IP address of the session.

**Returns**: `String` - The client IP address of the session.

#### session.getServoyClientID() ⇒ `String`

Gets the Servoy Client ID associated with the session (as shown on the Servoy app server admin page).

**Returns**: `String` - The Servoy Client ID associated with the session.

**Note**: Multiple user sessions can have the same Servoy Client ID if the client is not closed between different logins (for NG/Web clients this requires complete closing of the browser and not just a tab).

#### session.getSolutionName() ⇒ `String`

Gets the name of the Servoy solution that was accessed by this session

#### session.getStart() ⇒ `Date`

Gets the start date/time of this session. The session start date/time is set by [login](api-documentation.md#login-user-useruid-permissionstoapply-boolean).

**Returns**: `Date` - The start date/time of this session.

#### session.getTenant() ⇒ [`Tenant`](api-documentation.md#tenant)

Gets the tenant associated with this session. Returns null if the tenant has been deleted. In such cases use [getTenantName](api-documentation.md#session.gettenantname-string) as it will be preserved even if the tenant account is deleted.

#### session.getTenantName() ⇒ `String`

Gets the name of the tenant associated with this session. It will be available even if the associated tenant account is deleted.

**Returns**: `String` - The name of the tenant associated with this session.

#### session.getUser() ⇒ [`User`](api-documentation.md#user)

Gets the user who created this session. Returns null if the user account has been deleted. In such cases use [getUserName](api-documentation.md#session.getusername-string) as it will be preserved even if the user account is deleted.

**Returns**: [`User`](api-documentation.md#user) - The user who created this session or null if the user account has been deleted.

#### session.getUserAgentString() ⇒ `String`

Gets the client user agent string of the session. The user agent string will be null if the session was not browser-based.

**Returns**: `String` - The client user agent string of this session. Can be null.

#### session.getUserName() ⇒ `String`

The username of the user associated with this session. It will be available even if the associated user account is deleted.

**Returns**: `String` - The username of the user who created this session.

#### session.isAbandoned() ⇒ `Boolean`

Indicates if this session was abandoned and closed due to inactivity and was not closed by [logout](api-documentation.md#logout).

**Returns**: `Boolean` - True if this session was not terminated/closed normally, but has timed out due to inactivity.

#### session.isActive() ⇒ `Boolean`

Indicates if this session is still active.

**Returns**: `Boolean` - True if the session has not been terminated and has not been inactive for longer than the session inactivity timeout period.

#### session.isTerminated() ⇒ `Boolean`

Indicates if this session was terminated/closed using [logout](api-documentation.md#logout) or closed due to inactivity.

**Returns**: `Boolean` - True if the session was terminated/closed normally or by timeout from inactivity.

#### new Session(record)

Session objects cannot be created through the API. They are created automatically when a user is logged in. Use [getSession](api-documentation.md#getsession-session) to get the current session or [getActiveSessions](api-documentation.md#getactivesessions-array-.less-than-session-greater-than) to get all active sessions. Creating session objects with the new operator is reserved for internal use only.

| Param  | Type                        |
| ------ | --------------------------- |
| record | `[ 'JSRecord' ].<sessions>` |

***

### Tenant

Tenant account which is used to segregate all data. [Users](api-documentation.md#user) and [Roles](api-documentation.md#role) belong to a Tenant.

* [Tenant](api-documentation.md#tenant)
  * [.createRole(name)](api-documentation.md#tenant.createrole-name-role) ⇒ [`Role`](api-documentation.md#role)
  * [.createSlave(name)](api-documentation.md#tenant.createslave-name-tenant) ⇒ [`Tenant`](api-documentation.md#tenant)
  * [.createUser(userName, \[password\])](api-documentation.md#tenant.createuser-username-password-user) ⇒ [`User`](api-documentation.md#user)
  * [.deleteRole(role)](api-documentation.md#tenant.deleterole-role-tenant) ⇒ [`Tenant`](api-documentation.md#tenant)
  * [.deleteUser(user)](api-documentation.md#tenant.deleteuser-user-boolean) ⇒ `Boolean`
  * [.getActiveSessions()](api-documentation.md#tenant.getactivesessions-array-.less-than-session-greater-than) ⇒ [`[ 'Array' ].<Session>`](api-documentation.md#session)
  * [.getDisplayName()](api-documentation.md#tenant.getdisplayname-string) ⇒ `String`
  * [.getLockExpiration()](api-documentation.md#tenant.getlockexpiration-date) ⇒ `Date`
  * [.getLockReason()](api-documentation.md#tenant.getlockreason-string) ⇒ `String`
  * [.getName()](api-documentation.md#tenant.getname-string) ⇒ `String`
  * [.getRole(name)](api-documentation.md#tenant.getrole-name-role) ⇒ [`Role`](api-documentation.md#role)
  * [.getRoles()](api-documentation.md#tenant.getroles-array-.less-than-role-greater-than) ⇒ [`[ 'Array' ].<Role>`](api-documentation.md#role)
  * [.getSessionCount()](api-documentation.md#tenant.getsessioncount-number) ⇒ `Number`
  * [.getSlaves()](api-documentation.md#tenant.getslaves-array-.less-than-tenant-greater-than) ⇒ [`[ 'Array' ].<Tenant>`](api-documentation.md#tenant)
  * [.getUser(userName)](api-documentation.md#tenant.getuser-username-user) ⇒ [`User`](api-documentation.md#user)
  * [.getUsers()](api-documentation.md#tenant.getusers-array-.less-than-user-greater-than) ⇒ [`[ 'Array' ].<User>`](api-documentation.md#user)
  * [.isLocked()](api-documentation.md#tenant.islocked-boolean) ⇒ `Boolean`
  * [.isMasterTenant()](api-documentation.md#tenant.ismastertenant-boolean) ⇒ `Boolean`
  * [.isSlaveTenant()](api-documentation.md#tenant.isslavetenant-boolean) ⇒ `Boolean`
  * [.lock(\[reason\], \[duration\])](api-documentation.md#tenant.lock-reason-duration-tenant) ⇒ [`Tenant`](api-documentation.md#tenant)
  * [.setDisplayName(displayName)](api-documentation.md#tenant.setdisplayname-displayname-tenant) ⇒ [`Tenant`](api-documentation.md#tenant)
  * [.unlock()](api-documentation.md#tenant.unlock-tenant) ⇒ [`Tenant`](api-documentation.md#tenant)
  * [new Tenant(record)](api-documentation.md#new-tenant-record)

#### tenant.createRole(name) ⇒ [`Role`](api-documentation.md#role)

Creates a role associated with this tenant using the specified role name.\
If this is a Master Tenant the created role will be added to all slaves of this Tenant.\
Cannot create role for a master tenant when logged in as an user.

**Returns**: [`Role`](api-documentation.md#role) - The role which was created. If the role name is not unique to this tenant.

| Param | Type     | Description                                                        |
| ----- | -------- | ------------------------------------------------------------------ |
| name  | `String` | The name of the role to be created. Must be unique to this tenant. |

#### tenant.createSlave(name) ⇒ [`Tenant`](api-documentation.md#tenant)

Creates a slave of this tenant with the given name. Modifications to roles and permissions of this tenant will be propagated to all of its slaves.

\
WARNING: Cannot call this function when logged in as an user.

**Returns**: [`Tenant`](api-documentation.md#tenant) - slave The slave that has been created

| Param | Type     | Description                                                                                                                                        |
| ----- | -------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| name  | `String` | The name of the tenant. Must be unique and no longer than 50 characters. Throws an exception if this function is called when logged in as an user. |

#### tenant.createUser(userName, \[password]) ⇒ [`User`](api-documentation.md#user)

Creates a user with the specified user name.

**Returns**: [`User`](api-documentation.md#user) - The user which was created. If the user name is not specified or is not unique.

**Note**: If password is not specified the user account will be created with a blank password. Use [setPassword](api-documentation.md#user.setpassword-password-user) to set or change the user password.

| Param       | Type     | Description                           |
| ----------- | -------- | ------------------------------------- |
| userName    | `String` | Must be unique in system.             |
| \[password] | `String` | The password to use for the new user. |

#### tenant.deleteRole(role) ⇒ [`Tenant`](api-documentation.md#tenant)

Deletes the specified role from this tenant. All associated permissions and grants to users are removed immediately. Users with active sessions will be affected, but design-time security (CRUD, UI) will not be affected until next log-in.

\
If this is a Master Tenant the deleted role will be deleted also for all slaves of this Tenant.\
Cannot delete role of a master tenant when logged in as an user.

**Returns**: [`Tenant`](api-documentation.md#tenant) - This tenant for call-chaining support.

| Param | Type                                            | Description                                                                                                                                     |
| ----- | ----------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| role  | [`Role`](api-documentation.md#role) \| `String` | The role object or name of role to be deleted. The role must be associated with this tenant. throws an exception if the role cannot be deleted. |

#### tenant.deleteUser(user) ⇒ `Boolean`

Immediately and permanently deletes the specified user and all security-related records associated with it. The user will not be deleted if it has active sessions.

**Returns**: `Boolean` - True if the user is deleted, otherwise false.

**Note**: USE WITH CAUTION! There is no undo for this operation.

| Param | Type                                            | Description                                                                                                        |
| ----- | ----------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| user  | [`User`](api-documentation.md#user) \| `String` | The user object or the username of the user to be deleted. The specified user must be associated with this tenant. |

#### tenant.getActiveSessions() ⇒ [`[ 'Array' ].<Session>`](api-documentation.md#session)

Gets the active sessions for users associated with this tenant. This includes any sessions from any device and any location for users associated with this tenant.

**Returns**: [`[ 'Array' ].<Session>`](api-documentation.md#session) - An array with all active sessions for users associated with this tenant or an empty array if the are no active sessions.

**Note**: Any unterminated sessions are deemed to be active when they have not been idle for more than a set timeout period.

#### tenant.getDisplayName() ⇒ `String`

Gets the display name of this tenant. The display name can be set using [setDisplayName](api-documentation.md#tenant.setdisplayname-displayname-tenant).

**Returns**: `String` - The display name of this tenant. Can be null if a display name is not set.

#### tenant.getLockExpiration() ⇒ `Date`

Gets the expiration date/time of the lock created by [lock](api-documentation.md#tenant.lock-reason-duration-tenant). The lock will remain in place until it expires or it is removed using [unlock](api-documentation.md#tenant.unlock-tenant).

**Returns**: `Date` - The date/time when the lock expires. Can be null. The date/time is using the Servoy application server timezone.

#### tenant.getLockReason() ⇒ `String`

Gets the reason for the account lock created by [lock](api-documentation.md#tenant.lock-reason-duration-tenant).

**Returns**: `String` - The lock reason. Can be null.

#### tenant.getName() ⇒ `String`

Gets the name of this tenant. Tenant names are unique in the system and are specified when the tenant is created.

**Returns**: `String` - The name of this tenant.

#### tenant.getRole(name) ⇒ [`Role`](api-documentation.md#role)

Gets a role by name unique to this tenant.

**Returns**: [`Role`](api-documentation.md#role) - The matching role, or null if a role with the specified name and associated with this tenant is not found.

| Param | Type     | Description                  |
| ----- | -------- | ---------------------------- |
| name  | `String` | The name of the role to get. |

#### tenant.getRoles() ⇒ [`[ 'Array' ].<Role>`](api-documentation.md#role)

Gets the roles associated with this tenant.

**Returns**: [`[ 'Array' ].<Role>`](api-documentation.md#role) - An array with the roles associated with this tenant or an empty array if the tenant has no roles.

#### tenant.getSessionCount() ⇒ `Number`

Gets the number of all unique sessions which have ever been initialized in the system by users associated with this tenant. This includes both active sessions (for users currently logged in the application) and inactive sessions (sessions from the past which have already been terminated).

**Returns**: `Number` - The number of all sessions (active and inactive) for users associated with this tenant.

#### tenant.getSlaves() ⇒ [`[ 'Array' ].<Tenant>`](api-documentation.md#tenant)

Gets all slaves of this tenant When recursive is true, all slaves of this tenant's slaves are included\
WARNING: Cannot call this function when logged in as an user.

Throws an exception if this function is called when logged in as an user.

**Returns**: [`[ 'Array' ].<Tenant>`](api-documentation.md#tenant) - slaves Array of tenants that have this tenant as their master

#### tenant.getUser(userName) ⇒ [`User`](api-documentation.md#user)

Gets the user (associated with this tenant) specified by the username.

**Returns**: [`User`](api-documentation.md#user) - The matching user or null if a user with the specified username and associated with this tenant is not found.

| Param    | Type     | Description               |
| -------- | -------- | ------------------------- |
| userName | `String` | The username of the user. |

#### tenant.getUsers() ⇒ [`[ 'Array' ].<User>`](api-documentation.md#user)

Gets all users for this tenant.

**Returns**: [`[ 'Array' ].<User>`](api-documentation.md#user) - An array with all users associated with this tenant or an empty array if the tenant has no users.

#### tenant.isLocked() ⇒ `Boolean`

Indicates if the tenant account is locked using [lock](api-documentation.md#tenant.lock-reason-duration-tenant).

**Returns**: `Boolean` - True if the tenant account is currently locked and the lock has not expired.

#### tenant.isMasterTenant() ⇒ `Boolean`

Returns true if this Tenant is a master (template) tenant\
WARNING: When the user is already logged, can call this function only for the tenant of the logged user; cannot call this function for other tenants when logged in as an user.

**Returns**: `Boolean` - isMasterTenant Whether this tenant is a master to other tenants

Throws an exception when logged in as an user and called for another tenant than the tenant of the logged user.

#### tenant.isSlaveTenant() ⇒ `Boolean`

Returns true if this Tenant is a slave tenant

**Returns**: `Boolean` - isMasterTenant Whether this tenant is a master to other tenants

#### tenant.lock(\[reason], \[duration]) ⇒ [`Tenant`](api-documentation.md#tenant)

Locks the tenant account preventing its users from logging in. The lock will remain in place until it expires (if a duration was specified) or it is removed using {Tenant#unlock}. Users with active sessions will be unaffected until subsequent login attempts. Can be called even if the tenant is already locked. In such cases the lock reason and duration will be reset.

**Returns**: [`Tenant`](api-documentation.md#tenant) - This tenant for call-chaining support.

| Param       | Type     | Description                                                                                                                 |
| ----------- | -------- | --------------------------------------------------------------------------------------------------------------------------- |
| \[reason]   | `String` | The reason for the lock.                                                                                                    |
| \[duration] | `Number` | The duration of the lock (in milliseconds). If no duration specified, the lock will remain until {Tenant#unlock} is called. |

#### tenant.setDisplayName(displayName) ⇒ [`Tenant`](api-documentation.md#tenant)

Sets the display name of this tenant.

**Returns**: [`Tenant`](api-documentation.md#tenant) - This tenant for call-chaining support.

| Param       | Type     | Description              |
| ----------- | -------- | ------------------------ |
| displayName | `String` | The display name to use. |

#### tenant.unlock() ⇒ [`Tenant`](api-documentation.md#tenant)

Removes the lock on the tenant account which is created by [lock](api-documentation.md#tenant.lock-reason-duration-tenant). Can be safely called even if the tenant is not locked.

**Returns**: [`Tenant`](api-documentation.md#tenant) - This tenant for call-chaining support.

#### new Tenant(record)

Use [createTenant](api-documentation.md#createtenant-name-tenant) to create tenant objects. Creating tenant objects with the new operator is reserved for internal use only.

| Param  | Type                       | Description                                                         |
| ------ | -------------------------- | ------------------------------------------------------------------- |
| record | `[ 'JSRecord' ].<tenants>` | The database record where the tenant account information is stored. |

***

### User

Application user account associated with a [Tenant](api-documentation.md#tenant). Security [Permissions](api-documentation.md#permission) are granted to users through their [Role](api-documentation.md#role) membership.

* [User](api-documentation.md#user)
  * [.addRole(role)](api-documentation.md#user.addrole-role-user) ⇒ [`User`](api-documentation.md#user)
  * [.checkPassword(password)](api-documentation.md#user.checkpassword-password-boolean) ⇒ `Boolean`
  * [.generateAccessToken(\[duration\])](api-documentation.md#user.generateaccesstoken-duration-string) ⇒ `String`
  * [.getActiveSessions()](api-documentation.md#user.getactivesessions-array-.less-than-session-greater-than) ⇒ [`[ 'Array' ].<Session>`](api-documentation.md#session)
  * [.getDisplayName()](api-documentation.md#user.getdisplayname-string) ⇒ `String`
  * [.getEmail()](api-documentation.md#user.getemail-string) ⇒ `String`
  * [.getLockExpiration()](api-documentation.md#user.getlockexpiration-date) ⇒ `Date`
  * [.getLockReason()](api-documentation.md#user.getlockreason-string) ⇒ `String`
  * [.getPermissions()](api-documentation.md#user.getpermissions-array-.less-than-permission-greater-than) ⇒ [`[ 'Array' ].<Permission>`](api-documentation.md#permission)
  * [.getRoles()](api-documentation.md#user.getroles-array-.less-than-role-greater-than) ⇒ [`[ 'Array' ].<Role>`](api-documentation.md#role)
  * [.getSessionCount()](api-documentation.md#user.getsessioncount-number) ⇒ `Number`
  * [.getTenant()](api-documentation.md#user.gettenant-tenant) ⇒ [`Tenant`](api-documentation.md#tenant)
  * [.getUserName()](api-documentation.md#user.getusername-string) ⇒ `String`
  * [.hasPermission(permission)](api-documentation.md#user.haspermission-permission-boolean) ⇒ `Boolean`
  * [.hasRole(role)](api-documentation.md#user.hasrole-role-boolean) ⇒ `Boolean`
  * [.isLocked()](api-documentation.md#user.islocked-boolean) ⇒ `Boolean`
  * [.lock(\[reason\], \[duration\])](api-documentation.md#user.lock-reason-duration-user) ⇒ [`User`](api-documentation.md#user)
  * [.removeRole(role)](api-documentation.md#user.removerole-role-user) ⇒ [`User`](api-documentation.md#user)
  * [.setDisplayName(displayName)](api-documentation.md#user.setdisplayname-displayname-user) ⇒ [`User`](api-documentation.md#user)
  * [.setEmail(email)](api-documentation.md#user.setemail-email-user) ⇒ [`User`](api-documentation.md#user)
  * [.setPassword(password)](api-documentation.md#user.setpassword-password-user) ⇒ [`User`](api-documentation.md#user)
  * [.unlock()](api-documentation.md#user.unlock-user) ⇒ [`User`](api-documentation.md#user)
  * [new User(record)](api-documentation.md#new-user-record)

#### user.addRole(role) ⇒ [`User`](api-documentation.md#user)

Adds this user as member of the specified role and grants the user all permissions which the role has.

**Returns**: [`User`](api-documentation.md#user) - This user for call-chaining support.

| Param | Type                                            | Description                                                                                    |
| ----- | ----------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| role  | [`Role`](api-documentation.md#role) \| `String` | The role object or role name to use. The role must be associated with the tenant of this user. |

#### user.checkPassword(password) ⇒ `Boolean`

Checks if the specified password matches the password of this user. User password can be set when the user is created or by using [setPassword](api-documentation.md#user.setpassword-password-user).

**Returns**: `Boolean` - True if the specified password matches the password of this user.

| Param    | Type     | Description                         |
| -------- | -------- | ----------------------------------- |
| password | `String` | The password (plain-text) to check. |

#### user.generateAccessToken(\[duration]) ⇒ `String`

Generates a secure access token to authenticate this user within a window of validity of the specified duration. The generated access token can be used with [consumeAccessToken](api-documentation.md#consumeaccesstoken-token-user).

**Returns**: `String` - The generated access token.

| Param       | Type     | Description                                                                      |
| ----------- | -------- | -------------------------------------------------------------------------------- |
| \[duration] | `Number` | The duration of token validity in milliseconds. Default is 30 minutes in future. |

#### user.getActiveSessions() ⇒ [`[ 'Array' ].<Session>`](api-documentation.md#session)

Gets the active sessions this user. This includes any sessions from any device and any location for this user.

**Returns**: [`[ 'Array' ].<Session>`](api-documentation.md#session) - An array with all active sessions for this user or an empty array if the are no active sessions.

**Note**: Any unterminated sessions are deemed to be active when they have not been idle for more than a set timeout period.

#### user.getDisplayName() ⇒ `String`

Gets the display name of this user, i.e. "Jane Doe". The display name can be set using [setDisplayName](api-documentation.md#user.setdisplayname-displayname-user).

**Returns**: `String` - The display name of this user.

#### user.getEmail() ⇒ `String`

**Returns**: `String` - The email of this user.

#### user.getLockExpiration() ⇒ `Date`

Gets the expiration date/time of the lock created by [lock](api-documentation.md#user.lock-reason-duration-user). The lock will remain in place until it expires or it is removed using [unlock](api-documentation.md#user.unlock-user).

**Returns**: `Date` - The date/time when the lock expires. Can be null. The date/time is using the Servoy application server timezone.

#### user.getLockReason() ⇒ `String`

Gets the reason for the account lock created by [lock](api-documentation.md#user.lock-reason-duration-user).

**Returns**: `String` - The lock reason. Can be null.

#### user.getPermissions() ⇒ [`[ 'Array' ].<Permission>`](api-documentation.md#permission)

Gets all the permissions granted to this user via its roles membership. Result will exclude duplicates. Permissions cannot be granted directly to the user. Use [addRole](api-documentation.md#user.addrole-role-user) or [addUser](api-documentation.md#role.adduser-user-role) to make the user a member of specific roles and all role permissions will be granted to the user.

**Returns**: [`[ 'Array' ].<Permission>`](api-documentation.md#permission) - An array with the permissions granted to this user or an empty array if the user has no permissions.

#### user.getRoles() ⇒ [`[ 'Array' ].<Role>`](api-documentation.md#role)

Gets all the roles that this user is member of.

**Returns**: [`[ 'Array' ].<Role>`](api-documentation.md#role) - An array with all roles which this user is member of or an empty array if the user is not a member of any role.

#### user.getSessionCount() ⇒ `Number`

Gets the number of all unique sessions which have ever been initialized in the system by this user. This includes both active sessions (for users currently logged in the application) and inactive sessions (sessions from the past which have already been terminated).

**Returns**: `Number` - The number of all sessions (active and inactive) for this user.

#### user.getTenant() ⇒ [`Tenant`](api-documentation.md#tenant)

Returns the tenant that owns this user account.

**Returns**: [`Tenant`](api-documentation.md#tenant) - The parent tenant associated with this user.

#### user.getUserName() ⇒ `String`

Gets the username of this user which was specified when the user was created. The username cannot be changed after the user is created and is unique to the associated tenant.

**Returns**: `String` - The username of this user.

#### user.hasPermission(permission) ⇒ `Boolean`

Checks if the this user is granted the specified permission via the user's role membership. Permissions cannot be granted directly to the user. Use [addRole](api-documentation.md#user.addrole-role-user) or [addUser](api-documentation.md#role.adduser-user-role) to make the user a member of specific roles and all role permissions will be granted to the user.

**Returns**: `Boolean` - True if the user has been granted the specified permission.

| Param      | Type                                                        | Description                                        |
| ---------- | ----------------------------------------------------------- | -------------------------------------------------- |
| permission | [`Permission`](api-documentation.md#permission) \| `String` | The permission object or permission name to check. |

#### user.hasRole(role) ⇒ `Boolean`

Checks if this user is a member of the specified role.

**Returns**: `Boolean` - True if the user is a member of the specified role.

| Param | Type                                            | Description                                                                                      |
| ----- | ----------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| role  | [`Role`](api-documentation.md#role) \| `String` | The role object or role name to check. The role must be associated with the tenant of this user. |

#### user.isLocked() ⇒ `Boolean`

Indicates if the use account is locked using [lock](api-documentation.md#user.lock-reason-duration-user).

**Returns**: `Boolean` - True if the user account is currently locked and the lock has not expired.

#### user.lock(\[reason], \[duration]) ⇒ [`User`](api-documentation.md#user)

Locks the user account preventing it from logging in. The lock will remain in place until it expires (if a duration was specified) or it is removed using {User#unlock}. Users with active sessions will be unaffected until subsequent login attempts. Can be called even if the user account is already locked. In such cases the lock reason and duration will be reset.

**Returns**: [`User`](api-documentation.md#user) - This user for call-chaining support.

| Param       | Type     | Description                                                                                                               |
| ----------- | -------- | ------------------------------------------------------------------------------------------------------------------------- |
| \[reason]   | `String` | The reason for the lock.                                                                                                  |
| \[duration] | `Number` | The duration of the lock (in milliseconds). If no duration specified, the lock will remain until {User#unlock} is called. |

#### user.removeRole(role) ⇒ [`User`](api-documentation.md#user)

Removes the membership of this user from the specified role. All permissions of the role will no longer be granted to the user.

**Returns**: [`User`](api-documentation.md#user) - This user for call-chaining support.

| Param | Type                                            | Description                                                                                    |
| ----- | ----------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| role  | [`Role`](api-documentation.md#role) \| `String` | The role object or role name to use. The role must be associated with the tenant of this user. |

#### user.setDisplayName(displayName) ⇒ [`User`](api-documentation.md#user)

Sets the display name of this user.

**Returns**: [`User`](api-documentation.md#user) - This user for call-chaining support.

| Param       | Type     | Description              |
| ----------- | -------- | ------------------------ |
| displayName | `String` | The display name to use. |

#### user.setEmail(email) ⇒ [`User`](api-documentation.md#user)

**Returns**: [`User`](api-documentation.md#user) - This user for call-chaining support.

| Param | Type     |
| ----- | -------- |
| email | `String` |

#### user.setPassword(password) ⇒ [`User`](api-documentation.md#user)

Sets the users password. The specified plain-text password will not be stored. Only its hash will be stored and used for password validation. The actual plain-text password cannot be retrieved from the stored hash.

**Returns**: [`User`](api-documentation.md#user) - This user for call-chaining support.

| Param    | Type     | Description                     |
| -------- | -------- | ------------------------------- |
| password | `String` | The plain-text password to use. |

#### user.unlock() ⇒ [`User`](api-documentation.md#user)

Removes the lock on the user account which is created by [lock](api-documentation.md#user.lock-reason-duration-user). Can be safely called even if the user account is not locked.

**Returns**: [`User`](api-documentation.md#user) - This user for call-chaining support.

#### new User(record)

| Param  | Type                     |
| ------ | ------------------------ |
| record | `[ 'JSRecord' ].<users>` |

***

### changeExternalDBTransactionSupportFlag(mustSupportExternalTransactions)

Use this method to change the behavior of the svySecurity module with respect to DB transactions.

If the flag is set to false (default) then when saving or deleting security-related records if an external DB transaction is detected the operation will fail. If the flag is set to true then when saving or deleting security-related records the module will start/commit a DB transaction only if an external DB transaction is not detected. On exceptions any DB transaction will be rolled back regardless if it is started internally or externally (exceptions will be propagated to the external transaction so callers will be able to react on them accordingly)

**Note**: If using external DB transactions then callers are responsible for refreshing the state of security-related objects upon transaction rollbacks which occur after successful calls to the svySecurity API.

| Param                           | Type      | Description                                                 |
| ------------------------------- | --------- | ----------------------------------------------------------- |
| mustSupportExternalTransactions | `Boolean` | The value for the supportExternalDBTransaction flag to set. |

***

### cloneTenant(tenantToClone, name, \[makeSlave]) ⇒ [`Tenant`](api-documentation.md#tenant)

Creates and returns a new tenant with the specified name as a clone of the given tenant. The names of tenants must be unique in the system. The cloned tenant has the same roles and role permissions as the original. When makeSlave is true, the newly created clone will be a slave of the tenant to clone, inheriting all role / permission changes made to the master.\
WARNING: Cannot call this function when logged in as an user.

**Returns**: [`Tenant`](api-documentation.md#Tenant) - The cloned tenant that is created. Throws an exception if this function is called when logged in as an user.

| Param         | Type                                    | Description                                                                              |
| ------------- | --------------------------------------- | ---------------------------------------------------------------------------------------- |
| tenantToClone | [`Tenant`](api-documentation.md#tenant) | The tenant to clone from                                                                 |
| name          | `String`                                | The name of the tenant. Must be unique and no longer than 50 characters.                 |
| \[makeSlave]  | `Boolean`                               | When true, the cloned tenant will be a slave of the tenant to clone (defaults to false). |

***

### consumeAccessToken(token) ⇒ [`User`](api-documentation.md#user)

Consumes a secure-access token and returns the user associated with the token if a valid match was found. Tokens may be used only once to identify a user. Subsequent calls to consume the same token will fail. Secure-access tokens are created with [generateAccessToken](api-documentation.md#user.generateaccesstoken-duration-string)

**Returns**: [`User`](api-documentation.md#user) - The user associated with the specified token or null if the token is not valid or has expired.

**Note**: An error will be thrown if this method is called from within an active user session.

| Param | Type     | Description                     |
| ----- | -------- | ------------------------------- |
| token | `String` | The secure-access token to use. |

***

### createTenant(name) ⇒ [`Tenant`](api-documentation.md#tenant)

Creates and returns a new tenant with the specified name. The names of tenants must be unique in the system.

**Returns**: [`Tenant`](api-documentation.md#tenant) - The tenant that is created.

| Param | Type     | Description                                                              |
| ----- | -------- | ------------------------------------------------------------------------ |
| name  | `String` | The name of the tenant. Must be unique and no longer than 50 characters. |

***

### deleteTenant(tenant) ⇒ `Boolean`

Immediately and permanently deletes the specified tenant and all records associated with it, including all users and roles. Tenant will not be deleted if it has users with active sessions.\
If the deleted tenant is a Master tenant and is a slave of another master tenant, this operation will replace the master tenant of it's direct slaves with the master of the tenant that is deleted; If the delated tenant is a Master tenant and has no Master tenant, this operation will remove the master from all it's direct slaves.

**Returns**: `Boolean` - False if tenant could not be deleted, most commonly because of active user sessions associated with the tenant.

**Note**: USE WITH CAUTION! There is no undo for this operation.

| Param  | Type                                                | Description                                            |
| ------ | --------------------------------------------------- | ------------------------------------------------------ |
| tenant | [`Tenant`](api-documentation.md#tenant) \| `String` | The tenant object or the name of the tenant to delete. |

***

### getActiveSessions() ⇒ [`[ 'Array' ].<Session>`](api-documentation.md#session)

Gets all active sessions for the application.

**Returns**: [`[ 'Array' ].<Session>`](api-documentation.md#session) - An array will all active sessions or an empty array if there are no active sessions.

**Note**: If users close the application without [logging out](api-documentation.md#logout) then their sessions will remain active for a period of time.

***

### getPermission(name) ⇒ [`Permission`](api-documentation.md#permission)

Gets a permission by its unique permission name.

**Returns**: [`Permission`](api-documentation.md#permission) - The specified permission or null if a permission with the specified name is not found.

| Param | Type     | Description                 |
| ----- | -------- | --------------------------- |
| name  | `String` | The name of the permission. |

***

### getPermissions() ⇒ [`[ 'Array' ].<Permission>`](api-documentation.md#permission)

Gets all permissions available in this application.

**Returns**: [`[ 'Array' ].<Permission>`](api-documentation.md#permission) - An array with all permissions or an empty array if no permissions are defined.

***

### getRole(roleName, \[tenantName]) ⇒ [`Role`](api-documentation.md#role)

Gets a role by the specified role name and tenant name. If tenant name is not specified will use the tenant of the user currently logged in the application, if available.

**Returns**: [`Role`](api-documentation.md#role) - The specified role or null if not found.

**Note**: Will fail if tenant is not specified and user is not logged in and multiple roles are found with the specified role name but associated with different tenants.

| Param         | Type     | Description                                                                                            |
| ------------- | -------- | ------------------------------------------------------------------------------------------------------ |
| roleName      | `String` | The name of the role to get.                                                                           |
| \[tenantName] | `String` | If not specified will use the tenant of the current logged in user (if user is not currently logged in |

***

### getSession() ⇒ [`Session`](api-documentation.md#session)

Gets the current user session or null if no session initialized (no user is currently [logged in](api-documentation.md#login-user-useruid-permissionstoapply-boolean)).

**Returns**: [`Session`](api-documentation.md#session) - The current session or null if a user is not currently logged in.

**Note**: Sessions represent authenticated user sessions. They are not initialized until after user login.

***

### getSessionCount() ⇒ `Number`

Gets the number of all unique sessions which have ever been initialized in the application. This includes both active sessions (for users currently logged in the application) and inactive sessions (sessions from the past which have already been closed).

**Returns**: `Number` - The number of all sessions (active and closed).

***

### getTenant(\[name]) ⇒ [`Tenant`](api-documentation.md#tenant)

Gets a tenant by its unique tenant name. If tenant name is not specified then will return the tenant of the currently logged in user. If tenant name is not specified and no user is currently logged in then will return null.

**Returns**: [`Tenant`](api-documentation.md#tenant) - The tenant or null if not found / no user is logged in.

| Param   | Type     | Description                                                       |
| ------- | -------- | ----------------------------------------------------------------- |
| \[name] | `String` | The name of the tenant to get. Or null to get the current tenant. |

**Example**

```js
//get the tenant of the current user
var currentUserTenant = scopes.svySecurity.getTenant();
//get a specific tenant
var tenant = scopes.svySecurity.getTenant('tenantNameToGet');
```

***

### getTenants() ⇒ [`[ 'Array' ].<Tenant>`](api-documentation.md#tenant)

Gets all tenants in the system.

**Returns**: [`[ 'Array' ].<Tenant>`](api-documentation.md#tenant) - An array with all tenants or an empty array if no tenants are defined.

***

### getUser(\[userName], \[tenantName]) ⇒ [`User`](api-documentation.md#user)

Gets a user by the specified username and tenant name. If username is not specified will return the user currently logged in the application, if available.

**Returns**: [`User`](api-documentation.md#user) - The specified user (or current user if parameters are not specified) or null if the specified user does not exist (or if parameters are not specified and a user is not logged in currently).

**Note**: Will fail if tenant is not specified and user is not logged in and multiple users are found with the specified username but associated with different tenants.

| Param         | Type     | Description                                                                                                          |
| ------------- | -------- | -------------------------------------------------------------------------------------------------------------------- |
| \[userName]   | `String` | The username of the user to return. Can be null to get the current user.                                             |
| \[tenantName] | `String` | The name of the tenant associated with the user. Can be null if username is also null when getting the current user. |

***

### getUsers() ⇒ [`[ 'Array' ].<User>`](api-documentation.md#user)

Gets all users in the system.

**Returns**: [`[ 'Array' ].<User>`](api-documentation.md#user) - An array with all users or an empty array if no users are defined.

***

### getVersion() ⇒ `String`

Gets the version of this module

**Returns**: `String` - the version of the module using the format Major.Minor.Revision

***

### login(user, \[userUid], \[permissionsToApply]) ⇒ `Boolean`

Logs in the specified user and initializes a new [Session](api-documentation.md#session) for it. The login request will not be successful if the user account or the parent [tenant](api-documentation.md#user.gettenant-tenant) account [is locked](api-documentation.md#user.islocked-boolean) and the lock has not [expired](api-documentation.md#user.getlockexpiration-date) yet. The login request will not be successful also if no [permissions](api-documentation.md#user.getpermissions-array-.less-than-permission-greater-than) have been granted to the specified user. This method internally calls the standard Servoy security.login().

**Returns**: `Boolean` - Returns true if the login was successful and a user [Session](api-documentation.md#session) was created, otherwise false.

**Note**: This method does not perform any password checks - for validation of user passwords use [User.checkPassword](api-documentation.md#user.checkpassword-password-boolean).

| Param                 | Type                                 | Description                                                                                                                                      |
| --------------------- | ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| user                  | [`User`](api-documentation.md#user)  | The user to log in.                                                                                                                              |
| \[userUid]            | `String` \| `UUID`                   | The uid to log the user in with (defaults to userName)                                                                                           |
| \[permissionsToApply] | `[ 'Array' ].<(String\|Permission)>` | Optional permissions to assign to the user. Note that these permissions cannot be asked for using User.getPermissions() or User.hasPermission(). |

***

### logout()

Logs the current user out of the application and closes the associated [Session](api-documentation.md#session). This method internally calls security.logout() to end the Servoy client session.

***

### syncPermissions(\[forcePermissionRemoval])

Utility to sync permission records to the internal, design-time Servoy Security Groups. This should be called on solution import or on startup This action will create new permission records.

NOTE: This action will not delete permissions which have been removed from internal security. Design-time groups should never be renamed. They will be seen only as an ADD and will lose their tie to roles.

| Param                     | Type      | Description                                                                                                                                                                                                                                                                            |
| ------------------------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| \[forcePermissionRemoval] | `Boolean` | if true then permissions without a matching Servoy security group will be deleted regardless if they have been granted to any role or not; if false (default) then permissions without a matching Servoy security group will be deleted only if they have not been granted to any role |

***
