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

For Design II, I added 0.125-inch-radius fillets to the two lower inside corners of the T-slot, where the sidewalls meet the bottom crosspiece. Design I showed high stress near these corners, so the purpose of this modification was to test whether smoother transitions would improve the bracket’s strength. ASTM A36 steel, the 1,200 lbf downward load, and the fixed supports beneath the two upper lips were retained for comparison.


![Screenshot](Screenshot%202026-10-20%20at%2011.22.59%20AM.png)


Two high-quality solid meshes were evaluated using the blended curvature-based mesher. The first mesh used maximum and minimum element sizes of 0.32 and 0.16 inches. The second mesh reduced these sizes to 0.22 and 0.11 inches. Geometry, material, supports, and loading remained unchanged between these runs.


![Screenshot](Screenshot%202026-10-20%20at%2011.19.19%20AM.png)

Maximum stress changed by approximately 0.84%, displacement changed by 1.27%, and the calculated safety factor changed by 0.84%. All three changes were below the assignment’s 7% criterion, so the second mesh was used to report Design II’s results.

The final maximum von Mises stress was 73.50 MPa. The maximum-stress annotation indicated an upper inside corner beneath the right lip, near the fixed support. Using the material library’s yield strength of 250 MPa, the calculated safety factor was 3.40. This remained below the target safety factor of 4. Stress near the fully restrained support should be interpreted with the simplified boundary conditions in mind.

The maximum resultant displacement was 0.09445 mm, or approximately 0.003719 inches, near the free end of Feature A. This was below the 0.005-inch displacement comparison limit. Mass Properties reported a mass of 3.53 lb, matching Design I at the displayed precision.

Compared with Design I, Design II’s reported maximum stress increased from 66.54 to 73.50 MPa, while displacement increased slightly from 0.003687 to 0.003719 inches. Therefore, the lower-corner fillets did not improve the reported overall strength or stiffness. This result demonstrates why a proposed improvement must be tested through analysis. Design III will use these findings to guide the next geometry change.


![Screenshot](Screenshot%202026-10-20%20at%2011.24.08%20AM.png)



![Screenshot 1](Screenshot%202026-10-20%20at%2011.25.15%20AM.png)


![Screenshot 2](Screenshot%202026-10-20%20at%2011.25.54%20AM.png)


![Screenshot 3](Screenshot%202026-10-20%20at%2011.26.39%20AM.png)


![Screenshot 4](Screenshot%202026-10-20%20at%2011.27.17%20AM.png)


![Screenshot 5](Screenshot%202026-10-20%20at%2011.27.42%20AM.png)

## Design III - Thick upper lips 

For Design III, I increased the thickness of both upper lips, Feature E, from 0.85 in to 1.10 in while retaining the fillets from Design II. This change was intended to strengthen the support region. I kept ASTM A36 steel, the 1,200 lbf downward load, and the same fixed supports so that I could compare the designs.


![Screenshot](Screenshot%202026-10-20%20at%206.49.53%20PM.png)



![Screenshot](Screenshot%202026-10-20%20at%206.46.45%20PM.png)

Between the second and third meshes, maximum displacement changed by approximately 0.73%, satisfying the 7% convergence criterion. However, maximum stress increased by approximately 36.47%, so stress did not converge within three attempts. I reported the finest-mesh results and retained this limitation when interpreting the design.

The finest mesh produced a maximum stress of 117.6 MPa at the upper-left inside corner beneath Feature E, near the fixed support. Using the material yield strength of 250 MPa, the calculated yield-based safety factor was approximately 2.13. Because the peak stress did not converge, this safety factor remains mesh dependent and does not establish that the design meets the required safety factor of 4.

Maximum displacement was 0.09571 mm, or 0.003768 in, near the free end of cylinder A. The mass was 3.90 lb, approximately 10.5% greater than the previous designs. The thicker lips therefore increased mass without demonstrating an improvement in the reported displacement or peak stress.


![Screenshot 1](Screenshot%202026-10-20%20at%206.51.15%20PM.png)

![Screenshot 2](Screenshot%202026-10-20%20at%206.51.59%20PM.png)

![Screenshot 3](Screenshot%202026-10-20%20at%206.52.32%20PM.png)

![Screenshot 4](Screenshot%202026-10-20%20at%206.52.53%20PM.png)

![Screenshot 5](Screenshot%202026-10-20%20at%206.53.12%20PM.png)

![Screenshot 6](Screenshot%202026-10-20%20at%206.53.29%20PM.png)

![Screenshot 7](Screenshot%202026-10-20%20at%206.53.48%20PM.png)

![Screenshot 8](Screenshot%202026-10-20%20at%206.54.26%20PM.png)


**Comparison of the Three Designs**


![Screenshot](Screenshot%202026-10-20%20at%206.57.22%20PM.png)

## Reflections 

This assignment taught me to check mesh convergence before interpreting finite element results. For Design III, increasing the element count from 34,158 to 103,128 changed maximum displacement by only 0.73%, but maximum stress increased by 36.47%. This showed that displacement can stabilize while peak stress remains sensitive to mesh refinement. Although I reached the assignment’s three-attempt stopping point, I could not describe Design III’s peak stress as converged.

I also learned that adding material does not automatically improve a design’s overall performance. Increasing the upper-lip thickness from 0.85 in to 1.10 in increased mass from 3.53 lb to 3.90 lb without reducing the reported maximum displacement. Design I had the lowest reported displacement and converged peak stress among the designs tested. However, none of the calculated safety factors reached the original target of 4, and Design III’s safety factor remained mesh dependent.

Keeping the material, load, and support conditions consistent helped me compare the geometry changes. The stress concentration near the fixed upper-lip region also showed why support assumptions and local geometry require careful interpretation. Future work would investigate that region and the support representation before drawing firm conclusions about strength.

I spent approximately 8 hours completing the CAD modifications, simulation setup, mesh refinement, results review, and portfolio documentation.






## Analyze


## Decide


## Communicate

