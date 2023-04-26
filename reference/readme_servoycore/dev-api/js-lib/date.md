# Date

## Methods Summary

| Type                | Name                                                                                                                             | Summary                                                                                                                                                 |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Number](number.md) | [UTC(year, month)](date.md#utc-year-month)                                                                                       | Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.. |
| [Number](number.md) | [UTC(year, month, date)](date.md#utc-year-month-date)                                                                            | Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.. |
| [Number](number.md) | [UTC(year, month, date, hrs)](date.md#utc-year-month-date-hrs)                                                                   | Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.. |
| [Number](number.md) | [UTC(year, month, date, hrs, min)](date.md#utc-year-month-date-hrs-min)                                                          | Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.. |
| [Number](number.md) | [UTC(year, month, date, hrs, min, sec)](date.md#utc-year-month-date-hrs-min-sec)                                                 | Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.. |
| [Number](number.md) | [UTC(year, month, date, hrs, min, sec, ms)](date.md#utc-year-month-date-hrs-min-sec-ms)                                          | Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.. |
| [Number](number.md) | [getDate()](date.md#getdate)                                                                                                     | Gets the day of month in local time.                                                                                                                    |
| [Number](number.md) | [getDay()](date.md#getday)                                                                                                       | Gets the day of the week (sunday = 0) in local time.                                                                                                    |
| [Number](number.md) | [getFullYear()](date.md#getfullyear)                                                                                             | Gets the full year of the date in local time.                                                                                                           |
| [Number](number.md) | [getHours()](date.md#gethours)                                                                                                   | Gets the hours of the date in local time.                                                                                                               |
| [Number](number.md) | [getMilliseconds()](date.md#getmilliseconds)                                                                                     | Gets the milliseconds of the date in local time.                                                                                                        |
| [Number](number.md) | [getMinutes()](date.md#getminutes)                                                                                               | Gets the minutes of the date in local time.                                                                                                             |
| [Number](number.md) | [getMonth()](date.md#getmonth)                                                                                                   | Gets the month of the date in local time.                                                                                                               |
| [Number](number.md) | [getSeconds()](date.md#getseconds)                                                                                               | Gets the seconds of the date in local time.                                                                                                             |
| [Number](number.md) | [getTime()](date.md#gettime)                                                                                                     | The value returned by the getTime method is the number of milliseconds since 1 January 1970 00:00:00..                                                  |
| [Number](number.md) | [getTimezoneOffset()](date.md#gettimezoneoffset)                                                                                 | Gets the number of minutes between GMT and this date..                                                                                                  |
| [Number](number.md) | [getUTCDate()](date.md#getutcdate)                                                                                               | Gets the UTC date..                                                                                                                                     |
| [Number](number.md) | [getUTCDay()](date.md#getutcday)                                                                                                 | Gets the day in UTC time..                                                                                                                              |
| [Number](number.md) | [getUTCFullYear()](date.md#getutcfullyear)                                                                                       | Gets the full year in UTC time..                                                                                                                        |
| [Number](number.md) | [getUTCHours()](date.md#getutchours)                                                                                             | Gets the hours in UTC time..                                                                                                                            |
| [Number](number.md) | [getUTCMilliseconds()](date.md#getutcmilliseconds)                                                                               | Gets the milliseconds in UTC time..                                                                                                                     |
| [Number](number.md) | [getUTCMinutes()](date.md#getutcminutes)                                                                                         | Gets the minutes in UTC time..                                                                                                                          |
| [Number](number.md) | [getUTCMonth()](date.md#getutcmonth)                                                                                             | Gets the month in UTC time..                                                                                                                            |
| [Number](number.md) | [getUTCSeconds()](date.md#getutcseconds)                                                                                         | Gets the seconds in UTC time..                                                                                                                          |
| [Number](number.md) | [now()](date.md#now)                                                                                                             | Returns the milliseconds elapsed since 1 January 1970 00:00:00 UTC up until now..                                                                       |
| [Number](number.md) | [parse(s)](date.md#parse-s)                                                                                                      | Takes a date string (such as "Dec 25, 1995") and returns the number of milliseconds since January 1, 1970, 00:00:00 UTC..                               |
| void                | [setDate(dayValue)](date.md#setdate-dayvalue)                                                                                    | Sets the date..                                                                                                                                         |
| void                | [setFullYear(yearValue)](date.md#setfullyear-yearvalue)                                                                          | Sets the full year of the date..                                                                                                                        |
| void                | [setFullYear(yearValue, monthValue)](date.md#setfullyear-yearvalue-monthvalue)                                                   | Sets the full year of the date..                                                                                                                        |
| void                | [setFullYear(yearValue, monthValue, dayValue)](date.md#setfullyear-yearvalue-monthvalue-dayvalue)                                | Sets the full year of the date..                                                                                                                        |
| void                | [setHours(hoursValue)](date.md#sethours-hoursvalue)                                                                              | Sets the hours of the date..                                                                                                                            |
| void                | [setHours(hoursValue, minutesValue)](date.md#sethours-hoursvalue-minutesvalue)                                                   | Sets the hours of the date..                                                                                                                            |
| void                | [setHours(hoursValue, minutesValue, secondsValue)](date.md#sethours-hoursvalue-minutesvalue-secondsvalue)                        | Sets the hours of the date..                                                                                                                            |
| void                | [setHours(hoursValue, minutesValue, secondsValue, msValue)](date.md#sethours-hoursvalue-minutesvalue-secondsvalue-msvalue)       | Sets the hours of the date..                                                                                                                            |
| void                | [setMilliseconds(millisecondsValue)](date.md#setmilliseconds-millisecondsvalue)                                                  | Sets the milliseconds of the date..                                                                                                                     |
| void                | [setMinutes(minutesValue)](date.md#setminutes-minutesvalue)                                                                      | Sets the minutes of the date..                                                                                                                          |
| void                | [setMinutes(minutesValue, secondsValue)](date.md#setminutes-minutesvalue-secondsvalue)                                           | Sets the minutes of the date..                                                                                                                          |
| void                | [setMinutes(minutesValue, secondsValue, msValue)](date.md#setminutes-minutesvalue-secondsvalue-msvalue)                          | Sets the minutes of the date..                                                                                                                          |
| void                | [setMonth(monthValue)](date.md#setmonth-monthvalue)                                                                              | Sets the month of the date..                                                                                                                            |
| void                | [setMonth(monthValue, dayValue)](date.md#setmonth-monthvalue-dayvalue)                                                           | Sets the month of the date..                                                                                                                            |
| void                | [setSeconds(secondsValue)](date.md#setseconds-secondsvalue)                                                                      | Sets the seconds of the date..                                                                                                                          |
| void                | [setSeconds(secondsValue, msValue)](date.md#setseconds-secondsvalue-msvalue)                                                     | Sets the seconds of the date..                                                                                                                          |
| void                | [setTime(timeValue)](date.md#settime-timevalue)                                                                                  | Sets the milliseconds of the date..                                                                                                                     |
| void                | [setUTCDate(dayValue)](date.md#setutcdate-dayvalue)                                                                              | Sets the UTC date..                                                                                                                                     |
| void                | [setUTCFullYear(yearValue)](date.md#setutcfullyear-yearvalue)                                                                    | Sets the year in UTC time..                                                                                                                             |
| void                | [setUTCFullYear(yearValue, monthValue)](date.md#setutcfullyear-yearvalue-monthvalue)                                             | Sets the year in UTC time..                                                                                                                             |
| void                | [setUTCFullYear(yearValue, monthValue, dayValue)](date.md#setutcfullyear-yearvalue-monthvalue-dayvalue)                          | Sets the year in UTC time..                                                                                                                             |
| void                | [setUTCHours(hoursValue)](date.md#setutchours-hoursvalue)                                                                        | Sets the hours in UTC time..                                                                                                                            |
| void                | [setUTCHours(hoursValue, minutesValue)](date.md#setutchours-hoursvalue-minutesvalue)                                             | Sets the hours in UTC time..                                                                                                                            |
| void                | [setUTCHours(hoursValue, minutesValue, secondsValue)](date.md#setutchours-hoursvalue-minutesvalue-secondsvalue)                  | Sets the hours in UTC time..                                                                                                                            |
| void                | [setUTCHours(hoursValue, minutesValue, secondsValue, msValue)](date.md#setutchours-hoursvalue-minutesvalue-secondsvalue-msvalue) | Sets the hours in UTC time..                                                                                                                            |
| void                | [setUTCMilliseconds(millisecondsValue)](date.md#setutcmilliseconds-millisecondsvalue)                                            | Sets the milliseconds in UTC time..                                                                                                                     |
| void                | [setUTCMinutes(minutesValue)](date.md#setutcminutes-minutesvalue)                                                                | Sets the minutes in UTC time..                                                                                                                          |
| void                | [setUTCMinutes(minutesValue, secondsValue)](date.md#setutcminutes-minutesvalue-secondsvalue)                                     | Sets the minutes in UTC time..                                                                                                                          |
| void                | [setUTCMinutes(minutesValue, secondsValue, msValue)](date.md#setutcminutes-minutesvalue-secondsvalue-msvalue)                    | Sets the minutes in UTC time..                                                                                                                          |
| void                | [setUTCMonth(monthValue)](date.md#setutcmonth-monthvalue)                                                                        | Sets the month in UTC time..                                                                                                                            |
| void                | [setUTCMonth(monthValue, dayValue)](date.md#setutcmonth-monthvalue-dayvalue)                                                     | Sets the month in UTC time..                                                                                                                            |
| void                | [setUTCSeconds(secondsValue)](date.md#setutcseconds-secondsvalue)                                                                | Sets the seconds in UTC time..                                                                                                                          |
| void                | [setUTCSeconds(secondsValue, msValue)](date.md#setutcseconds-secondsvalue-msvalue)                                               | Sets the seconds in UTC time..                                                                                                                          |
| [String](string.md) | [toDateString()](date.md#todatestring)                                                                                           | Returns a string version of the date..                                                                                                                  |
| [String](string.md) | [toISOString()](date.md#toisostring)                                                                                             | Returns a string version of the UTC value of the date..                                                                                                 |
| [String](string.md) | [toLocaleDateString()](date.md#tolocaledatestring)                                                                               | Returns a string version of the local time zone of the date..                                                                                           |
| [String](string.md) | [toLocaleString()](date.md#tolocalestring)                                                                                       | Returns a string version of the local time zone of the date..                                                                                           |
| [String](string.md) | [toLocaleTimeString()](date.md#tolocaletimestring)                                                                               | Returns a string version of the local time zone of the date..                                                                                           |
| [String](string.md) | [toTimeString()](date.md#totimestring)                                                                                           | Returns a string version of the date..                                                                                                                  |
| [String](string.md) | [toUTCString()](date.md#toutcstring)                                                                                             | Returns a string version of the UTC value of the date..                                                                                                 |
| [Number](number.md) | [valueOf()](date.md#valueof)                                                                                                     | Return integer milliseconds count.                                                                                                                      |

## Methods Details

### UTC(year, month)

Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.

**Parameters**\
[Number](number.md) year A year after 1900.\
[Number](number.md) month A number between 0 and 11.

**Returns**\
[Number](number.md)

**Sample**

```javascript
// The number of milliseconds in the first minute after 1970 January 1st.
application.output(Date.UTC(1970, 00, 01, 00, 01, 00, 00)); // prints: 60000.0
```

### UTC(year, month, date)

Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.

**Parameters**\
[Number](number.md) year A year after 1900.\
[Number](number.md) month A number between 0 and 11.\
[Number](number.md) date A number between 1 and 31.

**Returns**\
[Number](number.md)

**Sample**

```javascript
// The number of milliseconds in the first minute after 1970 January 1st.
application.output(Date.UTC(1970, 00, 01, 00, 01, 00, 00)); // prints: 60000.0
```

### UTC(year, month, date, hrs)

Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.

**Parameters**\
[Number](number.md) year A year after 1900.\
[Number](number.md) month A number between 0 and 11.\
[Number](number.md) date A number between 1 and 31.\
[Number](number.md) hrs A number between 0 and 23.

**Returns**\
[Number](number.md)

**Sample**

```javascript
// The number of milliseconds in the first minute after 1970 January 1st.
application.output(Date.UTC(1970, 00, 01, 00, 01, 00, 00)); // prints: 60000.0
```

### UTC(year, month, date, hrs, min)

Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.

**Parameters**\
[Number](number.md) year A year after 1900.\
[Number](number.md) month A number between 0 and 11.\
[Number](number.md) date A number between 1 and 31.\
[Number](number.md) hrs A number between 0 and 23.\
[Number](number.md) min A number between 0 and 59.

**Returns**\
[Number](number.md)

**Sample**

```javascript
// The number of milliseconds in the first minute after 1970 January 1st.
application.output(Date.UTC(1970, 00, 01, 00, 01, 00, 00)); // prints: 60000.0
```

### UTC(year, month, date, hrs, min, sec)

Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.

**Parameters**\
[Number](number.md) year A year after 1900.\
[Number](number.md) month A number between 0 and 11.\
[Number](number.md) date A number between 1 and 31.\
[Number](number.md) hrs A number between 0 and 23.\
[Number](number.md) min A number between 0 and 59.\
[Number](number.md) sec A number between 0 and 59.

**Returns**\
[Number](number.md)

**Sample**

```javascript
// The number of milliseconds in the first minute after 1970 January 1st.
application.output(Date.UTC(1970, 00, 01, 00, 01, 00, 00)); // prints: 60000.0
```

### UTC(year, month, date, hrs, min, sec, ms)

Takes comma-delimited date parameters and returns the number of milliseconds between January 1, 1970, 00:00:00, universal time and the specified time.

**Parameters**\
[Number](number.md) year A year after 1900.\
[Number](number.md) month A number between 0 and 11.\
[Number](number.md) date A number between 1 and 31.\
[Number](number.md) hrs A number between 0 and 23.\
[Number](number.md) min A number between 0 and 59.\
[Number](number.md) sec A number between 0 and 59.\
[Number](number.md) ms A number between 0 and 999.

**Returns**\
[Number](number.md)

**Sample**

```javascript
// The number of milliseconds in the first minute after 1970 January 1st.
application.output(Date.UTC(1970, 00, 01, 00, 01, 00, 00)); // prints: 60000.0
```

### getDate()

Gets the day of month in local time

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getDate();
```

### getDay()

Gets the day of the week (sunday = 0) in local time

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getDay();
```

### getFullYear()

Gets the full year of the date in local time

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getFullYear();
```

### getHours()

Gets the hours of the date in local time

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getHours();
```

### getMilliseconds()

Gets the milliseconds of the date in local time

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getMilliseconds();
```

### getMinutes()

Gets the minutes of the date in local time

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getMinutes();
```

### getMonth()

Gets the month of the date in local time

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getMonth();
```

### getSeconds()

Gets the seconds of the date in local time

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getSeconds();
```

### getTime()

The value returned by the getTime method is the number of milliseconds since 1 January 1970 00:00:00.

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getTime();
```

### getTimezoneOffset()

Gets the number of minutes between GMT and this date.

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getTimezoneOffset();
```

### getUTCDate()

Gets the UTC date.

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getUTCDate();
```

### getUTCDay()

Gets the day in UTC time.

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getUTCDay();
```

### getUTCFullYear()

Gets the full year in UTC time.

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getUTCFullYear();
```

### getUTCHours()

Gets the hours in UTC time.

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getUTCHours();
```

### getUTCMilliseconds()

Gets the milliseconds in UTC time.

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getUTCMilliseconds();
```

### getUTCMinutes()

Gets the minutes in UTC time.

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getUTCMinutes();
```

### getUTCMonth()

Gets the month in UTC time.

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getUTCMonth();
```

### getUTCSeconds()

Gets the seconds in UTC time.

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.getUTCSeconds();
```

### now()

Returns the milliseconds elapsed since 1 January 1970 00:00:00 UTC up until now.

**Returns**\
[Number](number.md)

**Sample**

```javascript
var timestamp = Date.now();
```

### parse(s)

Takes a date string (such as "Dec 25, 1995") and returns the number of milliseconds since January 1, 1970, 00:00:00 UTC.

**Parameters**\
[String](string.md) s The date string to parse

**Returns**\
[Number](number.md)

**Sample**

```javascript
var str = Date.parse("Wed, 09 Aug 1995 00:00:00 GMT");
application.output(str);
```

### setDate(dayValue)

Sets the date.

**Parameters**\
[Number](number.md) dayValue ;

**Returns**\
void

**Sample**

```javascript
date.setDate(integer);
```

### setFullYear(yearValue)

Sets the full year of the date.

**Parameters**\
[Number](number.md) yearValue ;

**Returns**\
void

**Sample**

```javascript
date.setFullYear(integer);
```

### setFullYear(yearValue, monthValue)

Sets the full year of the date.

**Parameters**\
[Number](number.md) yearValue ;\
[Number](number.md) monthValue ;

**Returns**\
void

**Sample**

```javascript
date.setFullYear(integer);
```

### setFullYear(yearValue, monthValue, dayValue)

Sets the full year of the date.

**Parameters**\
[Number](number.md) yearValue ;\
[Number](number.md) monthValue ;\
[Number](number.md) dayValue ;

**Returns**\
void

**Sample**

```javascript
date.setFullYear(integer);
```

### setHours(hoursValue)

Sets the hours of the date.

**Parameters**\
[Number](number.md) hoursValue ;

**Returns**\
void

**Sample**

```javascript
date.setHours(integer);
```

### setHours(hoursValue, minutesValue)

Sets the hours of the date.

**Parameters**\
[Number](number.md) hoursValue ;\
[Number](number.md) minutesValue ;

**Returns**\
void

**Sample**

```javascript
date.setHours(integer);
```

### setHours(hoursValue, minutesValue, secondsValue)

Sets the hours of the date.

**Parameters**\
[Number](number.md) hoursValue ;\
[Number](number.md) minutesValue ;\
[Number](number.md) secondsValue ;

**Returns**\
void

**Sample**

```javascript
date.setHours(integer);
```

### setHours(hoursValue, minutesValue, secondsValue, msValue)

Sets the hours of the date.

**Parameters**\
[Number](number.md) hoursValue ;\
[Number](number.md) minutesValue ;\
[Number](number.md) secondsValue ;\
[Number](number.md) msValue ;

**Returns**\
void

**Sample**

```javascript
date.setHours(integer);
```

### setMilliseconds(millisecondsValue)

Sets the milliseconds of the date.

**Parameters**\
[Number](number.md) millisecondsValue ;

**Returns**\
void

**Sample**

```javascript
date.setMilliseconds(integer);
```

### setMinutes(minutesValue)

Sets the minutes of the date.

**Parameters**\
[Number](number.md) minutesValue ;

**Returns**\
void

**Sample**

```javascript
date.setMinutes(integer);
```

### setMinutes(minutesValue, secondsValue)

Sets the minutes of the date.

**Parameters**\
[Number](number.md) minutesValue ;\
[Number](number.md) secondsValue ;

**Returns**\
void

**Sample**

```javascript
date.setMinutes(integer);
```

### setMinutes(minutesValue, secondsValue, msValue)

Sets the minutes of the date.

**Parameters**\
[Number](number.md) minutesValue ;\
[Number](number.md) secondsValue ;\
[Number](number.md) msValue ;

**Returns**\
void

**Sample**

```javascript
date.setMinutes(integer);
```

### setMonth(monthValue)

Sets the month of the date.

**Parameters**\
[Number](number.md) monthValue ;

**Returns**\
void

**Sample**

```javascript
date.setMonth(integr);
```

### setMonth(monthValue, dayValue)

Sets the month of the date.

**Parameters**\
[Number](number.md) monthValue ;\
[Number](number.md) dayValue ;

**Returns**\
void

**Sample**

```javascript
date.setMonth(integr);
```

### setSeconds(secondsValue)

Sets the seconds of the date.

**Parameters**\
[Number](number.md) secondsValue ;

**Returns**\
void

**Sample**

```javascript
date.setSeconds(integer);
```

### setSeconds(secondsValue, msValue)

Sets the seconds of the date.

**Parameters**\
[Number](number.md) secondsValue ;\
[Number](number.md) msValue ;

**Returns**\
void

**Sample**

```javascript
date.setSeconds(integer);
```

### setTime(timeValue)

Sets the milliseconds of the date.

**Parameters**\
[Number](number.md) timeValue ;

**Returns**\
void

**Sample**

```javascript
date.setTime(integer);
```

### setUTCDate(dayValue)

Sets the UTC date.

**Parameters**\
[Number](number.md) dayValue ;

**Returns**\
void

**Sample**

```javascript
date.setUTCDate(integer);
```

### setUTCFullYear(yearValue)

Sets the year in UTC time.

**Parameters**\
[Number](number.md) yearValue ;

**Returns**\
void

**Sample**

```javascript
date.setUTCFullYear(integer);
```

### setUTCFullYear(yearValue, monthValue)

Sets the year in UTC time.

**Parameters**\
[Number](number.md) yearValue ;\
[Number](number.md) monthValue ;

**Returns**\
void

**Sample**

```javascript
date.setUTCFullYear(integer);
```

### setUTCFullYear(yearValue, monthValue, dayValue)

Sets the year in UTC time.

**Parameters**\
[Number](number.md) yearValue ;\
[Number](number.md) monthValue ;\
[Number](number.md) dayValue ;

**Returns**\
void

**Sample**

```javascript
date.setUTCFullYear(integer);
```

### setUTCHours(hoursValue)

Sets the hours in UTC time.

**Parameters**\
[Number](number.md) hoursValue ;

**Returns**\
void

**Sample**

```javascript
date.setUTCHours(integer);
```

### setUTCHours(hoursValue, minutesValue)

Sets the hours in UTC time.

**Parameters**\
[Number](number.md) hoursValue ;\
[Number](number.md) minutesValue ;

**Returns**\
void

**Sample**

```javascript
date.setUTCHours(integer);
```

### setUTCHours(hoursValue, minutesValue, secondsValue)

Sets the hours in UTC time.

**Parameters**\
[Number](number.md) hoursValue ;\
[Number](number.md) minutesValue ;\
[Number](number.md) secondsValue ;

**Returns**\
void

**Sample**

```javascript
date.setUTCHours(integer);
```

### setUTCHours(hoursValue, minutesValue, secondsValue, msValue)

Sets the hours in UTC time.

**Parameters**\
[Number](number.md) hoursValue ;\
[Number](number.md) minutesValue ;\
[Number](number.md) secondsValue ;\
[Number](number.md) msValue ;

**Returns**\
void

**Sample**

```javascript
date.setUTCHours(integer);
```

### setUTCMilliseconds(millisecondsValue)

Sets the milliseconds in UTC time.

**Parameters**\
[Number](number.md) millisecondsValue ;

**Returns**\
void

**Sample**

```javascript
date.setUTCMilliseconds(integer);
```

### setUTCMinutes(minutesValue)

Sets the minutes in UTC time.

**Parameters**\
[Number](number.md) minutesValue ;

**Returns**\
void

**Sample**

```javascript
date.setUTCMinutes(integer);
```

### setUTCMinutes(minutesValue, secondsValue)

Sets the minutes in UTC time.

**Parameters**\
[Number](number.md) minutesValue ;\
[Number](number.md) secondsValue ;

**Returns**\
void

**Sample**

```javascript
date.setUTCMinutes(integer);
```

### setUTCMinutes(minutesValue, secondsValue, msValue)

Sets the minutes in UTC time.

**Parameters**\
[Number](number.md) minutesValue ;\
[Number](number.md) secondsValue ;\
[Number](number.md) msValue ;

**Returns**\
void

**Sample**

```javascript
date.setUTCMinutes(integer);
```

### setUTCMonth(monthValue)

Sets the month in UTC time.

**Parameters**\
[Number](number.md) monthValue ;

**Returns**\
void

**Sample**

```javascript
date.setUTCMonth(integer);
```

### setUTCMonth(monthValue, dayValue)

Sets the month in UTC time.

**Parameters**\
[Number](number.md) monthValue ;\
[Number](number.md) dayValue ;

**Returns**\
void

**Sample**

```javascript
date.setUTCMonth(integer);
```

### setUTCSeconds(secondsValue)

Sets the seconds in UTC time.

**Parameters**\
[Number](number.md) secondsValue ;

**Returns**\
void

**Sample**

```javascript
date.setUTCSeconds(integer);
```

### setUTCSeconds(secondsValue, msValue)

Sets the seconds in UTC time.

**Parameters**\
[Number](number.md) secondsValue ;\
[Number](number.md) msValue ;

**Returns**\
void

**Sample**

```javascript
date.setUTCSeconds(integer);
```

### toDateString()

Returns a string version of the date.

**Returns**\
[String](string.md)

**Sample**

```javascript
date.toDateString();
```

### toISOString()

Returns a string version of the UTC value of the date.

**Returns**\
[String](string.md) the Date object as a string in simplified extended ISO format.

**Sample**

```javascript
date.toISOString();
```

### toLocaleDateString()

Returns a string version of the local time zone of the date.

**Returns**\
[String](string.md)

**Sample**

```javascript
date.toLocaleDateString();
```

### toLocaleString()

Returns a string version of the local time zone of the date.

**Returns**\
[String](string.md)

**Sample**

```javascript
date.toLocaleString();
```

### toLocaleTimeString()

Returns a string version of the local time zone of the date.

**Returns**\
[String](string.md)

**Sample**

```javascript
date.toLocaleTimeString();
```

### toTimeString()

Returns a string version of the date.

**Returns**\
[String](string.md)

**Sample**

```javascript
date.toTimeString();
```

### toUTCString()

Returns a string version of the UTC value of the date.

**Returns**\
[String](string.md)

**Sample**

```javascript
date.toUTCString();
```

### valueOf()

Return integer milliseconds count

**Returns**\
[Number](number.md)

**Sample**

```javascript
date.valueOf(integer);
```
