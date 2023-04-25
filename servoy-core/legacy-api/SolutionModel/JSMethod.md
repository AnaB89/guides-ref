#  JSMethod

## **Supported Clients**

    SmartClient
    WebClient
    NGClient
    MobileClient

## Property Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [code](JSMethod.md#code)                   | The full source code of this method (including doc and function declaration)..                                    |
| [Boolean](../JSLib/Boolean.md) | [showInMenu](JSMethod.md#showInMenu)                   | Flag that tells if the method appears or not in the "Methods" menu of Servoy Client..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Array](../JSLib/Array.md) | [getArguments()](JSMethod.md#getarguments)                   | Gets the argument array for this method if that is set for the specific action this method is taken from..                                    |
| [String](../JSLib/String.md) | [getName()](JSMethod.md#getname)                   | The name of the method..                                    |
| [String](../JSLib/String.md) | [getScopeName()](JSMethod.md#getscopename)                   | Get scope name.                                    |
| [UUID](../Application/UUID.md) | [getUUID()](JSMethod.md#getuuid)                   | Returns the UUID of the method object.                                    |

## Properties Details

### code

The full source code of this method (including doc and function declaration).

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var method = form.newMethod('function original() { application.output("Original function."); }');
application.output('original method name: ' + method.getName());
application.output('original method code: ' + method.code);
method.code = 'function changed() { application.output("This is another function."); }';
method.showInMenu = false;
var button = form.newButton('Click me!', 10, 10, 100, 30, method);
```
### showInMenu

Flag that tells if the method appears or not in the "Methods" menu of Servoy Client.

**Returns**\
[Boolean](../JSLib/Boolean.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var method = form.newMethod('function original() { application.output("Original function."); }');
application.output('original method name: ' + method.getName());
application.output('original method code: ' + method.code);
method.code = 'function changed() { application.output("This is another function."); }';
method.showInMenu = false;
var button = form.newButton('Click me!', 10, 10, 100, 30, method);
```

## Methods Details

### getArguments()

Gets the argument array for this method if that is set for the specific action this method is taken from.
Will return null by default. This is only for reading, you can't alter the arguments through this array,
for that you need to create a new object through solutionModel.wrapMethodWithArguments(..) and assign it again.


**Returns**\
[Array](../JSLib/Array.md) Array of the arguments, null if not specified.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var frm = solutionModel.getForm("myForm");
var button = frm.getButton("button");
// get the arguments from the button.
// NOTE: string arguments will be returned with quotes (comp.onAction.getArguments()[0] == '\'foo\' evals to true)
var arguments = button.onAction.getArguments();
if (arguments && arguments.length > 1 && arguments[1] == 10) {
	// change the value and assign it back to the onAction.
	arguments[1] = 50;
	button.onAction = solutionModel.wrapMethodWithArguments(button.onAction,arguments);
}
```
### getName()

The name of the method.


**Returns**\
[String](../JSLib/String.md) A String holding the name of this method.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var method = form.newMethod('function original() { application.output("Original function."); }');
application.output('original method name: ' + method.getName());
application.output('original method code: ' + method.code);
method.code = 'function changed() { application.output("This is another function."); }';
method.showInMenu = false;
var button = form.newButton('Click me!', 10, 10, 100, 30, method);
```
### getScopeName()

Get scope name


**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var methods = solutionModel.getGlobalMethods();
for (var x in methods)
	application.output(methods[x].getName() + ' is defined in scope ' + methods[x].getScopeName());
```
### getUUID()

Returns the UUID of the method object


**Returns**\
[UUID](../Application/UUID.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var method = form.newMethod('function original() { application.output("Original function."); }');
application.output(method.getUUID().toString());
```

