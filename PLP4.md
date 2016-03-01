###Conditional Statements
Like most programming languages, Ruby uses conditional statements to execute different tasks 
or actions depending on what the programmer wants done. These conditons are reserved words and
known as if/elsif/else. Note that every time you want to implement a conditional statement it has to start with and if statement and at the end of every if statment you have to type "end". For example, say you wanted to check and see if a number is great than another number.
The code would look like this:
```
x=1
if x > 2
  puts "x is greater than 2"

```
Now if you want to make your code a multi-step conditonal statement you can add and elsif condition afterwards. 
This means that if the if statement is not true it will default to the elsif statement. Building upon the code
we have above, here is what an added elsif statement would look like:

```
x=1
if x > 2
  puts "x is greater than 2"
elsif x <= 2 and x!=0
  puts "x is 1"
end


```
As you can see "x is 1" would get displayed because the condition of the if statement was not met so by 
default the code went to the elsif statement. It should also be noted that you can have an many elsif statements but they 
have to attached to an if statement. This means that they have to follow and if statement in the code. 
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
```




###Short-Curcit Evaluation
Short-curcit evaluation is when there is a conditional statement with two parts and the second part only gets checked if the first part is false. This applies to && (and) and || (or). For the && the second condition is not evaluated if the first condition is false. Now for the || the second condition is not evaluated if the first condition is true.  Below is an example for both cases:
```
x = 5
if x=!5 && x>10
end
```
```
x = 5
if x=5 || x>10
end
```


###Dangeling Else Problem
The dangeling else problem refers to a scenario where there is an ambiguous else statement meaning you don't know which if statement it belongs to. To fix this problem, Ruby uses statement sequences as clauses. This means that the placement of the if and else statements combined with and end statement allows tou to determine what if statement the else is refering to.  An example of this is shown below:
```
if sum == 0 then
    if count == 0 then
      result = 0
    else
      result = 1
    end
  end
   if sum == 0 then
    if count == 0 then
      result = 0
    end
  else
    result = 1
  end
  ```
###Loops, Loops And More Loops
Loops are used in programming to repeat the same code numerous times. In Ruby there are three types of loops. The first loop I am going to talk about is the while loop. This loop is executed when a condition is true and the [do] part separates the code from the condition. In general the code will look like this:
```
while condition [do]
  code
end
```
Another was to execute a while loop is like this:
```
code while condition
OR

begin 
  code 
end while conditional
```
The second loop I am going to look at is the until loop. Unlike the while look the until look is executed when the condition is false. in general the code looks like this:
```
until conditional [do]
  code
end
```
Another was to execute a until loop is like this:

```
code until conditional

OR

begin
  code
end until conditional
```
As ypou can see both the while loop an until loop have the same format the only difference it that the while loop gets executed when true and the until loop gets executed when false.

Finally the last loop we are going to look at is the for loop. This loop is used to execute code per each element and is usually used for incrementing a variable such as i. An example of this looks like:
```
(0..5).each do |i|
  puts "Value of local variable is #{i}"
end
```
Which gives you a display of this:
```
Value of local variable is 0
Value of local variable is 1
Value of local variable is 2
Value of local variable is 3
Value of local variable is 4
Value of local variable is 5
```

###Exiting Loops And Other Stuff
Sometime in your code you want to be able to exit out of a loop immediatly without going through the rest of the code this is where a break comes in. An example of this is:
```
for i in 0..5
  if i > 2 then
      break
    end
   puts "Value of local variable is #{i}"
end
```
Giving the result:
Value of local variable is 0

Value of local variable is 1

Value of local variable is 2


###Sources

http://code.tutsplus.com/tutorials/ruby-for-newbies-conditional-statements-and-loops--net-16537 Accessed February 20, 2016.

http://blog.revathskumar.com/2013/05/short-circuit-evaluation-in-ruby.html Accessed February 21, 2016.

http://webcache.googleusercontent.com/search?q=cache:ntS0lJxZw64J:www.csie.ntnu.edu.tw/~ghhwang/course_slices/PL/Chapter08.ppt+&cd=5&hl=en&ct=clnk&gl=us&client=safari Accessed February 21, 2016.

http://www.tutorialspoint.com/ruby/ruby_loops.htm Accessed February 21, 2016.

http://www.tutorialspoint.com/ruby/ruby_if_else.htm Accessed February 25, 2016.





