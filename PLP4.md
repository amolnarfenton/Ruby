###Conditional Statements
Like most programming languages, Ruby uses conditional statements to execute different tasks 
or actions depending on what the programmer wants done. These conditons are reserved words and
known as if/elsif/else. Note that every time you want to implement a conditional statement it has to start with and if statement and when you are done you have to type "end". For example, say you wanted to check and see if a number is great than another number.
The code would look like this:
```
x = 5
if x < 10
put "x is less than 10"
end
```
Now if you want to make your code a multi-step conditonal statement you can add and elsif condition afterwards. 
This means that if the if statement is not true it will default to the elsif statement. Building upon the code
we have above, here is what an added elsif statement would look like:

```
x = 5
if x > 10
put " x is greater than 10"
elsif
put "x is less than 10"
end

x is less than 10
```
As you can see "x is less than 10" would get displayed because the condition of the if statement was not met so by 
default the code went to the elsif statement. It should also be noted that you can have an many elsif statements but they 
have to attached to an if statement. This means that they hav to follow and if statement in the code. 
Finally we have reached the last conditonal statement, which is the else statement. Like the elsif statement this one gets exucuted as a default when every other statement is false. Although, unlike the elsif statment there can only be one else statment and it has to either follow an elsif or an if statetment. Expanding upon the code above we can see how the else statment is used.
```
x = 5
if x > 10
put " x is greater than 10"
elsif
put "x is less than 10"
else
put "This is a test"
end

x is less than 10
```

###Short-Curcit Evaluation


###Sources

http://code.tutsplus.com/tutorials/ruby-for-newbies-conditional-statements-and-loops--net-16537 Acessed



