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


![Assignment 03 Screenshot](Screenshot%202026-09-09%20at%2010.01.43%20PM.png)

The deformation map showed a maximum deformation of approximately 0.00913. While the design target was .009 in. Therefore the FEA result was very close to the analytical value, showing that the parametric calculation and finite element model produced similar results. 

![Assignment 03 Screenshot](Screenshot%202026-09-09%20at%2010.04.10%20PM.png)

The Maximum Von Mises stress from the FEA was approximately 2162.5 psi. The yield strength provided for aluminum was 40 ksi. Since 2.16 ksi is less that 40 ksi the bar remains below the material yield strength under the applied load. 

![Assignment 03 Screenshot](Screenshot%202026-09-09%20at%2010.06.47%20PM.png)

The factor of safety is used to determine how safley a component can carry an applied load before the material begins to yield. It compares the materials yield strength to the maximum stress actually experienced by the component. For this design the yield strength of aluminum was given, 40 ksi. From the FEA the maximum VON Mises stress in the bar was approximately 2.16 ksi. The factor of saftey is calculated using the strength of aluminum divided by the maximum Von Mises stres sin bar. 

After calculating, this design has a factor of saftey of about 18.5, the maximum stress produced by the 400 lbf is only about 5.4 percent of the aluminums specfied yield strength. 

This means there is a large margin between the stress procuded by the applied load and the stress required to beign yielding the material. Therfore the bar is safe agaisnt yielding for the specfifed 400 lbf load. 

**Design Reflection**

The axial deflection from my parametric hand calculation was 0.00900 in, while the FEA produced a maximum deflection of approximately 0.00913 in. The percent difference between the two results was approximately 1.5%, showing that the hand calculation and FEA were in very close agreement. This close agreement was expected because the bar has a uniform cross section and is subjected to a simple axial load, with no major geometric features causing stress concentrations. The small difference between the results could be caused by the FEA mesh, numerical approximations, or rounding of the model parameters. For this simple bar, I would trust the hand calculation because the geometry and loading closely match the assumptions of the direct-tension equation. However, the FEA provides additional verification that the analytical calculation is accurate and would become more useful for more complicated geometries and loading conditions.


![Assignment 03 Screenshot](Screenshot%202026-09-09%20at%2010.18.15%20PM.png)

The hand-calculated deflection and FEA deflection are essentially the same, with only about a 1.5% difference. This close agreement is expected because the bar has a uniform cross-section and is subjected to a simple axial load. There are no holes, notches, or other geometric features that would cause major stress concentrations. Because the geometry and loading are simple, the assumptions used in the direct-tension hand calculation closely represent the FEA model. Therefore, both methods produce very similar deflection results.

For this design, I would trust the hand-calculated result slightly more because the bar has a simple uniform cross-section and is subjected to a direct axial load, which closely matches the assumptions of the direct-tension equation. The FEA result is still very useful because it verifies the hand calculation, and the small 1.5% difference between the two results shows that both methods are consistent.

If a substantial pin hole were added to the bar, it would create a stress concentration around the edge of the hole. This happens because the hole removes material that would normally carry part of the load, forcing the stress to become concentrated around the opening. For a circular hole in a plate under tension, a stress concentration factor of approximately \(K_t=3\) can be used as an estimate. Using the nominal FEA stress of 2.16 ksi, the estimated peak stress is 6.48 ksi. This is still well below the aluminum yield strength of 40 ksi. The new factor of safety is 6.17. 

The pin hole reduces the factor of safety from approximately 18.5 to 6.17 because of the increased stress around the hole. However, since the peak stress is still below the 40 ksi yield strength, the bar would still be expected to remain below yielding under the applied load. This shows why holes and other changes in geometry are important to consider because they can significantly increase local stresses.

**Design Reflection** 

Throughout this project, I learned how to use engineering calculations, parametric CAD modeling, and FEA together to design and analyze a component. I learned how parameters such as the applied load, Young’s Modulus, cross-sectional area, and maximum deflection can be used to automatically determine the dimensions of a CAD model. I also learned how to set up an FEA by assigning the correct material, applying constraints and loads, and interpreting deformation and Von Mises stress results.

Some mistakes I made during the project included initially having difficulty assigning the correct material and units, selecting the correct direction for the applied force, and understanding how to display the FEA results. Correcting these mistakes helped me better understand how important units, material properties, loads, and boundary conditions are when creating an accurate simulation.

Overall, this project helped me understand how hand calculations can be compared with computer simulations to verify an engineering design. The close agreement between my calculated and FEA deflections also gave me more confidence in both methods. The total time I spent completing the project from start to finish was approximately 6 and half hours. 

**Modify Design Parameters**

Load: I predict that increasing the applied load will decrease the calculated length of the bar. A larger force causes more axial deformation, so the bar must become shorter to maintain the same maximum deflection of 0.009 in.

Diameter / Width: I predict that increasing the diameter of the bar will increase the calculated length. Increasing the diameter increases the cross-sectional area, making the bar stiffer and allowing it to be longer while maintaining the same maximum deflection.

Height: If the cross-sectional height were increased, I predict that the calculated length would increase. Increasing the height increases the cross-sectional area and stiffness of the bar, allowing a greater length for the same load and maximum deflection.

Thickness: If the thickness were increased, I predict that the calculated length would increase. A thicker cross section provides more area to resist the axial load, so the bar can be longer without exceeding the allowable deflection.

**CAD Link** 

[Download Creo Parametric FEA File](parametric_fea.prt.4)








