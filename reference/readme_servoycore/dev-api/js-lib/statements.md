# Statements

## Methods Summary

| Type | Name                                                   | Summary                                                                                             |
| ---- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------- |
| void | [break()](statements.md#break)                         | Break statement exits a loop..                                                                      |
| void | [const()](statements.md#const)                         | Constant declaration..                                                                              |
| void | [continue()](statements.md#continue)                   | Continue statement, jumps to next iteration of the loop..                                           |
| void | [do while()](statements.md#do-while)                   | do while loop.                                                                                      |
| void | [for()](statements.md#for)                             | for loop.                                                                                           |
| void | [for each in()](statements.md#for-each-in)             | foreach loop.                                                                                       |
| void | [if()](statements.md#if)                               | If statement.                                                                                       |
| void | [if else()](statements.md#if-else)                     | If/Else statement..                                                                                 |
| void | [label()](statements.md#label)                         | Provides a statement with an identifier that you can refer to using a break or continue statement.. |
| void | [switch()](statements.md#switch)                       | Switch statement..                                                                                  |
| void | [try catch()](statements.md#try-catch)                 | try/catch statement.                                                                                |
| void | [try catch finally()](statements.md#try-catch-finally) | try/catch/finally statement.                                                                        |
| void | [var()](statements.md#var)                             | Variable declaration.                                                                               |
| void | [while()](statements.md#while)                         | while loop.                                                                                         |

## Methods Details

### break()

Break statement exits a loop.

**Returns**\
void

**Sample**

```javascript
break
```

### const()

Constant declaration.

**Returns**\
void

**Sample**

```javascript
const #;
```

### continue()

Continue statement, jumps to next iteration of the loop.

**Returns**\
void

**Sample**

```javascript
continue
```

### do while()

do while loop

**Returns**\
void

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

For example, you can use a label to identify a loop, and then use the break or continue statements to indicate whether a program should interrupt the loop or continue its execution.

**Returns**\
void

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

**Sample**

```javascript
var #;
```

### while()

while loop

**Returns**\
void

**Sample**

```javascript
while ( # )
{
	#
}
```
