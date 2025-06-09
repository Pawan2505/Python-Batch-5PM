## Python Syntax and Comments

---

### Writing Your First Python Program

To write and run Python code, you can use any IDE or even a simple text editor.

Let’s write our first program:

```python
print("Hello, World!")
```

* This line tells Python to display the message `Hello, World!`
* `print()` is used to show output on the screen.

You can save this code in a file named `hello.py` and run it using the command:

```bash
python hello.py
```

---

### Indentation in Python

**Indentation means space at the beginning of a line.**

* In Python, indentation is **very important**. It tells Python which code belongs to which block.
* Other programming languages use `{}` for blocks, but Python uses **indentation** instead.

Example:

```python
if 10 > 5:
    print("10 is greater than 5")
```

* The second line is **indented**, which means it belongs to the `if` block.
* If you don’t indent correctly, Python will give an error.

Wrong indentation example:

```python
if 10 > 5:
print("10 is greater than 5")  # This will give an error
```

---

### Single-line and Multi-line Comments

**Comments** are lines in the code that Python will **not execute**.
We use comments to explain the code or leave notes for ourselves or others.

#### Single-line comment

Use `#` for a single-line comment.

```python
# This is a single-line comment
print("Welcome to Python")
```

#### Multi-line comment

There is no special multi-line comment in Python,
but you can use triple quotes (`'''` or `"""`) to write multi-line notes.

```python
'''
This is a multi-line comment.
It spans over multiple lines.
'''
print("This will still run")
```

---

### Using `print()` Function

The `print()` function is used to show output.

Examples:

```python
print("My name is Pawan")
print(10 + 5)
```

You can also print multiple values:

```python
name = "Fatima"
age = 21
print("Name:", name, "Age:", age)
```

---

### Using `input()` Function

The `input()` function is used to take input from the user.

Example:

```python
name = input("Enter your name: ")
print("Hello", name)
```

* Whatever you type will be stored in the `name` variable.
* Note: By default, input is taken as **string**.

Another example:

```python
age = input("Enter your age: ")
print("You are", age, "years old")
```

---

### Summary:

| Concept       | Use / Description          |
| ------------- | -------------------------- |
| `print()`     | Shows output on the screen |
| `input()`     | Takes input from the user  |
| `#`           | Single-line comment        |
| `''' or """`  | Multi-line comment         |
| Indentation   | Used to define code blocks |
| First program | `print("Hello, World!")`   |


