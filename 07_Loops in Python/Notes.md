## Loops in Python

**Loops** are used to **repeat a block of code** multiple times.

Python has two main loops:

* `while` loop
* `for` loop

We also have some **loop control statements** like:
→ `break`, `continue`, `pass`

---

### 1. `while` Loop

The `while` loop runs **as long as the condition is true**.

```python
i = 1

while i <= 5:
    print(i)
    i += 1
```

* Starts from `i = 1`
* Prints value of `i` until `i` becomes more than 5

⚠️ Don’t forget to **increase `i`**, or it will run forever.

---

### 2. `for` Loop

Used to **loop through a sequence** like a list, string, or range.

```python
for i in range(1, 6):
    print(i)
```

* This prints numbers from 1 to 5
* `range(1, 6)` generates: 1, 2, 3, 4, 5

Another example with string:

```python
for letter in "Python":
    print(letter)
```

---

### 3. `range()` Function

The `range()` function is often used with `for` loops.

```python
range(start, stop, step)
```

Examples:

```python
range(5)        # 0 to 4
range(1, 6)     # 1 to 5
range(1, 10, 2) # 1, 3, 5, 7, 9
```

Used like:

```python
for i in range(3):
    print("Hello")
```

---

### 4. Loop Control Statements

These are used to **control the flow inside loops**.

#### a. `break`

Used to **exit** the loop immediately.

```python
for i in range(1, 10):
    if i == 5:
        break
    print(i)
```

→ Output: 1 2 3 4
→ Loop stops when `i == 5`

---

#### b. `continue`

Used to **skip** the current iteration.

```python
for i in range(1, 6):
    if i == 3:
        continue
    print(i)
```

→ Output: 1 2 4 5
(Skips 3)

---

#### c. `pass`

Used as a **placeholder** when we don’t want any code for now.

```python
for i in range(3):
    pass  # Do nothing here, just a placeholder
```

Useful when you're planning to write code later.

---

### Summary:

| Statement  | Use                                           |
| ---------- | --------------------------------------------- |
| `while`    | Loop runs while condition is true             |
| `for`      | Loop through a sequence (list, string, range) |
| `range()`  | Generates a sequence of numbers               |
| `break`    | Exits the loop early                          |
| `continue` | Skips current loop iteration                  |
| `pass`     | Does nothing, used as a placeholder           |

---

