# **Python Lecture: Creating & Using Modules and Packages**


## **1. Creating a Module**

A **module** is simply a **Python file (.py)** that contains functions, variables, or classes that you can reuse.

**Example – `mymodule.py`**

```python
# mymodule.py

def greet(name):
    return f"Hello, {name}!"

pi = 3.14
```

---

## **2. Importing a Module**

You can use your module in another Python file.

**Example – `main.py`**

```python
import mymodule

print(mymodule.greet("Pawan"))
print("PI value is:", mymodule.pi)
```

---

## **3. Renaming a Module While Importing**

You can give a short name using **`as`**:

```python
import mymodule as mm

print(mm.greet("Pawan"))
print(mm.pi)
```

---

## **4. Importing Specific Items**

```python
from mymodule import greet

print(greet("Pawan"))  # No need for module name now
```

---

## **5. The `__name__` and `__main__` Trick**

In Python, each file has a special variable called **`__name__`**.
When you run a file directly, `__name__` becomes `"__main__"`.
When you import it, `__name__` becomes the **file name**.

**Example – `mymodule.py`**

```python
def greet(name):
    return f"Hello, {name}!"

if __name__ == "__main__":
    # This will run only if this file is executed directly
    print("Running mymodule directly!")
```

**Example – `main.py`**

```python
import mymodule

print(mymodule.greet("Pawan"))
```

💡 **Why use this?**

* Helps write code that **runs only when the file is executed directly**, not when imported.

---

## **6. Creating a Package**

A **package** is just a **folder** containing multiple Python modules, and a special file **`__init__.py`** (can be empty or contain code).

**Folder structure:**

```
mypackage/
    __init__.py
    module1.py
    module2.py
```

---

### **Example**

**`mypackage/module1.py`**

```python
def say_hello():
    return "Hello from module1!"
```

**`mypackage/module2.py`**

```python
def say_hi():
    return "Hi from module2!"
```

**`main.py`**

```python
import mypackage.module1 as m1
import mypackage.module2 as m2

print(m1.say_hello())
print(m2.say_hi())
```

---

## **7. Using `dir()` Function**

`dir()` shows you all the **functions, variables, and classes** inside a module.

```python
import math
print(dir(math))  # Shows everything inside math module
```

---

## **8. The `__init__.py` File**

* This file tells Python **"This folder is a package"**.
* Can be **empty** or contain **startup code** for the package.

**Example – `mypackage/__init__.py`**

```python
print("mypackage is ready to use!")
```

---

## **9. Note:**

| Feature                 | Purpose                                      | Example                      |
| ----------------------- | -------------------------------------------- | ---------------------------- |
| Create Module           | Reusable Python file                         | `mymodule.py`                |
| Import                  | Use module in another file                   | `import mymodule`            |
| Rename                  | Shorter name for module                      | `import mymodule as mm`      |
| Import specific         | Get only needed items                        | `from mymodule import greet` |
| `__name__` & `__main__` | Run code only when file is executed directly | `if __name__ == "__main__":` |
| Package                 | Folder of modules                            | `import mypackage.module1`   |
| `dir()`                 | List contents of module                      | `dir(math)`                  |
| `__init__.py`           | Marks folder as package                      | Can be empty or have code    |

---

