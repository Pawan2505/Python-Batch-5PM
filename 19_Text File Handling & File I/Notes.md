
# **Python Lecture: Text File Handling & File I/O**

---

## **1. What is File Handling in Python?**

File handling means **working with files** in your program.
You can:

* Read from a file 📖* Write to a file ✍️
* Update a file 🔄

Python gives us an easy way to do this using the **`open()`** function.

---

## **2. Opening a File – `open()` Function**

The basic syntax is:

```python
file_object = open("filename", "mode")
```

Here:

* **`filename`** → name of the file (example: `"data.txt"`)
* **`mode`** → tells Python what you want to do with the file

---

## **3. Modes of Opening a File**

| Mode   | Meaning       | Creates File? | Deletes Old Data?   | Example Use                  |
| ------ | ------------- | ------------- | ------------------- | ---------------------------- |
| `"r"`  | Read only     | ❌ No          | ❌ No                | Read existing file           |
| `"w"`  | Write only    | ✅ Yes         | ✅ Yes (clears file) | Create new or overwrite file |
| `"a"`  | Append only   | ✅ Yes         | ❌ No                | Add new data at end          |
| `"r+"` | Read + Write  | ❌ No          | ❌ No                | Read and update              |
| `"w+"` | Write + Read  | ✅ Yes         | ✅ Yes               | Create new and read/write    |
| `"a+"` | Append + Read | ✅ Yes         | ❌ No                | Add data and read            |

---

## **4. Closing a File – `close()`**

Always **close a file** when done so changes are saved and memory is freed.

```python
f = open("data.txt", "r")
# read/write operations
f.close()
```

---

## **5. Reading from a File**

### **Method 1: `read()`**

Reads the whole file as a single string.

```python
f = open("data.txt", "r")
content = f.read()
print(content)
f.close()
```

---

### **Method 2: `readline()`**

Reads **one line** at a time.

```python
f = open("data.txt", "r")
line = f.readline()
print(line)
f.close()
```

---

### **Method 3: `readlines()`**

Reads all lines into a **list**.

```python
f = open("data.txt", "r")
lines = f.readlines()
print(lines)
f.close()
```

---

## **6. Writing to a File**

### **`write()`** – Overwrites file

```python
f = open("data.txt", "w")
f.write("Hello World!")
f.close()
```

---

### **`writelines()`** – Writes multiple lines

```python
f = open("data.txt", "w")
f.writelines(["Line 1\n", "Line 2\n", "Line 3\n"])
f.close()
```

---

## **7. Appending to a File**

```python
f = open("data.txt", "a")
f.write("\nThis is a new line.")
f.close()
```

---

## **8. Using `with` Statement**

The `with` statement automatically **closes the file** for you (best practice).

```python
with open("data.txt", "r") as f:
    content = f.read()
    print(content)
```

---

## **9. File I/O Example with Exception Handling**

```python
try:
    with open("notes.txt", "r") as file:
        data = file.read()
        print("File content:")
        print(data)
except FileNotFoundError:
    print("The file was not found!")
except PermissionError:
    print("You don't have permission to open this file.")
finally:
    print("File operation finished.")
```

---

## **Note:**

1. **Open a file** with `open("file.txt", "mode")`
2. **Modes**: `"r"`, `"w"`, `"a"`, `"r+"`, `"w+"`, `"a+"`
3. **Read methods**: `read()`, `readline()`, `readlines()`
4. **Write methods**: `write()`, `writelines()`
5. **Close the file** with `close()` or use `with` for auto-close
6. **Handle exceptions** like `FileNotFoundError`

---

