# Basic Calculator Application

This is a simple command-line calculator application written in Python. It allows users to perform basic arithmetic operations such as addition, subtraction, multiplication, and division.

## Features
- Addition (+)
- Subtraction (-)
- Multiplication (*)
- Division (/) with error handling

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/Ntokozo-Paul-01.git
   ```
2. Navigate to the project directory:
   ```sh
   cd Ntokozo-Paul-01
   ```
3. Run the Python script:
   ```sh
   python calculator.py
   ```

## Usage Example
```
Simple Calculator
Select operation:
1. Add
2. Subtract
3. Multiply
4. Divide
Enter choice (1/2/3/4): 1
Enter first number: 5
Enter second number: 3
Result: 8
```

## Code
```python
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b

def divide(a, b):
    if b == 0:
        return "Error! Division by zero."
    return a / b

def main():
    print("Simple Calculator")
    print("Select operation:")
    print("1. Add")
    print("2. Subtract")
    print("3. Multiply")
    print("4. Divide")
    
    choice = input("Enter choice (1/2/3/4): ")
    
    if choice in ('1', '2', '3', '4'):
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))
        
        if choice == '1':
            print(f"Result: {add(num1, num2)}")
        elif choice == '2':
            print(f"Result: {subtract(num1, num2)}")
        elif choice == '3':
            print(f"Result: {multiply(num1, num2)}")
        elif choice == '4':
            print(f"Result: {divide(num1, num2)}")
    else:
        print("Invalid Input")

if __name__ == "__main__":
    main()
```
