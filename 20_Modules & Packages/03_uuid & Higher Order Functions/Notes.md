# **uuid & Higher Order Functions**


## **1. The `uuid` Module**

The **`uuid`** module generates **universally unique identifiers** (IDs).
They are often used for:

* Unique IDs in databases
* Tracking sessions in web apps
* File naming without conflicts

💡 **UUID** = *Universally Unique Identifier*

---

### **Importing**

```python
import uuid
```

---

### **Generating UUIDs**

```python
import uuid

# Generate a random UUID (version 4)
id1 = uuid.uuid4()
print(id1)  # Example: 123e4567-e89b-12d3-a456-426614174000
```

---

### **Other UUID Versions**

| Method                        | Purpose                                 |
| ----------------------------- | --------------------------------------- |
| `uuid.uuid1()`                | Based on time and machine address (MAC) |
| `uuid.uuid3(namespace, name)` | MD5 hash-based                          |
| `uuid.uuid4()`                | Random-based (most common)              |
| `uuid.uuid5(namespace, name)` | SHA-1 hash-based                        |

---

### **Example**

```python
import uuid

print("UUID1:", uuid.uuid1())  # time-based
print("UUID4:", uuid.uuid4())  # random-based
```

---

## **2. Higher Order Functions**

A **higher order function** is a function that:

1. **Takes another function as input**
2. **Or returns another function**

Python has several built-in higher order functions.

---

## **2.1 `sorted()` – Sorting**

Sorts a sequence (list, tuple, etc.).

```python
nums = [5, 2, 9, 1]
print(sorted(nums))           # Ascending: [1, 2, 5, 9]
print(sorted(nums, reverse=True))  # Descending: [9, 5, 2, 1]
```

**Sort by custom key:**

```python
words = ["apple", "banana", "cherry"]
print(sorted(words, key=len))  # By length: ['apple', 'banana', 'cherry']
```

---

## **2.2 `map()` – Apply Function to Each Item**

```python
nums = [1, 2, 3, 4]

def square(x):
    return x * x

result = map(square, nums)
print(list(result))  # [1, 4, 9, 16]
```

**Using lambda:**

```python
nums = [1, 2, 3, 4]
print(list(map(lambda x: x*x, nums)))
```

---

## **2.3 `reduce()` – Combine All Values into One**

`reduce()` is in the **`functools`** module.

```python
from functools import reduce

nums = [1, 2, 3, 4]

def multiply(a, b):
    return a * b

result = reduce(multiply, nums)
print(result)  # 24
```

**Using lambda:**

```python
from functools import reduce

nums = [1, 2, 3, 4]
print(reduce(lambda a, b: a + b, nums))  # 10
```

---

## **2.4 `filter()` – Keep Only Matching Items**

```python
nums = [1, 2, 3, 4, 5, 6]

def is_even(x):
    return x % 2 == 0

result = filter(is_even, nums)
print(list(result))  # [2, 4, 6]
```

**Using lambda:**

```python
nums = [1, 2, 3, 4, 5, 6]
print(list(filter(lambda x: x % 2 == 0, nums)))
```

---

## **3. Fun Example – Using All Together**

```python
import uuid
from functools import reduce

users = ["Alice", "Bob", "Charlie"]

# Give each user a UUID
users_with_id = list(map(lambda name: (name, uuid.uuid4()), users))

# Keep only users whose name length > 3
filtered_users = list(filter(lambda u: len(u[0]) > 3, users_with_id))

# Sort by name
sorted_users = sorted(filtered_users, key=lambda u: u[0])

# Count total characters in all names
total_chars = reduce(lambda a, b: a + len(b[0]), sorted_users, 0)

print("Users with ID:", users_with_id)
print("Filtered users:", filtered_users)
print("Sorted users:", sorted_users)
print("Total characters in names:", total_chars)
```

---

## **Note:**

| Function       | Purpose                     | Example              |
| -------------- | --------------------------- | -------------------- |
| `uuid.uuid4()` | Random unique ID            | `uuid.uuid4()`       |
| `sorted()`     | Sort sequence               | `sorted(list)`       |
| `map()`        | Apply function to each item | `map(func, list)`    |
| `reduce()`     | Reduce list to single value | `reduce(func, list)` |
| `filter()`     | Keep matching items         | `filter(func, list)` |

---

