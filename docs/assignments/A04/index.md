# A4 – [Motor Mount]

## Objective
I am to design a motor mount using a brushed 24V DC gear motor that attaches to a rigid wall, that can safely support the applied 300 N force. The motor mount will be designed using beam bending, stress, and deflection calculations while considering a factor safety of 3 and a maximum allowable deflection of 0.30mm. The final design will include calculations for both features of the motor mount, a free body diagram, sketches, and a 3D CAD model with the appropriate mounting and clearance holes. 

( ![Screenshot](Screenshot%202026-09-16%20at%205.41.58%20PM.png)) 

**Feature 1** 

Knowns

- P = 300 N
- N = 3
- δallow​ = 0.30 mmm
- Material = ABS
- σy​ = 26.6 MPA
- E = 1.79 GPa = 1790 MPa
- σallow​ = 29.6/3 = 9.87 MPa

Unknowns 

- L = effective length/moment arm
- b = width of feature 1
- h = thickness of feature 1
- I = area moment of inertia
- σmax = maximum bending stress
- δmax​ = maximum calculated deflection

Iv gathered everything I knew the value of and needed to find that was relevant to the first feature. 

![Screenshot](Screenshot%202026-09-16%20at%205.44.04%20PM.png)

(Insert image of Apendix B ) 

Feature 1 is modeled as a cantilever beam with a fixed connection at feature 2. the 300 n force acting on the motor shaft produces an applied bending moment M = PL as shown in appendix B. The fixed end provides and equal and opposite reaction moment MA. The loading dimensions will remain symbolic until numerical design analysis.  

Feature 1 is designed with a rectangular cross section. The force acting on the motor produces a bending moment on Feature 1. The design must satisfy two requirements: the stress must remain below the allowable stress of ABS with a safety factor of 3, and the maximum deflection must not exceed 0.30 mm. 

Bending Moment 

   The bending moment acting on feature 1 is M = PL where
   
   - P = applied force
   - L = perpendicular distance from the applied force to feature 1
   - M = bending moment

For a rectangular cross section, the area of moment of inertia is I = bh^3 / 12​. The distance from the neutral axis to the outermost surface is c = h/2. 

The bending stress equation is 

(Insert 2 images here, Images 2 and 3 ) 

I first analyzed the bending stress to make sure the ABS material would not reach its yield strength. A safety of 3 was included in this analysis. I then analyzed the deflection of feature 1 to make sure the mount would not bend more than the allowed 0.30 mm at the free end. The rectangular beam geometry was used to relate the width and thickness of the mount to its resistance to bending. From these analyses, two minimum thickness requirements were developed: one based on preventing yielding and another based on limiting deflection. The final thickness of Feature 1 will be selected so that it satieties both requirements. 

The motor has an approximate diameter of 28 mm. A Feature 1 width and length of 40 mm were selected as an initial design to provide additional material around the motor and space for the mounting features. The thickness of Feature 1 will be determined using the stress and deflection calculations.

( Enter calualtions of numerical cross sections, image 4 )

Numerical Analysis Summary: Feature 1 was initially designed with a width and length of 40 mm based on the approximate 28 mm diameter of the motor. A 20 mm moment arm was assumed to simplify the analysis, as permitted by the assignment. ABS was selected as the material, and conservative values of 29.6 MPa for yield strength and 1.79 GPa for Young's modulus were used. With a 300 N applied force and safety factor of 3, the minimum thickness based on yield strength was calculated to be approximately 9.55 mm. The minimum thickness required to limit the free-end deflection to 0.30 mm was approximately 13.89 mm. Since the deflection requirement controls the design, the thickness was rounded up to 14 mm. Therefore, the initial dimensions selected for Feature 1 are 40 mm × 40 mm × 14 mm.

**Feature 2** 

Feature 1 holds the motor, while feature 2 connects the entire mount to the wall using bolts. The load from feature 1 is transferred into feature 2, so Feature 2 also has to resist bending. 

Knowns 

- P = 300 N 
- Material: ABS 
- σy​=29.6 MPa
- δmax​=0.30 mm
- E = 1.79 GPA = 1790 MPa
- N = 3

Unknowns 

- b2 = width of Feature 2
- h2 = required thickness of feature 2
- Yield strength requirment
- Deflection requirement 


Feature 2 Design: Feature 2 is the vertical portion of the motor mount that connects the bracket to rigid wall A using bolts. ABS will continue to be used as the material for the mount. The feature will be analyzed for both bending stress and deflection under the 300 N applied load. A safety factor of 3 and a maximum allowable deflection of 0.30 mm will be used. The required cross-sectional dimensions of Feature 2 will be determined so that the mount does not yield or exceed the allowable deflection.

( insert FBD image 5 ) 

Feature 2 FBD: Feature 2 is attached to rigid wall A using bolts. The wall and bolted locations are treated as fixed supports, while the section of Feature 2 between the supports is allowed to bend. The loading from Feature 1 is transferred to Feature 2 as a bending moment. Using the assumed 20 mm moment arm and the 300 N applied force, the transferred bending moment is 6000 N·mm. This moment will be used to analyze the bending stress and deflection of Feature 2.

(insert image 6) 

Symbolic Analysis: Feature 2 was modeled as a rectangular beam subjected to the bending moment transferred from Feature 1. The beam bending equation was used to determine the minimum thickness required to prevent the ABS material from yielding while maintaining a safety factor of 3. A deflection analysis was also performed to determine the minimum thickness required to keep the deformation below 0.30 mm. The final Feature 2 thickness will be selected based on whichever requirement produces the larger minimum thickness

(insert image 7) 

Numerical Analysis: Feature 2 was analyzed using ABS with a yield strength of 29.6 MPa and Young's modulus of 1.79 GPa. A 300 N load, safety factor of 3, 20 mm moment arm, 40 mm width, and 40 mm free-to-bend length were used for the initial design. The minimum thickness based on yield strength was calculated as 9.55 mm, while the minimum thickness based on the 0.30 mm deflection limit was 13.89 mm. Since the deflection requirement produced the larger value, a final thickness of 14 mm was selected for Feature 2.

**Sketch**

 (insert image 8) 



**Feature 1** 


## Analyze


## Decide


## Communicate

