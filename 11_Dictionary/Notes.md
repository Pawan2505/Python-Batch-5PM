## Data Structures in Python – **Dictionaries**

---

### What is a Dictionary?

A **dictionary** is a collection of **key-value pairs**.

Each item has a **key** and a **value**:

```python
student = {
    "name": "Fatima",
    "age": 20,
    "course": "Python"
}
```

* Use **curly braces `{}`**
* Keys are **unique**
* Values can be any data type

---

### Accessing Values

You can access values using **keys**:

```python
print(student["name"])     # Output: Fatima
print(student["age"])      # Output: 20
```

---

### Adding New Items

Just assign a new key and value:

```python
student["city"] = "Surat"
```

---

### Updating Existing Items

Just assign a new value to an existing key:

```python
student["age"] = 21
```

You can also use `update()` method:

```python
student.update({"age": 22})
```

---

### Deleting Items

| Operation           | Code                    |
| ------------------- | ----------------------- |
| Delete specific key | `del student["course"]` |
| Use `pop()` method  | `student.pop("age")`    |
| Clear all items     | `student.clear()`       |

---

### Looping Through Dictionary

```python
for key in student:
    print(key, "=", student[key])
```

OR:

```python
for key, value in student.items():
    print(key, ":", value)
```

---

### Dictionary Methods

| Method          | Use                                      |
| --------------- | ---------------------------------------- |
| `keys()`        | Returns all keys                         |
| `values()`      | Returns all values                       |
| `items()`       | Returns key-value pairs                  |
| `get(key)`      | Returns value of key (safe way)          |
| `pop(key)`      | Removes and returns value of the key     |
| `clear()`       | Removes all key-value pairs              |
| `update(dict2)` | Updates with another dictionary’s values |

---

### Example:

```python
car = {
    "brand": "Toyota",
    "model": "Fortuner",
    "year": 2022
}

car["color"] = "White"       # Add new key
car["year"] = 2023           # Update key
del car["model"]             # Delete key
```

---

### Summary:

| Feature         | Dictionary                          |
| --------------- | ----------------------------------- |
| Syntax          | `{key: value}`                      |
| Access value    | `dict["key"]` or `dict.get("key")`  |
| Add/Update item | `dict["key"] = value`               |
| Delete item     | `del`, `pop()`                      |
| Loop            | `for key in dict` or `dict.items()` |

---

