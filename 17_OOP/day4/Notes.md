# **Python Lecture: Exception & File Handling**


## **1. What is an Exception?**

An **exception** is just a fancy word for **error** that happens while your program is running.

Example of common exceptions:

* Dividing by zero → `ZeroDivisionError`
* File not found → `FileNotFoundError`
* Wrong data type → `ValueError`

When an exception happens, your program will **stop** unless you handle it.

---

## **2. Why Handle Exceptions?**

If you don’t handle them:

* Program stops 

If you do handle them:

* Program continues 
* You can show a friendly message to the user

---

## **3. try … except**

Basic way to handle an error.

```python
try:
    num = int(input("Enter a number: "))
    result = 10 / num
    print(result)
except:
    print("Oops! Something went wrong.")
```

---

## **4. try … except … else**

The **else** block will run **only if no error happens**.

```python
try:
    num = int(input("Enter a number: "))
    result = 10 / num
except ZeroDivisionError:
    print("You can't divide by zero!")
except ValueError:
    print("Please enter a valid number!")
else:
    print("Result is:", result)
```

---

## **5. try … except … finally**

The **finally** block always runs, whether there’s an error or not.
Mostly used for cleanup like closing files.

```python
try:
    f = open("data.txt", "r")
    print(f.read())
except FileNotFoundError:
    print("File not found!")
finally:
    print("Done reading file.")
```

---

## **6. try … except … else … finally**

You can combine all of them.

```python
try:
    num = int(input("Enter a number: "))
    result = 10 / num
except ZeroDivisionError:
    print("Cannot divide by zero!")
except ValueError:
    print("Invalid number!")
else:
    print("Result is:", result)
finally:
    print("Thank you for using this program.")
```

---

## **7. raise – Throw Your Own Error**

You can make your own error happen if something is wrong.

```python
age = int(input("Enter your age: "))
if age < 18:
    raise ValueError("You must be 18 or older.")
else:
    print("Welcome!")
```

---

## **8. assert – Quick Checks**

`assert` checks if something is true.
If it’s not true, it stops the program with an error.

```python
x = int(input("Enter a positive number: "))
assert x > 0, "Number must be positive!"
print("You entered:", x)
```

---

## **9. Custom Exceptions – Your Own Error Type**

You can make your own type of error for special cases.

```python
class NegativeNumberError(Exception):
    pass

num = int(input("Enter a positive number: "))
if num < 0:
    raise NegativeNumberError("Negative numbers are not allowed!")
else:
    print("You entered:", num)
```

---

## **10. File Handling with Exceptions**

```python
try:
    with open("mydata.txt", "r") as file:
        print(file.read())
except FileNotFoundError:
    print("File not found!")
except PermissionError:
    print("You don’t have permission.")
finally:
    print("Program ended.")
```

---

### **Note:**

| Keyword          | Meaning               | Use                     |
| ---------------- | --------------------- | ----------------------- |
| try              | Test a block of code  | Write risky code        |
| except           | Catch the error       | Show friendly message   |
| else             | Run if no error       | Show success            |
| finally          | Always run            | Cleanup work            |
| raise            | Create your own error | Check custom conditions |
| assert           | Quick condition check | Stop if false           |
| Custom Exception | Your own error type   | Special cases           |

---

