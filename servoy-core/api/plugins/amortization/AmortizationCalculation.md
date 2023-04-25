#  AmortizationCalculation


## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [Number](../../JSLib/Number.md) | [NUMBER_UNLIMITED](AmortizationCalculation.md#NUMBER_UNLIMITED)                   | The numeric constant used to identify an unlimited number of repeated events..                                    |
| [Number](../../JSLib/Number.md) | [PERIOD_ANNUALY](AmortizationCalculation.md#PERIOD_ANNUALY)                   | The numeric constant used to identify an annual period..                                    |
| [Number](../../JSLib/Number.md) | [PERIOD_BI_ANNUALLY](AmortizationCalculation.md#PERIOD_BI_ANNUALLY)                   | The numeric constant used to identify a bi-annual period (twice every year)..                                    |
| [Number](../../JSLib/Number.md) | [PERIOD_BI_MONTHLY](AmortizationCalculation.md#PERIOD_BI_MONTHLY)                   | The numeric constant used to identify a bi-monthly period (twice every month)..                                    |
| [Number](../../JSLib/Number.md) | [PERIOD_DAILY](AmortizationCalculation.md#PERIOD_DAILY)                   | The numeric constant used to identify a daily period..                                    |
| [Number](../../JSLib/Number.md) | [PERIOD_FOUR_MONTHLY](AmortizationCalculation.md#PERIOD_FOUR_MONTHLY)                   | The numeric constant used to identify a four-monthly period (once every four months)..                                    |
| [Number](../../JSLib/Number.md) | [PERIOD_FOUR_WEEKLY](AmortizationCalculation.md#PERIOD_FOUR_WEEKLY)                   | The numeric constant used to identify a four-weekly period (once every four weeks)..                                    |
| [Number](../../JSLib/Number.md) | [PERIOD_MONTHLY](AmortizationCalculation.md#PERIOD_MONTHLY)                   | The numeric constant used to identify a monthly period..                                    |
| [Number](../../JSLib/Number.md) | [PERIOD_NONE](AmortizationCalculation.md#PERIOD_NONE)                   | The numeric constant used to identify that there is no period..                                    |
| [Number](../../JSLib/Number.md) | [PERIOD_QUARTERLY](AmortizationCalculation.md#PERIOD_QUARTERLY)                   | The numeric constant used to identify a quarterly period (once every three months)..                                    |
| [Number](../../JSLib/Number.md) | [PERIOD_TWO_MONTHLY](AmortizationCalculation.md#PERIOD_TWO_MONTHLY)                   | The numeric constant used to identify a two-monthly period (once every two months)..                                    |
| [Number](../../JSLib/Number.md) | [PERIOD_TWO_WEEKLY](AmortizationCalculation.md#PERIOD_TWO_WEEKLY)                   | The numeric constant used to identify a two-weekly period (once every two weeks)..                                    |
| [Number](../../JSLib/Number.md) | [PERIOD_WEEKLY](AmortizationCalculation.md#PERIOD_WEEKLY)                   | The numeric constant used to identify a weekly period..                                    |
| [Number](../../JSLib/Number.md) | [STARTDAY_NORMAL](AmortizationCalculation.md#STARTDAY_NORMAL)                   | The numeric constant used to identify that the same start day should be used as the day of the month of the starting date of the event..                                    |

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Boolean](../../JSLib/Boolean.md) | [addCompoundPeriodChange(newPeriod, date)](AmortizationCalculation.md#addcompoundperiodchange-newperiod-date)                   | Adds a compound period change..                                    |
| [Boolean](../../JSLib/Boolean.md) | [addLoan(amount, date)](AmortizationCalculation.md#addloan-amount-date)                   | Adds a loan..                                    |
| [Boolean](../../JSLib/Boolean.md) | [addLoan(amount, firstDate, lastDate, period)](AmortizationCalculation.md#addloan-amount-firstdate-lastdate-period)                   | Adds a loan..                                    |
| [Boolean](../../JSLib/Boolean.md) | [addLoan(amount, firstDate, lastDate, period, number)](AmortizationCalculation.md#addloan-amount-firstdate-lastdate-period-number)                   | Adds a loan..                                    |
| [Boolean](../../JSLib/Boolean.md) | [addLoan(amount, firstDate, lastDate, period, number, startday)](AmortizationCalculation.md#addloan-amount-firstdate-lastdate-period-number-startday)                   | Adds a loan..                                    |
| [Boolean](../../JSLib/Boolean.md) | [addPayment(amount, date)](AmortizationCalculation.md#addpayment-amount-date)                   | Adds a payment..                                    |
| [Boolean](../../JSLib/Boolean.md) | [addPayment(amount, firstDate, lastDate, period)](AmortizationCalculation.md#addpayment-amount-firstdate-lastdate-period)                   | Adds a payment..                                    |
| [Boolean](../../JSLib/Boolean.md) | [addPayment(amount, firstDate, lastDate, period, number)](AmortizationCalculation.md#addpayment-amount-firstdate-lastdate-period-number)                   | Adds a payment..                                    |
| [Boolean](../../JSLib/Boolean.md) | [addPayment(amount, firstDate, lastDate, period, number, startday)](AmortizationCalculation.md#addpayment-amount-firstdate-lastdate-period-number-startday)                   | Adds a payment..                                    |
| [Boolean](../../JSLib/Boolean.md) | [addRateChange(newRate, date)](AmortizationCalculation.md#addratechange-newrate-date)                   | Sets a new interest rate..                                    |
| [Boolean](../../JSLib/Boolean.md) | [calculateAmortizationSchedule()](AmortizationCalculation.md#calculateamortizationschedule)                   | Calculates the amortization schedule..                                    |
| [JSDataSet](../../Database%20Manager/JSDataSet.md) | [getAmortizationSchedule()](AmortizationCalculation.md#getamortizationschedule)                   | Gets the amortization schedule as a JSDataSet..                                    |
| [Number](../../JSLib/Number.md) | [getError()](AmortizationCalculation.md#geterror)                   | Returns the error that remains when solving for the unknown..                                    |
| [JSDataSet](../../Database%20Manager/JSDataSet.md) | [getEvents()](AmortizationCalculation.md#getevents)                   | Returns all the amortization events - such as rate changes, loan events, payment events, compounding period changes..                                    |
| [Number](../../JSLib/Number.md) | [getRestBalance()](AmortizationCalculation.md#getrestbalance)                   | Gets the rest balance after the amortization schedule..                                    |
| [Number](../../JSLib/Number.md) | [getUnknown()](AmortizationCalculation.md#getunknown)                   | Returns the solveForUnknown value..                                    |
| [Boolean](../../JSLib/Boolean.md) | [isValidPeriod(period)](AmortizationCalculation.md#isvalidperiod-period)                   | Returns true if the period is valid, or false if the period is not valid..                                    |
| [Number](../../JSLib/Number.md) | [roundMoney(amount)](AmortizationCalculation.md#roundmoney-amount)                   | Rounds a number up to the nearest cents..                                    |
| [Boolean](../../JSLib/Boolean.md) | [solveForUnknown()](AmortizationCalculation.md#solveforunknown)                   | Returns true if successful or false if the call failed..                                    |
|void | [sortEvents()](AmortizationCalculation.md#sortevents)                   | Sorts the amortization events ascending by date..                                    |

## Constants Details

### NUMBER_UNLIMITED

The numeric constant used to identify an unlimited number of repeated events.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addPayment(500, new Date(2005, 1, 28), null, 
			plugins.amortization.AmortizationCalculation.PERIOD_DAILY, 5, 
			plugins.amortization.AmortizationCalculation.STARTDAY_NORMAL);

var c2 = plugins.amortization.newCalculation();
c2.addPayment(300, new Date(2006, 11, 24), new Date(2006, 12, 24),
			plugins.amortization.AmortizationCalculation.PERIOD_BI_MONTHLY, 
			plugins.amortization.AmortizationCalculation.NUMBER_UNLIMITED, 30);
```
### PERIOD_ANNUALY

The numeric constant used to identify an annual period.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addPayment(500, new Date(2005, 1, 28), null, 
			plugins.amortization.AmortizationCalculation.PERIOD_DAILY, 5, 
			plugins.amortization.AmortizationCalculation.STARTDAY_NORMAL);

var c2 = plugins.amortization.newCalculation();
c2.addPayment(300, new Date(2006, 11, 24), new Date(2006, 12, 24),
			plugins.amortization.AmortizationCalculation.PERIOD_BI_MONTHLY, 
			plugins.amortization.AmortizationCalculation.NUMBER_UNLIMITED, 30);
```
### PERIOD_BI_ANNUALLY

The numeric constant used to identify a bi-annual period (twice every year).

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addPayment(500, new Date(2005, 1, 28), null, 
			plugins.amortization.AmortizationCalculation.PERIOD_DAILY, 5, 
			plugins.amortization.AmortizationCalculation.STARTDAY_NORMAL);

var c2 = plugins.amortization.newCalculation();
c2.addPayment(300, new Date(2006, 11, 24), new Date(2006, 12, 24),
			plugins.amortization.AmortizationCalculation.PERIOD_BI_MONTHLY, 
			plugins.amortization.AmortizationCalculation.NUMBER_UNLIMITED, 30);
```
### PERIOD_BI_MONTHLY

The numeric constant used to identify a bi-monthly period (twice every month).
TODO: this period is not supported yet.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addPayment(500, new Date(2005, 1, 28), null, 
			plugins.amortization.AmortizationCalculation.PERIOD_DAILY, 5, 
			plugins.amortization.AmortizationCalculation.STARTDAY_NORMAL);

var c2 = plugins.amortization.newCalculation();
c2.addPayment(300, new Date(2006, 11, 24), new Date(2006, 12, 24),
			plugins.amortization.AmortizationCalculation.PERIOD_BI_MONTHLY, 
			plugins.amortization.AmortizationCalculation.NUMBER_UNLIMITED, 30);
```
### PERIOD_DAILY

The numeric constant used to identify a daily period.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addPayment(500, new Date(2005, 1, 28), null, 
			plugins.amortization.AmortizationCalculation.PERIOD_DAILY, 5, 
			plugins.amortization.AmortizationCalculation.STARTDAY_NORMAL);

var c2 = plugins.amortization.newCalculation();
c2.addPayment(300, new Date(2006, 11, 24), new Date(2006, 12, 24),
			plugins.amortization.AmortizationCalculation.PERIOD_BI_MONTHLY, 
			plugins.amortization.AmortizationCalculation.NUMBER_UNLIMITED, 30);
```
### PERIOD_FOUR_MONTHLY

The numeric constant used to identify a four-monthly period (once every four months).

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addPayment(500, new Date(2005, 1, 28), null, 
			plugins.amortization.AmortizationCalculation.PERIOD_DAILY, 5, 
			plugins.amortization.AmortizationCalculation.STARTDAY_NORMAL);

var c2 = plugins.amortization.newCalculation();
c2.addPayment(300, new Date(2006, 11, 24), new Date(2006, 12, 24),
			plugins.amortization.AmortizationCalculation.PERIOD_BI_MONTHLY, 
			plugins.amortization.AmortizationCalculation.NUMBER_UNLIMITED, 30);
```
### PERIOD_FOUR_WEEKLY

The numeric constant used to identify a four-weekly period (once every four weeks).

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addPayment(500, new Date(2005, 1, 28), null, 
			plugins.amortization.AmortizationCalculation.PERIOD_DAILY, 5, 
			plugins.amortization.AmortizationCalculation.STARTDAY_NORMAL);

var c2 = plugins.amortization.newCalculation();
c2.addPayment(300, new Date(2006, 11, 24), new Date(2006, 12, 24),
			plugins.amortization.AmortizationCalculation.PERIOD_BI_MONTHLY, 
			plugins.amortization.AmortizationCalculation.NUMBER_UNLIMITED, 30);
```
### PERIOD_MONTHLY

The numeric constant used to identify a monthly period.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addPayment(500, new Date(2005, 1, 28), null, 
			plugins.amortization.AmortizationCalculation.PERIOD_DAILY, 5, 
			plugins.amortization.AmortizationCalculation.STARTDAY_NORMAL);

var c2 = plugins.amortization.newCalculation();
c2.addPayment(300, new Date(2006, 11, 24), new Date(2006, 12, 24),
			plugins.amortization.AmortizationCalculation.PERIOD_BI_MONTHLY, 
			plugins.amortization.AmortizationCalculation.NUMBER_UNLIMITED, 30);
```
### PERIOD_NONE

The numeric constant used to identify that there is no period.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addPayment(500, new Date(2005, 1, 28), null, 
			plugins.amortization.AmortizationCalculation.PERIOD_DAILY, 5, 
			plugins.amortization.AmortizationCalculation.STARTDAY_NORMAL);

var c2 = plugins.amortization.newCalculation();
c2.addPayment(300, new Date(2006, 11, 24), new Date(2006, 12, 24),
			plugins.amortization.AmortizationCalculation.PERIOD_BI_MONTHLY, 
			plugins.amortization.AmortizationCalculation.NUMBER_UNLIMITED, 30);
```
### PERIOD_QUARTERLY

The numeric constant used to identify a quarterly period (once every three months).

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addPayment(500, new Date(2005, 1, 28), null, 
			plugins.amortization.AmortizationCalculation.PERIOD_DAILY, 5, 
			plugins.amortization.AmortizationCalculation.STARTDAY_NORMAL);

var c2 = plugins.amortization.newCalculation();
c2.addPayment(300, new Date(2006, 11, 24), new Date(2006, 12, 24),
			plugins.amortization.AmortizationCalculation.PERIOD_BI_MONTHLY, 
			plugins.amortization.AmortizationCalculation.NUMBER_UNLIMITED, 30);
```
### PERIOD_TWO_MONTHLY

The numeric constant used to identify a two-monthly period (once every two months).

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addPayment(500, new Date(2005, 1, 28), null, 
			plugins.amortization.AmortizationCalculation.PERIOD_DAILY, 5, 
			plugins.amortization.AmortizationCalculation.STARTDAY_NORMAL);

var c2 = plugins.amortization.newCalculation();
c2.addPayment(300, new Date(2006, 11, 24), new Date(2006, 12, 24),
			plugins.amortization.AmortizationCalculation.PERIOD_BI_MONTHLY, 
			plugins.amortization.AmortizationCalculation.NUMBER_UNLIMITED, 30);
```
### PERIOD_TWO_WEEKLY

The numeric constant used to identify a two-weekly period (once every two weeks).

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addPayment(500, new Date(2005, 1, 28), null, 
			plugins.amortization.AmortizationCalculation.PERIOD_DAILY, 5, 
			plugins.amortization.AmortizationCalculation.STARTDAY_NORMAL);

var c2 = plugins.amortization.newCalculation();
c2.addPayment(300, new Date(2006, 11, 24), new Date(2006, 12, 24),
			plugins.amortization.AmortizationCalculation.PERIOD_BI_MONTHLY, 
			plugins.amortization.AmortizationCalculation.NUMBER_UNLIMITED, 30);
```
### PERIOD_WEEKLY

The numeric constant used to identify a weekly period.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addPayment(500, new Date(2005, 1, 28), null, 
			plugins.amortization.AmortizationCalculation.PERIOD_DAILY, 5, 
			plugins.amortization.AmortizationCalculation.STARTDAY_NORMAL);

var c2 = plugins.amortization.newCalculation();
c2.addPayment(300, new Date(2006, 11, 24), new Date(2006, 12, 24),
			plugins.amortization.AmortizationCalculation.PERIOD_BI_MONTHLY, 
			plugins.amortization.AmortizationCalculation.NUMBER_UNLIMITED, 30);
```
### STARTDAY_NORMAL

The numeric constant used to identify that the same start day should be used as
the day of the month of the starting date of the event.

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addPayment(500, new Date(2005, 1, 28), null, 
			plugins.amortization.AmortizationCalculation.PERIOD_DAILY, 5, 
			plugins.amortization.AmortizationCalculation.STARTDAY_NORMAL);

var c2 = plugins.amortization.newCalculation();
c2.addPayment(300, new Date(2006, 11, 24), new Date(2006, 12, 24),
			plugins.amortization.AmortizationCalculation.PERIOD_BI_MONTHLY, 
			plugins.amortization.AmortizationCalculation.NUMBER_UNLIMITED, 30);
```

## Methods Details

### addCompoundPeriodChange(newPeriod, date)

Adds a compound period change.

**Parameters**\
[Number](../../JSLib/Number.md) newPeriod  ;\
[Date](../../JSLib/Date.md) date  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addRateChange(r, new Date(2005, 0, 1));
c.addCompoundPeriodChange(12, new Date(2005, 0, 1));
c.addLoan(2000, new Date(2005, 0, 1));
c.addPayment(500, new Date(2005, 1, 28), null, 12, 5, 31);
```
### addLoan(amount, date)

Adds a loan.

**Parameters**\
[Number](../../JSLib/Number.md) amount  ;\
[Date](../../JSLib/Date.md) date  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addRateChange(r, new Date(2005, 0, 1));
c.addCompoundPeriodChange(12, new Date(2005, 0, 1));
c.addLoan(2000, new Date(2005, 0, 1));
c.addPayment(500, new Date(2005, 1, 28), null, 12, 5, 31);
```
### addLoan(amount, firstDate, lastDate, period)

Adds a loan.

**Parameters**\
[Number](../../JSLib/Number.md) amount  ;\
[Date](../../JSLib/Date.md) firstDate  ;\
[Date](../../JSLib/Date.md) lastDate  ;\
[Number](../../JSLib/Number.md) period  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addRateChange(r, new Date(2005, 0, 1));
c.addCompoundPeriodChange(12, new Date(2005, 0, 1));
c.addLoan(2000, new Date(2005, 0, 1));
c.addPayment(500, new Date(2005, 1, 28), null, 12, 5, 31);
```
### addLoan(amount, firstDate, lastDate, period, number)

Adds a loan.

**Parameters**\
[Number](../../JSLib/Number.md) amount  ;\
[Date](../../JSLib/Date.md) firstDate  ;\
[Date](../../JSLib/Date.md) lastDate  ;\
[Number](../../JSLib/Number.md) period  ;\
[Number](../../JSLib/Number.md) number  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addRateChange(r, new Date(2005, 0, 1));
c.addCompoundPeriodChange(12, new Date(2005, 0, 1));
c.addLoan(2000, new Date(2005, 0, 1));
c.addPayment(500, new Date(2005, 1, 28), null, 12, 5, 31);
```
### addLoan(amount, firstDate, lastDate, period, number, startday)

Adds a loan.

**Parameters**\
[Number](../../JSLib/Number.md) amount  ;\
[Date](../../JSLib/Date.md) firstDate  ;\
[Date](../../JSLib/Date.md) lastDate  ;\
[Number](../../JSLib/Number.md) period  ;\
[Number](../../JSLib/Number.md) number  ;\
[Number](../../JSLib/Number.md) startday  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addRateChange(r, new Date(2005, 0, 1));
c.addCompoundPeriodChange(12, new Date(2005, 0, 1));
c.addLoan(2000, new Date(2005, 0, 1));
c.addPayment(500, new Date(2005, 1, 28), null, 12, 5, 31);
```
### addPayment(amount, date)

Adds a payment.

**Parameters**\
[Number](../../JSLib/Number.md) amount  ;\
[Date](../../JSLib/Date.md) date  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addRateChange(r, new Date(2005, 0, 1));
c.addCompoundPeriodChange(12, new Date(2005, 0, 1));
c.addLoan(2000, new Date(2005, 0, 1));
c.addPayment(500, new Date(2005, 1, 28), null, 12, 5, 31);
```
### addPayment(amount, firstDate, lastDate, period)

Adds a payment.

**Parameters**\
[Number](../../JSLib/Number.md) amount  ;\
[Date](../../JSLib/Date.md) firstDate  ;\
[Date](../../JSLib/Date.md) lastDate  ;\
[Number](../../JSLib/Number.md) period  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addRateChange(r, new Date(2005, 0, 1));
c.addCompoundPeriodChange(12, new Date(2005, 0, 1));
c.addLoan(2000, new Date(2005, 0, 1));
c.addPayment(500, new Date(2005, 1, 28), null, 12, 5, 31);
```
### addPayment(amount, firstDate, lastDate, period, number)

Adds a payment.

**Parameters**\
[Number](../../JSLib/Number.md) amount  ;\
[Date](../../JSLib/Date.md) firstDate  ;\
[Date](../../JSLib/Date.md) lastDate  ;\
[Number](../../JSLib/Number.md) period  ;\
[Number](../../JSLib/Number.md) number  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addRateChange(r, new Date(2005, 0, 1));
c.addCompoundPeriodChange(12, new Date(2005, 0, 1));
c.addLoan(2000, new Date(2005, 0, 1));
c.addPayment(500, new Date(2005, 1, 28), null, 12, 5, 31);
```
### addPayment(amount, firstDate, lastDate, period, number, startday)

Adds a payment.

**Parameters**\
[Number](../../JSLib/Number.md) amount  ;\
[Date](../../JSLib/Date.md) firstDate  ;\
[Date](../../JSLib/Date.md) lastDate  ;\
[Number](../../JSLib/Number.md) period  ;\
[Number](../../JSLib/Number.md) number  ;\
[Number](../../JSLib/Number.md) startday  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addRateChange(r, new Date(2005, 0, 1));
c.addCompoundPeriodChange(12, new Date(2005, 0, 1));
c.addLoan(2000, new Date(2005, 0, 1));
c.addPayment(500, new Date(2005, 1, 28), null, 12, 5, 31);
```
### addRateChange(newRate, date)

Sets a new interest rate.

**Parameters**\
[Number](../../JSLib/Number.md) newRate  ;\
[Date](../../JSLib/Date.md) date  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
c.addRateChange(r, new Date(2005, 0, 1));
c.addCompoundPeriodChange(12, new Date(2005, 0, 1));
c.addLoan(2000, new Date(2005, 0, 1));
c.addPayment(500, new Date(2005, 1, 28), null, 12, 5, 31);
```
### calculateAmortizationSchedule()

Calculates the amortization schedule.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
plugins.amortization.calculateAmortizationSchedule();
```
### getAmortizationSchedule()

Gets the amortization schedule as a JSDataSet.


**Returns**\
[JSDataSet](../../Database%20Manager/JSDataSet.md) 


**Sample**

```javascript
plugins.amortization.getAmortizationSchedule();
```
### getError()

Returns the error that remains when solving for the unknown.
Please note that the error should be less or equal to 1E-8 - otherwise, the solveForUnknown value is incorrect.


**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var c = plugins.amortization.newCalculation();
// sets the rate to -1 for unknown.
c.addRateChange(-1, new Date(2005, 0, 1));
c.addCompoundPeriodChange(12, new Date(2005, 0, 1));
c.addLoan(2000, new Date(2005, 0, 1));
var lastDate = null;
var period = 12;
var number_count = 5;
var startday = 31;
c.addPayment(500, new Date(2005, 1, 28), lastDate, period,number_count, startday);
// solves for the interest rate.
c.solveForUnknown();
// gets the interest rate and the error in the calculation.
// which should be small (otherwise the calculation did
// not converge for some reason.
var r = c.getUnknown();
var e = c.getError();
```
### getEvents()

Returns all the amortization events - such as rate changes, loan events, payment events, compounding period changes.


**Returns**\
[JSDataSet](../../Database%20Manager/JSDataSet.md) 


**Sample**

```javascript
plugins.amortization.getEvents();
```
### getRestBalance()

Gets the rest balance after the amortization schedule.


**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
var rb = plugins.amortization.getRestBalance();
```
### getUnknown()

Returns the solveForUnknown value.


**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
plugins.amortization.getUnknown();
```
### isValidPeriod(period)

Returns true if the period is valid, or false if the period is not valid.

**Parameters**\
[Number](../../JSLib/Number.md) period  ;

**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
var v_period = plugins.amortization.isValidPeriod(12);
```
### roundMoney(amount)

Rounds a number up to the nearest cents.

**Parameters**\
[Number](../../JSLib/Number.md) amount  ;

**Returns**\
[Number](../../JSLib/Number.md) 


**Sample**

```javascript
//rounds the number up to 34.35
var rm = plugins.amortization.roundMoney(34.349384);
```
### solveForUnknown()

Returns true if successful or false if the call failed.


**Returns**\
[Boolean](../../JSLib/Boolean.md) 


**Sample**

```javascript
plugins.amortization.solveForUnknown();
```
### sortEvents()

Sorts the amortization events ascending by date.


**Returns**\
void 


**Sample**

```javascript
plugins.amortization.sortEvents();
```

