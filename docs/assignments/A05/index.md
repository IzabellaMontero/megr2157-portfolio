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

![Project screenshot](Screenshot%202026-09-24%20at%2012.28.20%20AM.png)

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

![Project screenshot](Screenshot%202026-09-23%20at%2011.09.01%20PM.png)

**Calculating Dimensions From Stiffness Analysis** 

Known values: Feature A is a solid circular cantilever fixed to B at its right end. Its total length is L = 2.00in. The two strap legs apply a combined downward load of P = 1,200 lbf located, a = 1.50in from the fixed end. For ASTM A36 steel, use E = 29,000,000 psi. The maximum permitted deflection is Sallow = 0.005 in.

Unknowns: The minimum diameter required for stiffness, dmin, and the deflection at our selected 1.30in diameter.

Assumptions: Treat A as a uniform cantilever and represent the strap’s load by one downward force. Neglect shear deflection, as the assignment directs. Check deflection at the free left tip, where this model predicts the greatest displacement.

![Project screenshot](Screenshot%202026-09-23%20at%2011.43.28%20PM.png)

The stiffness calculation requires a minimum cylinder diameter of approximately 0.730 to keep Feature A’s free-tip deflection within 0.005in . The selected 1.30 in diameter gives a calculated deflection of 0.000498, so Feature A meets the Part 2 deflection limit under the stated cantilever assumptions.

Feature B 

Knowns: P = 1,200 lbf Lb = 1.25, E = 29,000,000 psi, and allowable axial deformation Sallow = 0.005in. 

Unknowns: The minimum area required for stiffness and the deformation of the selected bar.

Assumptions: B is a uniform, axially loaded bar. Its top connection is held in place, and shear deformation is neglected.

![Project screenshot](Screenshot%202026-09-23%20at%2011.51.14%20PM.png)

Feature C 

Knowns: E = 29,000,000psi and the deflection limit is 0.005 in 

Unknowns: the minimum thickness for stiffness and the deflection of the selected section. We assume a uniform beam and neglect shear deflection.

Assumptions. I modeled Feature C as a uniform, straight beam with a rectangular cross section. I assumed the two supports are 2.40 in apart and that Feature B applies a 1,200 downward force and a 1,800 moment at the center. I assumed the end connections provide the reactions found in Part 1, including the downward hold-down reaction at the right end. I used a constant elastic modulus of E = 29,000,000 assumed small elastic deflections, and neglected shear deflection as directed in the assignment.

![Project screenshot](Screenshot%202026-09-23%20at%2011.58.20%20PM.png)

Feature D 

Knowns: PD = 150 lbf LD = 0.50 cross-section width w = 1.50 in , selected height 0.25 in, steel modulus E = 29,000,000, and deflection limit Sallow = 0.005 in

Unknowns: The minimum height required for stiffness and the free-end deflection at the selected height.

Assumptions: D is a straight, uniform rectangular cantilever. Its connection to E is fixed, the 150 lbf force acts at its free end, deflections are small and elastic, and shear deflection is negligible.

![Project screenshot](Screenshot%202026-09-24%20at%2012.04.27%20AM.png)

Feature E 

Known values: Use ASTM A36 steel with E = 29,000,000 psi. From Feature D, the load on E is 150 lbf upward and a 75 lbf·in counterclockwise moment. Use the chosen length LE = 0.75 in, width bE = 0.75 in, and height 0.25 in. The allowed deflection for this feature is 0.005 in.

Unknowns: The deflection of Feature E and the height needed to meet the deflection limit.

Assumptions: Model E as a uniform rectangular cantilever fixed at the T beam. Treat the force and moment from D as loads at its free end. Assume small elastic deflections and neglect shear deflection, as the assignment directs.

![Project screenshot](Screenshot%202026-09-24%20at%2012.12.32%20AM.png)

Generate Multiview Sketches 

![Project screenshot](Screenshot%202026-09-24%20at%2012.25.50%20AM.png)

 

 






## Objective


## Analyze


## Decide


## Communicate

