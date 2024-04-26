__FINAL PROJECT: The Effect of Temperature on a Box of Chlorine Gas -  Pressure and Collisions of Particles - Nathan Tokhi and Ahmad Zaghari__

**OBJECTIVE:** For this Final Project I wanted to take a look at how gas reacts in an enclosed space, and the pressure/collision of gas particles in the box's temperature increases. This project stemmed from my own ideas about collision being coded and now I think a better visual of collisions in code would be brought up by using this example.
In this Project we will focus specifically on demonstrating how to code this problem, starting with the original equations of pressure and atomic collision, as well as taking the time to explain what each main part of the code does to the problem (like setting up a function, making random integers or creating sets/arrays/graphs/etc.) This is a very complicated process so we want to fully show every step and reasoning. We will end it off by animating and visualizing the box and the pressure v. temperature graphs to enhance and expand on the visualization aspect of Python and show how we can create steady graphs from lines of code which don't need to be calculated over and over.


**MOTIVATION:** I mostly wanted to do this problem because calculating a constantly increasing temperature and having to constantly calculate more and more data points to make graphs and show the directly proportional reaction between gas pressure and temperature within enclosed spaces and their collisions. Accurately and expansively showing off the collisions that happen within the spaces between the atoms of gas are also incredibly difficult to demonstrate, so using our coding language to have accurate, neat, and moving graphs and examples of these physical phenomena are essential to showing it off. Coding language makes calculating and actually representing the data nicer than purely by hand calculations and rough drafting data points.

**CODE/RESULTS** I have only roughly adapted the code and gotten a head start on the data, but i have a few equations and lines to show off:
**Eq for Pressure and temp:**
$$PV = nRT, P = \frac{nRT}{T}$$

R = 0.0821 # Gas Constant atmL/MolK
V = 10**3  # Volume in cm
n = 1  # 1 mol of our gas
N = 1000  # Number of points

def Pressure_calc(T):
    return (n * R * T) / V
Temp = np.linspace(0, 300, N)

P = [Pressure_calc(T) for T in Temp]

This code here is just the calculations for the pressure in the box by defining our equation just for the pressure, and as we can see the temperature is directly proportional to our pressure and the moles of gas and our constant, and is inversely proportional to Volume. We use linspace to return our temperature from 0 to 300 degrees Kelvin, with N amount of points (1000(may be changed)), then we just return our Pressure under the calculation of our equation with the bounds of our temperature. Later on we can explain what happens in reality with gas and high temperatures.

**QUESTIONS AND ANSWERS:** We expect not too many, but definitely some questions including but not limited to:
-How can we apply this to other constants? Or other changing variables? And what about other factors like material, displacement, warping, etc.
-What can we use this data for in workplaces, jobs, education, etc.
-How can other gasses effect this, and what other factors would change the results?
-error analysis for what could go wrong if we *didnt* calculate our data with Python.