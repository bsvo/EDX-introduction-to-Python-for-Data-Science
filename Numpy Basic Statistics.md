## Numpy Basic Statistics - (EDX introduction to Python for Data Science)
# 1. Average versus median
**Exercise:** 
You now know how to use Numpy functions to a get a better feeling for your data. It basically comes down to importing Numpy and then calling several simple functions on the Numpy arrays:

import numpy as np

x = [1, 4, 8, 10, 12]

np.mean(x)

np.median(x)

The baseball data is available as a 2D Numpy array with 3 columns (height, weight, age) and 1015 rows. The name of this Numpy array is np_baseball. After restructuring the data, however, you notice that some height values are abnormally high. Follow the instructions and discover which summary statistic is best suited if you're dealing with so-called outliers.

*Instructions:*

*1. Create Numpy array np_height, that is equal to first column of np_baseball.*

*2. Print out the mean of np_height.*

*3. Print out the median of np_height.*

**Answer:**

```
# np_baseball is available

# Import numpy
import numpy as np

# Create np_height from np_baseball
np_height=np_baseball[:,0]

# Print out the mean of np_height
print(np.mean(np_height))

# Print out the median of np_height
print(np.median(np_height))
```

# 2. Explore the baseball data
**Exercise:** 
Because the mean and median are so far apart, you decide to complain to the MLB. They find the error and send the corrected data over to you. It's again available as a 2D Numpy array np_baseball, with three columns.

The Python script on the right already includes code to print out informative messages with the different summary statistics. Can you finish the job?

*Instructions:*

*1. The code to print out the mean height is already included. Complete the code for the median height. Replace None with the correct code.*

*2. Use np.std() on the first column of np_baseball to calculate stddev. Replace None with the correct code.*

*3. Do big players tend to be heavier? Use np.corrcoef() to store the correlation between the first and second column of np_baseball in corr. Replace None with the correct code.*

**Answer:**

```
# np_baseball is available

# Import numpy
import numpy as np

# Print mean height (first column)
avg = np.mean(np_baseball[:,0])
print("Average: " + str(avg))

# Print median height. Replace 'None'
med = np.median(np_baseball[:,0])
print("Median: " + str(med))

# Print out the standard deviation on height. Replace 'None'
stddev = np.std(np_baseball[:,0])
print("Standard Deviation: " + str(stddev))

# Print out correlation between first and second column. Replace 'None'
```

# 3. Blend it all together
**Exercise:** 
In the last few exercises you've learned everything there is to know about heights and weights of baseball players. Now it's time to dive into another sport: soccer.

You've contacted the FIFA for some data and they handed you two lists. The lists are the following:

    positions = ['GK', 'M', 'A', 'D', ...] heights = [191, 184, 185, 180, ...]
    
Each element in the lists corresponds to a player. The first list, positions, contains strings representing each player's position. The possible positions are: 'GK' (goalkeeper), 'M' (midfield), 'A' (attack) and 'D' (defense). The second list, heights, contains integers representing the height of the player in cm. The first player in the lists is a goalkeeper and is pretty tall (191 cm).

Each element in the lists corresponds to a player. The first list, positions, contains strings representing each player's position. The possible positions are: 'GK' (goalkeeper), 'M' (midfield), 'A' (attack) and 'D' (defense). The second list, heights, contains integers representing the height of the player in cm. The first player in the lists is a goalkeeper and is pretty tall (191 cm).

*Instructions:*

*Convert heights and positions, which are regular lists, to numpy arrays. Call them np_heights and np_positions.*

*2. Extract all the heights of the goalkeepers. You can use a little trick here: use np_positions == 'GK' as an index for np_heights. Assign the result to gk_heights.*

*3. Extract all the heights of the all the other players. This time use np_positions != 'GK' as an index for np_heights. Assign the result to other_heights.*

*4. Print out the median height of the goalkeepers using np.median(). Replace None with the correct code.*

*5. Do the same for the other players. Print out their median height. Replace None with the correct code.*


**Answer:**

```
# heights and positions are available as lists

# Import numpy
import numpy as np

# Convert positions and heights to numpy arrays: np_positions, np_heights
np_positions=np.array(positions)
np_heights=np.array(heights)


# Heights of the goalkeepers: gk_heights
gk_heights=np_heights[np_positions=='GK']

# Heights of the other players: other_heights
other_heights=np_heights[np_positions != 'GK']

# Print out the median height of goalkeepers. Replace 'None'
print("Median height of goalkeepers: " + str(np.median(gk_heights)))

# Print out the median height of other players. Replace 'None'
print("Median height of other players: " + str(np.median(other_heights)))
```
