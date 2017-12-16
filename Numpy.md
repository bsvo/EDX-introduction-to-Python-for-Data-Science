## Numpy - (EDX introduction to Python for Data Science)
# 1. Your First Numpy Array
**Exercise:** 
We're going to dive into the world of baseball. Along the way, you'll get comfortable with the basics of Numpy, a powerful package to do data science.

A list baseball has already been defined in the Python script, representing the height of some baseball players in centimeters. Can you add some code here and there to create a Numpy array from it?
*Instructions:*

*1. Import the numpy package as np, so that you can refer to numpy with np.*

*2. Use np.array() to create a Numpy array from baseball. Name this array np_baseball.*

*3. Print out the type of np_baseball to check that you got it right.*

**Answer:**

```
# Create list baseball
baseball = [180, 215, 210, 210, 188, 176, 209, 200]

# Import the numpy package as np
import numpy as np

# Create a Numpy array from baseball: np_baseball
np_baseball=np.array(baseball)

# Print out type of np_baseb
print(type(np_baseball))
```

# 2. Baseball players' height
**Exercise:** 
You are a huge baseball fan. You decide to call the MLB (Major League Baseball) and ask around for some more statistics on the height of the main players. They pass along data on more than a thousand players, which is stored as a regular Python list: height. The height is expressed in inches. Can you make a Numpy array out of it and convert the units to centimeters?

height is already available and the numpy package is loaded, so you can start straight away (Source: stat.ucla.edu).

*Instructions:*

*1. Create a Numpy array from height. Name this new array np_height.*

*2. Print np_height.*

*3. Multiply np_height with 0.0254 to convert all height measurements from inches to meters. Store the new values in a new array, np_height_m.*

*4. Print out np_height_m and check if the output makes sense.*

**Answer:**

```
# height is available as a regular list

# Import numpy
import numpy as np

# Create a Numpy array from height: np_height
np_height=np.array(height)

# Print out np_height
print(np_height)

# Convert np_height to m: np_height_m
np_height_m= np_height*.0254

# Print np_height_m
print(np_height_m)
```
