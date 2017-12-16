## Hello World - (EDX introduction to Python for Data Science)
# 1. Import package
**Exercise:** 
As a data scientist, some notions of geometry never hurt. Let's refresh some of the basics. For a fancy clustering algorithm, you want to find the circumference C and area A of a circle. When the radius of the circle is r, you can calculate C and A as:
  
  C=2πr
  
  A=πr2

To use the constant pi, you'll need the math package. A variable r is already coded in the script. Fill in the code to calculate C and A and see how the print() functions create some nice printouts.

*Instructions:*

*1. Import the math package. Now you can access the constant pi with math.pi.*

*2. Calculate the circumference of the circle and store it in C.*

*3. Calculate the area of the circle and store it in A.*

**Answer:**

```
# Definition of radius
r = 0.43

# Import the math package
import math

# Calculate C
C = 2*r*math.pi

# Calculate A
A = r*r*math.pi

# Build printout
print("Circumference: " + str(C))
print("Area: " + str(A))
```

# 2. Selective Import
**Exercise:** 
General imports, like import math, make all functionality from the math package available to you. However, if you decide to only use a specific part of a package, you can always make your import more selective:

  from math import pi
  
Let's say the Moon's orbit around planet Earth is a perfect circle, with a radius r (in km) that is defined in the script.

*Instructions:*

*1. Perform a selective import from the math package where you only import the radians function.*

*2. Calculate the distance travelled by the Moon over 12 degrees of its orbit. Assign the result to dist. You can calculate this as r∗ϕ where r is the radius and ϕ is the angle in radians. To convert an angle in degrees to an angle in radians, use the radians() function, which you just imported.*

*3. Print out dist.*

**Answer:**

```
# Definition of radius
r = 192500

# Import radians function of math package
from math import radians

# Travel distance of Moon if 12 degrees. Store in dist.
dist= radians(12)*r
# Print out dist
print(dist)
```

