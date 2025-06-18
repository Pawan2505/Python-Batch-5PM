### Q.1
The `sep` parameter in the `print()` function specifies the separator between multiple arguments, defaulting to a space. The `end` parameter specifies what to print at the end, defaulting to a newline.  
- Example: `print("Hello", "World", sep="-", end="!")` outputs `Hello-World!`.

### Q.2
In Python, single quotes (`'`) and double quotes (`"`) are interchangeable for strings, but triple quotes (`'''` or `"""`) are used for multi-line strings or docstrings.  
- Example: `'Hello'`, `"Hello"`, `'''Hello
World'''`.

### Q.3
The `input()` function returns a string by default. You can convert it using type conversion functions like `int()`, `float()`, etc.  
- Example: `num = int(input("Enter a number: "))`.

### Q.4
```python
num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))
print("Sum:", num1 + num2)
```

### Q.5
A variable in Python is a name that stores a value. It is important for storing and manipulating data during program execution.

### Q.6
- Rules: Variable names must start with a letter or underscore, can contain letters, numbers, and underscores, and are case-sensitive. No spaces or special characters (except `_`) are allowed.
- Valid: `my_var`, `_hidden`, `Var1`.
- Invalid: `2var`, `my var`, `@var`.

### Q.7
Variable reassignment means changing the value of a variable.  
- Example: `x = 5; x = 10` (now `x` is 10).

### Q.8
The `type()` function returns the data type of an object, useful for debugging or type checking.  
- Example: `print(type(5))` outputs `<class 'int'>`.

### Q.9
Mutable variables (e.g., lists) can be changed after creation; immutable variables (e.g., strings) cannot.  
- Example: `list1 = [1, 2]; list1[0] = 3` (mutable); `str1 = "hi"; str1[0] = 'a'` (immutable, raises error).

### Q.10
You can delete a variable using `del`.  
- Example: `x = 5; del x; print(x)` (raises error after deletion).

### Q.11
- `int`: Whole numbers (e.g., 5).
- `float`: Decimal numbers (e.g., 5.0).
- `complex`: Numbers with real and imaginary parts (e.g., 3 + 4j).
- Key differences: Precision and use cases (e.g., `float` for decimals, `complex` for mathematics).

### Q.12
A Boolean data type has values `True` or `False`. It’s used in conditionals and logical operations.  
- Example: `if x > 0: print(True)`.

### Q.13
Operators in Python perform operations on variables. Categories: arithmetic, comparison, logical, assignment, membership, identity.

### Q.14
Arithmetic operators (e.g., `+`, `-`) perform mathematical calculations; comparison operators (e.g., `==`, `>`) compare values.  
- Example: `print(2 + 3)` (arithmetic); `print(2 == 3)` (comparison, `False`).

### Q.15
Logical operators (`and`, `or`, `not`) combine conditions.  
- Example: `print(True and False)` (False); `print(not True)` (False).

### Q.16
The `=` operator assigns a value (e.g., `x = 5`), while `==` checks equality (e.g., `x == 5` returns `True` or `False`).

### Q.17
Membership operators (`in`, `not in`) check if a value is in a sequence.  
- Example: `print("a" in "cat")` (True); `print("b" not in "cat")` (True).

### Q.18
Identity operators (`is`, `is not`) compare object identities.  
- Example: `x = [1, 2]; y = x; print(x is y)` (True); `z = [1, 2]; print(x is z)` (False).

### Q.19
Operator precedence determines the order of evaluation. It’s important to avoid ambiguity.  
- Example: `print(2 + 3 * 4)` (14, as `*` has higher precedence than `+`).