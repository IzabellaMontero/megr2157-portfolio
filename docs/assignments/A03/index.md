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

![Assignment 03 Screenshot](Screenshot%202026-09-09%20at%2011.35.26%20AM.png)

One circular end of the bar was fixed so that it could not move. A tensile force of 400 lbf was applied to the opposite circular face along the axis of the bar.  

![Assignment 03 Screenshot](Screenshot%202026-09-09%20at%2011.39.41%20AM.png)


(Image upload) (deformation Map) 

The deformation map showed a maximum deformation of approximately 0.00913. While the design target was .009 in. Therefore the FEA result was very close to the analytical value, showing that the parametric calculation and finite element model produced similar results. 

(VON MiSSis IMage) 

The Maximum Von Mises stress from the FEA was approximately 2162.5 psi. The yield strength provided for aluminum was 40 ksi. Since 2.16 ksi is less that 40 ksi the bar remains below the material yield strength under the applied load. 

(Safety of factor Image)
The factor of safety is used to determine how Safley a component can carry an applied load before the material begins to yield. It compares the materials yield strength to the maximum stress actually experienced by the component. For this design the yield strength of aluminum was given, 40 ksi. From the FEA the maximum VON Mises stress in the bar was approximately 2.16 ksi. The factor of saftey is calculated using the strength of aluminum divided by the maximum Von Mises stres sin bar. 

After calculating this design has a factor of saftey of about 18.5, the maximum stress produced by the 400 lbf is only about 5.4 percent of the aluminums specfied yield strength. 

This means there is a large margin between the stress procuded by the applied load and the stress required to beign yeiling the material. Therfore the bar is safe agaisnt yeilding for the specfifed 400 lbf load. 







## Analyze


## Decide


## Communicate

