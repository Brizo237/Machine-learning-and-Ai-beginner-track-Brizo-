# 13: List Comprehensions - Pythonic Data Processing

**Duration:** 45 minutes | **Difficulty:** Intermediate | **Key Skill:** Elegant data transformation

---

## í¾¯ What You'll Learn

- List comprehensions syntax
- Conditional comprehensions
- Nested comprehensions
- Set and dictionary comprehensions

---

## í³š Basic List Comprehensions

\`\`\`python
# Traditional way
squares = []
for x in range(5):
    squares.append(x ** 2)

# List comprehension (more Pythonic!)
squares = [x ** 2 for x in range(5)]
print(squares)  # [0, 1, 4, 9, 16]
\`\`\`

## í³š With Conditions

\`\`\`python
# Filter even numbers
evens = [x for x in range(10) if x % 2 == 0]
print(evens)  # [0, 2, 4, 6, 8]

# Transform and filter
words = ["python", "is", "awesome"]
long_words = [w.upper() for w in words if len(w) > 2]
\`\`\`

## í³š Nested Comprehensions

\`\`\`python
# Flatten a matrix
matrix = [[1, 2], [3, 4], [5, 6]]
flat = [x for row in matrix for x in row]
print(flat)  # [1, 2, 3, 4, 5, 6]
\`\`\`

---

## í·  ML Context

\`\`\`python
# Normalize data
data = [100, 50, 75]
normalized = [(x - min(data)) / (max(data) - min(data)) for x in data]
\`\`\`

---
