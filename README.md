# graph-maker

Explore how to extract useful information from poorly extracted potentiometric titration data

## Problem Domain

In the ideal world, data collected from an experiment should fit to a smooth curve with minimally possible ambiguity. In chemistry, many standard procedures typically resolve to a curve to fits to a standard shape. However in reality, that's not always the case. This project explores the possiblity of using polynomials to approximate an analytical solution to a poorly collected dataset, which can be achieved by dividing the curve into smaller sections. 

The data sample used in this project is from a titration experiment. Titration is a standard chemistry procedure to determine the pH value of a given solution. Details of how a titration work can be viewed [here](https://en.wikipedia.org/wiki/Titration). If the titration is performed manually, a visual indicator can be used to apporximate the pH value. However, in order to quantify the data, the first or second derivative of the curve is used. Typically, a well-performed titration should resolve to curve closer to a sigmoid curve, where the inflection points are the pH vlaue of the given solution. 

Also note that in the example, the solution was Na<sub>2</sub>SO<sub>3</sub?, which has two inflection points. So the approach taken in this sample determines the first infelction point by fitting first half of the curve to a sigmoid ad the second half to a 5th-degree polynomial. 

## Libraries Used
  
Libarries used in this project included `scipy`, `numpy` and `pandas`, and `matplotlib`. `scipy.optimize` was used to find the best-fit curve to the given data. 
  
## Credits
  
This project was done as a class project for CHE155 at UC Davis.
