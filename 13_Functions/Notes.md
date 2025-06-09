## Python – **Functions**

---

### What is a Function?

A **function** is a block of code that performs a task and runs only when it is called.

It helps in:

* Reusing code
* Keeping code organized

---

### Defining and Calling a Function

```python
def greet():
    print("Hello, welcome to Python!")

greet()  # Function call
```

🔹 Use `def` keyword to define a function
🔹 Use parentheses `()` to call the function

---

### Function with Parameters (Arguments)

```python
def greet(name):
    print("Hello", name)

greet("Fatima")     # Output: Hello Fatima
```

---

### Return Values

```python
def add(a, b):
    return a + b

result = add(5, 3)
print(result)    # Output: 8
```

🔹 Use `return` to give a value back from a function

---

### Default Arguments

```python
def greet(name="Student"):
    print("Hello", name)

greet()            # Output: Hello Student
greet("Pawan")     # Output: Hello Pawan
```

🔹 If no value is given, the default will be used

---

### Keyword Arguments

You can pass arguments using **key=value** format:

```python
def student(name, age):
    print(name, age)

student(age=18, name="Raj")  # Order doesn't matter
```

---

### \*args → Multiple Positional Arguments

Use `*args` when you don't know how many arguments will be passed:

```python
def total(*nums):
    print(sum(nums))

total(1, 2, 3, 4)   # Output: 10
```

🔹 `args` is just a name, you can use anything, but `*` is necessary
🔹 Arguments are received as a **tuple**

---

### \*\*kwargs → Multiple Keyword Arguments

Use `**kwargs` for multiple named arguments:

```python
def student_info(**details):
    print(details)

student_info(name="Ravi", age=20)
# Output: {'name': 'Ravi', 'age': 20}
```

🔹 `kwargs` will be a **dictionary**

---

### Lambda Functions (Anonymous Functions)

Used for small/one-line functions:

```python
square = lambda x: x * x
print(square(4))   # Output: 16
```

🔹 No `def`, no `return` — just quick definition
🔹 Syntax: `lambda arguments: expression`

---

### Summary

| Concept           | Example                     |
| ----------------- | --------------------------- |
| Define function   | `def greet():`              |
| With parameters   | `def add(a, b):`            |
| With return value | `return a + b`              |
| Default argument  | `def hello(name="Student")` |
| Keyword argument  | `func(name="John", age=21)` |
| \*args            | `def fun(*args)`            |
| \*\*kwargs        | `def fun(**kwargs)`         |
| Lambda function   | `lambda x: x + 10`          |

---

