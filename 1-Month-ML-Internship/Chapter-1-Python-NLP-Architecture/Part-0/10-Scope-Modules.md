# 10: Scope & Modules

**Duration:** 40 minutes | **Difficulty:** Intermediate | **Key Skill:** Understanding variable scope

---

## í¾¯ What You'll Learn

- Global vs local variables
- Importing modules
- Using built-in and third-party modules

---

## í³š Variable Scope

\`\`\`python
# Global variable
x = 10

def func():
    # Local variable
    y = 20
    print(x)  # Can access global
    print(y)  # Can access local

func()
print(x)  # 10
# print(y)  # ERROR - y doesn't exist here
\`\`\`

## í³š Modules

\`\`\`python
# Import entire module
import math
print(math.sqrt(16))  # 4.0

# Import specific function
from math import sqrt
print(sqrt(16))  # 4.0

# Import with alias
import numpy as np
\`\`\`

---
