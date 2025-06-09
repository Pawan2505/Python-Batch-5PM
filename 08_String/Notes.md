## Data Structures in Python – **Strings**

---

### What is a String?

A **string** is a sequence of **characters** (letters, numbers, symbols) enclosed in **quotes**.

```python
name = "Pawan"
city = 'Surat'
```

Both single (`' '`) and double (`" "`) quotes are allowed.

---

### Accessing Characters (Indexing)

You can access individual characters using **index numbers**.

```python
text = "Python"
print(text[0])    # Output: P
print(text[3])    # Output: h
```

💡 Indexing starts from **0**

---

### String Slicing

You can extract a part of the string using **slicing**:

```python
word = "Programming"
print(word[0:4])     # Out: "Prog" (0 to 3)
print(word[4:])      # Out: "ramming" (from index 4 to end)
print(word[:6])      # Out: "Progra"
```

🔹 Syntax: `string[start:end]`
➡️ `start` index is included, `end` index is excluded.

---

### String Methods (Commonly Used)

| Method          | Purpose                        | Example                                 |
| --------------- | ------------------------------ | --------------------------------------- |
| `lower()`       | Convert to lowercase           | `"Hello".lower()` → `hello`             |
| `upper()`       | Convert to uppercase           | `"hello".upper()` → `HELLO`             |
| `title()`       | First letter capital           | `"hello world".title()` → `Hello World` |
| `strip()`       | Remove spaces from both ends   | `" hello ".strip()` → `hello`           |
| `replace(a, b)` | Replace a with b               | `"hi".replace("h", "H")` → `Hi`         |
| `find()`        | Find index of a substring      | `"Python".find("t")` → `2`              |
| `len()`         | Get length of string           | `len("apple")` → `5`                    |
| `count()`       | Count occurrences of substring | `"apple".count("p")` → `2`              |

---

### String Formatting (f-strings)

Used to insert variables inside strings.

```python
name = "Fatima"
age = 20
print(f"My name is {name} and I am {age} years old.")
```

🔹 Output: `"My name is Fatima and I am 20 years old."`

🟢 Easy and clean way to format strings.

---

### Multiline Strings

Use `'''triple quotes'''` or `"""triple quotes"""` for multiline text.

```python
msg = '''Hello students,
Welcome to Python programming!'''
print(msg)
```

---

### Summary

| Concept    | Example                                |
| ---------- | -------------------------------------- |
| String     | `"hello"`                              |
| Indexing   | `text[0]` → First character            |
| Slicing    | `text[1:4]` → Part of string           |
| Methods    | `lower()`, `upper()`, `replace()` etc. |
| Formatting | `f"My name is {name}"`                 |
| Multiline  | `'''text'''`                           |

---

