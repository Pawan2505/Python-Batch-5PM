### Q.1
**Question:** What is type casting in Python, and why is it used? Explain the difference between implicit type casting and explicit type casting with examples.  

**Answer:** Type casting in Python is converting one data type to another. It is used to ensure compatibility between operations. Implicit type casting (automatic) happens without user intervention (e.g., `int` to `float`), while explicit type casting requires manual conversion (e.g., using `int()`).  
- Example: Implicit: `x = 5 + 3.0` (result is `8.0`); Explicit: `x = int("5")`.

### Q.2
**Question:** What are type-casting constructors? List some commonly used type-casting constructors in Python.  

**Answer:** Type-casting constructors are functions that convert data types. Commonly used ones in Python: `int()`, `float()`, `str()`, `bool()`.

### Q.3
**Question:** What happens if you use `int()` on a string containing non-numeric characters?  

**Answer:** Using `int()` on a string with non-numeric characters raises a `ValueError`.  
- Example: `int("12a")` raises `ValueError: invalid literal for int() with base 10: '12a'`.

### Q.4
**Question:** What is the purpose of the `str()` constructor? Provide examples of converting numeric types to strings.  

**Answer:** The `str()` constructor converts values to strings, useful for display or concatenation.  
- Examples: `str(5)` → `"5"`, `str(3.14)` → `"3.14"`.

### Q.5
**Question:** Write a Python program that demonstrates the use of `int()`, `float()`, `str()`, `bool()`, and `complex()` constructors.  

**Answer:**  
```python
i = int("123")
f = float("123.45")
s = str(123)
b = bool(1)
c = complex(1, 2)
print("int:", i, "float:", f, "str:", s, "bool:", b, "complex:", c)
```

### Q.6
**Question:** What is the purpose of the `id()` function in Python? Explain how the `id()` function can be used to verify the identity of an object.  

**Answer:** The `id()` function returns the memory address of an object, used to verify object identity.  
- Example: `x = 10; print(id(x))` shows the address; `y = x; print(id(y) == id(x))` (True if same object).

### Q.7
**Question:** Write a Python program to demonstrate how the `id()` function changes when a variable is reassigned.  

**Answer:**  
```python
x = [1, 2]
print("Initial id:", id(x))
x = [3, 4]  # Reassignment creates new object
print("After reassignment id:", id(x))  # New id
```

### Q.8
**Question:** What does the `type()` function do in Python? How can the `type()` function be used to check the data type of a variable? Provide examples.  

**Answer:** The `type()` function returns the data type of a variable, used to check types.  
- Examples: `type(5)` → `<class 'int'>`, `type("hello")` → `<class 'str'>`.  
- Use: `if type(x) == int: print("Integer")`.