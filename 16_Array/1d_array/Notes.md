## 📘 **1D Array using List in Python**

---

### 1. What is 1D Array?

* 1D Array ka matlab hota hai **ek single line** (row) mein data ka group.
* Jaise: `[10, 20, 30, 40]`
* Har element ka **index** hota hai (0 se start hota hai).

---

### 2. Python mein 1D Array kaise banate hain?

👉 Python mein hum **list** ka use karke 1D array banate hain.

```python
numbers = [10, 20, 30, 40, 50]
```

* Ye ek 1D list hai jisme 5 numbers hain.

---

### 3. List ke Elements ko Access Karna

```python
print(numbers[0])   # 10
print(numbers[2])   # 30
```

* `numbers[0]` ka matlab hai **first element**
* Indexing **0 se shuru hoti hai**

---

### 4. Element ko Change Karna

```python
numbers[1] = 99
print(numbers)   # [10, 99, 30, 40, 50]
```

---

### 5. List ke Elements ko Loop se Print Karna

```python
for item in numbers:
    print(item)
```

Ya

```python
for i in range(len(numbers)):
    print(numbers[i])
```

---

### 6. List ke Common Functions

| Kaam              | Code                    | Result                      |
| ----------------- | ----------------------- | --------------------------- |
| Element add karna | `numbers.append(60)`    | \[10, 99, 30, 40, 50, 60]   |
| Insert karna      | `numbers.insert(2, 25)` | index 2 par 25 add hoga     |
| Remove karna      | `numbers.remove(30)`    | 30 delete ho jayega         |
| Delete by index   | `del numbers[0]`        | index 0 wala delete hoga    |
| Length of list    | `len(numbers)`          | total elements count karega |
| Slice             | `numbers[1:4]`          | index 1 se 3 tak ke items   |

---

### 7. Example: Sum of All Elements

```python
arr = [5, 10, 15]
total = 0
for i in arr:
    total += i
print("Sum =", total)
```

---

### 8. Real Example: Student Marks

```python
marks = [70, 80, 90, 75, 85]
average = sum(marks) / len(marks)
print("Average Marks:", average)
```

---

### 11. Summary

* Python mein list ka use karke 1D array banate hain.
* List indexing 0 se start hoti hai.
* Append, insert, remove jaise functions list ke sath use hote hain.
* List ka size dynamic hota hai (badhaya ya ghata sakte hain).


