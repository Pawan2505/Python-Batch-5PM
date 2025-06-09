## Conditional Statements in Python

Conditional statements allow us to **make decisions in code** based on conditions.

In Python, we mainly use:

* `if`
* `if-else`
* `if-elif-else`
* Nested `if`

Let’s understand each one step by step.

---

### 1. `if` Statement

The `if` statement is used when you want to do something **only if a condition is true**.

```python
age = 18

if age >= 18:
    print("You are eligible to vote")
```

* If the condition (`age >= 18`) is `True`, it runs the print line.
* Indentation is important! The print statement is **inside the if block**.

---

### 2. `if-else` Statement

Used when you want to do **one thing if condition is true**, and **something else if it's false**.

```python
age = 16

if age >= 18:
    print("You can vote")
else:
    print("You cannot vote")
```

* `if` checks the condition
* `else` handles the opposite case

---

### 3. `if-elif-else` Ladder

Used when you have **multiple conditions to check**, one after another.

```python
marks = 75

if marks >= 90:
    print("Grade: A")
elif marks >= 75:
    print("Grade: B")
elif marks >= 60:
    print("Grade: C")
else:
    print("Grade: D")
```

* Python checks conditions one by one
* As soon as one condition is `True`, it stops checking the rest

---

### 4. Nested `if` (if inside another if)

Sometimes, we need to check **more than one condition** inside each other.

```python
num = 10

if num > 0:
    if num % 2 == 0:
        print("Positive Even Number")
    else:
        print("Positive Odd Number")
else:
    print("Negative Number")
```

* First it checks if `num > 0`
* Then inside that, it checks if `num` is even or odd

---

### Example Program

```python
username = input("Enter username: ")
password = input("Enter password: ")

if username == "admin":
    if password == "1234":
        print("Login successful")
    else:
        print("Incorrect password")
else:
    print("Invalid username")
```

---

### Summary:

| Statement      | Use Case                                     |
| -------------- | -------------------------------------------- |
| `if`           | Only when condition is true                  |
| `if-else`      | Do this if true, otherwise do something else |
| `if-elif-else` | Multiple choices or levels                   |
| `nested if`    | When one condition depends on another        |

---

