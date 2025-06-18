### Q.1
**Question:** Write a Python program to demonstrate the use of type casting constructors (`int()`, `float()`, `str()`, and `bool()`).  
- Take input from the user as a string.  
- Convert the string into an integer, a float, and a boolean.  
- Print the converted values along with their types.  

```python
s = input("Enter a string: ")
i = int(s)
f_conv = float(s)
b_conv = bool(s)

print("Converted values:", i, "type:", type(i))
print("Converted values:", f_conv, "type:", type(f_conv))
print("Converted values:", b_conv, "type:", type(b_conv))
```

### Q.2
**Question:** Write a program where the user inputs a floating-point number.  
- Convert this number into an integer using `int()` and print both values with a message explaining the difference.  

```python
f = float(input("Enter a floating-point number: "))
i = int(f)
print(f"Original: {f}, Converted to int: {i}, Difference: {f - i} (decimal part)")
```

### Q.3
**Question:** Create a program that:  
- Takes a boolean value (True or False) as input.  
- Converts the boolean to an integer and a string, and prints all three values.  

```python
b = bool(input("Enter a boolean (True/False): "))
i = int(b)
s = str(b)
print("Boolean:", b, "Integer:", i, "String:", s)
```

### Q.4
**Question:** Write a Python program to:  
- Declare a variable of each datatype (integer, float, string, boolean, list, tuple, dictionary).  
- Print the value, type (using `type()`), and memory address (using `id()`) of each variable.  

```python
i = 5
f = 3.14
s = "hello"
b = True
l = [1, 2]
t = (1, 2)
d = {"a": 1}

print("Integer:", i, "type:", type(i), "id:", id(i))
print("Float:", f, "type:", type(f), "id:", id(f))
print("String:", s, "type:", type(s), "id:", id(s))
print("Boolean:", b, "type:", type(b), "id:", id(b))
print("List:", l, "type:", type(l), "id:", id(l))
print("Tuple:", t, "type:", type(t), "id:", id(t))
print("Dictionary:", d, "type:", type(d), "id:", id(d))
```

### Q.5
**Question:** Create a program that:  
- Declares two variables with the same value.  
- Prints their memory addresses using `id()` and checks if they are the same.  
- Modifies one of the variables and checks the memory addresses again.  

```python
x = 10
y = 10
print("x id:", id(x), "y id:", id(y), "Same?", id(x) == id(y))
x = 20
print("After modifying x, x id:", id(x), "y id:", id(y), "Same?", id(x) == id(y))
```