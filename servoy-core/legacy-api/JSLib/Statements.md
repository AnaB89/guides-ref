#  Statements

## **Supported Clients**

    SmartClient
    WebClient
    NGClient
    MobileClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [break()](Statements.md#break)                   | Break statement exits a loop..                                    |
|void | [const()](Statements.md#const)                   | Constant declaration..                                    |
|void | [continue()](Statements.md#continue)                   | Continue statement, jumps to next iteration of the loop..                                    |
|void | [do while()](Statements.md#do-while)                   | do while loop.                                    |
|void | [for()](Statements.md#for)                   | for loop.                                    |
|void | [for each in()](Statements.md#for-each-in)                   | foreach loop.                                    |
|void | [if()](Statements.md#if)                   | If statement.                                    |
|void | [if else()](Statements.md#if-else)                   | If/Else statement..                                    |
|void | [label()](Statements.md#label)                   | Provides a statement with an identifier that you can refer to using a break or continue statement..                                    |
|void | [switch()](Statements.md#switch)                   | Switch statement..                                    |
|void | [try catch()](Statements.md#try-catch)                   | try/catch statement.                                    |
|void | [try catch finally()](Statements.md#try-catch-finally)                   | try/catch/finally statement.                                    |
|void | [var()](Statements.md#var)                   | Variable declaration.                                    |
|void | [while()](Statements.md#while)                   | while loop.                                    |

## Methods Details

### break()

Break statement exits a loop.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
break
```
### const()

Constant declaration.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
const #;
```
### continue()

Continue statement, jumps to next iteration of the loop.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
continue
```
### do while()

do while loop


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
do
{
}
while ( # )
```
### for()

for loop


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
for ( var i = 0 ; i < # ; i++ )
{
}
```
### for each in()

foreach loop


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
for ( var item in obj )
{
}
```
### if()

If statement


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
if ( # )
{
}
```
### if else()

If/Else statement.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
if ( # )
{
}
else
{
}
```
### label()

Provides a statement with an identifier that you can refer to using a break or continue statement.

For example, you can use a label to identify a loop, and then use the break or continue statements to indicate 
whether a program should interrupt the loop or continue its execution.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var i = 0, j;
outer_loop: while (i < 10) {
	i++;
	j = 0;
	while (j < 10) {
		j++;
		if (j > i) continue outer_loop;
		application.output("i=" + i + ", j=" + j);
	}
}
```
### switch()

Switch statement.


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
switch( # )
{
case:
default:
}
```
### try catch()

try/catch statement


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
try 
{
	#
}
 catch(#) 
{
	#
}
```
### try catch finally()

try/catch/finally statement


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
try 
{
	#
}
 catch(#) 
{
	#
} finally 
{
	#
}
```
### var()

Variable declaration


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
var #;
```
### while()

while loop


**Returns**\
void 

**Supported Clients**\
SmartClient,WebClient,NGClient,MobileClient

**Sample**

```javascript
while ( # )
{
	#
}
```

