### Project Overview
The task involves writing a Python program to:
- Accept personal data (e.g., name, age, address) from the user.
- Store and process this data using functions.
- Demonstrate type conversion and display the results.

### Key Requirements
1. **Input Handling**: Use `input()` to collect data (e.g., name as string, age as integer).
2. **Type Conversion**: Convert data types where necessary (e.g., string to integer for age).
3. **Function Usage**: Define functions to process and display data.
4. **Output**: Show the data, including type and memory address using `type()` and `id()`.

### Sample Solution
Below is a Python program addressing the requirements based on the document:

```python
# Function to get personal data
def get_data():
    name = input("Enter your name: ")
    age = int(input("Enter your age: "))  # Type conversion from string to int
    address = input("Enter your address: ")
    return name, age, address

# Function to display data with type and memory address
def display_data(name, age, address):
    print(f"Name: {name}, Type: {type(name)}, ID: {id(name)}")
    print(f"Age: {age}, Type: {type(age)}, ID: {id(age)}")
    print(f"Address: {address}, Type: {type(address)}, ID: {id(address)}")

# Main program
if __name__ == "__main__":
    # Get data from user
    name, age, address = get_data()
    
    # Display the data
    print("\nPersonal Data:")
    display_data(name, age, address)
```

### Explanation
- **Input**: The `get_data()` function uses `input()` to collect name (string), age (converted to integer), and address (string).
- **Type Conversion**: `int()` is used to convert the age input from string to integer.
- **Functions**: Two functions are defined: `get_data()` to collect input and `display_data()` to show the data with types and memory addresses.
- **Output**: The program prints each variable's value, data type (using `type()`), and memory address (using `id()`).
