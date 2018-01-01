# Math
* Calculus
* Linear algebra
* Statistics

# Calculus
## 1. Analogy
Derivative: Split patterns apart, like **X-rays**.  
Integral: Glue patterns together, like **Time-lapses**.

![circle](https://betterexplained.com/wp-content/uploads/calculus/disc_rings.png)  
![ring](https://betterexplained.com/wp-content/uploads/calculus/disc_rings_area.png)

## 2. Diagram
**[X-Ray Vision](https://betterexplained.com/wp-content/uploads/calculus/course/tree_rings.png)**  
**[Time-Lapse Vision](https://betterexplained.com/wp-content/uploads/calculus/course/640px-Acropoclipse.jpg)**  
Calculus gives us two new options: split apart and glue together, it's a step-by-step view of the world.  

**Compare of X-Ray strategy**  
![X-Ray strategy](https://betterexplained.com/wp-content/uploads/calculus/course/xray-summary-table.png)  
To compare each X-Ray strategy:  
* With rings, steps increase steadily (upward sloping line)
* With slices, steps stay the same (flat line)
* With boards, steps get larger, peak, then get smaller (up and down)  

Therefore, the "ring-to-triangle" method tell us that the slices are increasing, and by the same amount each time (since the trend line is straight).  

**The 3d Perspective**  
![3d version](https://betterexplained.com/wp-content/uploads/calculus/course/lesson3/sphere-derivation.png)    
Diagrams and analogies are easy to expand our intuition, but hard to explain.  
The math abstraction could help us.  
* It's shorter.
* The rules do the work for us.
* We generalized our thinking.  

## 3. Technical Description
**Official Math terms**

Intuitive Concept | Formal Name | Symbol
------------ | ------------- | -------------
X-Ray (split apart) | Take the derivative (derive) | ![df00](http://latex.codecogs.com/gif.latex?%5Cfrac%7Bd%7D%7Bdr%7D)
Time-lapse (glue together) | together)	Take the integral (integrate) | ![if00](http://latex.codecogs.com/gif.latex?%5Cint_)


**The Derivative**

Intuitive Visualization | Formal description | Symbol
------------ | ------------- | -------------
![d01](https://betterexplained.com/wp-content/uploads/calculus/course/ring-arrow.png) | derive the area of a circle with respect to the radius | ![df01](http://latex.codecogs.com/gif.latex?%5Cfrac%7Bd%7D%7Bdr%7DArea)
![d02](https://betterexplained.com/wp-content/uploads/calculus/course/slice-arrow.png) | derive the area of a circle with respect to the perimeter | ![df02](http://latex.codecogs.com/gif.latex?%5Cfrac%7Bd%7D%7Bdp%7DArea)
![d03](https://betterexplained.com/wp-content/uploads/calculus/course/board-arrow.png) | derive the area of a circle with respect to the x-axis | ![df03](http://latex.codecogs.com/gif.latex?%5Cfrac%7Bd%7D%7Bdx%7DArea)

**The Integral**

Formal description | Symbol | Measures Total Size Of
------------ | ------------- | -------------
integrate 2 * pi * r * dr from r=0 to r=r | ![if01](http://latex.codecogs.com/gif.latex?%5Cint_%7B0%7D%5E%7Br%7D2%5Cpi%20r%5C%2C%20dr) | ![i01](https://betterexplained.com/wp-content/uploads/calculus/course/ring-chart.png)
integrate [a pizza slice] from [p = min perimeter] to [p = max perimeter] | ![if02](http://latex.codecogs.com/gif.latex?%5Cint_%7Bp%3Dmin%7D%5E%7Bp%3Dmax%7D%28pizza%5C%2C%20slice%29%5C%2C%20dp) | ![i02](https://betterexplained.com/wp-content/uploads/calculus/course/slice-chart.png)
integrate [a board] from [x = min value] to [x = max value] | ![if03](http://latex.codecogs.com/gif.latex?%5Cint_%7Bx%3Dmin%7D%5E%7Bx%3Dmax%7D%28board%29%5C%2C%20dx) | ![i03](https://betterexplained.com/wp-content/uploads/calculus/course/board-chart.png)

## 4. Basic Theory
**Better Multiplication And Division**

Operation | Example | Notes
------------ | ------------- | -------------
Division | ![bt01](http://latex.codecogs.com/gif.latex?%5Cfrac%7By%7D%7Bx%7D) | Split whole into identical parts
Differentiation | ![bt02](http://latex.codecogs.com/gif.latex?%5Cfrac%7Bd%7D%7Bdx%7Dy) | Split whole into (possibly different) parts
Multiplication | y*x | Accumulate identical steps
Integration | ![bt04](http://latex.codecogs.com/gif.latex?%5Cint%20y%5C%2C%20dx) | Accumulate (possibly different) steps

**Better Algebra**

Algebra + Calculus | Thinking process
------------ | -------------
Area of circle=? | The area of a circle is unknown...
![ba02](http://latex.codecogs.com/gif.latex?%5Cfrac%7Bd%7D%7Bdr%7DArea%3D2%5Cpi%20r) | …but I know it splits into rings (along the radius)
![ba03](http://latex.codecogs.com/gif.latex?%5Cint%20%5Cfrac%7Bd%7D%7Bdr%7DArea%3D%5Cint%202%5Cpi%20r) | Integrate both sides…
Area=πr^2 | …and I can recreate the original area

This helps think of integrals and derivatives like squares and square roots: operations that cancel!

**Find the derivative/integral of a line**

***Example***  
A line: f(x)=4x  
The derivative: ![line01](http://latex.codecogs.com/gif.latex?%5Cfrac%7Bdf%7D%7Bdx%7D%3D%5Cfrac%7B4dx%7D%7Bdx%7D%3D4)  
The definite integral: ![line02](http://latex.codecogs.com/gif.latex?%5Cint_%7B0%7D%5E%7Bx%7D4dx%3D4x)  
The indefinite integral:![line03](http://latex.codecogs.com/gif.latex?%5Cint%204dx%3D4x&plus;C)  

***Abstract Rules***  
![line04](http://latex.codecogs.com/gif.latex?%5Cfrac%7Bd%7D%7Bdx%7Da*x%3Da) and ![line05](http://latex.codecogs.com/gif.latex?%5Cint%20a%3Dax&plus;C)  
*The little secret of integrals is that we don't need to solve them directly. We just learn to recognize the derivatives of functions we've already seen.  

**Find the derivative/integral of squares**

***Example***  
f(x)=x^2  
Perimeter=4*x
d(Perimeter)/dx=4
df=f(x+1)−f(x)=(x+1)^2−x^2=(x^2+2x+1)−x^2=2x+1  

***Explain how squares change***  
d(x^2)dx={f(x+dx)−f(x)}/dx=2x+dx  

## 5. Basic Rules
**Working With Infinity**

TODO: "+1 hour: Theory II"
