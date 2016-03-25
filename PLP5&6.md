###Declaration of a Method

In Ruby in order to call upon a method you first have to define it. A method name has to start with a lower case letter. Also before the name the words def has to be there and after the word end is used to show the method is over. An example looks like this:
```
def method_name
end
```
A method can also take in values such as bellow:
```
def method_name(var1, var2)
end
```

###Calling Upon a Method

When calling upon a method you can simply just called the method name like so:
```
method_name
```
If your your method has paramaters you can call the method as such:
```
method_name 24, 6
```

Remember when you are passing in parameters you have to know how many there are. If you pass in too many or too few ou will get a error in your code when you run it. 

```
def test(a1="Ruby", a2="Perl")
   puts "The programming language is #{a1}"
   puts "The programming language is #{a2}"
end
test "C", "C++"
test
```
###Recursion
Like other programing languages, Ruby suppports recusive functions. Now what is a recursive? Well a recursive funtion is a function/method that call upon itself. A simple example is below:
```
def countdown(n)
  return if n.zero? 
  puts n
  countdown(n-1)    
end               

countdown(5)
5
4
3
2
1
```

A cool example of a recurive function is applying it to fibonacci sequence:
```
def fib(n)
  return n if (0..1).include? n
  fib(n-1) + fib(n-2) if n > 1
end
```
As you can see the method is called fib and in the actual method fib is called upon which initiates the recursive property.

###Function Parameters

Paramters in a programing language refer to what can get passed into a function for instance:
```
def method_name(var1, var2)
end
```
Now those are the same type but in Ruby you can also pass in values with different types such as a string and an interger.
```
def some_method(25,"hello", 45, 67)
end
```
In Ruby there is a typle of parameter called Arguments with Default Values. This means that if a function does not have enough paramaters it will use a default value to fill that parameter. For example:
```
def some_method(a, b, c=25)
end
```
To call this function you can do it two ways either:
```
some_method(25,"hello")
```
or
```
some_method(25,"hello", 48)
```
In the fist case there is not a value for the thid parameter so a default value is used which in this case would be 25.

Another parameter tpe is called Optional Arguments. This allows you to decided at run time how many parameters there are and it is denoted as such:
```
def some_method(*p)
end
```
Now you can call this method with either no argument or many arguments


```
some_method
some_method(25)
some_method (25,"hello", 45, 67)
```

###Returning Mutipule Values

In Ruby you are allowed to return multiplue value the only thing you have to know is before you do you need to break them into indepedent variables. This is so that each variable that is getting returned is explicitly stated. You should also note that a return value of any method in ruby is always an object.

```
def multiple
  return 1, 2
end

x = multiple
# => [ 1, 2 ]
x
# => [ 1, 2 ]
```

###Scope

In programing langauges it is important to know were you can access your variables, this is known as scope. For Ruby a varable that is declared in a loop or a method cannot be accessed by any thing outside of that loop or method. If you have varables of the same name in an inner section and an outer section they can not be written over eachother. For example if you have a variable x in a loop you can have a variable x out side of the loop and it will not conflict with the x in the loop. This is also true for methods. 

If you would like a variable to accessed in all aspects of the code you can set it to be a global variable. In order to create a global variable it is just like creating any other variable expect you need to have a $ before the name. For example:
```
$example = 5 
```

### Passed By Reference vs. Passed By Value
Before we get to the application of Ruby we should first talk about what by reference and by value mean because different languages handel there variables differently and it's a good idea to know the difference. When passing a varable by reference it mean that the variable does not get changed in memory when you decide to change the value of that variable. On the other hand passing by value means that the variable does get changed in memory so when you change a varaibles value it only seens that new value and is no longer asociated to the old value. I read a good explination of the two where it said that passing by value is like giving someone a link to a web page. Since the person has the web page link they can actually see the changes being made. Now think about if instead of giving them the web page link you only gave them the print out of it. Now they can make changes to the print out but it won't effect the web page and you can make changes to the web page but you won't seen them on the print out. With our knowlege of  the difference between value and reference we can look specifically at Ruby. In Ruby variables are passed by by value, which means they do get changed in memory.
### Sources 
http://www.tutorialspoint.com/ruby/ Accessed March 22,2016.

http://www.skorks.com/2009/08/method-arguments-in-ruby/ Accessed March 23,2016.

http://stackoverflow.com Accessed March 24,2016.







