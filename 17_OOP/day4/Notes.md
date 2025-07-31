## 📘 **Python OOP – Method Overloading & Overriding, issubclass(), super()**

---

### **1. Method Overloading (Same name, different inputs)**

In other languages (like Java, C++), we can write **multiple methods** with the **same name** but **different number of arguments**.

But in Python, we **can’t define multiple methods with the same name**.
If we do, the **last one overwrites** the previous ones.

### So how do we do overloading in Python?

We use **default arguments** or `*args` to simulate method overloading.

---

### Example using default values:

```python
class Calculator:
    def add(self, a=0, b=0, c=0):
        print("Sum:", a + b + c)

obj = Calculator()
obj.add(10, 20)        # Sum: 30
obj.add(5, 5, 5)       # Sum: 15
obj.add()              # Sum: 0
```

🧠 So technically, Python **supports overloading behavior**, but **not real method overloading**.

---

### **2. Method Overriding (Same name, same input, redefined in child class)**

When a **child class** has the **same method** as the **parent class**, and the **child version replaces the parent version** — this is **method overriding**.

---

### Example:

```python
class Animal:
    def speak(self):
        print("Animal speaks")

class Dog(Animal):
    def speak(self):
        print("Dog barks")

d = Dog()
d.speak()   # Output: Dog barks
```

Parent class method is **overridden** in the child class.

---

## **3. `issubclass()` Function**

`issubclass(child_class, parent_class)`
→ Returns `True` if the first class is **inherited from** the second class.

---

### Example:

```python
class A:
    pass

class B(A):
    pass

print(issubclass(B, A))   # True
print(issubclass(A, B))   # False
```

---

## **4. `super()` Function**

`super()` is used to call the **parent class method** from inside the **child class**.

This is useful when you override a method, but still want to run the original method from parent.

---

### Example:

```python
class Person:
    def show(self):
        print("Person class")

class Student(Person):
    def show(self):
        super().show()       # Calls parent method
        print("Student class")

s = Student()
s.show()
```

**Output:**

```
Person class  
Student class
```

`super()` helps to reuse parent functionality even after overriding the method.

---

## Summary

| Topic              | Meaning                                                              |
| ------------------ | -------------------------------------------------------------------- |
| Method Overloading | Same method name, different arguments (simulated using default args) |
| Method Overriding  | Same method in child class (replaces parent’s version)               |
| `issubclass()`     | Checks if a class is a child of another                              |
| `super()`          | Calls parent method inside child class                               |

---

