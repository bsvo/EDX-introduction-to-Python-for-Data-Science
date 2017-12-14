## Hello World - (EDX introduction to Python for Data Science)
# 1. The Python interface
*Instructions:*

*1. Experiment in the IPython Shell; type 5 / 8, for example.*

*2. Add another line of code to the Python script: print(7 + 10).*

*3. Hit Submit Answer to execute the Python script and receive feedback.*

**Answer:**
``` 
# Example, do not modify!
print(5 / 8)

# Put code below here
print(7/10)

```
# 2. Any Comments?
**Exercise**: Something that Filip didn't mention in his videos is that you can add comments to your Python scripts. Comments are important to make sure that you and others can understand what your code is about.

To add comments to your Python script, you can use the '#' tag. These comments are not run as Python code, so they will not influence your result. As an example, take the comment on the right, just testing division: it is completely ignored during execution.

*Instructions:*

 *1. Above the print(7 + 10), add the comment Addition works too.*

**Answer:**
``` 
# Just testing division
print(5 / 8)

#Addition works too
print(7 + 10)

```

# 3. Python as a calculator
**Exercise**: 
Python is perfectly suited to do basic calculations. Apart from addition, subtraction, multiplication and division, there is also support for more advanced operations such as:
* Exponentiation: ** . This operator raises the number to its left to the power of the number to its right: for example 4**2 will give 16.

* Modulo: %. It returns the remainder of the division of the number left by the number on its right, for example 18 % 7 equals 4.

The code in the script on the right gives some examples.

*Instructions:*

 *Suppose you have $100, which you can invest with a 10% return each year. After one year, it's 100×1.1=110
100×1.1=110 dollars, and after two years it's 100×1.1×1.1=121. Add code on the right to calculate how much money you end up with after 7 years.*

**Answer:**
``` 
# Addition and subtraction
print(5 + 5)
print(5 - 5)

# Multiplication and division
print(3 * 5)
print(10 / 2)

# Exponentiation
print(4 ** 2)

# Modulo
print(18 % 7)

# How much is your $100 worth after 7 years?
print(100*((1.1)**7))

```
