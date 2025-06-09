## Python – **Exception Handling**

---

### What is an Exception?

An **exception** is an **error** that occurs during program execution.

🔸 Example:

```python
a = 10 / 0   # ZeroDivisionError
```

Without handling, your program **stops** when an error occurs.

---

### Why Use Exception Handling?

To:

* Avoid program crash
* Show user-friendly error messages
* Handle errors gracefully

---

### try–except Block

```python
try:
    # risky code here
    a = 10 / 0
except:
    print("Something went wrong")
```

If an error occurs in `try`, the `except` block runs.

---

### Handling Specific Exceptions

You can catch specific types of errors:

```python
try:
    a = int("abc")
except ValueError:
    print("Only numbers allowed!")
```

```python
try:
    a = 5 / 0
except ZeroDivisionError:
    print("Cannot divide by zero")
```

---

### else Block

Runs **only if there is no error**:

```python
try:
    a = 10 / 2
except:
    print("Error occurred")
else:
    print("Success! No error")  # Runs if no error
```

---

### finally Block

This block **always runs**, whether there's an error or not:

```python
try:
    a = 10 / 2
except:
    print("Error")
finally:
    print("This will always run")  # Always runs
```

🔹 Good for **closing files**, **clean-up code**, etc.

---

### Using `raise` to Trigger Your Own Error

You can manually raise an error:

```python
x = -1
if x < 0:
    raise ValueError("Negative value not allowed")
```

---

### Example

```python
try:
    num = int(input("Enter a number: "))
    result = 10 / num
except ValueError:
    print("Please enter a valid number.")
except ZeroDivisionError:
    print("Can't divide by 0.")
else:
    print("Result is:", result)
finally:
    print("Program ended.")
```

---

### Summary

| Keyword   | Purpose                     |
| --------- | --------------------------- |
| `try`     | Code to test for error      |
| `except`  | Code to run if error occurs |
| `else`    | Runs if no error in try     |
| `finally` | Always runs                 |
| `raise`   | Manually throw an exception |

---

