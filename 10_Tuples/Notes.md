## Data Structures in Python – **Tuples**

---

### What is a Tuple?

A **tuple** is a collection that is:

* **Ordered**
* **Immutable** (cannot be changed after creation)
* **Allows duplicate values**

```python
my_tuple = (10, 20, 30)
```

* Tuples use **round brackets** `( )`
* Similar to a list, but **you can't modify** it

---

### Creating Tuples

```python
t1 = (1, 2, 3)
t2 = ("apple", "banana", "cherry")
t3 = (1, "hello", 3.5)
```

Tuple with one item:

```python
single = (5,)     # Important: comma is needed!
```

Without comma, Python treats it as a number, not tuple.

---

### Accessing Elements (Indexing)

```python
t = ("a", "b", "c", "d")
print(t[0])     # Output: 'a'
print(t[-1])    # Output: 'd'
```

Same as lists: Indexing starts at `0`, `-1` means last item.

---

### Slicing Tuples

```python
nums = (10, 20, 30, 40, 50)
print(nums[1:4])    # Output: (20, 30, 40)
```

Syntax is same as lists: `tuple[start:end]` (end excluded)

---

### uple is Immutable

Once created, you **cannot change** its items.

```python
t = (1, 2, 3)
t[0] = 100     # Error: 'tuple' object does not support item assignment
```

---

### Tuple Methods

Tuples have **limited built-in methods**:

| Method     | Use                                |
| ---------- | ---------------------------------- |
| `count(x)` | Returns how many times `x` appears |
| `index(x)` | Returns first index of value `x`   |

Example:

```python
t = (1, 2, 3, 2, 4)
print(t.count(2))   # Output: 2
print(t.index(4))   # Output: 4
```

---

### Why Use Tuples?

| Reason                              | Benefit                                       |
| ----------------------------------- | --------------------------------------------- |
| Tuples are faster than lists        | Better for performance                        |
| Safer to use (data is protected)    | Useful when you don't want accidental changes |
| Can be used as keys in dictionaries | (Lists cannot be keys)                        |

---

### Example: Tuple in a loop

```python
colors = ("red", "green", "blue")

for c in colors:
    print(c)
```

---

### Summary:

| Feature     | Tuple                |
| ----------- | -------------------- |
| Brackets    | `( )`                |
| Ordered?    | Yes                  |
| Changeable? | No (Immutable)     |
| Duplicates? | Yes                |
| Methods     | `count()`, `index()` |

---

