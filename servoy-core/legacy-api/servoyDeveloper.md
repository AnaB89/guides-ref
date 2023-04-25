#  servoyDeveloper

## **Supported Clients**

    SmartClient
    WebClient
    NGClient
    MobileClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [openForm(form)](servoyDeveloper.md#openform-form)                   | Opens the form FormEditor in the developer..                                    |
|void | [save()](servoyDeveloper.md#save)                   | Saves all changes made through the solution model into the workspace..                                    |
|void | [save(override)](servoyDeveloper.md#save-override)                   | Saves all changes made through the solution model into the workspace..                                    |
|void | [save(obj)](servoyDeveloper.md#save-obj)                   | Saves just the given form, valuelist, relation or in memory datasource into the developers workspace..                                    |
|void | [save(obj, override)](servoyDeveloper.md#save-obj-override)                   | Saves just the given form, valuelist, relation or in memory datasource into the developers workspace..                                    |
|void | [save(obj, solutionName)](servoyDeveloper.md#save-obj-solutionname)                   | Saves just the given form, valuelist, relation or in memory datasource into the developers workspace..                                    |
|void | [updateInMemDataSource(dataSource, dataset, types)](servoyDeveloper.md#updateinmemdatasource-datasource-dataset-types)                   | Updates the given in memory datasource and saves it into the developers workspace..                                    |

## Methods Details

### openForm(form)

Opens the form FormEditor in the developer.

**Parameters**\
[Object](JSLib/Object.md) form The form name or JSForm object to open in an editor.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### save()

Saves all changes made through the solution model into the workspace.
Please note that this method only saves the new in memory datasources,
if you would like to override the existing ones use servoyDeveloper.save(true).


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### save(override)

Saves all changes made through the solution model into the workspace.

**Parameters**\
[Boolean](JSLib/Boolean.md) override Override existing in memory tables.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### save(obj)

Saves just the given form, valuelist, relation or in memory datasource into the developers workspace.
This must be a solution created or altered form/in memory datasource.

**Parameters**\
[Object](JSLib/Object.md) obj The formname, JSForm, JSValueList, JSRelation, datasource name or JSDataSource object to save.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### save(obj, override)

Saves just the given form, valuelist, relation or in memory datasource into the developers workspace.
This must be a solution created or altered form/in memory datasource.

**Parameters**\
[Object](JSLib/Object.md) obj The formname, JSForm, JSValueList, JSRelation, datasource name or JSDataSource object to save.\
[Boolean](JSLib/Boolean.md) override Override an existing in memory table.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### save(obj, solutionName)

Saves just the given form, valuelist, relation or in memory datasource into the developers workspace.
This must be a solution created form/in memory datasource.
NOTE: The current method can only be used for new objects.
For existing objects, please use the save method with the override flag set to true.
It is not needed to specify the solution, because the object to be updated will be saved in the right solution.

**Parameters**\
[Object](JSLib/Object.md) obj The formname, JSForm, JSValueList, JSRelation, datasource name or JSDataSource object to save.\
[String](JSLib/String.md) solutionName The destination solution, a module of the active solution.

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```
### updateInMemDataSource(dataSource, dataset, types)

Updates the given in memory datasource and saves it into the developers workspace.

**Parameters**\
[Object](JSLib/Object.md) dataSource datasource name or JSDataSource object to save.\
[Object](JSLib/Object.md) dataset the dataset with the update columns\
[Object](JSLib/Object.md) types array of the update columns types

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript

```

