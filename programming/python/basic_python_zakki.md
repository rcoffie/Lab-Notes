# Python Programming 

## What is Python 
Python is a high-level, general-purpose programming language. Its design philosophy emphasizes code readability with the use of significant indentation. Python is dynamically typed and garbage-collected. It supports multiple programming paradigms, including structured, object-oriented and functional programming.

## Example

code 

```bash
  prinnt("Hello, World")
  
```
output

```bash
  Hello, World
  
```


## Variables 
A Python variable is a symbolic name that is a reference or pointer to an object. Once an object is assigned to a variable, you can refer to the object by that name.


## Usage

## Lessons Learned
open your code editor and create a file call **hello_world.py**. \

Let’s try using a variable in hello_world.py. Add a new line at the beginning of
the file, and modify the second line:


```bash
  message = "Hello Python World:
  print(message)
```
    
Run this program to see what happens. You should see the same output
you saw previously:


```bash
  Hello Python World
```

We’ve added a variable named message. Every variable is connected to a
value, which is the information associated with that variable. In this case the
value is the "Hello Python world!" text.
Adding a variable makes a little more work for the Python interpreter.
When it processes the first line, it associates the variable message with the
"Hello Python world!" text. When it reaches the second line, it prints the value
associated with message to the screen.


## Naming and Using Variables 
When you’re using variables in Python, you need to adhere to a few rules
and guidelines. Breaking some of these rules will cause errors; other
guidelines just help you write code that’s easier to read and understand. Be
sure to keep the following variable rules in mind:

* Variable names can contain only letters, numbers, and underscores.They can start with a letter or an underscore, but not with a number.For instance, you can call a variable message_1 but not 1_message.
* Spaces are not allowed in variable names, but underscores can be used to separate words in variable names. For example, greeting_message works, but greeting message will cause errors.
* Avoid using Python keywords and function names as variable names; that is, do not use words that Python has reserved for a particular programmatic purpose, such as the word print. (See “Python Keywords and Built-in Functions” on page 471.)
* Variable names should be short but descriptive. For example, name is better than n, student_name is better than s_n, and name_length is better than length_of_persons_name
* Be careful when using the lowercase letter l and the uppercase letter O
because they could be confused with the numbers 1 and 0.

## Strings
A string is a series of characters. Anything inside quotes is considered a
string in Python, and you can use single or double quotes around your
strings like this:

```bash
  "This is a string. "
  'This is also a string. '
```

This flexibility allows you to use quotes and apostrophes within your
strings:

```bash
'I told my friend, "Python is my favorite language!"'
"The language 'Python' is named after Monty Python, not the snake."
"One of Python's strengths is its diverse and supportive community."
```

## Numbers 
Python has three built-in numeric data types: integers, floating-point numbers, and complex numbers. In this section, you'll learn about integers and floating-point numbers, which are the two most commonly used number types. You'll learn about complex numbers in a later section

## integers

An integer is a whole number with no decimal places. For example, 1 is an integer, but 1.0 isn’t. The name for the integer data type is int, which you can see with type():

```bash
>>> type(1)
<class 'int'>
```

You can create an integer by typing the desired number. For instance, the following assigns the integer 25 to the variable num:

```bash
>>> num = 25
```

When you create an integer like this, the value 25 is called an integer literal because the integer is literally typed into the code.

## Floating-Points Numbers 
floating-point number, or float for short, is a number with a decimal place. 1.0 is a floating-point number, as is -2.75. The name of the floating-point data type is float:

```bash
>>> type(1.0)
<class 'float'>
```
Like integers, floats can be created from floating-point literals or by converting a string to a float with float():

```bash
>>>> float("1.25")
1.25
```

## Arithmetic Operators and Expressions 
Arithmetic operators ( +, -, *, /, **, % ) Arithmetic operators perform mathematical operations such as addition and subtraction with operands

## Addition
Addition is performed with the + operator:

```bash
>>> 1 + 2
3
```

The two numbers on either side of the + operator are called operands. In the above example, both operands are integers, but operands don’t need to be the same type.
You can add an int to a float with no problem:

```bash
>>> 1.0 + 2
3.0
```

Notice that the result of 1.0 + 2 is 3.0, which is a float. Anytime a float is added to a number, the result is another float. Adding two integers together always results in an int.

## Substraction 
To subtract two numbers, just put a - operator between them:

```bash
>>> 1 - 1
0

>>> 5.0 - 3
2.0
```

Just like adding two integers, subtracting two integers always results in an int. Whenever one of the operands is a float, the result is also a float.The - operator is also used to denote negative numbers:

```bash
>>> 1 - -3
4

>>> 1 --3
4

>>> 1- -3
4

>>> 1--3
4
```

Of the four examples above, the first is the most PEP 8 compliant. That said, you can surround -3 with parentheses to make it even clearer that the second - is modifying 3:

```python
>>> 1 - (-3)
4
```

# Multiplication
To multiply two numbers, use the * operator:

```python
>>> 3 * 3
9

>>> 2 * 8.0
16.0
```
The type of number you get from multiplication follows the same rules as addition and subtraction. Multiplying two integers results in an int, and multiplying a number with a float results in a float.

## Division
The / operator is used to divide two numbers:

```python
>>> 9 / 3
3.0

>>> 5.0 / 2
2.5
```
Unlike addition, subtraction, and multiplication, division with the / operator always returns a float. If you want to make sure that you get an integer after dividing two numbers, you can use int() to convert the result:

```python
>>> int(9 / 3)
3
```

Keep in mind that int() discards any fractional part of the number:


```python
>>> int(5.0 / 2)
2
```

5.0 / 2 returns the floating-point number 2.5, and int(2.5) returns the integer 2 with the .5 removed.

# The Modules Operator 

The % operator, or the modulus, returns the remainder of dividing the left operand by the right operand:

```python
>>> 5 % 3
2

>>> 20 % 7
6

>>> 16 % 8
0
```

3 divides 5 once with a remainder of 2, so 5 % 3 is 2. Similarly, 7 divides 20 twice with a remainder of 6. In the last example, 16 is divisible by 8, so 16 % 8 is 0. Anytime the number to the left of % is divisible by the number to the right, the result is 0.

One of the most common uses of % is to determine whether one number is divisible by another. For example, a number n is even if and only if n % 2 is 0. What do you think 1 % 0 returns? Let’s try it out:

```python
>>> 1 % 0
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ZeroDivisionError: integer division or modulo by zero
```
This makes sense because 1 % 0 gives the remainder of dividing 1 by 0. But you can’t divide 1 by 0, so Python raises a ZeroDivisionError

## Comments 
Comments are an extremely useful feature in most programming languages.
Everything you’ve written in your programs so far is Python code. As your
programs become longer and more complicated, you should add notes
within your programs that describe your overall approach to the problem
you’re solving. A comment allows you to write notes in English within your
programs.

In Python, the hash mark (#) indicates a comment. Anything following a
hash mark in your code is ignored by the Python interpreter

```python
# Say hello to everyone.
print("Hello Python people!")
```
Python ignores the first line and executes the second line.
Hello Python people!

## INTRODUCTIN LISTS 

## What is a list ?
A list is a collection of items in a particular order. You can make a list that
includes the letters of the alphabet, the digits from 0–9, or the names of all
the people in your family. You can put anything you want into a list, and the
items in your list don’t have to be related in any particular way. Because a list
usually contains more than one element, it’s a good idea to make the name of
your list plural, such as letters, digits, or names.
In Python, square brackets ([]) indicate a list, and individual elements in
the list are separated by commas. Here’s a simple example of a list that
contains a few kinds of bicycles:

```python
bicycles = ['trek', 'cannondale', 'redline', 'specialized']
print(bicycles)
```

If you ask Python to print a list, Python returns its representation of the
list, including the square brackets:

```python
['trek', 'cannondale', 'redline', 'specialized']
```
Because this isn’t the output you want your users to see, let’s learn how to
access the individual items in a list.

## Accessing Elements in a List
Lists are ordered collections, so you can access any element in a list by
telling Python the position, or index, of the item desired. To access an
element in a list, write the name of the list followed by the index of the item
enclosed in square brackets.
For example, let’s pull out the first bicycle in the list bicycles:

```python
['trek', 'cannondale', 'redline', 'specialized']
print(bicycles[0])
```
When we ask for a single item from a
list, Python returns just that element without square brackets:
```python
trek
```

## Index Positions Start at 0, Not 1
Python considers the first item in a list to be at position 0, not position 1.
This is true of most programming languages, and the reason has to do with
how the list operations are implemented at a lower level. If you’re receiving
unexpected results, determine whether you are making a simple off-by-one error.

The second item in a list has an index of 1. Using this counting system,
you can get any element you want from a list by subtracting one from its
position in the list. For instance, to access the fourth item in a list, you
request the item at index 3.
The following asks for the bicycles at index 1 and index 3:

```python
bicycles = ['trek', 'cannondale', 'redline', 'specialized']
print(bicycles[1])
print(bicycles[3])
```
This code returns the second and fourth bicycles in the list:


```python
bicycles = ['trek', 'cannondale', 'redline', 'specialized']
cannondale
specialized
```
Python has a special syntax for accessing the last element in a list. By
asking for the item at index -1, Python always returns the last item in the list:

```python
bicycles = ['trek', 'cannondale', 'redline', 'specialized']
print(bicycles[-1])
```

This code returns the value 'specialized'. This syntax is quite useful,
because you’ll often want to access the last items in a list without knowing
exactly how long the list is. This convention extends to other negative index
values as well. The index -2 returns the second item from the end of the list,
the index -3 returns the third item from the end, and so forth.

## Using Individual Values from a List
You can use individual values from a list just as you would any other variable.
For example, you can use f-strings to create a message based on a value from
a list.
Let’s try pulling the first bicycle from the list and composing a message
using that value.

```python
bicycles = ['trek', 'cannondale', 'redline', 'specialized']
print(bicycles[-1])
```

## Using Individual Values from a List
You can use individual values from a list just as you would any other variable.
For example, you can use f-strings to create a message based on a value from
a list.
Let’s try pulling the first bicycle from the list and composing a message
using that value.

```python
bicycles = ['trek', 'cannondale', 'redline', 'specialized']
message = f"My first bicycle was a {bicycles[0].title()}."
print(message) 
```
## output 

```python
My first bicycle was a Trek.
```

# Dictionaries in python 
A dictionary in Python is a collection of key-value pairs. Each key is connected
to a value, and you can use a key to access the value associated with that key.
A key’s value can be a number, a string, a list, or even another dictionary. In
fact, you can use any object that you can create in Python as a value in a
dictionary.
In Python, a dictionary is wrapped in braces, {}, with a series of key-value
pairs inside the braces, as shown in the earlier example:



```python
lien_0 = {'color': 'green', 'points': 5}
```
A key-value pair is a set of values associated with each other. When you
provide a key, Python returns the value associated with that key. Every key is
connected to its value by a colon, and individual key-value pairs are
separated by commas. You can store as many key-value pairs as you want in a
dictionary.
The simplest dictionary has exactly one key-value pair, as shown in this
modified version of the alien_0 dictionary:

```python
alien_0 = {'color': 'green'}
```

This dictionary stores one piece of information about alien_0, namely the
alien’s color. The string 'color' is a key in this dictionary, and its associated
value is 'green'.

## Accessing Values in a Dictionary
To get the value associated with a key, give the name of the dictionary and
then place the key inside a set of square brackets, as shown here:

```python
alien_0 = {'color': 'green'}
print(alien_0['color'])
```
This returns the value associated with the key 'color' from the dictionary
alien_0:

```python
green
```
You can have an unlimited number of key-value pairs in a dictionary. For
example, here’s the original alien_0 dictionary with two key-value pairs:

```python
alien_0 = {'color': 'green', 'points': 5}
```
Now you can access either the color or the point value of alien_0. If a
player shoots down this alien, you can look up how many points they should
earn using code like this:

```python
alien_0 = {'color': 'green', 'points': 5}
➊ new_points = alien_0['points]
➋ print(f"You just earned (new_points) points")
```
Once the dictionary has been defined, the code at ➊ pulls the value
associated with the key 'points' from the dictionary. This value is then
assigned to the variable new_points. The line at ➋ prints a statement about
how many points the player just earned:

```python
You just earned 5 points 
```
## Adding New Key-Value Pairs
Dictionaries are dynamic structures, and you can add new key-value pairs to
a dictionary at any time. For example, to add a new key-value pair, you
would give the name of the dictionary followed by the new key in square
brackets along with the new value.
Let’s add two new pieces of information to the alien_0 dictionary: the
alien’s x- and y-coordinates, which will help us display the alien in a
particular position on the screen. Let’s place the alien on the left edge of the
screen, 25 pixels down from the top. Because screen coordinates usually start
at the upper-left corner of the screen, we’ll place the alien on the left edge of
the screen by setting the x-coordinate to 0 and 25 pixels from the top by
setting its y-coordinate to positive 25, as shown here:

```python
alien_0 = {'color': 'green', 'points': 5}
print(alien_0)
➊ alien_0['x_position'] = 0
➋ alien_0['y_position'] = 25
print(alien_0)
```

We start by defining the same dictionary that we’ve been working with.
We then print this dictionary, displaying a snapshot of its information. At ➊
we add a new key-value pair to the dictionary: key 'x_position' and value 0.
We do the same for key 'y_position' at ➋. When we print the modified
dictionary, we see the two additional key-value pairs:

```python
{'color': 'green', 'points': 5}
{'color': 'green', 'points': 5, 'y_position': 25, 'x_position': 0}
```
The final version of the dictionary contains four key-value pairs. The
original two specify color and point value, and two more specify the alien’s
position.

## Loops in Python
## What are loops 
A loop is an instruction that repeats multiple times as long as some condition is met.

# For loop 

A for loop in Python is used to iterate over a sequence (list, tuple, set, dictionary, and string).


## Flow Chat 

![for-loop](https://user-images.githubusercontent.com/34107104/218073117-3ffa3003-c5e9-4d2d-ba68-43009cf1ef04.JPG)

```python
#iterate throught a list 
x = ["python","django","flask","FastAPI"]
for i in x:
  print(i)

  python
  django
  flask
  FastAPI
```
The preceding code executes as follows: The variable i is a placeholder for every item in your iterable object. The loop iterates as many times as the number of elements and prints the elements serially.

## While Loop 

The while loop is used to execute a set of statements as long as a condition is true. 

## Flow Chat 

![whileloop](https://user-images.githubusercontent.com/34107104/218073183-267b187e-eaa7-48ee-bc8a-a9ab0de68b06.JPG)

```python
#while loop 
x = 1 
while x <3: 
  print(x)
  x= x+1 

  1
  2
```

The preceding code executes as follows: We assign the value to variable x as 1. Until the value of x is less than 3, the loop continues and prints the numbers. 

##Condtional Statement 

Decision making statements are used to execute the statements onlyu when a particular condition is fulfilled. 

## Flow Chat 


![conditional-statement](https://user-images.githubusercontent.com/34107104/218073246-fe42f0b3-3514-4cf3-9a2e-116da0ce8cf0.JPG)



## Introduction to the if Statement
We’ll start by looking at the most basic type of if statement. In its simplest form, it looks like this:

```python
if <expr>:
    <statement>

```

In the form shown above:

* <expr> is an expression evaluated in a Boolean context, as discussed in the section on Logical Operators in the Operators and Expressions in Python tutorial.
* <statement> is a valid Python statement, which must be indented. (You will see why very soon.)

If <expr> is true (evaluates to a value that is “truthy”), then <statement> is executed. If <expr> is false, then <statement> is skipped over and not executed.

Note that the colon (:) following <expr> is required. Some programming languages require <expr> to be enclosed in parentheses, but Python does not.

Here are several examples of this type of if statement:

```python

>>> x = 0
>>> y = 5

>>> if x < y:                            # Truthy
...     print('yes')
...
yes
>>> if y < x:                            # Falsy
...     print('yes')
...

>>> if x:                                # Falsy
...     print('yes')
...
>>> if y:                                # Truthy
...     print('yes')
...
yes

>>> if x or y:                           # Truthy
...     print('yes')
...
yes
>>> if x and y:                          # Falsy
...     print('yes')
...

>>> if 'aul' in 'grault':                # Truthy
...     print('yes')
...
yes
>>> if 'quux' in ['foo', 'bar', 'baz']:  # Falsy
...     print('yes')
...

```

## The else and elif Clauses

Now you know how to use an if statement to conditionally execute a single statement or a block of several statements. It’s time to find out what else you can do.

Sometimes, you want to evaluate a condition and take one path if it is true but specify an alternative path if it is not. This is accomplished with an else clause:

```python
if <expr>:
    <statement(s)>
else:
    <statement(s)>

```

If <expr> is true, the first suite is executed, and the second is skipped. If <expr> is false, the first suite is skipped and the second is executed. Either way, execution then resumes after the second suite. Both suites are defined by indentation, as described above.

In this example, x is less than 50, so the first suite (lines 4 to 5) are executed, and the second suite (lines 7 to 8) are skipped:


```python
>>> x = 20

>>> if x < 50:
...     print('(first suite)')
...     print('x is small')
... else:
...     print('(second suite)')
...     print('x is large')
...
(first suite)
x is small

```
Here, on the other hand, x is greater than 50, so the first suite is passed over, and the second suite executed:

```python
>>> x = 120
>>>
>>> if x < 50:
...     print('(first suite)')
...     print('x is small')
... else:
...     print('(second suite)')
...     print('x is large')
...
(second suite)
x is large
```

There is also syntax for branching execution based on several alternatives. For this, use one or more elif (short for else if) clauses. Python evaluates each <expr> in turn and executes the suite corresponding to the first that is true. If none of the expressions are true, and an else clause is specified, then its suite is executed:


```python
if <expr>:
    <statement(s)>
elif <expr>:
    <statement(s)>
elif <expr>:
    <statement(s)>
    ...
else:
    <statement(s)>
```

## Functions in Python 
A function is a block of code which only runs when it is called.
You can pass data, known as parameters, into a function.
A function can return data as a result.

## Creating Functions 

In Python a function is defined using the def keyword:


```python
def my_function():
  print("Hello from a function") 
```

## Calling a Function

To call a function, use the function name followed by parenthesis:



```python
def my_function():
  print("Hello from a function")

my_function()
```
output 
```python
Hello from a function 
```

## Arguments

Information can be passed into functions as arguments.

Arguments are specified after the function name, inside the parentheses. You can add as many arguments as you want, just separate them with a comma.

The following example has a function with one argument (fname). When the function is called, we pass along a first name, which is used inside the function to print the full name:

```python
def my_function(fname):
  print(fname + " Refsnes")

my_function("Emil")
my_function("Tobias")
my_function("Linus")
```
output

```python
Emil Refsnes
Tobias Refsnes
Linus Refsnes 

```

## Number of Arguments

By default, a function must be called with the correct number of arguments. Meaning that if your function expects 2 arguments, you have to call the function with 2 arguments, not more, and not less.

```python
def my_function(fname, lname):
  print(fname + " " + lname)

my_function("Emil", "Refsnes") 
```

output

```python
Emil Refsnes  
```

## Source and References

- [w3schools](https://www.w3schools.com/python/python_functions.asp)
- [realpython](https://realpython.com/)
- [Geek for Geeks ](https://www.geeksforgeeks.org/)
