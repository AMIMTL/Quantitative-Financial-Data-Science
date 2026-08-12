# Section 33: Appendix 1: Python (& Finance) Basics

**Course:** Algorithmic Stock Trading and Equity Investing with Python  
**Section:** 33 - Appendix 1: Python (& Finance) Basics  
**Status:** ✅ Completed  
**Completed on:** [Add Date]

---

## 📚 Section Overview
This comprehensive appendix covers the **fundamentals of Python programming** combined with **finance concepts** like the Time Value of Money (TVM). It's designed for beginners, covering everything from variables and data types to loops, functions, and financial calculations.

### Lecture Breakdown
| # | Lecture | Duration | Status |
|---|---------|----------|--------|
| 309 | Intro to the Time Value of Money (TVM) Concept (Theory) | 6min | ✅ |
| 310 | How to open and work with the Course Appendix Notebooks | 1min | ✅ |
| 311 | Calculate Future Values (FV) with Python / Compounding | 3min | ✅ |
| 312 | Calculate Present Values (PV) with Python / Discounting | 3min | ✅ |
| 313 | Interest Rates and Returns (Theory) | 4min | ✅ |
| 314 | Calculate Interest Rates and Returns with Python | 4min | ✅ |
| 315 | Introduction to Variables | 5min | ✅ |
| 316 | Excursus: How to add inline comments | 3min | ✅ |
| 317 | Variables and Memory (Theory) | 2min | ✅ |
| 318 | More on Variables and Memory | 7min | ✅ |
| 319 | Variables - Dos, Don'ts and Conventions | 4min | ✅ |
| 320 | The print() Function | 4min | ✅ |
| 321 | Coding Exercise 1 | 9min | ✅ |
| 322 | TVM Problems with many Cashflows | 3min | ✅ |
| 323 | Intro to Python Lists | 2min | ✅ |
| 324 | Zero-based Indexing and negative Indexing in Python (Theory) | 3min | ✅ |
| 325 | Indexing Lists | 3min | ✅ |
| 326 | For Loops - Iterating over Lists | 8min | ✅ |
| 327 | The range Object - another Iterable | 5min | ✅ |
| 328 | Calculate FV and PV for many Cashflows | 8min | ✅ |
| 329 | The Net Present Value - NPV (Theory) | 8min | ✅ |
| 330 | Calculate an Investment Project's NPV | 3min | ✅ |
| 331 | Coding Exercise 2 | 9min | ✅ |
| 332 | Data Types in Action | 6min | ✅ |
| 333 | The Data Type Hierarchy (Theory) | 4min | ✅ |
| 334 | Excursus: Dynamic Typing in Python | 2min | ✅ |
| 335 | Built-in Functions | 6min | ✅ |
| 336 | Integers | 3min | ✅ |
| 337 | Floats | 6min | ✅ |
| 338 | How to round Floats (and Integers) with round() | 5min | ✅ |
| 339 | More on Lists | 5min | ✅ |
| 340 | Lists and Element-wise Operations | 4min | ✅ |
| 341 | Slicing Lists | 5min | ✅ |
| 342 | Slicing Cheat Sheet | 1min | ✅ |
| 343 | Changing Elements in Lists | 3min | ✅ |
| 344 | Sorting and Reversing Lists | 4min | ✅ |
| 345 | Adding and removing Elements from/to Lists | 10min | ✅ |
| 346 | Mutable vs. immutable Objects (Part 1) | 9min | ✅ |
| 347 | Mutable vs. immutable Objects (Part 2) | 5min | ✅ |
| 348 | Coding Exercise 3 | 12min | ✅ |
| 349 | Tuples | 7min | ✅ |
| 350 | Dictionaries | 6min | ✅ |
| 351 | Intro to Strings | 9min | ✅ |
| 352 | String Replacement | 4min | ✅ |
| 353 | Booleans | 2min | ✅ |
| 354 | Operators (Theory) | 5min | ✅ |
| 355 | Comparison, Logical and Membership Operators in Action | 8min | ✅ |
| 356 | Coding Exercise 4 | 9min | ✅ |
| 357 | Conditional Statements | 9min | ✅ |
| 358 | Keywords pass, continue and break | 10min | ✅ |
| 359 | Calculate a Project's Payback Period | 5min | ✅ |
| 360 | Introduction to while loops | 8min | ✅ |
| 361 | Coding Exercise 5 | 1min | ✅ |

**Total Time:** 4hr 35min (All Completed ✅)

---

## 🎯 Key Learning Points (All Mastered ✅)

### Finance Fundamentals
- ✅ Time Value of Money (TVM) concept
- ✅ Future Value (FV) and Present Value (PV) calculations
- ✅ Interest rates and returns
- ✅ Net Present Value (NPV) for investment projects
- ✅ Payback period calculation

### Python Basics
- ✅ Variables (creation, memory, conventions)
- ✅ Comments and documentation
- ✅ The print() function
- ✅ Data types (integers, floats, booleans, strings)
- ✅ Data type hierarchy and dynamic typing
- ✅ Built-in functions
- ✅ Rounding numbers

### Data Structures
- ✅ Lists (creation, indexing, slicing, modification)
- ✅ List operations (sorting, reversing, adding/removing elements)
- ✅ Tuples (immutable sequences)
- ✅ Dictionaries (key-value pairs)
- ✅ Strings (introduction and replacement)

### Control Flow
- ✅ For loops (iterating over lists and ranges)
- ✅ While loops
- ✅ Conditional statements (if, elif, else)
- ✅ Keywords: pass, continue, break

### Operators
- ✅ Comparison operators
- ✅ Logical operators
- ✅ Membership operators

### Coding Exercises
- ✅ 5 coding exercises completed
- ✅ TVM problems with multiple cashflows
- ✅ Investment project analysis

---

## 📝 Personal Notes
*Add your own notes, code snippets, or tips here:*

### TVM Formulas in Python
```python
# Future Value
fv = pv * (1 + r) ** n

# Present Value
pv = fv / (1 + r) ** n

# Net Present Value
npv = sum(cf / (1 + r) ** t for t, cf in enumerate(cashflows))
```

### Key Python Concepts
```python
# Lists
my_list = [1, 2, 3, 4, 5]
my_list[0]  # First element (zero-based indexing)
my_list[-1]  # Last element (negative indexing)
my_list[1:4]  # Slicing (elements 1, 2, 3)

# Dictionaries
my_dict = {'key1': 'value1', 'key2': 'value2'}
my_dict['key1']  # Access by key

# Loops
for item in my_list:
    print(item)

# Conditionals
if x > 0:
    print("Positive")
elif x < 0:
    print("Negative")
else:
    print("Zero")
```

---

## 🚀 All Lectures Completed ✅

| Topic Area | Lectures Completed |
|------------|-------------------|
| TVM Fundamentals | 309-314, 322, 328-330 |
| Python Variables | 315-319 |
| Lists & Indexing | 323-327, 339-345 |
| Data Types | 332-338 |
| Tuples, Dictionaries, Strings | 349-353 |
| Operators & Conditionals | 354-357 |
| Loops & Control Flow | 358, 360 |
| Coding Exercises | 321, 331, 348, 356, 361 |

---

## 🔗 Resources
- [Python Official Documentation](https://docs.python.org/3/)
- [Python Tutorial for Beginners](https://docs.python.org/3/tutorial/)
- [Time Value of Money - Investopedia](https://www.investopedia.com/terms/t/timevalueofmoney.asp)

---

## 💡 Key Takeaways from This Section
- **TVM** is the foundation of finance - master it early.
- **Python lists** are zero-indexed and support negative indexing from the end.
- **Slicing** creates a new list with the specified range.
- **Tuples** are immutable - use them for fixed data.
- **Dictionaries** are key-value pairs - great for structured data.
- **Loops** and **conditionals** are essential for controlling program flow.
- **Coding exercises** are the best way to solidify learning.
- The combination of **Python + Finance** is powerful for algorithmic trading.
