# python Task
## 🐍 Python Fundamentals Overview

This section provides a summary of important Python topics covered in the project, including operators, strings, lists, tuples, file handling, and exception handling.

---

### ⚙️ Python Operators
Python operators are special symbols used to perform operations on variables and values.

| Type | Description | Example |
|------|--------------|----------|
| **Arithmetic Operators** | Perform mathematical operations | `+`, `-`, `*`, `/`, `//`, `%`, `**` |
| **Comparison Operators** | Compare two values | `==`, `!=`, `>`, `<`, `>=`, `<=` |
| **Logical Operators** | Combine conditional statements | `and`, `or`, `not` |
| **Assignment Operators** | Assign values to variables | `=`, `+=`, `-=`, `*=`, `/=`, `%=` |
| **Bitwise Operators** | Operate on bits | `&`, `|`, `^`, `~`, `<<`, `>>` |
| **Membership Operators** | Test membership in a sequence | `in`, `not in` |
| **Identity Operators** | Compare memory locations | `is`, `is not` |

---

### 🔤 String Methods
Strings in Python are immutable sequences of characters.  
Commonly used methods include:

| Method | Description | Example |
|--------|--------------|----------|
| `upper()` | Converts to uppercase | `"python".upper()` → `PYTHON` |
| `lower()` | Converts to lowercase | `"HELLO".lower()` → `hello` |
| `strip()` | Removes whitespace | `" Hello ".strip()` → `"Hello"` |
| `replace(a, b)` | Replaces substring | `"Netflix".replace("Net", "Hot")` → `"Hotflix"` |
| `split()` | Splits string by spaces | `"data science".split()` → `['data', 'science']` |
| `join()` | Joins elements with separator | `" ".join(['Hello', 'World'])` → `"Hello World"` |
| `find()` | Returns index of substring | `"Python".find("th")` → `2` |

---

### 🧺 List Methods
Lists are ordered, mutable collections.

| Method | Description | Example |
|--------|--------------|----------|
| `append(x)` | Adds an element | `[1,2].append(3)` → `[1,2,3]` |
| `extend(iterable)` | Adds multiple elements | `[1,2].extend([3,4])` → `[1,2,3,4]` |
| `insert(i, x)` | Inserts element at position | `[1,2].insert(1,9)` → `[1,9,2]` |
| `remove(x)` | Removes first occurrence | `[1,2,3].remove(2)` → `[1,3]` |
| `pop(i)` | Removes and returns element | `[1,2,3].pop()` → `3` |
| `sort()` | Sorts list | `[3,1,2].sort()` → `[1,2,3]` |
| `reverse()` | Reverses list | `[1,2,3].reverse()` → `[3,2,1]` |

---

### 🧱 Tuple Methods
Tuples are ordered and **immutable** collections.

| Method | Description | Example |
|--------|--------------|----------|
| `count(x)` | Returns number of occurrences | `(1,2,2,3).count(2)` → `2` |
| `index(x)` | Returns first index of value | `(1,2,3).index(2)` → `1` |

*(Tuples cannot be changed after creation.)*

---

### 📁 File Handling
Python provides built-in functions to handle files easily.

| Mode | Description |
|------|--------------|
| `'r'` | Read mode (default) |
| `'w'` | Write mode (overwrites existing file) |
| `'a'` | Append mode (adds to existing file) |
| `'r+'` | Read and write mode |

**Example:**
```python
# Writing to a file
with open("data.txt", "w") as f:
    f.write("Hello, Netflix Project!")

# Reading from a file
with open("data.txt", "r") as f:
    content = f.read()
    print(content)
