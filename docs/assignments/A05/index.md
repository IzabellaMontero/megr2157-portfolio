# A5 – [Bracket Design]

**Objective** 

The objective of this assignment is to design a bracket that attaches to the specified T-beam and holds a polyester strap under load. The bracket must be analyzed as five connected features, A through E. For each feature, I will draw a free-body diagram, identify the loads and reactions, determine a minimum dimension from stress, and determine a minimum dimension from stiffness. I will use a safety factor of 4 and limit the deflection of each feature to 0.005 in. I will then compare the two required dimensions and document the design in separate stress and stiffness multiview sketches.

I selected ASTM A36 steel for the bracket. The assignment permits A36 steel, aluminum 6061-T6, or Ti-6Al-4V titanium. I prioritized resistance to deflection because the assignment specifies a small allowable deflection of 0.005 in per feature. A36 steel has a high elastic modulus, making it a reasonable choice for a stiffness-focused design. For my calculations, I used a yield strength of 36,000 psi and an elastic modulus of 29,000,000 psi. I will use the same material properties throughout the five feature analyses.


**Calculating dimensions from Stress Analysis**

I selected F = 600lbs. I decided to choose ASTM A36 Steel for this assignment. The bracket has a strict 0.005 in deflection limit, and A36 has the highest elastic modulus of the three permitted materials. That means it resists bending deflection well. The safety Factor is N = 4. The 0.75 wide strap is centered at the chosen force location. Its contact area extends from 0.125 into 0.875 in from the left tip. For the beam calculations, that contact is represented by a single 1200 lbf resultant at its center.

Assumptions 

- Feature A is a solid circular cantilever, fixed at its right end where it joins B.
- Both strap legs carry equal loads of 600. Their combined downward load is 1200 lbf.
- The distributed strap contact is simplified as a concentrated force at its center.
- The load is static, and ordinary linear elastic beam equations apply.
- Shear deflection is negligible, and direct shear failure is excluded as the assignment instructs.
- The fixed connection is idealized; the detailed shape and strength of that joint require separate consideration.

 ![Screenshot](Screenshot%202026-09-23%20at%202.13.01%20PM.png) 

Feature A is the cylindrical strap support, modeled as a cantilever fixed to Feature B. I chose a 2.00 in length and a total strap load of 1,200 lbf acting 1.50 in from the fixed connection. Using ASTM A36 steel and a safety factor of 4, the minimum diameter from bending stress is 1.268 in. The minimum diameter needed to limit free-tip deflection to 0.005 in is 0.730 in. Since bending stress requires the larger diameter, I selected 1.30 in. At this size, the calculated stress is 8,345 psi and the deflection is 0.000498 in, both within the required limits. The 1,200 lbf force and 1,800 lbf·in moment are carried forward to Feature B.

Feature B 
Insert iImage b 

Assumptions: B has a uniform rectangular cross section; the load and moment from A are transferred into B; A36 steel remains below its allowable normal stress. 

Feature B is the upright rectangular bar connecting the strap-support cylinder (Feature A) to the upper bracket. I selected ASTM A36 steel and used the load transferred from Feature A: a downward force of 1,200 and a 1,800 moment. The free-body diagram shows an equal upward reaction and an opposing moment at the top of B. I assumed a uniform rectangular cross section and, as directed in the assignment, did not check failure due to direct shear.

Feature C

Assumptions: Model C as a uniform beam with the load from B applied at its center, following Appendix D. Assume the end connections transfer the reactions shown on the FBD. As instructed, do not check failure from direct shear.

known values: Feature C is the lower horizontal bar of the upper bracket. Following Appendix D, I modeled it as a beam supported at both ends, with Feature B connected at its center. Feature B transfers a 1200 downward force and a 1800 counterclockwise moment to C. I selected a trial distance of Lc=2.40 between supports.

Unknowns: The unknowns are the reactions at C’s left and right supports, Rl and Rr, the minimum required vertical thickness Tc and the bending stress at the selected thickness

![Project screenshot](Screenshot%202026-09-23%20at%2010.23.29%20PM.png)

Since 8,000 < 9,000 psi, the trial cross section passes the Part 1 bending-stress calculation.

Feature D - Stress analysis 

Feature D connects the right end of Feature C to Feature E. For this analysis, I modeled D as a rectangular cantilever fixed where it joins E. From the Feature C analysis, C applies a 150 lbf upward force to D at its free end. This is a trial model that assumes the D–E connection can transfer both force and moment. 

Known values. The applied force is Pd = 150lbf. I selected ASTM A36 steel with an assumed yield strength of Sy = 36,000 psi. For the required safety factor of N=4

 I chose a trial distance of Ld = 0.50 in from the applied force to the fixed connection and a rectangular cross-section width of w = 1.50 in. 

 Unknowns. The unknowns are the reaction force and moment at E, the minimum required cross-section height hmin and the bending stress at the selected height.

 Assumptions. Feature D has a uniform rectangular cross section. Its connection to E acts as a fixed support, and the force from C acts at D’s free end. I used elementary beam bending to size D and, as directed by the assignment, did not check failure due to direct shear.

 ![Project screenshot](Screenshot%202026-09-23%20at%2010.50.34%20PM.png)

 Feature E - Stress Analysis 
 
Known values. Feature D transfers an upward force of PE = 150 lbf and a counterclockwise couple of MD = 75 lbf to Feature E. I selected ASTM A36 steel with an assumed yield strength of Sy = 36,000 psi. For a safety factor of N = 4, the allowable normal stress is Sy/an = 9,000psi

Unknowns. The unknowns are the reaction force and moment at the T beam, and the minimum cross-section height required to keep E’s bending stress below the allowable value.

Assumptions. For this trial calculation, I modeled E as a uniform rectangular beam, with D connected at its left end and a fixed T-beam restraint at its right end. I chose a trial distance e = 0.75in between those locations and a cross-section width WE = 1.50 in. These are design choices. I did not check failure due to direct shear, as instructed.
 

 

 






## Objective


## Analyze


## Decide


## Communicate

