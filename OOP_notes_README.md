
# Python OOP (Object-Oriented Programming) Notes

These notes explain the core Object-Oriented Programming (OOP) concepts in Python with definitions and examples.

---

# Table of Contents

1. Classes and Objects
2. Instance Methods
3. Bank Account Project
4. Inheritance
5. Single Inheritance
6. Multiple Inheritance
7. Polymorphism
8. Method Overriding

---

# 1. Classes and Objects

## Definition

**Object-Oriented Programming (OOP)** is a programming paradigm that uses **objects** to design software. It models real-world entities using **classes** and **objects**.

- **Class:** A blueprint used to create objects.
- **Object:** An instance of a class.
- **Constructor (`__init__`)**: Initializes object attributes automatically when an object is created.

```python
class Dog:
    def __init__(self, name, age):
        self.name = name
        self.age = age

dog1 = Dog("Buddy", 3)
print(dog1.name)
print(dog1.age)
```

---

# 2. Instance Methods

Instance methods operate on object data and always receive `self` as the first parameter.

```python
class Dog:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def bark(self):
        print(f"{self.name} says Woof!")
```

---

# 3. Bank Account Project

This example models a real-world bank account.

Features:
- Deposit
- Withdraw
- Check Balance

---

# 4. Inheritance

Inheritance allows a child class to inherit the attributes and methods of a parent class.

Advantages:
- Code Reusability
- Easy Maintenance
- Extensibility

---

# 5. Single Inheritance

One child class inherits from one parent class.

Example: `Tesla` inherits from `Car`.

---

# 6. Multiple Inheritance

One child class inherits from more than one parent class.

Example: `Dog` inherits from both `Animal` and `Pet`.

---

# 7. Polymorphism

Polymorphism allows different objects to respond differently to the same method name.

It is commonly implemented using **Method Overriding**.

---

# 8. Method Overriding

Method Overriding allows a child class to redefine a method already defined in the parent class.

Example:

```python
class Animal:
    def speak(self):
        return "Animal Sound"

class Dog(Animal):
    def speak(self):
        return "Woof!"

class Cat(Animal):
    def speak(self):
        return "Meow!"
```

Output:

```
Woof!
Meow!
```



---

## Polymorphism

**Definition**

Polymorphism is a core concept of Object-Oriented Programming (OOP) that allows objects of different classes to be treated through a common interface. The same method can perform different actions depending on the object.

**Hinglish:** Ek hi method alag-alag objects ke liye alag behavior perform karta hai.

### Method Overriding
Method Overriding allows a child class to redefine a method already available in its parent class.

Example:
- Animal -> Dog
- Animal -> Cat

### Function-based Polymorphism
Functions can accept different object types as long as they implement the required method.

### Abstract Base Class (ABC)
Abstract Base Classes define a common interface and force child classes to implement required methods.

---

## Encapsulation

**Definition**

Encapsulation means wrapping variables (data) and methods (functions) into a single class while restricting direct access to important data.

### Access Modifiers
- Public
- Protected
- Private

### Getter and Setter
Getter methods read private variables.
Setter methods safely modify private variables.

---

## Abstraction

**Definition**

Abstraction hides implementation details and exposes only the essential functionality.

It is commonly implemented using Abstract Base Classes.

---

## Operator Overloading

Operator Overloading allows operators like +, -, == etc. to work with user-defined objects.

Example:
- __add__()
- __sub__()
- __repr__()

---

## Custom Exceptions

Custom Exceptions are user-defined exceptions created by inheriting from Exception.

They help represent application-specific errors.

Example:
dobException

---

## Custom List

A Custom List is a user-defined dynamic array implementation that helps understand how Python lists work internally.

---

This README is intended as structured notes for Python OOP concepts. Add your full code examples under each topic for a complete study guide.


# Summary
 ## Topics
 
- Classes
- Objects
- Constructors
- Instance Methods
- Inheritance
- Single Inheritance
- Multiple Inheritance
- Polymorphism
- Method Overriding
- Polymorphism
- Method Overriding
- Polymorphism with Functions
- Polymorphism with Abstract Base Class (ABC)
- Encapsulation
- Public, Protected and Private Variables
- Getter and Setter
- Abstraction
- Operator Overloading
- Custom Exceptions
- Custom List


These concepts are the foundation of Object-Oriented Programming in Python.
