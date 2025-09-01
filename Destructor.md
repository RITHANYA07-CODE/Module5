# Destructor in Python

This project demonstrates how to implement a **destructor** in Python using a simple class.

## 🚀 Overview

The program defines a class `Demo` with:

- A **constructor** `__init__` that initializes an instance variable and prints a message.
- A **destructor** `__del__` that prints a message when the object is destroyed.

## 🧠 Algorithm

1. Define a class named `Demo`.
2. Inside the class, define the `__init__` method:
   - Initialize an instance variable `status` with the value `"Alive"`.
   - Print the value of `status`.
3. Define the `__del__` method:
   - Print a message indicating the object is being destroyed.
4. Outside the class:
   - Create an instance of the `Demo` class.
   - Delete the object using the `del` keyword.
## Program
```
class Demo:
    
    def __init__(self):
        self.status = "Alive"
        
    def __del__(self):
        print("The object no longer exists")
    
obj = Demo()
# The status has been initialized to Alive
print(obj.status)
# This calls the destructor
del obj
```
## 🧪 Output
<img width="934" height="178" alt="image" src="https://github.com/user-attachments/assets/d3e039f4-66fd-4ee8-a256-b476861335a3" />

## Result
The program successfully demonstrates the use of a destructor in Python.
