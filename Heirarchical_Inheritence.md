# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `id`, `name`, `gender`
  - Provides methods: inherited by child classes for display

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `company`, `department`
  - Method: `displayEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `hospital`, `department`
  - Method: `displayPatientDetails()`

## 🧠 Algorithm

1. Create a base class Details with common attributes: id, name, gender.
2. Create a child class Employee that inherits from Details and adds company and department.
3. Create a child class Patient that inherits from Details and adds hospital and department.
4. Accept input from the user for employee details.
5. Accept input from the user for patient details.
6. Create objects for Employee and Patient.
7. Call the respective display methods to show details in a formatted way.

## Program
```
# Base class
class Details:
    def __init__(self, id, name, gender):
        self.id = id
        self.name = name
        self.gender = gender

# Derived class 1
class Employee(Details):
    def __init__(self, id, name, gender, company, department):
        super().__init__(id, name, gender)
        self.company = company
        self.department = department

    def displayEmployeeDetails(self):
        print("\nEmployee Object")
        print("Id: ", self.id)
        print("Name: ", self.name)
        print("Gender: ", self.gender)
        print("Company: ", self.company)
        print("Department: ", self.department)

# Derived class 2
class Patient(Details):
    def __init__(self, id, name, gender, hospital, department):
        super().__init__(id, name, gender)
        self.hospital = hospital
        self.department = department

    def displayPatientDetails(self):
        print("\nPatient Object")
        print("Id: ", self.id)
        print("Name: ", self.name)
        print("Gender: ", self.gender)
        print("Hospital: ", self.hospital)
        print("Department: ", self.department)

# Input Employee details
emp_id = input()
emp_name = input()
emp_gender = input()
emp_company = input()
emp_department = input()

# Input Patient details
pat_id = input()
pat_name = input()
pat_gender = input()
pat_hospital = input()
pat_department = input()

# Create objects
employee = Employee(emp_id, emp_name, emp_gender, emp_company, emp_department)
patient = Patient(pat_id, pat_name, pat_gender, pat_hospital, pat_department)

# Display details
employee.displayEmployeeDetails()
patient.displayPatientDetails()

```
## Sample Output
<img width="593" height="447" alt="image" src="https://github.com/user-attachments/assets/d1b6793c-3304-43c7-aa75-a8298f8e46c6" />

## Result
The program successfully demonstrates Hierarchical Inheritance:
