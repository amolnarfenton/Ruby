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




