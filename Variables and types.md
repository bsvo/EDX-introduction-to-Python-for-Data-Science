## Hello World - (EDX introduction to Python for Data Science)
# 1. Variable Assignment
**Exercise:**
In Python, a variable allows you to refer to a value with a name. To create a variable use =, like this example:

x = 5

You can now use the name of this variable, x, instead of the actual value, 5.

*Instructions:*

*1. Create a variable savings with the value 100.*

*2. Check out this variable by typing print(savings) in the script.*

**Answer:**

```# Create a variable savings
savings=100

# Print out savings
print(savings)
```

# 2. Calculations with variables
**Exercise:**
Remember how you calculated the money you ended up with after 7 years of investing $100? You did something like this:

100 * 1.10 ** 7

Instead of calculating with the actual values, you can use variables instead. The savings variable you've created in the previous exercise represents the $100 you started with. It's up to you to create a new variable to represent 1.10 and then redo the calculations!

*Instructions:*

*1. Create a variable factor, equal to 1.10.*

*2. Use savings and factor to calculate the amount of money you end up with after 7 years. Store the result in a new variable, result.*

*3. Print out the value of result.*

**Answer:**

```# Create a variable savings
savings = 100

# Create a variable factor
factor=1.1

# Calculate result
result= savings*(factor**7)

# Print out result
print(result)
```
