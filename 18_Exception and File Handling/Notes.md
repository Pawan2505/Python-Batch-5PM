

# **Exception & File Handling in Python**


## **1. What is an Exception?**

Imagine you’re writing Python code and suddenly—boom 💥—an error occurs while running it.
This unexpected situation is called an **Exception**.

💡 **In simple words:**

> Exception = A run-time error that stops your program unless you handle it.

---

### **Common Examples of Exceptions:**

* Dividing by zero → `ZeroDivisionError`
* Accessing a file that doesn’t exist → `FileNotFoundError`
* Using a variable that isn’t defined → `NameError`
* Converting `"abc"` to integer → `ValueError`

---

## **2. Why Handle Exceptions?**

If you **don’t handle exceptions**, Python will:

1. Stop the program immediately
2. Print an error message

If you **handle exceptions**, Python will:

1. Catch the error 
2. Let you control what happens next

---

## **3. try … except**

The most basic way to handle exceptions.

**Syntax:**

```python
try:
    # Code that might cause an error
except:
    # What to do if an error happens
```

**Example:**

```python
try:
    num = int(input("Enter a number: "))
    result = 10 / num
    print("Result:", result)
except:
    print("Oops! Something went wrong.")
```

---

## **4. try … except … else**

Here, the **else block** runs **only if there is no exception**.

**Syntax:**

```python
try:
    # risky code
except:
    # handle error
else:
    # runs only if try succeeds
```

**Example:**

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

The **finally block** runs **no matter what happens** —
whether there’s an exception or not.

**Syntax:**

```python
try:
    # risky code
except:
    # handle error
finally:
    # always runs
```

**Example:**

```python
try:
    f = open("data.txt", "r")
    content = f.read()
    print(content)
except FileNotFoundError:
    print("File not found!")
finally:
    print("Closing file... Done!")
```

---

## **6. try … except … else … finally**

Yes! You can combine them all.

**Example:**

```python
try:
    num = int(input("Enter a number: "))
    result = 10 / num
except ZeroDivisionError:
    print("Cannot divide by zero!")
except ValueError:
    print("Invalid input! Please enter a number.")
else:
    print("Result is:", result)
finally:
    print("Thank you for using my program.")
```

---

## **7. File Handling with Exception Handling**

When working with files, exceptions are common — like missing files, permission issues, etc.

**Example:**

```python
try:
    with open("mydata.txt", "r") as file:
        data = file.read()
        print("File content:")
        print(data)
except FileNotFoundError:
    print("The file does not exist!")
except PermissionError:
    print("You don't have permission to open this file.")
finally:
    print("Operation finished.")
```





