## Python – **File Handling**

---

### What is File Handling?

File handling allows you to:

* **Create**
* **Read**
* **Write**
* **Append**
  data in files using Python.

This is useful for storing user data, logs, or saving output.

---

### Opening a File

Use the built-in `open()` function:

```python
file = open("data.txt", "r")  # open file in read mode
```

**Syntax**:

```python
open(filename, mode)
```

---

### Modes in File Handling

| Mode   | Meaning                           |
| ------ | --------------------------------- |
| `"r"`  | Read (default), file must exist   |
| `"w"`  | Write, creates file or overwrites |
| `"a"`  | Append, adds to end of file       |
| `"rb"` | Read in binary mode               |
| `"wb"` | Write in binary mode              |

---

### Reading from a File

```python
file = open("data.txt", "r")
content = file.read()
print(content)
file.close()
```

Other ways to read:

```python
file.readline()   # Read one line
file.readlines()  # Read all lines in a list
```

---

### Writing to a File

```python
file = open("data.txt", "w")
file.write("Hello, Python!")
file.close()
```

🔸 If file exists, it will be **overwritten**

---

### Appending to a File

```python
file = open("data.txt", "a")
file.write("\nNew line added")
file.close()
```

🔸 New content will be **added at the end**

---

### Using `with open()` → Context Manager

It automatically closes the file (better practice):

```python
with open("data.txt", "r") as file:
    content = file.read()
    print(content)
```

```python
with open("data.txt", "w") as file:
    file.write("Writing with 'with'")
```

---

### Example: Write and then Read

```python
# Write
with open("hello.txt", "w") as f:
    f.write("Welcome to Python file handling.")

# Read
with open("hello.txt", "r") as f:
    print(f.read())
```

---

### Summary

| Action            | Code Example              |
| ----------------- | ------------------------- |
| Read file         | `open("file.txt", "r")`   |
| Write file        | `open("file.txt", "w")`   |
| Append file       | `open("file.txt", "a")`   |
| Binary read/write | `"rb"`, `"wb"`            |
| Best practice     | `with open(...) as file:` |

---

