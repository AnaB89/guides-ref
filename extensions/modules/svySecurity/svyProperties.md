This wiki provides comprehensive documentation to using the svyProperties module. 

The module is designed to provide a persistent storage for properties (key-value), multi-tenant and multi-user capable, required by all modern business applications in an easy to learn and use format.

Please note the **svyProperties** module is independent from the svySecurity module; it can be used either with or without the **svySecurity** module.

Even if the svyProperties module is used without the svySecurity module, it still requires the **svy_security** database.


# Getting Started

The module is available since Servoy 2019.12; it can be imported into your workspace via the Servoy's Web Package Manager.


### Requirements
* Servoy 2019.12 or later version
* To be successfully imported this module requires an existing or empty database **svy_security**

### Quick start

The svyProperties API can be used to store Global properties, Tenant's properties or User's properties. Each property value is stored as String and identified by the unique tuple: **(key, type, user, tenant)**; you are therefore allowed to persist the same property, identified by the tuple (key, type), at different levels: User's, Tenant's, Global's.
A common use case for such structure: you can define the Theme colors of your solution as Global properties, which can be overridden by Tenant's preferences and possibly be overridden again by User's preferences.

API Structure:

* get/setProperty(propertyKey, propertyType, value, userName, tenantName)
* get/setGlobalProperty(propertyKey, propertyType, value)
* get/setTenantProperty(propertyKey, propertyType, value)
* get/setUserProperty(propertyKey, propertyType, value)

### How svyProperties knows about my user/tenant name ?

If you are using svyProperties in conjunction with svySecurity (v1.3.0 or higher) there is nothing you have to do. Everything is already taken care by the svySecurity module.

If you are not using svySecurity (v.1.3.0 or higher) instead you must tell the svyProperties module which are the user and tenant (if any) the user has logged with.
Use the svyProperties API _setUserName_ to let svyProperties know which is the unique user name (or ID) and tenant name (or ID) during the initialization of your application.

```
function onSolutionOpen(arg, queryParams) {
   // don't set the tenant if the solution doesn't support multi-tenancy
   // scopes.svyProperties.setUserName(loggedUserName);
 
   scopes.svyProperties.setUserName(loggedUniqueUserName, loggedUniqueTenantName);
}
```

### How can i use the svyProperties ?

A common use case is to persist the state of the Grid as User's property; when the user will come back to the same Grid he will the state persisted from it's last visit.

```
 //persist the state of the NG Grid as user property  
 function onColumnStateChanged(columnState) {
	 var propertyNameSpace = application.getSolutionName() + "-" + controller.getName() + "." + elements.table.getName();	
	 scopes.svyProperties.setUserProperty(propertyNameSpace, 'table-state', columnState);
}

 function onShow(firstShow, event) {
 	var propertyKey = application.getSolutionName() + "-" + controller.getName() + "-" + elements.table.getName();
	var columnState = scopes.svyProperties.getUserProperty(propertyKey, 'table-state');
	
	// restore the ng-grid state 
	if (columnState) elements.table.restoreColumnState(columnState.getPropertyValue());
  }
```

### How are properties stored ?

The properties are stored into the table _svy_properties _which is part of the database _svy_security_. If you wish to deploy the properties from your Developer environment to the deployed Acceptance and Production environment you can consider to seed the database using Servoy post-import modules.

### How can i tune svyProperties perfomances ?

Since properties are stored into a DB table, you can tune the performances by tuning the DB indexes of the svy_properties table in the svy_security Database. How to tune table index depends from your DB vendor and from the use you do of the svyProperties module.

### How can i use the Property Type ?

The use of the property Key & Type is at your discretion; depending on the usage you do of the Properties in your solution the table used to store the properties may grow with many records stored in it; in such scenario you would like take advantage of the Property Type to easily group them into categories and be able to index the queries by type.
