# What I Learn Today

## Command Line Argument  (Sys Module)
1. Command Line Arguments

These are values passed when running the Python file from terminal.

2. sys module 

it is inbuil module, which is used for command line argument

***Exampal:***

```python
# Command Line Argument 
import sys

def add(n1 , n2):
    add = n1 + n2
    return  add

def sub(n1, n2):
    sub = n1 - n2
    return sub

def mul(n1, n2):
    mul = n1 * n2
    return  mul

#Pass the argument using Sys Library

n1 = float(sys.argv[1])
operation = sys.argv[2]
n2 = float(sys.argv[3])

if operation == "add":
    output = add(n1, n2)
    print(output)

if operation == "sub":
    output = sub(n1, n2)
    print(output)

if operation == "mul":
    output = mul(n1, n2)
    print(output)
```


## Environment Variables (Use the os module.)

Environment variables are system-level variables stored outside the program.

They are commonly used for:

-Passwords

-API keys

-Database URLs

***Exampal:***

```python
import os
print(os.getenv("Password"))
print(os.getenv("apitoken"))
```