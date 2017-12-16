## Hello World - (EDX introduction to Python for Data Science)
# 1. Familiar functions
**Exercise:** 
Out of the box, Python offers a bunch of built-in functions to make your life as a data scientist easier. You already know two such functions: print() and type(). You've also used the functions str(), int(), bool() and float() to switch between data type. These are built-in functions as well.

Calling a function is easy. To get the type of 3.0 and store the output as a new variable, result, you can use the following:

result = type(3.0)

The general recipe for calling functions is thus:

output = function_name(input)

*Instructions:*

*1. Use print() in combination with type() to print out the type of var1.*

*2. Use len() to get the length of the list var1. Wrap it in a print() call to directly print it out.*

*3. Use int() to convert var2 to an integer. Store the output as out2.*
**Answer:**

```
# Create variables var1 and var2
var1 = [1, 2, 3, 4]
var2 = True

# Print out type of var1
print(type(var1))

# Print out length of var1
print(len(var1))

# Convert var2 to an integer: out2
out2=int(var2)
```

# 2. Multiple functions
**Exercise:** 
In the previous exercise, the square brackets around imag in the documentation showed us that the imag argument is optional. But Python also uses a different way to tell users about arguments being optional.

Have a look at the documentation of sorted() by typing help(sorted) in the IPython Shell.

You'll see that sorted() takes three arguments: iterable, key and reverse.

key=None means that if you don't specify the key argument, it will be None. reverse=False means that if you don't specify the reverse argument, it will be False.

In this exercise, you'll only have to specify iterable and reverse, not key. The first input you pass to sorted() will obviously be matched to the iterable argument, but what about the second input? To tell Python you want to specify reverse without changing anything about key, you can use =:

sorted(___, reverse = ___)
    
Two lists have been created for you on the right. Can you paste them together and sort them in descending order?

*Instructions:*

*1. Use + to merge the contents of first and second into a new list: full.*

*2. Call sorted() on full and specify the reverse argument to be True. Save the sorted list as full_sorted.*

*3. Finish off by printing out full_sorted.*
**Answer:**

```
# Create lists first and second
first = [11.25, 18.0, 20.0]
second = [10.75, 9.50]

# Paste together first and second: full
full = first + second

# Sort full in descending order: full_sorted
full_sorted = sorted(full,key=None,reverse=True)

# Print out full_sorted
print(full_sorted)
```
