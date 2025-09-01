# # Constructors in Python: Welcome Message with Student Name

## 🎯 Aim
To write a Python program that creates a **Student** class with a **default constructor** and a method to display a welcome message along with the student’s name provided by the user.

## 🧠 Algorithm
1. **Get user input**: Accept the student's name from the user.
2. **Define the class**: Create a class `Student` with a default constructor (`__init__`).
3. **Default Constructor**: In the constructor, assign the user input (student name) to an instance variable `self.a`.
4. **Display Message**: Define a method `display` that prints "This is non-parameterized constructor" and a welcome message with the student’s name.
5. **Execute the Program**: Instantiate the `Student` class and call the `display` method.

## 🧾 Program
```
class student:
    
    #default constructor
    def __init__(self):
        print("This is non parametrized constructor")
        
    def display(self, name):
        print("Hello", name)
        
obj = student()
student_name = input()
obj.display(student_name)
```
## Output
<img width="1088" height="244" alt="image" src="https://github.com/user-attachments/assets/584b11ae-43e9-42ae-a5b2-3154e52106c6" />

## Result
The program successfully creates a Student class with a default constructor and displays a personalized welcome message with the student’s name entered by the user.
