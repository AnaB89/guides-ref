#  scheduler


## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [addCronJob(jobname, cronTimings, method)](scheduler.md#addcronjob-jobname-crontimings-method)                   | Adds a cron job to the scheduler..                                    |
|void | [addCronJob(jobname, cronTimings, method, startDate)](scheduler.md#addcronjob-jobname-crontimings-method-startdate)                   | Adds a cron job to the scheduler..                                    |
|void | [addCronJob(jobname, cronTimings, method, startDate, endDate)](scheduler.md#addcronjob-jobname-crontimings-method-startdate-enddate)                   | Adds a cron job to the scheduler..                                    |
|void | [addCronJob(jobname, cronTimings, method, startDate, endDate, arguments)](scheduler.md#addcronjob-jobname-crontimings-method-startdate-enddate-arguments)                   | Adds a cron job to the scheduler..                                    |
|void | [addJob(jobname, startDate, method)](scheduler.md#addjob-jobname-startdate-method)                   | Adds a job to the scheduler..                                    |
|void | [addJob(jobname, startDate, method, repeatInterval)](scheduler.md#addjob-jobname-startdate-method-repeatinterval)                   | Adds a job to the scheduler..                                    |
|void | [addJob(jobname, startDate, method, repeatInterval, repeatCount)](scheduler.md#addjob-jobname-startdate-method-repeatinterval-repeatcount)                   | Adds a job to the scheduler..                                    |
|void | [addJob(jobName, startDate, method, repeatInterval, repeatCount, endDate)](scheduler.md#addjob-jobname-startdate-method-repeatinterval-repeatcount-enddate)                   | Adds a job to the scheduler..                                    |
|void | [addJob(jobname, startDate, method, repeatInterval, repeatCount, endDate, arguments)](scheduler.md#addjob-jobname-startdate-method-repeatinterval-repeatcount-enddate-arguments)                   | Adds a job to the scheduler..                                    |
|void | [addJob(jobname, startDate, method, arguments)](scheduler.md#addjob-jobname-startdate-method-arguments)                   | Adds a job to the scheduler..                                    |
| [Array](../../JSLib/Array.md) | [getCurrentJobNames()](scheduler.md#getcurrentjobnames)                   | Returns an array with the current jobs..                                    |
| [String](../../JSLib/String.md) | [getLastRunJobName()](scheduler.md#getlastrunjobname)                   | Returns the last job run from the scheduler..                                    |
| [Boolean](../../JSLib/Boolean.md) | [removeJob(jobname)](scheduler.md#removejob-jobname)                   | Removes a job from the scheduler..                                    |

## Methods Details

### addCronJob(jobname, cronTimings, method)

Adds a cron job to the scheduler. A cron job must have at least one minute between each execution (otherwise it won't execute).

**Parameters**\
[String](../../JSLib/String.md) jobname  ;\
[String](../../JSLib/String.md) cronTimings  ;\
[Function](../../JSLib/Function.md) method  ;

**Returns**\
void 


**Sample**

```javascript
// see: http://www.quartz-scheduler.org/documentation/quartz-2.3.0/tutorials/tutorial-lesson-06.html for more info
// add a job that runs every 20 minutes after the hour (0,20,40)
plugins.scheduler.addCronJob('20mins','0 0/20 * * * ?',method)
// add a job that runs every day at 23:30 between now and 5 days from now
var dateNow = new Date();
var date5Days = new Date(dateNow.getTime()+5*24*60*60*1000);
plugins.scheduler.addCronJob('23:30','0 30 23 ? * *',method,dateNow,date5Days)
```
### addCronJob(jobname, cronTimings, method, startDate)

Adds a cron job to the scheduler. A cron job must have at least one minute between each execution (otherwise it won't execute).

**Parameters**\
[String](../../JSLib/String.md) jobname  ;\
[String](../../JSLib/String.md) cronTimings  ;\
[Function](../../JSLib/Function.md) method  ;\
[Date](../../JSLib/Date.md) startDate  ;

**Returns**\
void 


**Sample**

```javascript
// see: http://www.quartz-scheduler.org/documentation/quartz-2.3.0/tutorials/tutorial-lesson-06.html for more info
// add a job that runs every 20 minutes after the hour (0,20,40)
plugins.scheduler.addCronJob('20mins','0 0/20 * * * ?',method)
// add a job that runs every day at 23:30 between now and 5 days from now
var dateNow = new Date();
var date5Days = new Date(dateNow.getTime()+5*24*60*60*1000);
plugins.scheduler.addCronJob('23:30','0 30 23 ? * *',method,dateNow,date5Days)
```
### addCronJob(jobname, cronTimings, method, startDate, endDate)

Adds a cron job to the scheduler. A cron job must have at least one minute between each execution (otherwise it won't execute).

**Parameters**\
[String](../../JSLib/String.md) jobname  ;\
[String](../../JSLib/String.md) cronTimings  ;\
[Function](../../JSLib/Function.md) method  ;\
[Date](../../JSLib/Date.md) startDate  ;\
[Date](../../JSLib/Date.md) endDate  ;

**Returns**\
void 


**Sample**

```javascript
// see: http://www.quartz-scheduler.org/documentation/quartz-2.3.0/tutorials/tutorial-lesson-06.html for more info
// add a job that runs every 20 minutes after the hour (0,20,40)
plugins.scheduler.addCronJob('20mins','0 0/20 * * * ?',method)
// add a job that runs every day at 23:30 between now and 5 days from now
var dateNow = new Date();
var date5Days = new Date(dateNow.getTime()+5*24*60*60*1000);
plugins.scheduler.addCronJob('23:30','0 30 23 ? * *',method,dateNow,date5Days)
```
### addCronJob(jobname, cronTimings, method, startDate, endDate, arguments)

Adds a cron job to the scheduler. A cron job must have at least one minute between each execution (otherwise it won't execute).

**Parameters**\
[String](../../JSLib/String.md) jobname  ;\
[String](../../JSLib/String.md) cronTimings  ;\
[Function](../../JSLib/Function.md) method  ;\
[Date](../../JSLib/Date.md) startDate  ;\
[Date](../../JSLib/Date.md) endDate  ;\
[Array](../../JSLib/Array.md) arguments  ;

**Returns**\
void 


**Sample**

```javascript
// see: http://www.quartz-scheduler.org/documentation/quartz-2.3.0/tutorials/tutorial-lesson-06.html for more info
// add a job that runs every 20 minutes after the hour (0,20,40)
plugins.scheduler.addCronJob('20mins','0 0/20 * * * ?',method)
// add a job that runs every day at 23:30 between now and 5 days from now
var dateNow = new Date();
var date5Days = new Date(dateNow.getTime()+5*24*60*60*1000);
plugins.scheduler.addCronJob('23:30','0 30 23 ? * *',method,dateNow,date5Days)
```
### addJob(jobname, startDate, method)

Adds a job to the scheduler.

**Parameters**\
[String](../../JSLib/String.md) jobname  ;\
[Date](../../JSLib/Date.md) startDate  ;\
[Function](../../JSLib/Function.md) method  ;

**Returns**\
void 


**Sample**

```javascript
// add a job that runs at the given date (20 seconds in the future)
// and repeats that every 20 seconds for 40 times or the enddate is reached (0 for no repeats = just one call)
var startDate = new Date();
startDate.setTime(startDate.getTime()+20000);
var endDate = new Date(startDate.getTime()+100000);
plugins.scheduler.addJob('in20seconds',startDate,method,20000,40,endDate)
```
### addJob(jobname, startDate, method, repeatInterval)

Adds a job to the scheduler.

**Parameters**\
[String](../../JSLib/String.md) jobname  ;\
[Date](../../JSLib/Date.md) startDate  ;\
[Function](../../JSLib/Function.md) method  ;\
[Number](../../JSLib/Number.md) repeatInterval ms

**Returns**\
void 


**Sample**

```javascript
// add a job that runs at the given date (20 seconds in the future)
// and repeats that every 20 seconds for 40 times or the enddate is reached (0 for no repeats = just one call)
var startDate = new Date();
startDate.setTime(startDate.getTime()+20000);
var endDate = new Date(startDate.getTime()+100000);
plugins.scheduler.addJob('in20seconds',startDate,method,20000,40,endDate)
```
### addJob(jobname, startDate, method, repeatInterval, repeatCount)

Adds a job to the scheduler.

**Parameters**\
[String](../../JSLib/String.md) jobname  ;\
[Date](../../JSLib/Date.md) startDate  ;\
[Function](../../JSLib/Function.md) method  ;\
[Number](../../JSLib/Number.md) repeatInterval ms\
[Number](../../JSLib/Number.md) repeatCount  ;

**Returns**\
void 


**Sample**

```javascript
// add a job that runs at the given date (20 seconds in the future)
// and repeats that every 20 seconds for 40 times or the enddate is reached (0 for no repeats = just one call)
var startDate = new Date();
startDate.setTime(startDate.getTime()+20000);
var endDate = new Date(startDate.getTime()+100000);
plugins.scheduler.addJob('in20seconds',startDate,method,20000,40,endDate)
```
### addJob(jobName, startDate, method, repeatInterval, repeatCount, endDate)

Adds a job to the scheduler.

**Parameters**\
[String](../../JSLib/String.md) jobName  ;\
[Date](../../JSLib/Date.md) startDate  ;\
[Function](../../JSLib/Function.md) method  ;\
[Number](../../JSLib/Number.md) repeatInterval ms\
[Number](../../JSLib/Number.md) repeatCount  ;\
[Date](../../JSLib/Date.md) endDate  ;

**Returns**\
void 


**Sample**

```javascript
// add a job that runs at the given date (20 seconds in the future)
// and repeats that every 20 seconds for 40 times or the enddate is reached (0 for no repeats = just one call)
var startDate = new Date();
startDate.setTime(startDate.getTime()+20000);
var endDate = new Date(startDate.getTime()+100000);
plugins.scheduler.addJob('in20seconds',startDate,method,20000,40,endDate)
```
### addJob(jobname, startDate, method, repeatInterval, repeatCount, endDate, arguments)

Adds a job to the scheduler.

**Parameters**\
[String](../../JSLib/String.md) jobname  ;\
[Date](../../JSLib/Date.md) startDate  ;\
[Function](../../JSLib/Function.md) method  ;\
[Number](../../JSLib/Number.md) repeatInterval ms\
[Number](../../JSLib/Number.md) repeatCount  ;\
[Date](../../JSLib/Date.md) endDate  ;\
[Array](../../JSLib/Array.md) arguments  ;

**Returns**\
void 


**Sample**

```javascript
// add a job that runs at the given date (20 seconds in the future)
// and repeats that every 20 seconds for 40 times or the enddate is reached (0 for no repeats = just one call)
var startDate = new Date();
startDate.setTime(startDate.getTime()+20000);
var endDate = new Date(startDate.getTime()+100000);
plugins.scheduler.addJob('in20seconds',startDate,method,20000,40,endDate)
```
### addJob(jobname, startDate, method, arguments)

Adds a job to the scheduler.

**Parameters**\
[String](../../JSLib/String.md) jobname  ;\
[Date](../../JSLib/Date.md) startDate  ;\
[Function](../../JSLib/Function.md) method  ;\
[Array](../../JSLib/Array.md) arguments  ;

**Returns**\
void 


**Sample**

```javascript
// add a job that runs at the given date (20 seconds in the future)
// and repeats that every 20 seconds for 40 times or the enddate is reached (0 for no repeats = just one call)
var startDate = new Date();
startDate.setTime(startDate.getTime()+20000);
var endDate = new Date(startDate.getTime()+100000);
plugins.scheduler.addJob('in20seconds',startDate,method,20000,40,endDate)
```
### getCurrentJobNames()

Returns an array with the current jobs.


**Returns**\
[Array](../../JSLib/Array.md) 


**Sample**

```javascript
plugins.scheduler.getCurrentJobNames()
```
### getLastRunJobName()

Returns the last job run from the scheduler.


**Returns**\
[String](../../JSLib/String.md) 


**Sample**

```javascript
plugins.scheduler.getLastRunJobName();
```
### removeJob(jobname)

Removes a job from the scheduler.

**Parameters**\
[String](../../JSLib/String.md) jobname  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
// removes a job 'myjob' from the scheduler
plugins.scheduler.removeJob('myjob');
```

