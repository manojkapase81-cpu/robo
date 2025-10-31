 a = float(input("Enter first number: "))
ch = input("Enter operation (+, -, *, /): ")
b = float(input("Enter second number: "))

try:
    if ch == '+':
        result = a + b
    elif ch == '-':
        result = a - b
    elif ch == '*':
        result = a * b
    elif ch == '/':
        if b == 0:
            result = "Error: Division by zero"
        else:
            result = a / b
    else:
        result = "Error: Invalid operation"

    print(f"Output = {result}")

except ValueError:
    print("Error: Invalid number entered.")
