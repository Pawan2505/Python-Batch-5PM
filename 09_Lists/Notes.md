## Data Structures in Python – **Lists**

---

### What is a List?

A **list** is a collection of items that are **ordered**, **changeable (mutable)**, and allows **duplicate values**.

```python
fruits = ["apple", "banana", "cherry"]
```

* Lists use **square brackets `[ ]`**
* Items are separated by **commas**

---

### Creating a List

```python
numbers = [10, 20, 30, 40]
mixed = [1, "hello", 3.14, True]
empty = []
```

You can store:

* Same type data
* Different type data
* Even another list inside a list (nested list)

---

### Indexing in Lists

Just like strings, lists use indexing.

```python
fruits = ["apple", "banana", "cherry"]
print(fruits[0])   # apple
print(fruits[-1])  # cherry (last item)
```

💡 Indexing starts from `0`
💡 Negative index starts from end (`-1` is last item)

---

### Slicing a List

```python
fruits = ["apple", "banana", "cherry", "mango"]
print(fruits[1:3])   # ['banana', 'cherry']
print(fruits[:2])    # ['apple', 'banana']
print(fruits[2:])    # ['cherry', 'mango']
```

🔹 Syntax: `list[start:end]` (end is excluded)

---

### Built-in Methods for Lists

Here are some most used list methods:

| Method         | Description                                               | Example                      |
| -------------- | --------------------------------------------------------- | ---------------------------- |
| `append(x)`    | Adds item at the end                                      | `fruits.append("grape")`     |
| `insert(i, x)` | Inserts item at index `i`                                 | `fruits.insert(1, "orange")` |
| `remove(x)`    | Removes first occurrence of `x`                           | `fruits.remove("banana")`    |
| `pop(i)`       | Removes and returns item at index `i` (last if not given) | `fruits.pop()`               |
| `clear()`      | Removes all items                                         | `fruits.clear()`             |
| `sort()`       | Sorts the list in ascending order                         | `numbers.sort()`             |
| `reverse()`    | Reverses the order of the list                            | `fruits.reverse()`           |
| `len()`        | Returns the length of the list                            | `len(fruits)`                |
| `index(x)`     | Returns the first index of value `x`                      | `fruits.index("banana")`     |
| `count(x)`     | Counts how many times value `x` occurs                    | `fruits.count("apple")`      |

---

### Example Program

```python
students = ["Fatima", "Ravi", "Pawan"]
students.append("Zara")
students[1] = "Raj"       # Changing value
print(students)
```

🔹 Output: `['Fatima', 'Raj', 'Pawan', 'Zara']`

---

### Summary:

| Feature    | Details                              |
| ---------- | ------------------------------------ |
| Ordered    | Items have a fixed index             |
| Mutable    | You can change, add, delete elements |
| Duplicates | Allowed                              |
| Indexing   | `list[0]`, `list[-1]`                |
| Slicing    | `list[1:3]`, `list[:2]`              |
| Methods    | `append()`, `pop()`, `sort()`, etc.  |

---

