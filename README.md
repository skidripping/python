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
