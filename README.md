# Python for Finance: Investment Fundamentals & Data Analytics

## Table of Contents
1. [Course Outline](#Course-Outline)
### [Part 1 - Python](#Part1)
2. [Intro to Python](#Intro-to-Python)
3. [Python Variables and Data Types](#Python-Variables-and-Data-Types)
4. [Basic Python Syntax](#Basic-Python-Syntax)
5. [Python Operators (cont.)](#Python-Operators-cont)
6. [Conditional Statements](#Conditional-Statements)
7. [Python Functions](#Python-Functions)
8. [Python Sequences](#Python-Sequences)
9. [Using Iterations in Python](#Using-Iterations-in-Python)
10. [Advanced Python Tools](#Advanced-Python-Tools)
### [Part 2 - Finance](#Part2)
11. [Calculating and Comparing Rates of Return](#Calculating-and-Comparing-Rates-of-Return)
12. [Measuring Investment Risk](#Measuring-Investment-Risk)
13. [Using Regressions for Financial Analysis](#Using-Regressions-for-Financial-Analysis)
14. [Markowitz Portfolio Optinmization](#Markowitz-Portfolio-Optinmization)
15. [The Capital Asset Pricing Model](#The-Capital-Asset-Pricing-Model)
16. [Multivariate Regression Analysis](#Multivariate-Regression-Analysis)
17. [Monte Carlo Simulations as a Decision-Making Tool](#Monte-Carlo-Simulations-as-a-Decision-Making-Tool)
### [Appendix](#Appendix)
18. [pandas Fundamentals](#pandas-Fundamentals)
19. [Technical Analysis](#Technical-Analysis)

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


### 5. Python Operators (cont.) <a name="Python-Operators-cont"></a>
### 6. Conditional Statements <a name="Conditional-Statements"></a>

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
    
### 7. Python Functions <a name="Python-Functions"></a>

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
### 8. Python Sequences <a name="Python-Sequences"></a>
### 9. Using Iterations in Python <a name="Using-Iterations-in-Python"></a>
### 10. Advanced Python Tools <a name="Advanced-Python-Tools"></a>
## Part 2 - Finance <a name="Part2"></a>
### 11. Calculating and Comparing Rates of Return <a name="Calculating-and-Comparing-Rates-of-Return"></a>
### 12. Measuring Investment Risk <a name="Measuring-Investment-Risk"></a>
### 13. Using Regressions for Financial Analysis <a name="Using-Regressions-for-Financial-Analysis"></a>
### 14. Markowitz Portfolio Optinmization <a name="Markowitz-Portfolio-Optinmization"></a>
### 15. The Capital Asset Pricing Model <a name="The-Capital-Asset-Pricing-Model"></a>
### 16. Multivariate Regression Analysis <a name="Multivariate-Regression-Analysis"></a>
### 17. Monte Carlo Simulations as a Decision-Making Tool <a name="Monte-Carlo-Simulations-as-a-Decision-Making-Tool"></a>

## Appendix <a name="Appendix"></a>
### 18. pandas Fundamentals <a name="pandas-Fundamentals"></a>
### 19. Technical Analysis <a name="Technical-Analysis"></a>
