## Operators in Python

**Operators** are special symbols used to perform operations on values or variables.

Example:

```python
a = 10
b = 5
print(a + b)   # '+' is an operator
```

---

### 1. Arithmetic Operators

Used to perform basic math operations:

| Operator | Name           | Example  | Result |
| -------- | -------------- | -------- | ------ |
| `+`      | Addition       | `a + b`  | 15     |
| `-`      | Subtraction    | `a - b`  | 5      |
| `*`      | Multiplication | `a * b`  | 50     |
| `/`      | Division       | `a / b`  | 2.0    |
| `//`     | Floor Division | `a // b` | 2      |
| `%`      | Modulus        | `a % b`  | 0      |
| `**`     | Exponent       | `a ** b` | 100000 |

---

### 2. Comparison (Relational) Operators

Used to compare two values. Result is either `True` or `False`.

| Operator | Meaning          | Example  |
| -------- | ---------------- | -------- |
| `==`     | Equal to         | `a == b` |
| `!=`     | Not equal to     | `a != b` |
| `>`      | Greater than     | `a > b`  |
| `<`      | Less than        | `a < b`  |
| `>=`     | Greater or equal | `a >= b` |
| `<=`     | Less or equal    | `a <= b` |

Example:

```python
a = 10
b = 5
print(a > b)   # True
```

---

### 3. Logical Operators

Used to combine multiple conditions.

| Operator | Description           | Example            |
| -------- | --------------------- | ------------------ |
| `and`    | True if both are True | `a > 5 and b < 10` |
| `or`     | True if one is True   | `a > 5 or b > 10`  |
| `not`    | Reverses the result   | `not(a > b)`       |

Example:

```python
a = 10
b = 5
print(a > 5 and b < 10)  # True
```

---

### 4. Assignment Operators

Used to assign values to variables.

| Operator | Meaning             | Example                |
| -------- | ------------------- | ---------------------- |
| `=`      | Assign              | `a = 5`                |
| `+=`     | Add and assign      | `a += 3` → `a = a + 3` |
| `-=`     | Subtract and assign | `a -= 2`               |
| `*=`     | Multiply and assign | `a *= 2`               |
| `/=`     | Divide and assign   | `a /= 2`               |
| `//=`    | Floor divide assign | `a //= 2`              |
| `%=`     | Modulus and assign  | `a %= 2`               |
| `**=`    | Power and assign    | `a **= 2`              |

---

### 5. Bitwise Operators

Used to work with binary values (0s and 1s).

| Operator | Meaning          | Example  |     |     |
| -------- | ---------------- | -------- | --- | --- |
| `&`      | AND              | `a & b`  |     |     |
| \`       | \`               | OR       | \`a | b\` |
| `^`      | XOR              | `a ^ b`  |     |     |
| `~`      | NOT (complement) | `~a`     |     |     |
| `<<`     | Left Shift       | `a << 1` |     |     |
| `>>`     | Right Shift      | `a >> 1` |     |     |

Example:

```python
a = 5      # 0101 in binary
b = 3      # 0011 in binary
print(a & b)  # 1 (0001)
```

---

### 6. Identity and Membership Operators

#### a. Identity Operators

Check if two variables refer to the same object in memory.

| Operator | Meaning       | Example      |
| -------- | ------------- | ------------ |
| `is`     | Same identity | `a is b`     |
| `is not` | Not same      | `a is not b` |

#### b. Membership Operators

Check if a value is part of a sequence (like list, string, etc.)

| Operator | Meaning        | Example              |
| -------- | -------------- | -------------------- |
| `in`     | Exists         | `"a" in "apple"`     |
| `not in` | Does not exist | `"z" not in "apple"` |

---

### Summary Table

| Type       | Examples                 |                 |
| ---------- | ------------------------ | --------------- |
| Arithmetic | +, -, \*, /, %, \*\*, // |                 |
| Comparison | ==, !=, >, <, >=, <=     |                 |
| Logical    | and, or, not             |                 |
| Assignment | =, +=, -=, \*=, /=       |                 |
| Bitwise    | &,                       | , ^, \~, <<, >> |
| Identity   | is, is not               |                 |
| Membership | in, not in               |                 |

---

