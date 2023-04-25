#  OfflineDataDescription

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [addFoundSet(fs)](OfflineDataDescription.md#addfoundset-fs)                   | Exposes an unrelated foundset to the mobile client..                                    |
|void | [addFoundSet(fs, relationNamesToTraverse)](OfflineDataDescription.md#addfoundset-fs-relationnamestotraverse)                   | Exposes an unrelated foundset to the mobile client..                                    |

## Methods Details

### addFoundSet(fs)

Exposes an unrelated foundset to the mobile client. If service solution has a module of type Mobile shared module all possible relations from that module are traversed automatically.

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) fs the foundset

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var retval = plugins.mobileservice.createOfflineDataDescription('data_');
var ff = databaseManager.getFoundSet('bug_db','mytable');
ff.loadAllRecords();
retval.addFoundSet(ff);
```
### addFoundSet(fs, relationNamesToTraverse)

Exposes an unrelated foundset to the mobile client.
which can be used in the mobile client in an unrelated way like in a (first) form or databaseManager.getFoundset(...).
For each record in the provided (unrelated) foundset the specified relation names are traversed and all data taken. Providing the relation names to traverse overrides the automatic traversal of the relations found in the "Mobile Shared Module".

**Parameters**\
[JSFoundSet](../../Database%20Manager/JSFoundSet.md) fs the root foundset\
[Array](../../JSLib/Array.md) relationNamesToTraverse the relations to traverse from records found in root root foundset

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var data = plugins.mobileservice.createOfflineDataDescription('data_');
var fs_contact = globals.accountmanager_contacts; //contains the account manager contact
var traverse = new Array();
traverse.push('accountmanager_to_companies');
data.addFoundSet(fs_contact, traverse);
```

