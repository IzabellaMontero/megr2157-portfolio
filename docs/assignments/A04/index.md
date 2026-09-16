# A4 – [Motor Mount]

## Objective
I am to design a motor mount using a brushed 24V DC gear motor that attaches to a rigid wall, that can safely support the applied 300 N force. The motor mount will be designed using beam bending, stress, and deflection calculations while considering a factor safety of 3 and a maximum allowable deflection of 0.30mm. The final design will include calculations for both features of the motor mount, a free body diagram, sketches, and a 3D CAD model with the appropriate mounting and clearance holes. 

( Insert Image of Figure 1 ) 

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

(Insert Image of FBD 1 ) 
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




**Feature 1** 


## Analyze


## Decide


## Communicate

