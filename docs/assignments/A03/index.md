# A3 – [Parametric and FEA]

## Objective
The objective of this assignment is to design a bar which has a circular cross section. I am to use the criteria given for the material, maximum deflection, and load. I need to determine the bars minimum geometry through parametric design while under direct tension. The goal is to understand how FEA can be used to make sure the requirements for strength and deflection are met. 

**Cross Sectional Area** 
![Assignment 03 Screenshot](Screenshot%202026-09-08%20at%2011.48.13%20PM.png)
I selected a bar with a diameter of 0.50 in. Using the area equation for a circle, I calculated the cross sectional area to be 0.1963 in^2. 

**Parametric Length**

![Assignment 03 Screenshot](Screenshot%202026-09-09%20at%209.17.28%20AM.png)

The direct tension elongation equation was used to determine the length of the bar. The equation was rearranged to solve for length as L=... Using a maximum deflection of 0.009in, a cross-sectional area of 0.1963 in^2, a Youngs Modulus of 10x10^6 psi, and an applied force of 400 lbf. The calculated bar length was approximately 44.2 in. 

**Design Specs (CREO)**

With the initial dimensions and calculated length, I moved to Creo to create the bar as a parametric model. Instead of manually entering the calculated length, I created parameters and relations. That allowed Creo to calculate the length from the design inputs.

I first started by making sure I was using the correct units. Inch Pound Seconds (IPS). The IPS unit was selected because the design requirements were provided in pounds force, inches and pounds per square inch. Using a consistent unit system allowed the parametric calculation to be performed without additional unit conversions.  

![Assignment 03 Screenshot](Screenshot%202026-09-09%20at%209.26.50%20AM.png)

I then started the drawing by extruding a circle with a diameter of 0.500. I did not select a length and just left it as is. 

![Assignment 03 Screenshot](Screenshot%202026-09-09%20at%209.30.35%20AM.png)

I then created parameters for the applied force, maximum deflection, modulus of elasticity, diameter, cross sectional area, and length. The values were a 400 lbf load, 0.009 maximum deflection, 10,000,000 psi modulus of elasticity, and 0.50 in diameter. 

![Assignment 03 Screenshot](Screenshot%202026-09-09%20at%209.35.24%20AM.png)

The cross-sectional area was determined from the diameter and was calculated as 0.19635 in^2. I then used the direct tension elongation equation as a parametric relation in Creo. Instead of manually entering the final bar length, Creo calulated the length based on the assigned parameters. The resulting bar length was approximately 44.18 in. 

The calculated length and diameter parameters were linked to the actual dimensions of the CAD model. This made the model parametric, meaning that changing values such as the load, modulus of elasticity, maximum deflection, or diameter can automatically update the calculated length of the bar. 

![Assignment 03 Screenshot](Screenshot%202026-09-09%20at%209.40.13%20AM.png)

**Finite Element Analysis (FEA)**

After completing the parametric CAD model, a finite element analysis was performed using Creo Live Simulation. 

The material selected was Aluminum 6061, which has a Youngs Modulus of approximately 10,000,000 psi, matching the value used in the parametric calculation.  





## Analyze


## Decide


## Communicate

