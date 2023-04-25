**Available since v1.3.0**

Each tenant has it's own set of roles with associated permissions; different tenants can therefore have different set of roles granting different permissions. However is a common requirement for all tenants, or for a group of tenants, to share the same set of roles and associated permissions. In such scenario a Master tenant can be linked to multiple sub-tenants; any change to the Master tenant's roles and associated permissions will be propagated to all it's sub-tenants; the master and all it's sub-tenants will therefore share the same set of roles and associated permissions. 

Note that a sub-tenant should never modify independently it's roles and associated permissions, all changes should be done in the master tenant only.

**READ CAREFULLY** if you are using a master-sub-tentant setup you should never change roles and their assigned permission of a master tenant while the user is logged in. That's because any change will be applied only to the tenant of the logged user and will not be propagated to the sub-tenants.

## How does it work ?

Any time you create a new tenant _mySubTenant_ you can decide to create it as a sub-tenant of tenant _myMaster_ using the svySecurity APIs.

```
// create the tenant myClone as clone of existing tenant master
var master = scopes.svySecurity.getTenant("master");
master.createSubTenant("mySubTenant");
```

The sub-tenant created will have same roles, having same assigned permissions, of the master tenant.
Being a sub-tenant means that any change in the roles of the master tenant, like creating a new role or assigning permissions to an existing role or removing a role, will be propagated and applied to the sub-tenant.