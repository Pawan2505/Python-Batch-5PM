# **Modules & Packages (datetime & time)**


## **1. What is a Module in Python?**

A **module** is just a **Python file** that contains code — variables, functions, and classes — that you can **reuse** in your programs.

Example:

* Python comes with many built-in modules like `math`, `os`, `random`, `datetime`, `time`.
* You can also create your own module.

💡 **Importing a module:**

```python
import module_name
```

---

## **2. What is a Package in Python?**

A **package** is a **collection of modules** kept together in a folder with a special file called `__init__.py`.

Think of it like:

* **Module** → one tool
* **Package** → a toolbox full of tools

Example:

* The `datetime` module is part of the **Python Standard Library** package.

---

## **3. The `datetime` Module**

The `datetime` module helps us work with **dates** and **times**.

### **Importing datetime**

```python
import datetime
```

---

### **Get Current Date & Time**

```python
import datetime

now = datetime.datetime.now()
print(now)  # Example: 2025-07-31 19:15:22.123456
```

---

### **Get Today’s Date Only**

```python
today = datetime.date.today()
print(today)  # Example: 2025-07-31
```

---

### **Access Year, Month, Day**

```python
d = datetime.date.today()
print("Year:", d.year)
print("Month:", d.month)
print("Day:", d.day)
```

---

### **Formatting Date & Time**

```python
now = datetime.datetime.now()
print(now.strftime("%d/%m/%Y"))  # 31/07/2025
print(now.strftime("%I:%M %p"))  # 07:15 PM
```

---

### **Create Your Own Date**

```python
custom_date = datetime.date(2023, 5, 10)
print(custom_date)  # 2023-05-10
```

---

### **Date Difference**

```python
d1 = datetime.date(2025, 8, 1)
d2 = datetime.date(2025, 7, 31)
diff = d1 - d2
print("Difference in days:", diff.days)  # 1
```

---

## **4. The `time` Module**

The `time` module helps us work with **time-related tasks** like sleeping, measuring execution time, etc.

---

### **Importing time**

```python
import time
```

---

### **Get Current Time in Seconds**

```python
seconds = time.time()
print(seconds)  # Example: 1733062715.123
```

(Useful for measuring speed of code.)

---

### **Sleep / Delay Program**

```python
print("Hello")
time.sleep(3)  # Wait 3 seconds
print("World")
```

---

### **Get Local Time**

```python
local = time.localtime()
print(local)
```

---

### **Formatted Local Time**

```python
formatted = time.strftime("%d-%m-%Y %H:%M:%S", time.localtime())
print(formatted)  # Example: 31-07-2025 19:15:00
```

---

### **Measure Execution Time**

```python
start = time.time()

# Some code to test
for i in range(1000000):
    pass

end = time.time()

print("Time taken:", end - start, "seconds")
```

---

## **5. Note:**

| Module     | Purpose                 | Example                   |
| ---------- | ----------------------- | ------------------------- |
| `datetime` | Work with dates & times | `datetime.datetime.now()` |
| `time`     | Time-related tasks      | `time.sleep(2)`           |
| `strftime` | Format date/time        | `%d/%m/%Y`                |
| `time()`   | Seconds since 1970      | `time.time()`             |

---

