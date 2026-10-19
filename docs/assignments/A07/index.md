# A7 – [Bracket FEA]

## Objective

- Use Finite Element Analysis (FEA) to improve the bracket design from previous assignments.
- Ensure high stiffness, strength, and lightweight optimization through iterative design.
- Conduct multiple FEA simulations, refining geometry based on results.
- Perform static stress analysis, including constraints, loading, and meshing selection.
- Interpret data by identifying max stress, displacement, and safety factors.
- Optimize the design by modifying geometry to enhance performance.
- Document the entire process with images, calculations, and insights.
- Reflect on key engineering lessons learned and time spent.

I am to use finite element analysis to learn and comprehend a deeper understanding of how FEA can be used in a design process. Using previous design projects, 5 and 6. 

The task is to create a high stiff, high strength and light weight component. Use FEA to influence my decision making throughout the design. Each step throughout the analysis and before I make geometric changes, I need to make sure the components results (stress/displacement/safety factor) converge on a 7% difference. I can achieve this by modifying the number of elements. If after three attempts to converge use the stiffness and stress from the finer mesh size use the finest mesh size and proceed through. 
 

## Bracket FEA - Design 1: Initial Analysis

I created a static study and applied fixed restraints to the undersides of the two upper lips that engage the rigid T-beam. This simplifies the supporting connection as fully restrained at those surfaces. I applied a total downward force of 1,200 lbf, representing two strap legs carrying 600 lbf each. Split lines defined a 0.75-inch-wide band on Feature A, centered 0.50 inch from its free end. The force was distributed over this band in a single downward direction as a simplified representation of the strap loading.

I generated a high-quality solid mesh using the blended curvature-based mesher. The initial coarse mesh contained 1,240 elements and 2,381 nodes. The maximum element size was 0.463707 inch, and the minimum element size was 0.231854 inch. The mesh report listed zero distorted elements. This mesh provides the first result for comparison with subsequent finer meshes.

**Preliminary Stress Results** 

The initial coarse-mesh solution produced a maximum von Mises stress of approximately 62.61 MPa, or 9,081 psi. Using the simulation material’s displayed yield strength of 250 MPa gives an approximate yield safety factor of 3.99, slightly below the target of 4. These results are preliminary because mesh convergence has not yet been checked. The displayed deformation was magnified by approximately 180.7 times to make the bending visible.

**Mesh Refinement**

Two high-quality solid meshes were evaluated using the blended curvature-based mesher. The geometry, material, load, and supports remained unchanged during refinement.


![Screenshot](Screenshot%202026-10-19%20at%2010.17.40%20AM.png)

Using the first mesh as the reference, the maximum stress changed by 6.28%, and maximum displacement changed by 1.27%. Both changes were below 7%, satisfying the assignment’s mesh-convergence criterion after two runs. The second mesh was therefore used to report the Design I results. This satisfies the specified comparison criterion; it does not eliminate all modeling or mesh uncertainty, particularly near sharp inside corners.

**Stress Results**

The second mesh produced a maximum von Mises stress of 66.54 MPa. The maximum occurred at an inside lower corner of the T-slot, where the sidewall, Feature D, meets the bottom crosspiece, Feature C. This identified the corner as an important area to consider when modifying the bracket.

Dividing the material yield strength of 250 MPa by the maximum stress of 66.54 MPa gave a calculated safety factor of 3.76. Although the maximum stress was below yield strength, the safety factor did not meet the original target of 4.

**Displacement and Mass Results**

The maximum resultant displacement was 0.09364 mm, equivalent to approximately 0.003687 inches. It occurred near the free end of the cylindrical strap support, Feature A. This whole-bracket displacement was below 0.005 inches, providing a conservative comparison with the original per-feature deflection limit. The Mass Properties tool reported a bracket mass of 3.53 lb

**Design I Conclusion**

Design I established the baseline for evaluating the modified brackets. The two mesh runs met the assignment’s 7% convergence criterion. The reported maximum displacement was below 0.005 inches, but the calculated safety factor of 3.76 was below the target of 4. The stress concentration at the lower inside corner of the T-slot provides a reason to modify this region in Design II. Later designs will be compared using the same material, applied load, and support assumptions to evaluate changes in stress, displacement, safety factor, and mass.

![Screenshot](Screenshot%202026-10-19%20at%209.38.44%20AM.png)

![Screenshot](Screenshot%202026-10-19%20at%209.36.13%20AM.png)


![Screenshot](Screenshot%202026-10-19%20at%2010.23.29%20AM.png)


![Screenshot](Screenshot%202026-10-19%20at%2010.24.34%20AM.png)'


![Screenshot](Screenshot%202026-10-19%20at%2010.25.46%20AM.png)



![Screenshot](Screenshot%202026-10-19%20at%2010.26.37%20AM.png)


![Screenshot](Screenshot%202026-10-19%20at%2010.27.37%20AM.png)

## Design II - Modified Bracket Design and FEA






## Analyze


## Decide


## Communicate

