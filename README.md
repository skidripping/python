# Introduction
Python is a high level language used for anything software, as in cli projects, ai, cryptography, etc...
It has multiple uses, it's not only those specified.
# Upsides
 - Easy to learn
 - A lot of support & developers
 - High memory safety
# Downsides
 - Slow sometimes
 - Uses alot of the CPU if not managed right
 - not good for compiling applications (easy to decompile)
 - 99% of compiled apps have been detected as malware in python
# Basics
## Printing
```python
print ("Hello World!")
```
`print()` is your standard output function, it basically prints the given object to your terminal screen

## Variables
```python
message = "Hello!"
username = "root"

print (f"{message} {root}")
```
the thing we provided aka `f` is a f-string, it's used to put in variables easily using brackets aka `{variable}` or even functions `{os.system("clear")`


Or if you want to print a variable by itself
```python
message = "I'm lonely!"

print(message)
```
## User input
```python
username = input("username> ")
print("Hello "+username+"!")
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
