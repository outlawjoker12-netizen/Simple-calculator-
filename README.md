# Simple-calculator-
# simple calculator

def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b

def divide(a, b):
    return a / b

def greet(name):
    print(f"Welcome {name}!")

# welcome user
name = input("What is your name? ")
greet(name)

# calculator part
while True:
    print("\n1. Add")
    print("2. Subtract")
    print("3. Multiply")
    print("4. Divide")

    option = int(input("Please select an option (1-4): "))

    a = int(input("Please enter first number: "))
    b = int(input("Please enter second number: "))

    if option == 1:
        result = add(a, b)
    elif option == 2:
        result = subtract(a, b)
    elif option == 3:
        result = multiply(a, b)
    elif option == 4:
        result = divide(a, b)
    else:
        print("Invalid option")
        continue

    print("Result:", result)

    retry = input("Would you like to redo? (yes/no): ").lower()
    if retry != "yes":
        break
