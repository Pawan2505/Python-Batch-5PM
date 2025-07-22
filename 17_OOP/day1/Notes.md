## 📘 **Object Oriented Programming (OOP) in Python**

**Topics:**

* Class & Object
* `self` and `del` keyword
* Encapsulation

---

### What is OOP?

OOP stands for **Object Oriented Programming**.
It is a style of writing programs where we use **real-world thinking**.

We use objects and classes to represent things like students, cars, bank accounts, etc.

OOP helps us to keep code clean, reusable, and organized.

---

## **1. Class and Object**

### What is a Class?

* A class is like a **blueprint** or **template**.
* It describes **how an object should be** — what data it should have and what it can do.

> Example: Student class → should have name, age, and a method to show info.

### What is an Object?

* Object is the **actual thing** created from the class.
* You can make many objects from one class.

### Example:

```python
class Student:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def show(self):
        print("Name:", self.name)
        print("Age:", self.age)

s1 = Student("Roshni", 20)
s1.show()
```

**Output:**

```
Name: Roshni  
Age: 20
```

---

## **2. What is `self` keyword?**

* `self` means **current object**.
* It is used inside the class to **refer to the object** that is calling the method.

```python
def show(self):
    print(self.name)
```

* Jab hum `s1.show()` likhte hain, toh `self` = `s1`.

---

## **3. What is `del` keyword?**

* `del` is used to **delete** an object.

```python
s1 = Student("Pawan", 21)
del s1
```

* Ab agar aap `s1.show()` likhenge, toh error aayega because `s1` has been deleted.

---

## **4. What is Encapsulation?**

* Encapsulation means **hiding the data**.
* We protect the data so that **nobody can directly access it** from outside the class.
* We give access through methods (functions).

### Example:

```python
class BankAccount:
    def __init__(self, balance):
        self.__balance = balance  # private variable

    def show_balance(self):
        print("Balance:", self.__balance)

    def deposit(self, amount):
        if amount > 0:
            self.__balance += amount

acc = BankAccount(1000)
acc.show_balance()       # 1000
acc.deposit(500)
acc.show_balance()       # 1500
```

### Direct access is not allowed:

```python
print(acc.__balance)  # Error
```

---

## Summary:

| Concept       | Explanation                         |
| ------------- | ----------------------------------- |
| Class         | Blueprint or template               |
| Object        | Real object made from class         |
| `self`        | Refers to current object            |
| `del`         | Deletes the object                  |
| Encapsulation | Hiding data using private variables |

---


