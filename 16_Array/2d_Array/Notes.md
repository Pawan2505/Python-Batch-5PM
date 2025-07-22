
## 📘 **2D Array using List in Python**

---

### 1. What is a 2D Array?

* 2D array ka matlab hota hai: **list of lists**
* Matlab: har element bhi ek list hoti hai
* Example:

```python
matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]
```

Ye ek 3x3 matrix hai – 3 rows aur 3 columns

---

### 2. Accessing Elements from 2D Array

```python
print(matrix[0][0])   # 1 (first row, first column)
print(matrix[1][2])   # 6 (second row, third column)
```

👉 Pehla index = row number
👉 Dusra index = column number

---

### 3. Looping Through 2D Array

#### 🔁 Using Nested `for` Loop:

```python
for row in matrix:
    for item in row:
        print(item, end=' ')
    print()
```

Output:

```
1 2 3  
4 5 6  
7 8 9
```

---

### 4. Taking Input in 2D Array

```python
rows = 2
cols = 3
matrix = []

for i in range(rows):
    row = []
    for j in range(cols):
        val = int(input(f"Enter element at [{i}][{j}]: "))
        row.append(val)
    matrix.append(row)

print(matrix)
```

---

### 5. Updating Values in 2D Array

```python
matrix[0][1] = 99
print(matrix)
```

---

## 🔄 **Sorting in Python Collections**

---

### 1. `sort()` Method

* `sort()` sirf **lists** par kaam karta hai.
* Ye list ko **original list mein hi** sort kar deta hai (in-place).
* **Ascending by default**, `reverse=True` for descending.

```python
numbers = [5, 2, 9, 1, 7]
numbers.sort()
print(numbers)      # [1, 2, 5, 7, 9]

numbers.sort(reverse=True)
print(numbers)      # [9, 7, 5, 2, 1]
```

---

### 2. `sorted()` Function

* `sorted()` kisi bhi **iterable** (list, tuple, string, etc.) pe kaam karta hai.
* Ye **nayi sorted list** return karta hai. Original data change nahi hota.

```python
data = [3, 1, 4, 2]
result = sorted(data)
print(result)       # [1, 2, 3, 4]
print(data)         # [3, 1, 4, 2]  (unchanged)
```

👉 `sorted()` also works with:

```python
print(sorted((3, 1, 2)))     # tuple
print(sorted("pawan"))       # string → ['a', 'n', 'p', 'w', 'w']
```

---

### Difference Between `sort()` and `sorted()`

| Feature       | `sort()`                  | `sorted()`              |
| ------------- | ------------------------- | ----------------------- |
| Data type     | Works only on lists       | Works on any iterable   |
| Return type   | Returns `None` (in-place) | Returns new sorted list |
| Original data | Modified                  | Not modified            |

---


## Summary

* 2D array in Python = **list of lists**
* Use nested loops to access and update 2D arrays
* `sort()` list ko inplace sort karta hai
* `sorted()` koi bhi iterable ko sort karke nayi list deta hai
