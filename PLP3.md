### Variable Naming
In Ruby local variable names either start with lowercase letters (a-z) or an underscore(_), it cannot start with a number, followed by anything such as more lowercase, uppercase and or numbers. A local variable is only valid inside of a method, block or module. Instance variable names start with an at sign(@) then they follow the local variable naming rules. Global variables also follow local variable rules but they have to start witha dollar sign ($). Unlike local variables, gobal variables are vaild everywhere. When creating variable names you want to make sure that they are relevant to the project so when you come back to it or someone else has to read it they can understand what is going on. A good example of a varible would be name if your asking for someones name a bad example would be volcano as a variable name.  Ruby is also a case sensetive language meaning that name and Name represent two different variables. 


###Language Type
Since Ruby is a dynamically typed language variables are interpreted at runtime and because it is also a strongly typed language all type errors are identified at the runtime.  

###Strings and Integers
Lets look at an example to get familar with Ruby:
```
x = "5" + 6
puts x
```
This peice of code will not compile because ruby cannot add a string type with an integer type. To fix this so it can compile either the string 5 has to becoming a number as such:
```
x = 5 + 6
puts x
11
```
Or the whole statment has to become a string like such:
```
x = "5 + 6"
puts x
5 + 6
```

###Conversion
To convert objcts in to new ones with different types, Ruby uses conversion methods. In Ruby there are two types of conversion methods, non strict (explicit)and strict (implicit). To elaborate, explicit type converstion is when a cast operater is required and implicit conversion is when the work is done by a compiler. 



### Source
http://rubylearning.com/satishtalim/ruby_names.html Accessed February 7, 2016.

http://zetcode.com/lang/rubytutorial/variables/ Accessed February 9, 2016.

http://codeloveandboards.com/blog/2014/03/18/explicit-vs-implicit-conversion-methods/ Accessed February 11, 2016.

