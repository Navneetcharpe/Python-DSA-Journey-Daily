
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

# Summary

- Classes
- Objects
- Constructors
- Instance Methods
- Inheritance
- Single Inheritance
- Multiple Inheritance
- Polymorphism
- Method Overriding

These concepts are the foundation of Object-Oriented Programming in Python.
