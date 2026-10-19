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

(Insert image here) 

**Bracket FEA - Design 1: Initial Analysis"**

I created a static study and applied fixed restraints to the undersides of the two upper lips that engage the rigid T-beam. This simplifies the supporting connection as fully restrained at those surfaces. I applied a total downward force of 1,200 lbf, representing two strap legs carrying 600 lbf each. Split lines defined a 0.75-inch-wide band on Feature A, centered 0.50 inch from its free end. The force was distributed over this band in a single downward direction as a simplified representation of the strap loading.

I generated a high-quality solid mesh using the blended curvature-based mesher. The initial coarse mesh contained 1,240 elements and 2,381 nodes. The maximum element size was 0.463707 inch, and the minimum element size was 0.231854 inch. The mesh report listed zero distorted elements. This mesh provides the first result for comparison with subsequent finer meshes.

Preliminary Stress Results 

The initial coarse-mesh solution produced a maximum von Mises stress of approximately 62.61 MPa, or 9,081 psi. Using the simulation material’s displayed yield strength of 250 MPa gives an approximate yield safety factor of 3.99, slightly below the target of 4. These results are preliminary because mesh convergence has not yet been checked. The displayed deformation was magnified by approximately 180.7 times to make the bending visible.


## Analyze


## Decide


## Communicate

