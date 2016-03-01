###Conditional Statements
Like most programming languages, Ruby uses conditional statements to execute different tasks 
or actions depending on what the programmer wants done. These conditons are reserved words and
known as if/elsif/else.Note that every time you want to implement a conditional statement it has to start with and if statement. For example, say you wanted to check and see if a number is great than another number.
The code would look like this:
```
x = 5
if x < 10
put "x is less than 10"
```
Now if you want to make your code a multi-step conditonal statement you can add and elsif condition afterwards. 
This means that if the if statement not true it will default to the elsif statement. Building upon the code
we have above, here is what and added elsif statement would look like:

```
x = 5
if x > 10
put " x is greater than 10"
elsif
put "x is less than 10"

x is less than 10
```
As you can see "x is less than 10" would get displayed because the condition of the if statement was not met so by 
default the code went to the elsif statement. It should also be noted that you can have an many elsif statement but they 
have to follow an if statement.
