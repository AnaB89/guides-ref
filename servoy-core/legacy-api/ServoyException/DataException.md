#  DataException

## **Supported Clients**

    SmartClient
    WebClient
    NGClient

## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../JSLib/Number.md) | [ABSTRACT_FORM](DataException.md#ABSTRACT_FORM)                   | Exception code for ABSTRACT_FORM..                                    |
| [Number](../JSLib/Number.md) | [ACQUIRE_LOCK_FAILURE](DataException.md#ACQUIRE_LOCK_FAILURE)                   | Exception code for ACQUIRE_LOCK_FAILURE..                                    |
| [Number](../JSLib/Number.md) | [BAD_SQL_SYNTAX](DataException.md#BAD_SQL_SYNTAX)                   | Exception code for BAD_SQL_SYNTAX..                                    |
| [Number](../JSLib/Number.md) | [CLIENT_NOT_AUTHORIZED](DataException.md#CLIENT_NOT_AUTHORIZED)                   | Exception code for CLIENT_NOT_AUTHORIZED..                                    |
| [Number](../JSLib/Number.md) | [DATA_ACCESS_RESOURCE_FAILURE](DataException.md#DATA_ACCESS_RESOURCE_FAILURE)                   | Exception code for DATA_ACCESS_RESOURCE_FAILURE..                                    |
| [Number](../JSLib/Number.md) | [DATA_INTEGRITY_VIOLATION](DataException.md#DATA_INTEGRITY_VIOLATION)                   | Exception code for DATA_INTEGRITY_VIOLATION..                                    |
| [Number](../JSLib/Number.md) | [DEADLOCK](DataException.md#DEADLOCK)                   | Exception code for DEADLOCK..                                    |
| [Number](../JSLib/Number.md) | [DELETE_NOT_GRANTED](DataException.md#DELETE_NOT_GRANTED)                   | Exception code for DELETE_NOT_GRANTED..                                    |
| [Number](../JSLib/Number.md) | [EXECUTE_PROGRAM_FAILED](DataException.md#EXECUTE_PROGRAM_FAILED)                   | Exception code for EXECUTE_PROGRAM_FAILED..                                    |
| [Number](../JSLib/Number.md) | [INCORRECT_LOGIN](DataException.md#INCORRECT_LOGIN)                   | Exception code for INCORRECT_LOGIN..                                    |
| [Number](../JSLib/Number.md) | [INVALID_INPUT](DataException.md#INVALID_INPUT)                   | Exception code for INVALID_INPUT..                                    |
| [Number](../JSLib/Number.md) | [INVALID_RESULTSET_ACCESS](DataException.md#INVALID_RESULTSET_ACCESS)                   | Exception code for INVALID_RESULTSET_ACCESS..                                    |
| [Number](../JSLib/Number.md) | [MAINTENANCE_MODE](DataException.md#MAINTENANCE_MODE)                   | Exception code for MAINTENANCE_MODE..                                    |
| [Number](../JSLib/Number.md) | [MUST_ROLLBACK](DataException.md#MUST_ROLLBACK)                   | Exception code for MUST_ROLLBACK..                                    |
| [Number](../JSLib/Number.md) | [NO_ACCESS](DataException.md#NO_ACCESS)                   | Exception code for NO_ACCESS..                                    |
| [Number](../JSLib/Number.md) | [NO_CREATE_ACCESS](DataException.md#NO_CREATE_ACCESS)                   | Exception code for NO_CREATE_ACCESS..                                    |
| [Number](../JSLib/Number.md) | [NO_DELETE_ACCESS](DataException.md#NO_DELETE_ACCESS)                   | Exception code for NO_DELETE_ACCESS..                                    |
| [Number](../JSLib/Number.md) | [NO_LICENSE](DataException.md#NO_LICENSE)                   | Exception code for NO_LICENSE..                                    |
| [Number](../JSLib/Number.md) | [NO_MODIFY_ACCESS](DataException.md#NO_MODIFY_ACCESS)                   | Exception code for NO_MODIFY_ACCESS..                                    |
| [Number](../JSLib/Number.md) | [NO_PARENT_DELETE_WITH_RELATED_RECORDS](DataException.md#NO_PARENT_DELETE_WITH_RELATED_RECORDS)                   | Exception code for NO_PARENT_DELETE_WITH_RELATED_RECORDS..                                    |
| [Number](../JSLib/Number.md) | [NO_RELATED_CREATE_ACCESS](DataException.md#NO_RELATED_CREATE_ACCESS)                   | Exception code for NO_RELATED_CREATE_ACCESS..                                    |
| [Number](../JSLib/Number.md) | [PERMISSION_DENIED](DataException.md#PERMISSION_DENIED)                   | Exception code for PERMISSION_DENIED..                                    |
| [Number](../JSLib/Number.md) | [RECORD_LOCKED](DataException.md#RECORD_LOCKED)                   | Exception code for RECORD_LOCKED..                                    |
| [Number](../JSLib/Number.md) | [RECORD_VALIDATION_FAILED](DataException.md#RECORD_VALIDATION_FAILED)                   | Exception code for RECORD_VALIDATION_FAILED..                                    |
| [Number](../JSLib/Number.md) | [SAVE_FAILED](DataException.md#SAVE_FAILED)                   | Exception code for SAVE_FAILED..                                    |
| [Number](../JSLib/Number.md) | [UNEXPECTED_UPDATE_COUNT](DataException.md#UNEXPECTED_UPDATE_COUNT)                   | Exception code for UNEXPECTED_UPDATE_COUNT..                                    |
| [Number](../JSLib/Number.md) | [UNKNOWN_DATABASE_EXCEPTION](DataException.md#UNKNOWN_DATABASE_EXCEPTION)                   | Exception code for UNKNOWN_DATABASE_EXCEPTION..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [String](../JSLib/String.md) | [getContext()](DataException.md#getcontext)                   | .                                    |
| [Number](../JSLib/Number.md) | [getErrorCode()](DataException.md#geterrorcode)                   | Returns the error code for this ServoyException..                                    |
| [String](../JSLib/String.md) | [getMessage()](DataException.md#getmessage)                   | Returns the string message for this ServoyException..                                    |
| [Array](../JSLib/Array.md) | [getParameters()](DataException.md#getparameters)                   | Returns the parameters of the SQL query that caused this DataException in an array..                                    |
| [String](../JSLib/String.md) | [getSQL()](DataException.md#getsql)                   | Returns the SQL query that caused this DataException..                                    |
| [String](../JSLib/String.md) | [getSQLState()](DataException.md#getsqlstate)                   | Returns the SQLState for this DataException..                                    |
| [String](../JSLib/String.md) | [getScriptStackTrace()](DataException.md#getscriptstacktrace)                   | Returns the script stack trace for this ServoyException if this could be created..                                    |
| [String](../JSLib/String.md) | [getStackTrace()](DataException.md#getstacktrace)                   | Returns the stack trace for this ServoyException..                                    |
| [Object](../JSLib/Object.md) | [getValue()](DataException.md#getvalue)                   | Returns the value for this DataException..                                    |
| [Number](../JSLib/Number.md) | [getVendorErrorCode()](DataException.md#getvendorerrorcode)                   | Returns the error code of the error thrown by the back-end database server..                                    |

## Constants Details

### ABSTRACT_FORM

Exception code for ABSTRACT_FORM.

This code is used when a form, that cannot be created, is shown (for example, a form without parts).

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### ACQUIRE_LOCK_FAILURE

Exception code for ACQUIRE_LOCK_FAILURE.

This code is used when a database failed to lock a row or table.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### BAD_SQL_SYNTAX

Exception code for BAD_SQL_SYNTAX.

This code is used when a database exception is recognized as an sql syntax error.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### CLIENT_NOT_AUTHORIZED

Exception code for CLIENT_NOT_AUTHORIZED.

This code is used when an client performs an action that requires the user to be logged in and the user has not logged in yet.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### DATA_ACCESS_RESOURCE_FAILURE

Exception code for DATA_ACCESS_RESOURCE_FAILURE.

This code is used when a database exception received an error accessing storage devices.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### DATA_INTEGRITY_VIOLATION

Exception code for DATA_INTEGRITY_VIOLATION.

This code is used when a database exception is recognized as an integrity exception (like constraint violation).

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### DEADLOCK

Exception code for DEADLOCK.

This code is used when a deadlock is detected by the database.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### DELETE_NOT_GRANTED

Exception code for DELETE_NOT_GRANTED.

This code is used when a record deletion was rejected by a pre-delete Servoy trigger.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### EXECUTE_PROGRAM_FAILED

Exception code for EXECUTE_PROGRAM_FAILED.

This code is used when an external program was not executed correctly.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### INCORRECT_LOGIN

Exception code for INCORRECT_LOGIN.

This code is used when the user enters invalid credentials.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### INVALID_INPUT

Exception code for INVALID_INPUT.

This code is used when the user enters data that could not be validated.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### INVALID_RESULTSET_ACCESS

Exception code for INVALID_RESULTSET_ACCESS.

This code is used when a data is requested that is not selected in the sql.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### MAINTENANCE_MODE

Exception code for MAINTENANCE_MODE.

This code is used when a client could not be registered with the server because the server is in maintenance mode.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### MUST_ROLLBACK

Exception code for MUST_ROLLBACK.

This code is used when an update is not performed because of a previous sql-exception within a transaction.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### NO_ACCESS

Exception code for NO_ACCESS.

This code is used when a user wants to view data and this is disallowed by security settings.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### NO_CREATE_ACCESS

Exception code for NO_CREATE_ACCESS.

This code is used when a user wants to create new records and this is disallowed by security settings.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### NO_DELETE_ACCESS

Exception code for NO_DELETE_ACCESS.

This code is used when a user wants to delete data and this is disallowed by security settings.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### NO_LICENSE

Exception code for NO_LICENSE.

This code is used when a client could not be registered with the server because of license limitations.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### NO_MODIFY_ACCESS

Exception code for NO_MODIFY_ACCESS.

This code is used when a user wants to update data and this is disallowed by security settings.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### NO_PARENT_DELETE_WITH_RELATED_RECORDS

Exception code for NO_PARENT_DELETE_WITH_RELATED_RECORDS.

This code is used when a record could not be deleted because a non-empty relation exists for the record that does not allow parent delete when having related records.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### NO_RELATED_CREATE_ACCESS

Exception code for NO_RELATED_CREATE_ACCESS.

This code is used when a user wants to create new related records and this is disallowed by security settings.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### PERMISSION_DENIED

Exception code for PERMISSION_DENIED.

This code is used when a database exception is recognized as a authorization error.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### RECORD_LOCKED

Exception code for RECORD_LOCKED.

This code is used when a record could not be updated or deleted because it is locked by another client.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### RECORD_VALIDATION_FAILED

Exception code for RECORD_VALIDATION_FAILED.

This code is used when a record update/insert was rejected by a pre-update/insert Servoy trigger.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### SAVE_FAILED

Exception code for SAVE_FAILED.

This code is used when a javascript exception occurred during saving data to the database.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### UNEXPECTED_UPDATE_COUNT

Exception code for UNEXPECTED_UPDATE_COUNT.

This code is used when a data could not be deleted or updated when expected (for example
when a record was deleted outside Servoy and a Servoy client wants to update the record).

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### UNKNOWN_DATABASE_EXCEPTION

Exception code for UNKNOWN_DATABASE_EXCEPTION.

This code is used when an unrecognized database exception has occurred.

**Returns**\
[Number](../JSLib/Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```

## Methods Details

### getContext()




**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript

```
### getErrorCode()

Returns the error code for this ServoyException. Can be one of the constants declared in ServoyException.


**Returns**\
[Number](../JSLib/Number.md) the error code for this ServoyException. Can be one of the constants declared in ServoyException.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### getMessage()

Returns the string message for this ServoyException.


**Returns**\
[String](../JSLib/String.md) the string message for this ServoyException.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### getParameters()

Returns the parameters of the SQL query that caused this DataException in an array.


**Returns**\
[Array](../JSLib/Array.md) the parameters of the SQL query that caused this DataException in an array.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var record = array[i];
application.output(record.exception);
if (record.exception instanceof DataException)
{
	var param = record.exception.getParameters();
	for (j = 0; j < param.length; j++)
	{
		application.output("SQL Parameter [" + j + "]: " + param[j]);
	}
}
```
### getSQL()

Returns the SQL query that caused this DataException.


**Returns**\
[String](../JSLib/String.md) the SQL query that caused this DataException.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var record = array[i];
application.output(record.exception);
if (record.exception instanceof DataException)
{
	application.output("SQL: " + record.exception.getSQL());
}
```
### getSQLState()

Returns the SQLState for this DataException.
This is a "SQLstate" string, which follows either the XOPEN SQLstate conventions or the SQL 99 conventions.
The values of the SQLState string are described in the appropriate spec.


**Returns**\
[String](../JSLib/String.md) the SQLState for this DataException.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var record = array[i];
application.output(record.exception);
if (record.exception instanceof DataException)
{
	application.output("SQLState: " + record.exception.getSQLState());
}
```
### getScriptStackTrace()

Returns the script stack trace for this ServoyException if this could be created.


**Returns**\
[String](../JSLib/String.md) the string stack trace for this ServoyException.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### getStackTrace()

Returns the stack trace for this ServoyException.


**Returns**\
[String](../JSLib/String.md) the string stack trace for this ServoyException.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
//this sample script should be attached to onError method handler in the solution settings
application.output('Exception Object: '+ex)
application.output('MSG: '+ex.getMessage())
if (ex instanceof ServoyException)
{
	/** @type {ServoyException} */
	var servoyException = ex;
	application.output("is a ServoyException")
	application.output("Errorcode: "+servoyException.getErrorCode())
	var trace = "";
	if (ex.getScriptStackTrace) trace = servoyException.getScriptStackTrace();
	else if (servoyException.getStackTrace)  trace = servoyException.getStackTrace();
	if (servoyException.getErrorCode() == ServoyException.SAVE_FAILED)
	{
		plugins.dialogs.showErrorDialog( 'Error',  'It seems you did not fill in a required field', 'OK');
		//Get the failed records after a save
		var array = databaseManager.getFailedRecords()
		for( var i = 0 ; i < array.length ; i++ )
		{
			var record = array[i];
			application.output(record.exception);
			if (record.exception instanceof DataException)
			{
				/** @type {DataException} */
				var dataException = record.exception;
				application.output('SQL: '+dataException.getSQL())
				application.output('SQLState: '+dataException.getSQLState())
				application.output('VendorErrorCode: '+dataException.getVendorErrorCode())
			}
		}
		return false
	}
}
//if returns false or no return, error is not reported to client; if returns true error is reported
//by default error report means logging the error, in smart client an error dialog will also show up
return true
```
### getValue()

Returns the value for this DataException.
The value is the object thrown in table pre-insert, pre-update or pre-delete triggers.


**Returns**\
[Object](../JSLib/Object.md) the value for this DataException.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var record = array[i];
application.output(record.exception);
if (record.exception instanceof DataException)
{
	application.output("VALUE: " + record.exception.getValue());
}
```
### getVendorErrorCode()

Returns the error code of the error thrown by the back-end database server.


**Returns**\
[Number](../JSLib/Number.md) the error code of the error thrown by the back-end database server.

**Supported Clients**\
SmartClient,WebClient,NGClient

**Sample**

```javascript
var record = array[i];
application.output(record.exception);
if (record.exception instanceof DataException)
{
	application.output("VendorErrorCode: " + record.exception.getVendorErrorCode());
}
```

