#  Date

## **Supported Clients**

    SmartClient
    WebClient
    NGClient
    MobileClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Number](./Number.md) | [UTC(year, month)](Date.md#utc-year-month)                   | Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time..                                    |
| [Number](./Number.md) | [UTC(year, month, date)](Date.md#utc-year-month-date)                   | Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time..                                    |
| [Number](./Number.md) | [UTC(year, month, date, hrs)](Date.md#utc-year-month-date-hrs)                   | Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time..                                    |
| [Number](./Number.md) | [UTC(year, month, date, hrs, min)](Date.md#utc-year-month-date-hrs-min)                   | Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time..                                    |
| [Number](./Number.md) | [UTC(year, month, date, hrs, min, sec)](Date.md#utc-year-month-date-hrs-min-sec)                   | Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time..                                    |
| [Number](./Number.md) | [UTC(year, month, date, hrs, min, sec, ms)](Date.md#utc-year-month-date-hrs-min-sec-ms)                   | Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time..                                    |
| [Number](./Number.md) | [getDate()](Date.md#getdate)                   | Gets the day of month in local time.                                    |
| [Number](./Number.md) | [getDay()](Date.md#getday)                   | Gets the day of the week (sunday = 0) in local time.                                    |
| [Number](./Number.md) | [getFullYear()](Date.md#getfullyear)                   | Gets the full year of the date in local time.                                    |
| [Number](./Number.md) | [getHours()](Date.md#gethours)                   | Gets the hours of the date in local time.                                    |
| [Number](./Number.md) | [getMilliseconds()](Date.md#getmilliseconds)                   | Gets the milliseconds of the date in local time.                                    |
| [Number](./Number.md) | [getMinutes()](Date.md#getminutes)                   | Gets the minutes of the date in local time.                                    |
| [Number](./Number.md) | [getMonth()](Date.md#getmonth)                   | Gets the month of the date in local time.                                    |
| [Number](./Number.md) | [getSeconds()](Date.md#getseconds)                   | Gets the seconds of the date in local time.                                    |
| [Number](./Number.md) | [getTime()](Date.md#gettime)                   | The value returned by the getTime method is the number of milliseconds since 1 January 1970 00:00:00..                                    |
| [Number](./Number.md) | [getTimezoneOffset()](Date.md#gettimezoneoffset)                   | Gets the number of minutes between GMT and this date..                                    |
| [Number](./Number.md) | [getUTCDate()](Date.md#getutcdate)                   | Gets the UTC date..                                    |
| [Number](./Number.md) | [getUTCDay()](Date.md#getutcday)                   | Gets the day in UTC time..                                    |
| [Number](./Number.md) | [getUTCFullYear()](Date.md#getutcfullyear)                   | Gets the full year in UTC time..                                    |
| [Number](./Number.md) | [getUTCHours()](Date.md#getutchours)                   | Gets the hours in UTC time..                                    |
| [Number](./Number.md) | [getUTCMilliseconds()](Date.md#getutcmilliseconds)                   | Gets the milliseconds in UTC time..                                    |
| [Number](./Number.md) | [getUTCMinutes()](Date.md#getutcminutes)                   | Gets the minutes in UTC time..                                    |
| [Number](./Number.md) | [getUTCMonth()](Date.md#getutcmonth)                   | Gets the month in UTC time..                                    |
| [Number](./Number.md) | [getUTCSeconds()](Date.md#getutcseconds)                   | Gets the seconds in UTC time..                                    |
| [Number](./Number.md) | [now()](Date.md#now)                   | Returns the milliseconds elapsed since 1 January 1970 00:00:00 UTC up until now..                                    |
| [Number](./Number.md) | [parse(s)](Date.md#parse-s)                   | Takes a date string (such as "Dec 25, 1995") and returns the number of milliseconds since January 1, 1970, 00:00:00 UTC..                                    |
|void | [setDate(dayValue)](Date.md#setdate-dayvalue)                   | Sets the date..                                    |
|void | [setFullYear(yearValue)](Date.md#setfullyear-yearvalue)                   | Sets the full year of the date..                                    |
|void | [setFullYear(yearValue, monthValue)](Date.md#setfullyear-yearvalue-monthvalue)                   | Sets the full year of the date..                                    |
|void | [setFullYear(yearValue, monthValue, dayValue)](Date.md#setfullyear-yearvalue-monthvalue-dayvalue)                   | Sets the full year of the date..                                    |
|void | [setHours(hoursValue)](Date.md#sethours-hoursvalue)                   | Sets the hours of the date..                                    |
|void | [setHours(hoursValue, minutesValue)](Date.md#sethours-hoursvalue-minutesvalue)                   | Sets the hours of the date..                                    |
|void | [setHours(hoursValue, minutesValue, secondsValue)](Date.md#sethours-hoursvalue-minutesvalue-secondsvalue)                   | Sets the hours of the date..                                    |
|void | [setHours(hoursValue, minutesValue, secondsValue, msValue)](Date.md#sethours-hoursvalue-minutesvalue-secondsvalue-msvalue)                   | Sets the hours of the date..                                    |
|void | [setMilliseconds(millisecondsValue)](Date.md#setmilliseconds-millisecondsvalue)                   | Sets the milliseconds of the date..                                    |
|void | [setMinutes(minutesValue)](Date.md#setminutes-minutesvalue)                   | Sets the minutes of the date..                                    |
|void | [setMinutes(minutesValue, secondsValue)](Date.md#setminutes-minutesvalue-secondsvalue)                   | Sets the minutes of the date..                                    |
|void | [setMinutes(minutesValue, secondsValue, msValue)](Date.md#setminutes-minutesvalue-secondsvalue-msvalue)                   | Sets the minutes of the date..                                    |
|void | [setMonth(monthValue)](Date.md#setmonth-monthvalue)                   | Sets the month of the date..                                    |
|void | [setMonth(monthValue, dayValue)](Date.md#setmonth-monthvalue-dayvalue)                   | Sets the month of the date..                                    |
|void | [setSeconds(secondsValue)](Date.md#setseconds-secondsvalue)                   | Sets the seconds of the date..                                    |
|void | [setSeconds(secondsValue, msValue)](Date.md#setseconds-secondsvalue-msvalue)                   | Sets the seconds of the date..                                    |
|void | [setTime(timeValue)](Date.md#settime-timevalue)                   | Sets the milliseconds of the date..                                    |
|void | [setUTCDate(dayValue)](Date.md#setutcdate-dayvalue)                   | Sets the UTC date..                                    |
|void | [setUTCFullYear(yearValue)](Date.md#setutcfullyear-yearvalue)                   | Sets the year in UTC time..                                    |
|void | [setUTCFullYear(yearValue, monthValue)](Date.md#setutcfullyear-yearvalue-monthvalue)                   | Sets the year in UTC time..                                    |
|void | [setUTCFullYear(yearValue, monthValue, dayValue)](Date.md#setutcfullyear-yearvalue-monthvalue-dayvalue)                   | Sets the year in UTC time..                                    |
|void | [setUTCHours(hoursValue)](Date.md#setutchours-hoursvalue)                   | Sets the hours in UTC time..                                    |
|void | [setUTCHours(hoursValue, minutesValue)](Date.md#setutchours-hoursvalue-minutesvalue)                   | Sets the hours in UTC time..                                    |
|void | [setUTCHours(hoursValue, minutesValue, secondsValue)](Date.md#setutchours-hoursvalue-minutesvalue-secondsvalue)                   | Sets the hours in UTC time..                                    |
|void | [setUTCHours(hoursValue, minutesValue, secondsValue, msValue)](Date.md#setutchours-hoursvalue-minutesvalue-secondsvalue-msvalue)                   | Sets the hours in UTC time..                                    |
|void | [setUTCMilliseconds(millisecondsValue)](Date.md#setutcmilliseconds-millisecondsvalue)                   | Sets the milliseconds in UTC time..                                    |
|void | [setUTCMinutes(minutesValue)](Date.md#setutcminutes-minutesvalue)                   | Sets the minutes in UTC time..                                    |
|void | [setUTCMinutes(minutesValue, secondsValue)](Date.md#setutcminutes-minutesvalue-secondsvalue)                   | Sets the minutes in UTC time..                                    |
|void | [setUTCMinutes(minutesValue, secondsValue, msValue)](Date.md#setutcminutes-minutesvalue-secondsvalue-msvalue)                   | Sets the minutes in UTC time..                                    |
|void | [setUTCMonth(monthValue)](Date.md#setutcmonth-monthvalue)                   | Sets the month in UTC time..                                    |
|void | [setUTCMonth(monthValue, dayValue)](Date.md#setutcmonth-monthvalue-dayvalue)                   | Sets the month in UTC time..                                    |
|void | [setUTCSeconds(secondsValue)](Date.md#setutcseconds-secondsvalue)                   | Sets the seconds in UTC time..                                    |
|void | [setUTCSeconds(secondsValue, msValue)](Date.md#setutcseconds-secondsvalue-msvalue)                   | Sets the seconds in UTC time..                                    |
| [String](./String.md) | [toDateString()](Date.md#todatestring)                   | Returns a string version of the date..                                    |
| [String](./String.md) | [toISOString()](Date.md#toisostring)                   | Returns a string version of the UTC value of the date..                                    |
| [String](./String.md) | [toLocaleDateString()](Date.md#tolocaledatestring)                   | Returns a string version of the local time zone of the date..                                    |
| [String](./String.md) | [toLocaleString()](Date.md#tolocalestring)                   | Returns a string version of the local time zone of the date..                                    |
| [String](./String.md) | [toLocaleTimeString()](Date.md#tolocaletimestring)                   | Returns a string version of the local time zone of the date..                                    |
| [String](./String.md) | [toTimeString()](Date.md#totimestring)                   | Returns a string version of the date..                                    |
| [String](./String.md) | [toUTCString()](Date.md#toutcstring)                   | Returns a string version of the UTC value of the date..                                    |
| [Number](./Number.md) | [valueOf()](Date.md#valueof)                   | Return integer milliseconds count.                                    |

## Methods Details

### UTC(year, month)

Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.

**Parameters**\
[Number](./Number.md) year A year after 1900.\
[Number](./Number.md) month A number between 0 and 11.

**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
// The number of milliseconds in the first minute after 1970 January 1st.
application.output(Date.UTC(1970, 00, 01, 00, 01, 00, 00)); // prints: 60000.0
```
### UTC(year, month, date)

Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.

**Parameters**\
[Number](./Number.md) year A year after 1900.\
[Number](./Number.md) month A number between 0 and 11.\
[Number](./Number.md) date A number between 1 and 31.

**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
// The number of milliseconds in the first minute after 1970 January 1st.
application.output(Date.UTC(1970, 00, 01, 00, 01, 00, 00)); // prints: 60000.0
```
### UTC(year, month, date, hrs)

Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.

**Parameters**\
[Number](./Number.md) year A year after 1900.\
[Number](./Number.md) month A number between 0 and 11.\
[Number](./Number.md) date A number between 1 and 31.\
[Number](./Number.md) hrs A number between 0 and 23.

**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
// The number of milliseconds in the first minute after 1970 January 1st.
application.output(Date.UTC(1970, 00, 01, 00, 01, 00, 00)); // prints: 60000.0
```
### UTC(year, month, date, hrs, min)

Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.

**Parameters**\
[Number](./Number.md) year A year after 1900.\
[Number](./Number.md) month A number between 0 and 11.\
[Number](./Number.md) date A number between 1 and 31.\
[Number](./Number.md) hrs A number between 0 and 23.\
[Number](./Number.md) min A number between 0 and 59.

**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
// The number of milliseconds in the first minute after 1970 January 1st.
application.output(Date.UTC(1970, 00, 01, 00, 01, 00, 00)); // prints: 60000.0
```
### UTC(year, month, date, hrs, min, sec)

Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.

**Parameters**\
[Number](./Number.md) year A year after 1900.\
[Number](./Number.md) month A number between 0 and 11.\
[Number](./Number.md) date A number between 1 and 31.\
[Number](./Number.md) hrs A number between 0 and 23.\
[Number](./Number.md) min A number between 0 and 59.\
[Number](./Number.md) sec A number between 0 and 59.

**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
// The number of milliseconds in the first minute after 1970 January 1st.
application.output(Date.UTC(1970, 00, 01, 00, 01, 00, 00)); // prints: 60000.0
```
### UTC(year, month, date, hrs, min, sec, ms)

Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.

**Parameters**\
[Number](./Number.md) year A year after 1900.\
[Number](./Number.md) month A number between 0 and 11.\
[Number](./Number.md) date A number between 1 and 31.\
[Number](./Number.md) hrs A number between 0 and 23.\
[Number](./Number.md) min A number between 0 and 59.\
[Number](./Number.md) sec A number between 0 and 59.\
[Number](./Number.md) ms A number between 0 and 999.

**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
// The number of milliseconds in the first minute after 1970 January 1st.
application.output(Date.UTC(1970, 00, 01, 00, 01, 00, 00)); // prints: 60000.0
```
### getDate()

Gets the day of month in local time


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getDate();
```
### getDay()

Gets the day of the week (sunday = 0) in local time


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getDay();
```
### getFullYear()

Gets the full year of the date in local time


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getFullYear();
```
### getHours()

Gets the hours of the date in local time


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getHours();
```
### getMilliseconds()

Gets the milliseconds of the date in local time


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getMilliseconds();
```
### getMinutes()

Gets the minutes of the date in local time


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getMinutes();
```
### getMonth()

Gets the month of the date in local time


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getMonth();
```
### getSeconds()

Gets the seconds of the date in local time


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getSeconds();
```
### getTime()

The value returned by the getTime method is the number of milliseconds since 1 January 1970 00:00:00.


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getTime();
```
### getTimezoneOffset()

Gets the number of minutes between GMT and this date.


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getTimezoneOffset();
```
### getUTCDate()

Gets the UTC date.


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getUTCDate();
```
### getUTCDay()

Gets the day in UTC time.


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getUTCDay();
```
### getUTCFullYear()

Gets the full year in UTC time.


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getUTCFullYear();
```
### getUTCHours()

Gets the hours in UTC time.


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getUTCHours();
```
### getUTCMilliseconds()

Gets the milliseconds in UTC time.


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getUTCMilliseconds();
```
### getUTCMinutes()

Gets the minutes in UTC time.


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getUTCMinutes();
```
### getUTCMonth()

Gets the month in UTC time.


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getUTCMonth();
```
### getUTCSeconds()

Gets the seconds in UTC time.


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.getUTCSeconds();
```
### now()

Returns the milliseconds elapsed since 1 January 1970 00:00:00 UTC up until now.


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var timestamp = Date.now();
```
### parse(s)

Takes a date string (such as "Dec 25, 1995") and returns the number of milliseconds since January 1, 1970, 00:00:00 UTC.

**Parameters**\
[String](./String.md) s The date string to parse

**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var str = Date.parse("Wed, 09 Aug 1995 00:00:00 GMT");
application.output(str);
```
### setDate(dayValue)

Sets the date.

**Parameters**\
[Number](./Number.md) dayValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setDate(integer);
```
### setFullYear(yearValue)

Sets the full year of the date.

**Parameters**\
[Number](./Number.md) yearValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setFullYear(integer);
```
### setFullYear(yearValue, monthValue)

Sets the full year of the date.

**Parameters**\
[Number](./Number.md) yearValue  ;\
[Number](./Number.md) monthValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setFullYear(integer);
```
### setFullYear(yearValue, monthValue, dayValue)

Sets the full year of the date.

**Parameters**\
[Number](./Number.md) yearValue  ;\
[Number](./Number.md) monthValue  ;\
[Number](./Number.md) dayValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setFullYear(integer);
```
### setHours(hoursValue)

Sets the hours of the date.

**Parameters**\
[Number](./Number.md) hoursValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setHours(integer);
```
### setHours(hoursValue, minutesValue)

Sets the hours of the date.

**Parameters**\
[Number](./Number.md) hoursValue  ;\
[Number](./Number.md) minutesValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setHours(integer);
```
### setHours(hoursValue, minutesValue, secondsValue)

Sets the hours of the date.

**Parameters**\
[Number](./Number.md) hoursValue  ;\
[Number](./Number.md) minutesValue  ;\
[Number](./Number.md) secondsValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setHours(integer);
```
### setHours(hoursValue, minutesValue, secondsValue, msValue)

Sets the hours of the date.

**Parameters**\
[Number](./Number.md) hoursValue  ;\
[Number](./Number.md) minutesValue  ;\
[Number](./Number.md) secondsValue  ;\
[Number](./Number.md) msValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setHours(integer);
```
### setMilliseconds(millisecondsValue)

Sets the milliseconds of the date.

**Parameters**\
[Number](./Number.md) millisecondsValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setMilliseconds(integer);
```
### setMinutes(minutesValue)

Sets the minutes of the date.

**Parameters**\
[Number](./Number.md) minutesValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setMinutes(integer);
```
### setMinutes(minutesValue, secondsValue)

Sets the minutes of the date.

**Parameters**\
[Number](./Number.md) minutesValue  ;\
[Number](./Number.md) secondsValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setMinutes(integer);
```
### setMinutes(minutesValue, secondsValue, msValue)

Sets the minutes of the date.

**Parameters**\
[Number](./Number.md) minutesValue  ;\
[Number](./Number.md) secondsValue  ;\
[Number](./Number.md) msValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setMinutes(integer);
```
### setMonth(monthValue)

Sets the month of the date.

**Parameters**\
[Number](./Number.md) monthValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setMonth(integr);
```
### setMonth(monthValue, dayValue)

Sets the month of the date.

**Parameters**\
[Number](./Number.md) monthValue  ;\
[Number](./Number.md) dayValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setMonth(integr);
```
### setSeconds(secondsValue)

Sets the seconds of the date.

**Parameters**\
[Number](./Number.md) secondsValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setSeconds(integer);
```
### setSeconds(secondsValue, msValue)

Sets the seconds of the date.

**Parameters**\
[Number](./Number.md) secondsValue  ;\
[Number](./Number.md) msValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setSeconds(integer);
```
### setTime(timeValue)

Sets the milliseconds of the date.

**Parameters**\
[Number](./Number.md) timeValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setTime(integer);
```
### setUTCDate(dayValue)

Sets the UTC date.

**Parameters**\
[Number](./Number.md) dayValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setUTCDate(integer);
```
### setUTCFullYear(yearValue)

Sets the year in UTC time.

**Parameters**\
[Number](./Number.md) yearValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setUTCFullYear(integer);
```
### setUTCFullYear(yearValue, monthValue)

Sets the year in UTC time.

**Parameters**\
[Number](./Number.md) yearValue  ;\
[Number](./Number.md) monthValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setUTCFullYear(integer);
```
### setUTCFullYear(yearValue, monthValue, dayValue)

Sets the year in UTC time.

**Parameters**\
[Number](./Number.md) yearValue  ;\
[Number](./Number.md) monthValue  ;\
[Number](./Number.md) dayValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setUTCFullYear(integer);
```
### setUTCHours(hoursValue)

Sets the hours in UTC time.

**Parameters**\
[Number](./Number.md) hoursValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setUTCHours(integer);
```
### setUTCHours(hoursValue, minutesValue)

Sets the hours in UTC time.

**Parameters**\
[Number](./Number.md) hoursValue  ;\
[Number](./Number.md) minutesValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setUTCHours(integer);
```
### setUTCHours(hoursValue, minutesValue, secondsValue)

Sets the hours in UTC time.

**Parameters**\
[Number](./Number.md) hoursValue  ;\
[Number](./Number.md) minutesValue  ;\
[Number](./Number.md) secondsValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setUTCHours(integer);
```
### setUTCHours(hoursValue, minutesValue, secondsValue, msValue)

Sets the hours in UTC time.

**Parameters**\
[Number](./Number.md) hoursValue  ;\
[Number](./Number.md) minutesValue  ;\
[Number](./Number.md) secondsValue  ;\
[Number](./Number.md) msValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setUTCHours(integer);
```
### setUTCMilliseconds(millisecondsValue)

Sets the milliseconds in UTC time.

**Parameters**\
[Number](./Number.md) millisecondsValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setUTCMilliseconds(integer);
```
### setUTCMinutes(minutesValue)

Sets the minutes in UTC time.

**Parameters**\
[Number](./Number.md) minutesValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setUTCMinutes(integer);
```
### setUTCMinutes(minutesValue, secondsValue)

Sets the minutes in UTC time.

**Parameters**\
[Number](./Number.md) minutesValue  ;\
[Number](./Number.md) secondsValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setUTCMinutes(integer);
```
### setUTCMinutes(minutesValue, secondsValue, msValue)

Sets the minutes in UTC time.

**Parameters**\
[Number](./Number.md) minutesValue  ;\
[Number](./Number.md) secondsValue  ;\
[Number](./Number.md) msValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setUTCMinutes(integer);
```
### setUTCMonth(monthValue)

Sets the month in UTC time.

**Parameters**\
[Number](./Number.md) monthValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setUTCMonth(integer);
```
### setUTCMonth(monthValue, dayValue)

Sets the month in UTC time.

**Parameters**\
[Number](./Number.md) monthValue  ;\
[Number](./Number.md) dayValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setUTCMonth(integer);
```
### setUTCSeconds(secondsValue)

Sets the seconds in UTC time.

**Parameters**\
[Number](./Number.md) secondsValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setUTCSeconds(integer);
```
### setUTCSeconds(secondsValue, msValue)

Sets the seconds in UTC time.

**Parameters**\
[Number](./Number.md) secondsValue  ;\
[Number](./Number.md) msValue  ;

**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.setUTCSeconds(integer);
```
### toDateString()

Returns a string version of the date.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.toDateString();
```
### toISOString()

Returns a string version of the UTC value of the date.


**Returns**\
[String](./String.md) the Date object as a string in simplified extended ISO format.

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.toISOString();
```
### toLocaleDateString()

Returns a string version of the local time zone of the date.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.toLocaleDateString();
```
### toLocaleString()

Returns a string version of the local time zone of the date.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.toLocaleString();
```
### toLocaleTimeString()

Returns a string version of the local time zone of the date.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.toLocaleTimeString();
```
### toTimeString()

Returns a string version of the date.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.toTimeString();
```
### toUTCString()

Returns a string version of the UTC value of the date.


**Returns**\
[String](./String.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.toUTCString();
```
### valueOf()

Return integer milliseconds count


**Returns**\
[Number](./Number.md) 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
date.valueOf(integer);
```

