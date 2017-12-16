## Basic Plots with mathplotlib - (EDX introduction to Python for Data Science)
# 1. Line plot (1)
**Exercise:** 
With matplotlib, you can create a bunch of different plots in Python. The most basic plot is the line plot. A general recipe is given here.

import matplotlib.pyplot as plt

plt.plot(x,y)

plt.show()

In the video, you already saw how much the world population has grown over the past years. Will it continue to do so? The world bank has estimates of the world population for the years 1950 up to 2100. The years are loaded in your workspace as a list called year, and the corresponding populations as a list called pop.

*Instructions:*

*1. print() the last item from both the year and the pop list to see what the predicted population for the year 2100 is.*

*2. Before you can start, you should import matplotlib.pyplot as plt. pyplot is a sub-package of matplotlib, hence the dot.*

*3. Use plt.plot() to build a line plot. year should be mapped on the horizontal axis, pop on the vertical axis. Don't forget to finish off with the show() function to actually display the plot.*

**Answer:**

```
# Print the last item from year and pop
print(year[-1])
print(pop[-1])

# Import matplotlib.pyplot as plt
import matplotlib.pyplot as plt

# Make a line plot: year on the x-axis, pop on the y-axis
plt.plot(year,pop)
plt.show()

```

# 2. Line plot (3)
**Exercise:** 
Now that you've built your first line plot, let's start working on the data that professor Hans Rosling used to build his beautiful bubble chart. It was collected in 2007. Two lists are available for you:

* life_exp which contains the life expectancy for each country

* gdp_cap, which contains the GDP per capita, for each country expressed in US Dollar.

GDP stands for Gross Domestic Product. It basically represents the size of the economy of a country. Divide this by the population and you get the GDP per capita.

matplotlib.pyplot is already imported as plt, so you can get started straight away.

*Instructions:*

*1. Print the last item from both the list gdp_cap, and the list life_exp; it is information about Zimbabwe.*

*2. Build a line chart, with gdp_cap on the x-axis, and life_exp on the y-axis. Does it make sense to plot this data on a line plot?.*

*3. Don't forget to finish off with a plt.show() command, to actually display the plot.*

**Answer:**

```
# Print the last item of gdp_cap and life_exp
print(gdp_cap[-1])
print(life_exp[-1])

# Make a line plot, gdp_cap on the x-axis, life_exp on the y-axis

plt.plot(gdp_cap, life_exp)

# Display the plot
plt.show()

```

# 3. Scatter plot (1)
**Exercise:** 
When you have a time scale along the horizontal axis, the line plot is your friend. But in many other cases, when you're trying to assess if there's a correlation between two variables, for example, the scatter plot is the better choice. Below is an example of how to build a scatter plot.

import matplotlib.pyplot as plt

plt.scatter(x,y)

plt.show()

Let's continue with the gdp_cap versus life_exp plot, the GDP and life expectancy data for different countries in 2007. Maybe a scatter plot will be a better alternative?

Again, the matploblib.pyplot package is available as plt.

*Instructions:*

*1. Change the line plot that's coded in the script to a scatter plot.*

*2. A correlation will become clear when you display the GDP per capita on a logarithmic scale. Add the line plt.xscale('log').*

*3. Finish off your script with plt.show() to display the plot.*

**Answer:**

```
# Change the line plot below to a scatter plot
plt.scatter(gdp_cap, life_exp)

# Put the x-axis on a logarithmic scale
plt.xscale('log')

# Show plot
plt.show()

```
# 4. Scatter plot (2)
**Exercise:** 
In the previous exercise, you saw that that the higher GDP usually corresponds to a higher life expectancy. In other words, there is a positive correlation.

Do you think there's a relationship between population and life expectancy of a country? The list life_exp from the previous exercise is already available. In addition, now also pop is available, listing the corresponding populations for the countries in 2007. The populations are in millions of people.


*Instructions:*

*1. Start from scratch: import matplotlib.pyplot as plt.*

*2. Build a scatter plot, where pop is mapped on the horizontal axis, and life_exp is mapped on the vertical axis.*

*3. Finish the script with plt.show() to actually display the plot. Do you see a correlation?*

**Answer:**

```
# Import package
import matplotlib.pyplot as plt
# Build Scatter plot
plt.scatter(pop,life_exp)

# Show plot
plt.show()

```
