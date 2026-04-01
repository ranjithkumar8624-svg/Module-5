# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
class Details: def init(self): self.__id="" self.__name="" self.__gender="" def
setData(self,id,name,gender): self.__id=id self.__name=name self.__gender=gender def
showData(self): print("Id: ",self.__id) print("Name: ", self.__name) print("Gender: ",
self.__gender) class Employee(Details): #Inheritance def init(self): self.__company=""
self.__dept="" def setEmployee(self,id,name,gender,comp,dept):
self.setData(id,name,gender) self.__company=comp self.__dept=dept def
showEmployee(self): self.showData() print("Hospital: ", self.__company)
print("Department: ", self.__dept) class Patient(Details): #Inheritance def init(self):
self.__hospital="" self.__dept="" def setEmployee(self,id,name,gender,hos,dept):
self.setData(id,name,gender) self.__hospital=hos self.__dept=dept def
showEmployee(self): self.showData() print("Hospital: ", self.__hospital)
print("Department: ", self.__dept) id=int(input()) name=input() gender=input()
comp=input() dept=input() id1=int(input()) nam=input() gen=input() hosp=input()
dep=input() print("Doctor Object") e=Employee()
e.setEmployee(id,name,gender,comp,dept) e.showEmployee() print("\nPatient Object") d
= Patient() d.setEmployee(id1, nam, gen, hosp, dep) d.showEmployee()
## Sample Output
<img width="650" height="308" alt="image" src="https://github.com/user-attachments/assets/fca105dc-f0cf-42bb-8614-a0825e5b6980" />
## Result
Thus, the program has been successfully executed.
