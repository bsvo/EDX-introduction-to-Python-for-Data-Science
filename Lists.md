## Hello World - (EDX introduction to Python for Data Science)
# 1. Create a list
**Exercise:**
As opposed to int, bool etc, a list is a compound data type: you can group values together:

a = "is"
b = "nice"
my_list = ["my", "list", a, b]

After measuring the height of your family, you decide to collect some information on the house you're living in. The areas of the different parts of your house are stored in separate variables for now, as shown in the script.

*Instructions:*

*1. Create a list, areas, that contains the area of the hallway (hall), kitchen (kit), living room (liv), bedroom (bed) and bathroom (bath), in this order. Use the predefined variables.*

*2. Print areas with the print() function.*

**Answer:**

```
# area variables (in square meters)
hall = 11.25
kit = 18.0
liv = 20.0
bed = 10.75
bath = 9.50

# Create list areas
areas= [hall,kit,liv,bed,bath]

# Print areas
print(areas)

```
 # 2. Create list with different types
**Exercise:**
A list can contain any Python type. Although it's not really common, a list can also contain a mix of Python types including strings, floats, booleans, etc.

The printout of the previous exercise wasn't really satisfying. It's just a list of numbers representing the areas, but you can't tell which area corresponds to which part of your house.

The code in the script is the start of a solution. For some of the areas, the name of the corresponding room is already placed in front. Pay attention here! "bathroom" is a string, while bath is a variable that represents the float 9.50 you specified earlier.

*Instructions:*

*1. Finish the line of code that creates the areas list such that the list first contains the name of each room as a string, and then its area. More specifically, add the strings "hallway", "kitchen" and "bedroom" at the appropriate locations.*

*2. Print areas again; is the printout more informative this time?*

**Answer:**

```
# area variables (in square meters)
hall = 11.25
kit = 18.0
liv = 20.0
bed = 10.75
bath = 9.50

# Adapt list areas
areas = ["hallway",hall, "kitchen", kit, "living room", liv, "bedroom",bed, "bathroom", bath]

# Print areas
print(areas)

```
