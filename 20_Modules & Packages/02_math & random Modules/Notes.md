# **math & random Modules**

---

## **1. The `math` Module**

The **`math`** module gives us **mathematical functions and constants**.

💡 **Importing:**

```python
import math
```

---

### **Common `math` Functions**

| Function            | Description         | Example                         |
| ------------------- | ------------------- | ------------------------------- |
| `math.sqrt(x)`      | Square root         | `math.sqrt(16)` → `4.0`         |
| `math.pow(x, y)`    | x raised to power y | `math.pow(2, 3)` → `8.0`        |
| `math.floor(x)`     | Round down          | `math.floor(4.9)` → `4`         |
| `math.ceil(x)`      | Round up            | `math.ceil(4.1)` → `5`          |
| `math.factorial(x)` | Factorial of x      | `math.factorial(5)` → `120`     |
| `math.pi`           | Constant π          | `math.pi` → `3.141592653589793` |
| `math.e`            | Constant e          | `math.e` → `2.718281828459045`  |

---

### **Example**

```python
import math

print("Square root of 25:", math.sqrt(25))
print("2 raised to 5:", math.pow(2, 5))
print("Floor of 4.7:", math.floor(4.7))
print("Ceil of 4.2:", math.ceil(4.2))
print("Factorial of 5:", math.factorial(5))
print("Value of pi:", math.pi)
```

---

## **2. The `random` Module**

The **`random`** module helps us generate **random numbers**.

💡 **Importing:**

```python
import random
```

---

### **Common `random` Functions**

| Function                       | Description                              | Example                              |
| ------------------------------ | ---------------------------------------- | ------------------------------------ |
| `random.random()`              | Random float between 0 & 1               | `0.731`                              |
| `random.randint(a, b)`         | Random integer between a & b (inclusive) | `random.randint(1, 10)`              |
| `random.randrange(a, b, step)` | Random number in range                   | `random.randrange(0, 10, 2)`         |
| `random.choice(seq)`           | Random element from list/tuple/string    | `random.choice(["apple", "banana"])` |
| `random.shuffle(list)`         | Shuffle list elements                    |                                      |
| `random.uniform(a, b)`         | Random float between a & b               | `random.uniform(1, 5)`               |

---

### **Example**

```python
import random

print("Random float (0-1):", random.random())
print("Random int (1-10):", random.randint(1, 10))
print("Random choice:", random.choice(["red", "green", "blue"]))

numbers = [1, 2, 3, 4, 5]
random.shuffle(numbers)
print("Shuffled list:", numbers)

print("Random float between 10 and 20:", random.uniform(10, 20))
```

---

## **3. Fun Example: Dice Roll Game**

```python
import random

print("Rolling dice...")
dice = random.randint(1, 6)
print("You got:", dice)
```

---

## **Note:**

| Module   | Purpose                  | Example                 |
| -------- | ------------------------ | ----------------------- |
| `math`   | Math functions/constants | `math.sqrt(25)`         |
| `random` | Random numbers           | `random.randint(1, 10)` |

---

