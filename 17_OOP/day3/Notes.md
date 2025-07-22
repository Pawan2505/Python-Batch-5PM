# 📘 Python OOP – Part 2

### Topics:

* Types of Inheritance
* Reflection Enabling Functions
* Nested Function

---

## 🧬 **1. Types of Inheritance in Python**

Inheritance means one class can **use properties and methods** of another class.
The existing class is called **Parent (Base)**, and the new class is called **Child (Derived)**.

---

### a) **Single Inheritance**

One child class inherits from one parent class.

```python
class Parent:
    def speak(self):
        print("I am Parent")

class Child(Parent):
    pass

c = Child()
c.speak()
```

---

### b) **Multilevel Inheritance**

Child → Parent → Grandparent

```python
class Grandparent:
    def who(self):
        print("I am Grandparent")

class Parent(Grandparent):
    pass

class Child(Parent):
    pass

c = Child()
c.who()
```

---

### c) **Multiple Inheritance**

One child inherits from **multiple parents**.

```python
class A:
    def showA(self):
        print("A class")

class B:
    def showB(self):
        print("B class")

class C(A, B):
    pass

obj = C()
obj.showA()
obj.showB()
```

---

### d) **Hierarchical Inheritance**

One parent → many children

```python
class Parent:
    def speak(self):
        print("Parent speaking")

class Child1(Parent):
    pass

class Child2(Parent):
    pass

c1 = Child1()
c2 = Child2()

c1.speak()
c2.speak()
```

---

### e) **Hybrid Inheritance**

Combination of multiple types.

```python
# Mix of multiple and multilevel
```

> Note: In complex cases, Python uses **MRO (Method Resolution Order)** to decide which method to call.

---

## **2. Reflection Enabling Functions in Python**

Reflection means checking or modifying the program **at runtime**.

Python provides some built-in **functions** for this:

| Function    | Use                                 |
| ----------- | ----------------------------------- |
| `type(obj)` | Returns the type/class of object    |
| `id(obj)`   | Returns memory address of object    |
| `hasattr()` | Checks if object has that attribute |
| `getattr()` | Gets the value of an attribute      |
| `setattr()` | Sets or updates the attribute value |
| `delattr()` | Deletes an attribute                |

---

### Example:

```python
class Student:
    def __init__(self):
        self.name = "Pawan"

s = Student()

print(type(s))              # <class '__main__.Student'>
print(hasattr(s, 'name'))   # True
print(getattr(s, 'name'))   # Pawan

setattr(s, 'age', 20)
print(s.age)                # 20

delattr(s, 'name')
print(hasattr(s, 'name'))   # False
```

---

## **3. Nested Function**

A function **inside another function** is called a nested function.

---

### Why use nested functions?

* To keep code clean and organized
* To use **inner functions** only inside outer ones
* To implement closures

---

### Example:

```python
def outer():
    print("This is outer function")

    def inner():
        print("This is inner function")

    inner()

outer()
```

**Output:**

```
This is outer function  
This is inner function
```

---

## Summary

| Topic           | Key Point                                      |
| --------------- | ---------------------------------------------- |
| Inheritance     | Allows child class to use parent class methods |
| Reflection      | Let us check/change object at runtime          |
| Nested Function | Function inside another function               |

---




Happy to help! 😊
