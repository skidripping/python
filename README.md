# Contributors
[caden](https://discord.gg/users/941864953965592636)

[virtual](https://t.me/skidripping)
# Introduction
Python is a high level language used for anything software, as in cli projects, ai, cryptography, etc...
It has multiple uses, it's not only those specified.
# Upsides
 - Easy to learn
 - A lot of support & developers
 - High memory safety
 - Almost like English syntax
# Downsides
 - Slow sometimes
 - Uses alot of the CPU if not managed right
 - not good for compiling applications (easy to decompile)
 - 99% of compiled apps have been detected as malware in python
# Basics
## Data types
Text: `str`\
Numeric: `int`, `float`, `complex`\
Sequence Types:	`list`, `tuple`, `range`\
Mapping Type: `dict`\
Set Types: `set`, `frozenset`\
Boolean Type: `bool`\
Binary Types: `bytes`, `bytearray`, `memoryview`\
None Type: `NoneType`
## Printing
```python
print("Hello World!")
```
`print()` is your standard output function, it basically prints the given object to your terminal screen
## Comments
Comments is basically as it's said, putting comments in your code, parts of code that don't get called by the interpreter
```python
# Wow that's a comment

"""
Wow I'm a comment too!!
"""

print("comments didn't get called?!?")
```
## Variables
```python
message = "Hello!"
username = "root"
print (f"{message} {root}")
```
the thing we provided aka `f` is a f-string, it's used to put in variables easily using brackets aka `{variable}` or even functions `{os.system("clear")}`


Or if you want to print a variable by itself
```python
message = "I'm lonely!"
print(message)
```
Or assign multiple variables and give them one value
```python
x, y, z = "wow we all are the same that's cool!"
```
## User input
```python
username = input("username> ")
print(f"Hello {username}")
```
`input()` is your standard input handler, it gets the data written to the terminal and stores it to a variable (if you set it to a variable, otherwise it wouldnt get stored)
## Arrays
There is two types of arrays, you have lists, and tuples
Let's start with lists then at the end of both we will compare each of them and go in depth
### Lists
A list is a data structure in Python that is a mutable, or changeable, ordered sequence of elements. Each element or value that is inside of a list is called an item
```python
mylist = ["Aaron", "Jake", "Markus", "Carroll"]
print(mylist[3])
```
Note: it starts from 0, so basically if you type `print(mylist[0])` it should print `Aaron`
### Tuples
Tuples are used to store multiple items in a single variable. Tuple is one of 4 built-in data types in Python used to store collections of data, the other 3 are List, Set, and Dictionary, all with different qualities and usage. A tuple is a collection which is ordered and unchangeable.
```python
mytuple = ("apple", "banana", "cherry")
```
With index numbers aka `[0]` it's the same for tuples.
### Differences
The differences between tuples and lists are, lists are changable, tuples are not, tuples are more memory efficient, tuples are also time efficient aswell.
## `if`/`else`/`elif` statements
### `if` statements
If statements help you run functions when a specific thing happens, or a specific thing matches, etc...
```python
if 1 == 1:
    print("1 does equal 1!")
```
### `else` statements
```python
username = input("username> ")
if username == "virtual":
    print("Hey, you made this documentation!")
else:
    print("Hey!, Your not virtual but your cool too!")
```
### `elif` statements
```python
username = input("username> ")
if username == "virtual":
    print("Hey, you made this documentation!")
elif username == "skidripping":
    print("Well, your virtual, just a different username!")
else:
    print("Hey, you're not virtual but you're cool too!")
```
## Loops
### `for` loops
A for loop is used for iterating over a sequence (that is either a list, a tuple, a dictionary, a set, or a string).\
In this example, you will see how `items` would be a element of the `list` list, and you are iterating over `list`.
```python
list = ["caden", "layta", "virtual"]
for items in list:
    print(items)
```
```python
Output:
caden
layta
virtual
```
### Looping through a string
Strings are iterable objects, they contain a sequence of characters and work with for loops.\
In this example, you will see how `letters` would be a string, and you are iterating over `"caden"`.
```python
for letters in "caden":
    print(letters)
```
```python
Output:
c
a
d
e
n
```
### `for` loop in `range()`
To loop through a set of code a specified number of times, we can use the `range()` function, The `range()` function returns a sequence of numbers, starting from 0 by default, and increments by 1, and ends at a specified integer. Example below:
```python
for numbers in range(6):
    print(numbers)
```
```python
Output:
0
1
2
3
4
5
```
### `while` loops
a `while` loop is used for an unknown number of times until a specific condition is met, and that's used through `break`/`continue` statements, that is mentioned right after this section
```python
while 1==1:
    print("haha funny")
    if 1==2:
    print("1 will never become 2, i will always keep looping :(")
    break
```
### `break`/`continue` statements
#### `break` statements
A break statement is used for ending loops overall, it can be used with a specified if statement of your choosing
```python
for i in range(15):
    if i == 10:
        break
```
or
```python
for letter in "skid":
    if letter == "i":
        print("you are about to say skid, breaking the statement")
        break
```
#### `continue` statements
A continue statements, well as advertised used to continue loops, but it skips the rest of the code and just continues the loop to the next iteration
```python
for letter in "skiddy":
    if letter == "d":
        print("hey!, you called me a skid, but i'll let it pass i'm not butthurt")
        continue
```
## Functions
Creating a function is quite simple, it can be done with one line of code
```python
def function(arguments):
    print("function has been ran!")

function(argument)
```
The terms parameter and argument can be used for the same thing: information that are passed into a function. From a function's perspective: A parameter is the variable listed inside the parentheses in the function definition. An argument is the value that are sent to the function when it is called.
### `global` statements
The `global` statement is used so you could bring a local variable and turn it into a global variable, it's pretty neat to use.
```python
def function():
    global love
    love = "haha love is cool"
    print("love was set")

function()
print(love)
```
## Classes
```python
class MyClass:
    x = 4

print(MyClass.x)
```
### `__init__()` function
The examples above are classes and objects in their simplest form, and are not really useful in real life applications.
To understand the meaning of classes we have to understand the built-in `__init__()` function.
All classes have a function called `__init__()`, which is always executed when the class is being initiated.
Use the `__init__()` function to assign values to object properties, or other operations that are necessary to do when the object is being created:
```python
class MyClass:
    def __init__():
        print("Hello, you have called the class!")

MyClass()
```
### `self` object
The self parameter is a reference to the current instance of the class, and is used to access variables that belongs to the class.
It does not have to be named self , you can call it whatever you like, but it has to be the first parameter of any function in the class:
```python
class Person:
  def __init__(mysillyobject, name, age):
    mysillyobject.name = name
    mysillyobject.age = age

  def myfunc(abc):
    print("Hello my name is " + abc.name)

p1 = Person("John", 36)
p1.myfunc()
```
