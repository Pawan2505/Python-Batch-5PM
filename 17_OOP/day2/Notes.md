## 📘 **Topic: Constructor and Destructor in Python**

---

### What is a Constructor?

* A **constructor** is a special method in a class.
* It runs **automatically** when we **create an object**.
* In Python, constructor ka naam hota hai: `__init__()`

> We use constructor to **initialize data** (like name, age, etc.) when the object is created.

---

### Example of Constructor:

```python
class Student:
    def __init__(self, name):
        self.name = name
        print("Object created!")

    def show(self):
        print("Name:", self.name)

s1 = Student("Fatima")   # constructor called here
s1.show()
```

**Output:**

```
Object created!  
Name: Fatima
```

### Note:

* `self` refers to the current object.
* Constructor is called **only once**, when the object is created.

---

### What is a Destructor?

* A **destructor** is a special method that runs **when the object is deleted**.
* In Python, destructor ka naam hota hai: `__del__()`
* We use destructor to **clean up** (like closing files, freeing memory, etc.)

---

### Example of Destructor:

```python
class Student:
    def __init__(self, name):
        self.name = name
        print("Constructor called")

    def __del__(self):
        print("Destructor called for", self.name)

s1 = Student("Pawan")
del s1   # Destructor called here
```

**Output:**

```
Constructor called  
Destructor called for Pawan
```

---

### Key Differences

| Feature      | Constructor (`__init__`) | Destructor (`__del__`)                                    |
| ------------ | ------------------------ | --------------------------------------------------------- |
| When it runs | When object is created   | When object is deleted                                    |
| Purpose      | Initialize variables     | Clean-up work                                             |
| Called by    | Automatically by Python  | Automatically when object is removed or manually by `del` |

---

### Real-Life Example

* **Constructor** → Jab koi student class mein enter karta hai, unka name list mein likhna = `__init__()`
* **Destructor** → Jab student class se bahar jaata hai, unka name list se hata dena = `__del__()`

---


### 🧾 Summary:

* Constructor = `__init__()` → Runs when object is created
* Destructor = `__del__()` → Runs when object is deleted
* Both are special methods (also called magic methods or dunder methods – because they start and end with `__`)

---
