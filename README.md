# Python for Finance: Investment Fundamentals & Data Analytics

## Table of Contents
1. [Course Outline](#Course-Outline)
### [Part 1 - Python](#Part1)
2. [Intro to Python](#Intro-to-Python)
3. [Python Variables and Data Types](#Python-Variables-and-Data-Types)
4. [Basic Python Syntax](#Basic-Python-Syntax)
5. [Conditional Statements](#Conditional-Statements)
6. [Python Functions](#Python-Functions)
7. [Python Sequences](#Python-Sequences)
8. [Using Iterations in Python](#Using-Iterations-in-Python)
9. [Advanced Python Tools](#Advanced-Python-Tools)
### [Part 2 - Finance](#Part2)
10. [Calculating and Comparing Rates of Return](#Calculating-and-Comparing-Rates-of-Return)
11. [Measuring Investment Risk](#Measuring-Investment-Risk)
12. [Using Regressions for Financial Analysis](#Using-Regressions-for-Financial-Analysis)
13. [Markowitz Portfolio Optinmization](#Markowitz-Portfolio-Optinmization)
14. [The Capital Asset Pricing Model](#The-Capital-Asset-Pricing-Model)
15. [Multivariate Regression Analysis](#Multivariate-Regression-Analysis)
16. [Monte Carlo Simulations as a Decision-Making Tool](#Monte-Carlo-Simulations-as-a-Decision-Making-Tool)
### [Appendix](#Appendix)
17. [pandas Fundamentals](#pandas-Fundamentals)
18. [Technical Analysis](#Technical-Analysis)

### 1. Course Outline <a name="Course-Outline"></a>

#### PART 1 - Python
- Step 1 - Learn the basics
  - Syntax
  - Data Types
  - Operators
  - Conditional Statements
  - Functions
  - Lists
  - Tuples
  - Dictionaries
  - Loops
- Step 2 - More Advanced Python
  - Object-oriented programming
  - Import libraries & modules
  - Load & Organise data

#### PART 2 - Finance
- Stock returns
- Risk
- Form investment portfolios (risk and return)
- Correlation
- Diversify a portfolio
- Regression
- Markowitz's efficient frontier analysis
- What is a stock's beta?
- How to apply CAPM (Capital Asset Pricing Model) in practice
- Multivariate regressions
- Monte Carlo simulations
  - Corporate Finance context
  - Estimate stock option price
  - Price a stock

Approach:
- Finance theory behind a concept
- How to apply the theory in practice using python


## Part 1 - Python <a name="Part1"></a>
### 2. Intro to Python <a name="Intro-to-Python"></a>

#### Why Python?
- Technical advantages over other programming languages
  - Open source
    - Free
    - Multi-platform  
  - General Purpose
  - High Level
    - Intuitive syntax   
- Practical applications as a computational tool
  - Excel is not equipped to deal with BIG data

#### Why Jupyter?
- We need a client to help us read the python code
- We will be using IPython Notebook documents (*.ipynb)

#### IDE
Commands:
- Ctrl + Enter => execute code
- Shift + Enter => execute code and create a new cell
- X => cut
- C => copy
- V => paste
- A => insert new cell above
- B => insert new cell below
- D + D => delete a cell
- Y => convert cell to Code cell
- M => convert cell to Markdown cell

#### Python 2 vs Python 3
- print vs print()
- Integer Division: Python 2 does not convert remainders to floats when it comes to division of integers
- range() vs xrange()

### 3. Python Variables and Data Types <a name="Python-Variables-and-Data-Types"></a>

Assign multiple values to multiple variables
e.g. x,y = (1,2)

### 4. Basic Python Syntax <a name="Basic-Python-Syntax"></a>

Strings
- Strings are an array of characters in Python

Arithmetic operations
- To the power of - use `**` e.g. 5 to the power of 2 => `5**2`

Indexing
- Use square brackets `[]` to get an element from an array e.g. `'Hello'[3] => 'l'`
- Indexing is **zero based**

Indentation
- Indentation defines blocks of code

Logical Operators
- Order of Importance
  1. NOT
  2. AND
  3. OR

Identity Operators
- IS
- IS NOT

### 5. Conditional Statements <a name="Conditional-Statements"></a>

If statement
e.g. 
```
if x > 200:
    print ("Big")
elif x > 100 and x <= 200:
    print ("Average")
elif x >= 0 and x <= 100:
    print ("Small")
else: 
    print ("Negative")
```
    
### 6. Python Functions <a name="Python-Functions"></a>

Syntax
```
def compare_the_two(a, b):
    if a > b:
        print ("Greater")
    elif a < b:
        print ("Less")
    else:
        print ("Equal")
```

Calling a function
```
compare_the_two(1, 2)
```
OR
```
compare_the_two(b=2, a=1)
```

Built-in functions
- Types
  - int()
  - float()
  - str()
  - type()
- Mathematical
  - max(a,b,c,etc)
  - min(a,b,c,etc)
  - abs(-10) = 10
  - sum(list) => `list = [1,2,3.4]`
  - round(x,y)
  - pow(a,b) => `a ** b`
- Other
  - len()
- And many many more....

### 7. Python Sequences <a name="Python-Sequences"></a>

Lists
- Define using `[]` e.g. `Numbers = [1,2,3]`
- To delete an element - use the `del` keyword e.g. `del Numbers[1]`
- To add a single entry to the end - use the `.append()` operator e.g. `Numbers.append(4)`
- To add multiple entries to the end - use the `.extend([])` operator e.g. `Numbers.extend([5,6])`

List Slicing
- To obtain a range of elements from a list - use `[a:b]` - where a is the starting element and b is the ending element plus 1
- If you want to slice from the beginning - use `[:b]`
- If you want to slice to the end - use `[a:]` or `[-c:]` where c is the number of elements from the end
- Obtain index of an entry - use `.index()`
- You can also append 2 lists within a list - e.g. `[Numbers, MoreNumbers]` where both entries are defined as lists
- To order elements in a list - use `.sort()` or `.sort(reverse=True)` to sort in descending order

Tuples
- Like list but they are immutable - you cannot append or change them
- Define using `()` e.g. `x = (1,2,3)`
- Tuple is the default sequence type e.g. `y = 1,2,3,4` will be a tuple
- This is how you can assign multiple values to mutiple variables on the same line e.g. `a, b, c = 1, 2, 3`
  - This is just a tuple of variables on the left and a tuple of values on the right
- Indexing works the same as in lists
- You can place tuples within a list and then each tuple becomes a separate element within the list e.g. `List = [x,y]`
- Tuples can be helpful for variable assignment e.g. `(age, years_of_school) = "30,17".split(',')` will assign 30 to age and 17 to years_of_school
- Functions can return a tuple!

Dictionaries
- Consist of key-value pairs
- Define using `{key:value}` e.g. `dict = {"k1":"a", "k2":"b"}`
- Obtain elements of a dictionary using the key (not the index) e.g. `dict["k1"]`
- Add new key value pairs by assigning a new key to a value e.g. `dict["k3"] = "c"`
- Change an existing value by assigning an existing key to a new value e.g. `dict["k2"] = "z"`
- Values can be lists/tuples e.g. `dict["k4"] = ["x","y","z"]`
- We can create an empty dictionary by `empty_dict = {}` and add to the dictionary by assigning keys and values one by one
- Can use the `.get()` method to get a value for a key. If that key does not exist then it will return 'None' (default value)

### 8. Using Iterations in Python <a name="Using-Iterations-in-Python"></a>
### 9. Advanced Python Tools <a name="Advanced-Python-Tools"></a>
## Part 2 - Finance <a name="Part2"></a>
### 10. Calculating and Comparing Rates of Return <a name="Calculating-and-Comparing-Rates-of-Return"></a>
### 11. Measuring Investment Risk <a name="Measuring-Investment-Risk"></a>
### 12. Using Regressions for Financial Analysis <a name="Using-Regressions-for-Financial-Analysis"></a>
### 13. Markowitz Portfolio Optinmization <a name="Markowitz-Portfolio-Optinmization"></a>
### 14. The Capital Asset Pricing Model <a name="The-Capital-Asset-Pricing-Model"></a>
### 15. Multivariate Regression Analysis <a name="Multivariate-Regression-Analysis"></a>
### 16. Monte Carlo Simulations as a Decision-Making Tool <a name="Monte-Carlo-Simulations-as-a-Decision-Making-Tool"></a>

## Appendix <a name="Appendix"></a>
### 17. pandas Fundamentals <a name="pandas-Fundamentals"></a>
### 18. Technical Analysis <a name="Technical-Analysis"></a>
