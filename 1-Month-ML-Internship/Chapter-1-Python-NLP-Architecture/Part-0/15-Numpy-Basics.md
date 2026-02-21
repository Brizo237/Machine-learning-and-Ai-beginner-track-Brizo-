# 15: NumPy Basics - Numerical Computing

**Duration:** 60 minutes | **Difficulty:** Intermediate | **Key Skill:** Working with numerical arrays

---

## í¾¯ What You'll Learn

- Creating NumPy arrays
- Array operations and broadcasting
- Common NumPy functions
- Why NumPy matters for ML

---

## í³š Creating Arrays

\`\`\`python
import numpy as np

# From list
arr = np.array([1, 2, 3, 4, 5])

# Using range
arr = np.arange(0, 10, 2)  # [0, 2, 4, 6, 8]

# Zeros and ones
zeros = np.zeros(5)  # [0., 0., 0., 0., 0.]
ones = np.ones(5)    # [1., 1., 1., 1., 1.]

# Random
rand = np.random.random(5)
\`\`\`

## í³š Array Operations

\`\`\`python
arr = np.array([1, 2, 3, 4])

# Element-wise operations
print(arr + 10)    # [11, 12, 13, 14]
print(arr * 2)     # [2,  4,  6,  8]
print(arr / 2)     # [0.5, 1., 1.5, 2.]

# Statistical operations
print(np.mean(arr))    # 2.5
print(np.std(arr))     # 1.118...
print(np.max(arr))     # 4
print(np.min(arr))     # 1
\`\`\`

## í³š 2D Arrays (Matrices)

\`\`\`python
# Create matrix
matrix = np.array([
    [1, 2, 3],
    [4, 5, 6]
])

print(matrix.shape)  # (2, 3)
print(matrix[0, 1])  # 2 (row 0, col 1)

# Transpose
transposed = matrix.T
\`\`\`

---

## í·  ML Context

NumPy is ESSENTIAL for ML:
- Store features and targets
- Efficient numerical computations
- Element-wise operations on large datasets
- Matrix operations for neural networks

\`\`\`python
# ML dataset
X = np.array([[1.0, 2.0], [2.0, 3.0]])  # Features
y = np.array([0, 1])  # Labels

# Normalize
X_normalized = (X - np.mean(X)) / np.std(X)
\`\`\`

---

## í´‘ Key Takeaways

âœ… NumPy arrays are efficient for numerical computing
âœ… Element-wise operations vs list operations
âœ… Shape, indexing, slicing work like lists
âœ… Statistical functions available
âœ… Essential for ML preprocessing

---
