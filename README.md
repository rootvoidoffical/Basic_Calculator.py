# Basic_Calculator.py

<img width="1280" height="800" alt="Screenshot From 2026-08-01 17-24-56" src="https://github.com/user-attachments/assets/dccf29b3-ea43-4890-95c6-6f320eee55be" />

Just a python program for basic calculator.

```
CYAN = "\033[96m"
YELLOW = "\033[93m"
RESET = "\033[0m"
RED = "\033[91m"
GREEN = "\033[92m"

print(CYAN + r"""
╔══════════════════════════════════════════════════════════════╗
║                                                              ║
║    ██████╗ █████╗ ██╗      ██████╗██╗   ██╗██╗      █████╗   ║
║   ██╔════╝██╔══██╗██║     ██╔════╝██║   ██║██║     ██╔══██╗  ║
║   ██║     ███████║██║     ██║     ██║   ██║██║     ███████║  ║
║   ██║     ██╔══██║██║     ██║     ██║   ██║██║     ██╔══██║  ║
║   ╚██████╗██║  ██║███████╗╚██████╗╚██████╔╝███████╗██║  ██║  ║
║    ╚═════╝╚═╝  ╚═╝╚══════╝ ╚═════╝ ╚═════╝ ╚══════╝╚═╝  ╚═╝  ║
║                                                              ║
║                  ★ PYTHON BASIC CALCULATOR ★                ║
║                                                              ║
╚══════════════════════════════════════════════════════════════╝
""" + RESET)

print(YELLOW + "Welcome! Perform basic arithmetic operations." + RESET)


num1 = float(input("Enter first number: "))
operator = input("Enter operator (+, -, *, /): ")
num2 = float(input("Enter second number: "))

if operator == '+':
    result = num1 + num2
elif operator == '-':
    result = num1 - num2
elif operator == '*':
    result = num1 * num2
elif operator == '/':
    if num2 != 0:
        result = num1 / num2
    else:
        result = RED + "Error: Division by zero is not allowed." + RESET
else:
    result = RED + "Error: Invalid operator." + RESET

print(GREEN + "Result: " + str(result) + RESET)


```
