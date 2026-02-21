# 09: Functions - Reusable Code

**Duration:** 60 minutes | **Difficulty:** Intermediate | **Key Skill:** Creating and using functions

---

## í¾¯ What You'll Learn

- Defining functions with def
- Parameters and arguments
- Return values
- Default parameters
- ML Context: Functions for modular, testable code

---

## í³š Creating Functions

\`\`\`python
# Basic function
def greet():
    print("Hello!")

greet()  # Call the function

# Function with parameters
def greet_person(name):
    print(f"Hello, {name}!")

greet_person("Alice")  # Hello, Alice!

# Function with return value
def add(a, b):
    return a + b

result = add(5, 3)
print(result)  # 8
\`\`\`

## í³š Parameters & Args

\`\`\`python
# Default parameters
def greet(name="Friend"):
    return f"Hello, {name}!"

print(greet())  # Hello, Friend!
print(greet("Bob"))  # Hello, Bob!

# Multiple return values
def divide_and_remainder(a, b):
    return a // b, a % b

quotient, remainder = divide_and_remainder(10, 3)
print(quotient, remainder)  # 3, 1
\`\`\`

---

## í·  ML Context

\`\`\`python
# Normalize data
def normalize(data):
    min_val = min(data)
    max_val = max(data)
    return [(x - min_val) / (max_val - min_val) for x in data]

scores = [50, 75, 100]
normalized = normalize(scores)
\`\`\`

---
