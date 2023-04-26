# DataException

## Constants Summary

| Type                          | Name                                                                                                      | Summary                                                         |
| ----------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------- |
| [Number](../js-lib/number.md) | [ABSTRACT\_FORM](dataexception.md#ABSTRACT\_FORM)                                                         | Exception code for ABSTRACT\_FORM..                             |
| [Number](../js-lib/number.md) | [ACQUIRE\_LOCK\_FAILURE](dataexception.md#ACQUIRE\_LOCK\_FAILURE)                                         | Exception code for ACQUIRE\_LOCK\_FAILURE..                     |
| [Number](../js-lib/number.md) | [BAD\_SQL\_SYNTAX](dataexception.md#BAD\_SQL\_SYNTAX)                                                     | Exception code for BAD\_SQL\_SYNTAX..                           |
| [Number](../js-lib/number.md) | [CLIENT\_NOT\_AUTHORIZED](dataexception.md#CLIENT\_NOT\_AUTHORIZED)                                       | Exception code for CLIENT\_NOT\_AUTHORIZED..                    |
| [Number](../js-lib/number.md) | [DATA\_ACCESS\_RESOURCE\_FAILURE](dataexception.md#DATA\_ACCESS\_RESOURCE\_FAILURE)                       | Exception code for DATA\_ACCESS\_RESOURCE\_FAILURE..            |
| [Number](../js-lib/number.md) | [DATA\_INTEGRITY\_VIOLATION](dataexception.md#DATA\_INTEGRITY\_VIOLATION)                                 | Exception code for DATA\_INTEGRITY\_VIOLATION..                 |
| [Number](../js-lib/number.md) | [DEADLOCK](dataexception.md#DEADLOCK)                                                                     | Exception code for DEADLOCK..                                   |
| [Number](../js-lib/number.md) | [DELETE\_NOT\_GRANTED](dataexception.md#DELETE\_NOT\_GRANTED)                                             | Exception code for DELETE\_NOT\_GRANTED..                       |
| [Number](../js-lib/number.md) | [EXECUTE\_PROGRAM\_FAILED](dataexception.md#EXECUTE\_PROGRAM\_FAILED)                                     | Exception code for EXECUTE\_PROGRAM\_FAILED..                   |
| [Number](../js-lib/number.md) | [INCORRECT\_LOGIN](dataexception.md#INCORRECT\_LOGIN)                                                     | Exception code for INCORRECT\_LOGIN..                           |
| [Number](../js-lib/number.md) | [INVALID\_INPUT](dataexception.md#INVALID\_INPUT)                                                         | Exception code for INVALID\_INPUT..                             |
| [Number](../js-lib/number.md) | [INVALID\_RESULTSET\_ACCESS](dataexception.md#INVALID\_RESULTSET\_ACCESS)                                 | Exception code for INVALID\_RESULTSET\_ACCESS..                 |
| [Number](../js-lib/number.md) | [MAINTENANCE\_MODE](dataexception.md#MAINTENANCE\_MODE)                                                   | Exception code for MAINTENANCE\_MODE..                          |
| [Number](../js-lib/number.md) | [MUST\_ROLLBACK](dataexception.md#MUST\_ROLLBACK)                                                         | Exception code for MUST\_ROLLBACK..                             |
| [Number](../js-lib/number.md) | [NO\_ACCESS](dataexception.md#NO\_ACCESS)                                                                 | Exception code for NO\_ACCESS..                                 |
| [Number](../js-lib/number.md) | [NO\_CREATE\_ACCESS](dataexception.md#NO\_CREATE\_ACCESS)                                                 | Exception code for NO\_CREATE\_ACCESS..                         |
| [Number](../js-lib/number.md) | [NO\_DELETE\_ACCESS](dataexception.md#NO\_DELETE\_ACCESS)                                                 | Exception code for NO\_DELETE\_ACCESS..                         |
| [Number](../js-lib/number.md) | [NO\_LICENSE](dataexception.md#NO\_LICENSE)                                                               | Exception code for NO\_LICENSE..                                |
| [Number](../js-lib/number.md) | [NO\_MODIFY\_ACCESS](dataexception.md#NO\_MODIFY\_ACCESS)                                                 | Exception code for NO\_MODIFY\_ACCESS..                         |
| [Number](../js-lib/number.md) | [NO\_PARENT\_DELETE\_WITH\_RELATED\_RECORDS](dataexception.md#NO\_PARENT\_DELETE\_WITH\_RELATED\_RECORDS) | Exception code for NO\_PARENT\_DELETE\_WITH\_RELATED\_RECORDS.. |
| [Number](../js-lib/number.md) | [NO\_RELATED\_CREATE\_ACCESS](dataexception.md#NO\_RELATED\_CREATE\_ACCESS)                               | Exception code for NO\_RELATED\_CREATE\_ACCESS..                |
| [Number](../js-lib/number.md) | [PERMISSION\_DENIED](dataexception.md#PERMISSION\_DENIED)                                                 | Exception code for PERMISSION\_DENIED..                         |
| [Number](../js-lib/number.md) | [RECORD\_LOCKED](dataexception.md#RECORD\_LOCKED)                                                         | Exception code for RECORD\_LOCKED..                             |
| [Number](../js-lib/number.md) | [RECORD\_VALIDATION\_FAILED](dataexception.md#RECORD\_VALIDATION\_FAILED)                                 | Exception code for RECORD\_VALIDATION\_FAILED..                 |
| [Number](../js-lib/number.md) | [SAVE\_FAILED](dataexception.md#SAVE\_FAILED)                                                             | Exception code for SAVE\_FAILED..                               |
| [Number](../js-lib/number.md) | [UNEXPECTED\_UPDATE\_COUNT](dataexception.md#UNEXPECTED\_UPDATE\_COUNT)                                   | Exception code for UNEXPECTED\_UPDATE\_COUNT..                  |
| [Number](../js-lib/number.md) | [UNKNOWN\_DATABASE\_EXCEPTION](dataexception.md#UNKNOWN\_DATABASE\_EXCEPTION)                             | Exception code for UNKNOWN\_DATABASE\_EXCEPTION..               |

## Methods Summary

| Type                          | Name                                                          | Summary                                                                              |
| ----------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------------------------------ |
| [String](../js-lib/string.md) | [getContext()](dataexception.md#getcontext)                   | .                                                                                    |
| [Number](../js-lib/number.md) | [getErrorCode()](dataexception.md#geterrorcode)               | Returns the error code for this ServoyException..                                    |
| [String](../js-lib/string.md) | [getMessage()](dataexception.md#getmessage)                   | Returns the string message for this ServoyException..                                |
| [Array](../js-lib/array.md)   | [getParameters()](dataexception.md#getparameters)             | Returns the parameters of the SQL query that caused this DataException in an array.. |
| [String](../js-lib/string.md) | [getSQL()](dataexception.md#getsql)                           | Returns the SQL query that caused this DataException..                               |
| [String](../js-lib/string.md) | [getSQLState()](dataexception.md#getsqlstate)                 | Returns the SQLState for this DataException..                                        |
| [String](../js-lib/string.md) | [getScriptStackTrace()](dataexception.md#getscriptstacktrace) | Returns the script stack trace for this ServoyException if this could be created..   |
| [String](../js-lib/string.md) | [getStackTrace()](dataexception.md#getstacktrace)             | Returns the stack trace for this ServoyException..                                   |
| [Object](../js-lib/object.md) | [getValue()](dataexception.md#getvalue)                       | Returns the value for this DataException..                                           |
| [Number](../js-lib/number.md) | [getVendorErrorCode()](dataexception.md#getvendorerrorcode)   | Returns the error code of the error thrown by the back-end database server..         |

## Constants Details

### ABSTRACT\_FORM

Exception code for ABSTRACT\_FORM.

This code is used when a form, that cannot be created, is shown (for example, a form without parts).

**Returns**\
[Number](../js-lib/number.md)

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

### ACQUIRE\_LOCK\_FAILURE

Exception code for ACQUIRE\_LOCK\_FAILURE.

This code is used when a database failed to lock a row or table.

**Returns**\
[Number](../js-lib/number.md)

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

### BAD\_SQL\_SYNTAX

Exception code for BAD\_SQL\_SYNTAX.

This code is used when a database exception is recognized as an sql syntax error.

**Returns**\
[Number](../js-lib/number.md)

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

### CLIENT\_NOT\_AUTHORIZED

Exception code for CLIENT\_NOT\_AUTHORIZED.

This code is used when an client performs an action that requires the user to be logged in and the user has not logged in yet.

**Returns**\
[Number](../js-lib/number.md)

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

### DATA\_ACCESS\_RESOURCE\_FAILURE

Exception code for DATA\_ACCESS\_RESOURCE\_FAILURE.

This code is used when a database exception received an error accessing storage devices.

**Returns**\
[Number](../js-lib/number.md)

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

### DATA\_INTEGRITY\_VIOLATION

Exception code for DATA\_INTEGRITY\_VIOLATION.

This code is used when a database exception is recognized as an integrity exception (like constraint violation).

**Returns**\
[Number](../js-lib/number.md)

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
[Number](../js-lib/number.md)

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

### DELETE\_NOT\_GRANTED

Exception code for DELETE\_NOT\_GRANTED.

This code is used when a record deletion was rejected by a pre-delete Servoy trigger.

**Returns**\
[Number](../js-lib/number.md)

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

### EXECUTE\_PROGRAM\_FAILED

Exception code for EXECUTE\_PROGRAM\_FAILED.

This code is used when an external program was not executed correctly.

**Returns**\
[Number](../js-lib/number.md)

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

### INCORRECT\_LOGIN

Exception code for INCORRECT\_LOGIN.

This code is used when the user enters invalid credentials.

**Returns**\
[Number](../js-lib/number.md)

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

### INVALID\_INPUT

Exception code for INVALID\_INPUT.

This code is used when the user enters data that could not be validated.

**Returns**\
[Number](../js-lib/number.md)

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

### INVALID\_RESULTSET\_ACCESS

Exception code for INVALID\_RESULTSET\_ACCESS.

This code is used when a data is requested that is not selected in the sql.

**Returns**\
[Number](../js-lib/number.md)

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

### MAINTENANCE\_MODE

Exception code for MAINTENANCE\_MODE.

This code is used when a client could not be registered with the server because the server is in maintenance mode.

**Returns**\
[Number](../js-lib/number.md)

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

### MUST\_ROLLBACK

Exception code for MUST\_ROLLBACK.

This code is used when an update is not performed because of a previous sql-exception within a transaction.

**Returns**\
[Number](../js-lib/number.md)

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

### NO\_ACCESS

Exception code for NO\_ACCESS.

This code is used when a user wants to view data and this is disallowed by security settings.

**Returns**\
[Number](../js-lib/number.md)

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

### NO\_CREATE\_ACCESS

Exception code for NO\_CREATE\_ACCESS.

This code is used when a user wants to create new records and this is disallowed by security settings.

**Returns**\
[Number](../js-lib/number.md)

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

### NO\_DELETE\_ACCESS

Exception code for NO\_DELETE\_ACCESS.

This code is used when a user wants to delete data and this is disallowed by security settings.

**Returns**\
[Number](../js-lib/number.md)

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

### NO\_LICENSE

Exception code for NO\_LICENSE.

This code is used when a client could not be registered with the server because of license limitations.

**Returns**\
[Number](../js-lib/number.md)

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

### NO\_MODIFY\_ACCESS

Exception code for NO\_MODIFY\_ACCESS.

This code is used when a user wants to update data and this is disallowed by security settings.

**Returns**\
[Number](../js-lib/number.md)

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

### NO\_PARENT\_DELETE\_WITH\_RELATED\_RECORDS

Exception code for NO\_PARENT\_DELETE\_WITH\_RELATED\_RECORDS.

This code is used when a record could not be deleted because a non-empty relation exists for the record that does not allow parent delete when having related records.

**Returns**\
[Number](../js-lib/number.md)

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

### NO\_RELATED\_CREATE\_ACCESS

Exception code for NO\_RELATED\_CREATE\_ACCESS.

This code is used when a user wants to create new related records and this is disallowed by security settings.

**Returns**\
[Number](../js-lib/number.md)

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

### PERMISSION\_DENIED

Exception code for PERMISSION\_DENIED.

This code is used when a database exception is recognized as a authorization error.

**Returns**\
[Number](../js-lib/number.md)

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

### RECORD\_LOCKED

Exception code for RECORD\_LOCKED.

This code is used when a record could not be updated or deleted because it is locked by another client.

**Returns**\
[Number](../js-lib/number.md)

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

### RECORD\_VALIDATION\_FAILED

Exception code for RECORD\_VALIDATION\_FAILED.

This code is used when a record update/insert was rejected by a pre-update/insert Servoy trigger.

**Returns**\
[Number](../js-lib/number.md)

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

### SAVE\_FAILED

Exception code for SAVE\_FAILED.

This code is used when a javascript exception occurred during saving data to the database.

**Returns**\
[Number](../js-lib/number.md)

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

### UNEXPECTED\_UPDATE\_COUNT

Exception code for UNEXPECTED\_UPDATE\_COUNT.

This code is used when a data could not be deleted or updated when expected (for example when a record was deleted outside Servoy and a Servoy client wants to update the record).

**Returns**\
[Number](../js-lib/number.md)

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

### UNKNOWN\_DATABASE\_EXCEPTION

Exception code for UNKNOWN\_DATABASE\_EXCEPTION.

This code is used when an unrecognized database exception has occurred.

**Returns**\
[Number](../js-lib/number.md)

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
[String](../js-lib/string.md)

**Sample**

```javascript
```

### getErrorCode()

Returns the error code for this ServoyException. Can be one of the constants declared in ServoyException.

**Returns**\
[Number](../js-lib/number.md) the error code for this ServoyException. Can be one of the constants declared in ServoyException.

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
[String](../js-lib/string.md) the string message for this ServoyException.

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
[Array](../js-lib/array.md) the parameters of the SQL query that caused this DataException in an array.

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
[String](../js-lib/string.md) the SQL query that caused this DataException.

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

Returns the SQLState for this DataException. This is a "SQLstate" string, which follows either the XOPEN SQLstate conventions or the SQL 99 conventions. The values of the SQLState string are described in the appropriate spec.

**Returns**\
[String](../js-lib/string.md) the SQLState for this DataException.

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
[String](../js-lib/string.md) the string stack trace for this ServoyException.

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
[String](../js-lib/string.md) the string stack trace for this ServoyException.

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

Returns the value for this DataException. The value is the object thrown in table pre-insert, pre-update or pre-delete triggers.

**Returns**\
[Object](../js-lib/object.md) the value for this DataException.

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
[Number](../js-lib/number.md) the error code of the error thrown by the back-end database server.

**Sample**

```javascript
var record = array[i];
application.output(record.exception);
if (record.exception instanceof DataException)
{
	application.output("VendorErrorCode: " + record.exception.getVendorErrorCode());
}
```
