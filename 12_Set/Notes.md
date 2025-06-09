## Data Structures in Python – **Sets**

---

### What is a Set?

A **set** is a collection of **unordered**, **unindexed**, and **unique** items.

```python
s = {1, 2, 3, 4}
```

* **Curly braces `{}`** are used.
* **Duplicates are not allowed**
* **Unordered**: No index, so you can’t use `s[0]`
* **Mutable**: You can add/remove items.

---

### Creating a Set

```python
nums = {1, 2, 3, 4}
words = set(["apple", "banana", "apple"])   # Duplicates removed
empty_set = set()     # Don’t use {} → it creates dictionary
```

---

### Adding Elements

```python
s = {10, 20}
s.add(30)
print(s)     # Output: {10, 20, 30}
```

---

### Removing Elements

```python
s.remove(10)     # Removes 10; gives error if not found
s.discard(40)    # Safe to use; no error if 40 not found
s.pop()          # Removes any random item
s.clear()        # Empties the whole set
```

---

### Looping Through a Set

```python
for item in s:
    print(item)
```

---

### Set Operations

| Operation       | Symbol/Method           | Example                          |                           |
| --------------- | ----------------------- | -------------------------------- | ------------------------- |
| Union           | \`set1                  | set2\`                           | Combines all unique items |
| Intersection    | `set1 & set2`           | Common items in both sets        |                           |
| Difference      | `set1 - set2`           | Items in set1 but not in set2    |                           |
| Symmetric Diff. | `set1 ^ set2`           | Items in either set but not both |                           |
| isSubset        | `set1.issubset(set2)`   | True if set1 is part of set2     |                           |
| isSuperset      | `set1.issuperset(set2)` | True if set1 contains set2       |                           |

---

### Example

```python
a = {1, 2, 3}
b = {3, 4, 5}

print(a | b)   # Union → {1, 2, 3, 4, 5}
print(a & b)   # Intersection → {3}
print(a - b)   # Difference → {1, 2}
print(a ^ b)   # Symmetric Difference → {1, 2, 4, 5}
```

---

### Summary

| Feature        | Set                                              |
| -------------- | ------------------------------------------------ |
| Brackets       | `{}` or `set()`                                  |
| Ordered?       | No                                             |
| Indexing?      | No                                             |
| Duplicates?    | Not allowed                                    |
| Mutable?       | Yes                                            |
| Common Methods | `add()`, `remove()`, `union()`, `intersection()` |

---

