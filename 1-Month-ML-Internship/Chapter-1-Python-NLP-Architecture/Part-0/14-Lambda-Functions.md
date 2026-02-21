# 14: Lambda Functions - Anonymous Functions

**Duration:** 40 minutes | **Difficulty:** Intermediate | **Key Skill:** Functional programming basics

---

## í¾¯ What You'll Learn

- Lambda syntax
- Using with map(), filter(), sort()
- When to use lambdas

---

## í³š Lambda Basics

\`\`\`python
# Regular function
def add(x, y):
    return x + y

# Lambda equivalent
add_lambda = lambda x, y: x + y
print(add_lambda(3, 5))  # 8
\`\`\`

## í³š With map() and filter()

\`\`\`python
# map() - apply function to each item
numbers = [1, 2, 3, 4]
doubled = list(map(lambda x: x * 2, numbers))
print(doubled)  # [2, 4, 6, 8]

# filter() - keep items where function returns True
evens = list(filter(lambda x: x % 2 == 0, numbers))
print(evens)  # [2, 4]
\`\`\`

## í³š Sorting with Lambda

\`\`\`python
students = [("Alice", 95), ("Bob", 87), ("Charlie", 92)]
sorted_by_grade = sorted(students, key=lambda x: x[1])
\`\`\`

---

## í·  ML Context

\`\`\`python
# Sort predictions by confidence
predictions = [("cat", 0.95), ("dog", 0.82)]
top_pred = sorted(predictions, key=lambda x: x[1], reverse=True)[0]
\`\`\`

---
