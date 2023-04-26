# servoyDeveloper

## Methods Summary

| Type | Name                                                                                                                   | Summary                                                                                                |
| ---- | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| void | [openForm(form)](servoydeveloper.md#openform-form)                                                                     | Opens the form FormEditor in the developer..                                                           |
| void | [save()](servoydeveloper.md#save)                                                                                      | Saves all changes made through the solution model into the workspace..                                 |
| void | [save(override)](servoydeveloper.md#save-override)                                                                     | Saves all changes made through the solution model into the workspace..                                 |
| void | [save(obj)](servoydeveloper.md#save-obj)                                                                               | Saves just the given form, valuelist, relation or in memory datasource into the developers workspace.. |
| void | [save(obj, override)](servoydeveloper.md#save-obj-override)                                                            | Saves just the given form, valuelist, relation or in memory datasource into the developers workspace.. |
| void | [save(obj, solutionName)](servoydeveloper.md#save-obj-solutionname)                                                    | Saves just the given form, valuelist, relation or in memory datasource into the developers workspace.. |
| void | [updateInMemDataSource(dataSource, dataset, types)](servoydeveloper.md#updateinmemdatasource-datasource-dataset-types) | Updates the given in memory datasource and saves it into the developers workspace..                    |

## Methods Details

### openForm(form)

Opens the form FormEditor in the developer.

**Parameters**\
[Object](js-lib/object.md) form The form name or JSForm object to open in an editor.

**Returns**\
void

**Sample**

```javascript
```

### save()

Saves all changes made through the solution model into the workspace. Please note that this method only saves the new in memory datasources, if you would like to override the existing ones use servoyDeveloper.save(true).

**Returns**\
void

**Sample**

```javascript
```

### save(override)

Saves all changes made through the solution model into the workspace.

**Parameters**\
[Boolean](js-lib/boolean.md) override Override existing in memory tables.

**Returns**\
void

**Sample**

```javascript
```

### save(obj)

Saves just the given form, valuelist, relation or in memory datasource into the developers workspace. This must be a solution created or altered form/in memory datasource.

**Parameters**\
[Object](js-lib/object.md) obj The formname, JSForm, JSValueList, JSRelation, datasource name or JSDataSource object to save.

**Returns**\
void

**Sample**

```javascript
```

### save(obj, override)

Saves just the given form, valuelist, relation or in memory datasource into the developers workspace. This must be a solution created or altered form/in memory datasource.

**Parameters**\
[Object](js-lib/object.md) obj The formname, JSForm, JSValueList, JSRelation, datasource name or JSDataSource object to save.\
[Boolean](js-lib/boolean.md) override Override an existing in memory table.

**Returns**\
void

**Sample**

```javascript
```

### save(obj, solutionName)

Saves just the given form, valuelist, relation or in memory datasource into the developers workspace. This must be a solution created form/in memory datasource. NOTE: The current method can only be used for new objects. For existing objects, please use the save method with the override flag set to true. It is not needed to specify the solution, because the object to be updated will be saved in the right solution.

**Parameters**\
[Object](js-lib/object.md) obj The formname, JSForm, JSValueList, JSRelation, datasource name or JSDataSource object to save.\
[String](js-lib/string.md) solutionName The destination solution, a module of the active solution.

**Returns**\
void

**Sample**

```javascript
```

### updateInMemDataSource(dataSource, dataset, types)

Updates the given in memory datasource and saves it into the developers workspace.

**Parameters**\
[Object](js-lib/object.md) dataSource datasource name or JSDataSource object to save.\
[Object](js-lib/object.md) dataset the dataset with the update columns\
[Object](js-lib/object.md) types array of the update columns types

**Returns**\
void

**Sample**

```javascript
```
