# Section 34: Appendix 2: User-defined Functions

**Course:** Algorithmic Stock Trading and Equity Investing with Python  
**Section:** 34 - Appendix 2: User-defined Functions  
**Status:** ✅ Completed  
**Completed on:** [Add Date]

---

## 📚 Section Overview
This appendix covers **user-defined functions** in Python, a fundamental building block for writing reusable, organized, and efficient code. You'll learn about function definition, arguments, scope, and advanced function concepts.

### Lecture Breakdown
| # | Lecture | Duration | Status |
|---|---------|----------|--------|
| 362 | Defining your first user-defined Function | 6min | ✅ |
| 363 | What's the difference between Positional Arguments vs. Keyword Arguments? | 6min | ✅ |
| 364 | How to work with Default Arguments | 5min | ✅ |
| 365 | The Default Argument None | 6min | ✅ |
| 366 | How to unpack iterables | 5min | ✅ |
| 367 | Sequences as arguments and *args | 5min | ✅ |
| 368 | How to return many results | 3min | ✅ |
| 369 | Scope - easily explained | 8min | ✅ |
| 370 | Coding Exercise 6 | 1min | ✅ |

**Total Time:** 44min (All Completed ✅)

---

## 🎯 Key Learning Points (All Mastered ✅)

### Function Basics
- ✅ Defining user-defined functions with `def`
- ✅ Function syntax and structure
- ✅ Calling functions
- ✅ Return statements

### Arguments and Parameters
- ✅ Positional Arguments vs. Keyword Arguments
- ✅ Default Arguments
- ✅ Using `None` as a default argument
- ✅ Unpacking iterables (`*` and `**` operators)
- ✅ Sequences as arguments and `*args`
- ✅ Returning multiple results

### Scope
- ✅ Local vs. global scope
- ✅ Variable visibility
- ✅ Function scope rules

### Practical Application
- ✅ Completed Coding Exercise 6

---

## 📝 Personal Notes
*Add your own notes, code snippets, or tips here:*

### Basic Function Syntax
```python
# Define a function
def greet(name):
    """This function greets the user."""
    return f"Hello, {name}!"

# Call the function
greet("Alice")
```

### Arguments and Parameters
```python
# Positional Arguments
def describe_animal(animal_type, name):
    return f"A {animal_type} named {name}"

# Default Arguments
def greet(name, greeting="Hello"):
    return f"{greeting}, {name}!"

# *args (variable number of arguments)
def sum_numbers(*args):
    return sum(args)

# Returning multiple values
def get_min_max(numbers):
    return min(numbers), max(numbers)
```

### Scope Example
```python
global_var = "I'm global"

def scope_demo():
    local_var = "I'm local"
    print(local_var)  # Works
    print(global_var)  # Works

# print(local_var)  # Error - local_var not accessible outside function
```

### Unpacking Iterables
```python
# Unpacking a list
numbers = [1, 2, 3]
def add_three(a, b, c):
    return a + b + c

add_three(*numbers)  # Equivalent to add_three(1, 2, 3)

# Unpacking a dictionary
def describe_person(name, age):
    return f"{name} is {age} years old"

person = {"name": "Bob", "age": 30}
describe_person(**person)  # Equivalent to describe_person(name="Bob", age=30)
```

---

## 🚀 All Lectures Completed ✅

| Lecture | Status |
|---------|--------|
| 362. Defining your first user-defined Function | ✅ |
| 363. Positional vs. Keyword Arguments | ✅ |
| 364. Default Arguments | ✅ |
| 365. The Default Argument None | ✅ |
| 366. How to unpack iterables | ✅ |
| 367. Sequences as arguments and *args | ✅ |
| 368. How to return many results | ✅ |
| 369. Scope - explained | ✅ |
| 370. Coding Exercise 6 | ✅ |

---

## 🔗 Resources
- [Python Functions Documentation](https://docs.python.org/3/tutorial/controlflow.html#defining-functions)
- [*args and **kwargs in Python](https://docs.python.org/3/tutorial/controlflow.html#more-on-defining-functions)
- [Python Scope Rules](https://docs.python.org/3/tutorial/classes.html#python-scopes-and-namespaces)

---

## 💡 Key Takeaways from This Section
- **Functions** promote code reuse and organization.
- **Positional arguments** are matched by order; **keyword arguments** are matched by name.
- **Default arguments** allow flexible function calls.
- **`None`** is a great default argument for indicating "no value provided."
- **`*args`** and `**kwargs` allow flexible function definitions.
- **Scope** determines where variables are accessible.
- Functions can **return multiple values** as a tuple.
- **Unpacking** makes function calls cleaner and more flexible.
- This section builds a strong foundation for writing professional Python code for algorithmic trading.
