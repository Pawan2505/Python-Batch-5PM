### Q1: Demonstrate formatting options in print()
```python
# Using sep to separate values with a custom character
print("Hello", "World", sep="-")

# Using end to customize what appears at the end
print("First line", end=" ")
print("Second line")
```

### Q2: Ask for name, age, and hobby, then display a formatted message
```python
# Ask user for input
name = input("Enter your name: ")
age = input("Enter your age: ")
hobby = input("Enter your favourite hobby: ")

# Display formatted message
print("Hello,", name, "! At", age, "enjoying", hobby, "sounds fun!")
```

### Q3: Perform arithmetic operations on two numbers
```python
# Get two numbers from user
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

# Perform operations
add = num1 + num2
sub = num1 - num2
mul = num1 * num2
div = num1 / num2
floor_div = num1 // num2
mod = num1 % num2
exp = num1 ** num2

# Display results
print("Addition:", add)
print("Subtraction:", sub)
print("Multiplication:", mul)
print("Division:", div)
print("Floor Division:", floor_div)
print("Modulus:", mod)
print("Exponentiation:", exp)
```

### Q4: Declare variables of different datatypes and print their types
```python
# Declare variables of different datatypes
int_var = 10
float_var = 5.5
str_var = "Hello"
bool_var = True
complex_var = 3 + 4j

# Print values and types
print("Integer:", int_var, "Type:", type(int_var))
print("Float:", float_var, "Type:", type(float_var))
print("String:", str_var, "Type:", type(str_var))
print("Boolean:", bool_var, "Type:", type(bool_var))
print("Complex:", complex_var, "Type:", type(complex_var))
```

### Q5: Program for user to input height and weight
```python
# Ask user for height and weight
height = float(input("Enter your height (in cm): "))
weight = float(input("Enter your weight (in kg): "))

# Display formatted message
print("Your height is", height, "cm and weight is", weight, "kg.")
```

### Q6: Demonstrate logical operators
```python
# Ask user for boolean inputs
a = input("Enter true or false for a: ").lower() == "true"
b = input("Enter true or false for b: ").lower() == "true"

# Perform logical operations
and_result = a and b
or_result = a or b
not_a = not a
not_b = not b

# Display results
print("a and b:", and_result)
print("a or b:", or_result)
print("not a:", not_a)
print("not b:", not_b)
```

### Q7: Demonstrate assignment operators
```python
# Use a single variable
x = 10

# Demonstrate assignment operators
x += 5  # x = x + 5
print("After += 5:", x)

x -= 3  # x = x - 3
print("After -= 3:", x)

x *= 2  # x = x * 2
print("After *= 2:", x)

x /= 4  # x = x / 4
print("After /= 4:", x)
```
