## Variables and Data Types

---

### Declaring Variables in Python

In Python, you **don’t need to declare the type** of variable.
You can directly assign a value.

Example:

```python
name = "Pawan"
age = 21
price = 49.99
```

Here:

* `name` is a string
* `age` is an integer
* `price` is a float

Python automatically understands the type based on the value.

---

### Dynamic Typing

Python is a **dynamically typed language**, which means:

* You don’t have to tell Python what type the variable is.
* You can even **change the type later** by assigning a new value.

Example:

```python
x = 5        # x is an integer
x = "hello"  # now x is a string
```

No error will occur. Python allows this flexibility.

---

### Basic Data Types in Python

1. **int** – Integer numbers (without decimal)

```python
a = 10
```

2. **float** – Numbers with decimal point

```python
b = 3.14
```

3. **str** – String (text or characters inside quotes)

```python
name = "Fatima"
```

4. **bool** – Boolean values: `True` or `False`

```python
is_student = True
```

5. **complex** – Complex numbers like `a + bj`

```python
z = 2 + 3j
```

---

### Type Casting (Type Conversion)

You can **change data types** using functions:

* `int()` – to convert to integer
* `float()` – to convert to float
* `str()` – to convert to string
* `bool()` – to convert to boolean

Example:

```python
x = "10"
y = int(x)     # Converts string "10" to integer 10
z = float(x)   # Converts to 10.0
```

Another example:

```python
num = 5
print(str(num))    # Output: "5" as a string
```

---

### `type()` Function

Use the `type()` function to **check the data type** of a variable.

Example:

```python
a = 10
b = "hello"
print(type(a))   # Output: <class 'int'>
print(type(b))   # Output: <class 'str'>
```

This helps you understand what type a variable currently holds.

---

### Summary:

| Data Type | Example      | Description    |
| --------- | ------------ | -------------- |
| int       | 10           | Whole number   |
| float     | 3.14         | Decimal number |
| str       | "Pawan"      | Text/string    |
| bool      | True / False | Boolean value  |
| complex   | 2 + 3j       | Complex number |

---

