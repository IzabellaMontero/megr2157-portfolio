# A2 – Truss Stress Analysis

# Constraints 

For this assignment, I was tasked with creating a truss that fits the constraints below. 

![Truss design screenshot](Screenshot 2026-09-01 at 10.44.23 AM.png) 

Point A is a pin while point B is a roller. The length of a is, a=.4m. The height of b is, b=.3m. I was given the choice to chose a number between 20-30 for P. I chose P=24kN. 

The design process started by assigning geometry to the structure. I decided to go with a simple design and add 2 more connecting points to maximize structural support. Point E an point F. 

![Truss design screenshot](Screenshot 2026-09-01 at 11.23.43 PM.png)

The lengths of members CD, BE, EF, and FA equal .4m. Members EC and FD have a length equal to .3m. To determine the diagonal member lengths, which includes, BC, AD, CF, I used pythagorean theorem. L is equal to the square root of x^2 + y^2. I found that the length is equal to .50m. 

I drew free body diagrams for all 6 joints to be able to visualize how the forces act on one another. 

![Truss design screenshot](Screenshot 2026-09-01 at 11.46.55 PM.png)

The next step in this design process was to calculate all the external forces acting on the truss. Point B is a roller point so there is a reaction on the Y direction. Point A is pin support so there is a reaction in the Y and x direction. 


![Truss design screenshot](Screenshot 2026-09-01 at 11.50.25 PM.png)

After I found all the internal forces, identified the member with the greates internal force. Using that member, I then found an equation to find the cross sectional area. It is used to ensure that the structure can safley support the calculated internal forces withouth yielding. From the joints of anaylsis, member CF experienced the alrgest internal force of 26.67 kn in compression. This force was used as the controlling load of the design. A factor of saftey of 3.5 was applied to the yeild strength of the selecte A500 structural steel, and the minimum required cross sectional area was calulated using the allowable normal stess equation. 

**Figure: Cross sectional area** 
![Cross Section 1](Screenshot%202026-09-02%20at%2012.47.52%20PM.png)

ASTM A500 Grade C structural steel was slecte for the truss design. A yeild strength of 345 MPa was used based on published AISC meterial properties for rectuangular A500 Grade C HSS. Using the maximum calculated member force of 26.67 kN and the required factor of saftey of 3.5, the minimum cross-sectional area was calculated to be 270.8 mm^2. 


![Truss Design Screenshot](Screenshot%202026-09-02%20at%201.00.03%20PM.png)

The approximate weight of the truss was determined using the total length of all truss members, the minium required cross-sectinoal area, and the density of strucuarl steel. The lengths of all members were added to obtain a total member length of 3.7m and a steel density of 7850 kg/m^3 was used. Using the calulated cross sectiional area of 270.6mm^2, the truss has an approximate mass of 7.86kg, corresponding to a weight of approximately 77.1 N. 

## Pin Structure 

To find the cross sectional area of the connecting pins I first started with the knowns and all unknowns. The connecting pins must be designed to safely transfer forces between the members of the truss without failing in shear. The pins are made of hardened tool steel and are designed as signle shear connections. Meaning that each pin has one shear plane resisting the applied force. It has a yeild shear strength of 170 ksi and a density of 0.278 lb/in^3. A factor of safety of 4 will be applied to the given shear yeild strength to provide additional protectin against failure. The pin experiencing the largest reaction force will be used to determine the minimum required cross sectional area. The main unknown is the minimum required cross sectional area of the pins, which will be determined using the largest cross sectional area of a pin. Once the area is calulated, it can be use to determine an appropriate diameter for the pins. 

Critical Pin Free Body Diagram: The critical pin was identified using the largest internal force obtained from the truss analysis. Member CF carries the largest magnitude of force at 26.67 kN in compression, so the pin connection associated with this member was selected as the controlling case. Since the connection is designed in a single shear, the pin resists the 26.67 kN load across one shear plane, which equal and opposite forces acting on the pin to maintain equilibrium. 

![Free Body Diagram](Screenshot%202026-09-02%20at%2010.47.43%20PM.png) 


![Truss Design](Screenshot%202026-09-02%20at%2010.57.23%20PM.png) 

The minimum cross sectional area of the pin was determined by using average shear stress equation. Because the pin is designed for a single shear, only one cross sectional area resists the applied shear force. A factor of safety is include by reducing the allowable shear stress bellow the materials yield shear strength. 
- Vmax = maximum shear force on the critical pin
- FS = factor of safety
- Ty = yield strength of the pin material
- Amin = minimum required pin cross sectional area.

The minimum required pin area was calculated by substituting the maximum pin shear force, factor of safety, and the yield shear strength of the hardened tool steel into the symbolic equation. The maximum force was converted from kilonewtons to pounds force so that the units were consistent with the material strength given in 0.141 in^2. 

![Truss Design](Screenshot%202026-09-02%20at%2011.08.15%20PM.png) 

Next I have to approximate combined weight of the pins. Since the pin length was not specified in the design requirements, I selected a 1.00 inch pin length. The calculated minimum pin diameter is approximately 0.424 inches, so a 1.00 inch length provides a length to diameter ratio of approximately 1/0.424 = 2.36, giving sufficient length for the pin to pass through the connected members while allowing additional space for clearance and retention. 

All six truss joints use identical pins, so the volume of one pin was calculated and multiplied by six to determine the total pin volume. I then used the density of hardened tool steel, 0.278 lb/in^3, to determine the combined weight of the pins. 

![Truss Design](Screenshot%202026-09-02%20at%2011.33.24%20PM.png)

Therefore, using six identical pins with an assumed length of 1.00 in, the approximate combined weight of the connecting pins is 0.24lb. 

## CAD
I utilized Creo to model my truss. The truss geometry was modeled in Creo using the dimensions established during the analytical design process. The members were designed with a cross section of 0.030m x 0.010m, giving each member a cross sectional area of 0.000300 m^2 which is greater than the calculated minimum required area of 0.0002706 m^2. The two dimensional truss geometry was first created using the required a = 0.4m and b = 0.3m dimensions, and the member profiles were then extruded to 0.01o m to produce the three dimensional truss. This approach allows the truss to remain in a single CAD part while maintaing the required member dimensions and structural geometry. 

![Truss Design](Screenshot%202026-09-03%20at%201.57.33%20AM.png)

The truss was constructed in Creo as a single solid part using a series of sketches and extrusion features. The initial geometry established the overall dimensions of the truss, and material was then removed from selected region to create the open spaces between the structural members. Each member was designed with a width of 0.030m and thickness of 0.010m, maintaing the cross sectional area selected from the analytical calculations. 

![Truss Design](Screenshot%202026-09-03%20at%202.04.56%20AM.png)

![Truss Design](Screenshot%202026-09-03%20at%202.15.29%20AM.png)

The final truss geometry was created in Cro using the dimensions determined from the inital truss design and hand calulation. Material was reomved from the solid profile to form horizontal, vertical, and diagonal members while keeping all members connected as a single part. 

![Pin CAD Model](Screenshot%202026-09-03%20at%202.32.31%20AM.png)

![Pin CAD Model](Screenshot%202026-09-03%20at%202.32.38%20AM.png)

The connecting pins were modeled separately in Creo as cylindrical components. A diameter of 0.0127 m (0.500in) was selected, which is greater than the calculated minimum diameter of approximately 0.424in. A pin length of 0.0254m (1.00in) was used as the previosly established design assumption, providing a consistent pin geometry for all six joints. 

## Lesson Learned 
Through this project, I learned how structural analysis and material properties are used together to design a truss that can safely support an applied load. I learned how to determine the internal forces within each truss member and identify whether each member is subjected to tension or compression. These forces were then used to calculate the required cross-sectional areas while considering the material's yield strength and the required factor of safety. I also learned that increasing the dimensions of a structural member can improve its load-carrying capability but also increases the overall weight of the structure, demonstrating the importance of weight optimization in engineering design. Additionally, I learned how pin dimensions can be selected based on the forces transferred through the joints and how the final calculated dimensions can be incorporated into a three-dimensional CAD model. Overall, this project demonstrated how structural analysis, material selection, safety factors, geometric constraints, and CAD modeling must work together to produce a structurally stable and weight-efficient truss.
## Objective


## Analyze


## Decide
_Which geometry did you select, and why? This is your first open design choice in the course — defend it._

## Communicate

