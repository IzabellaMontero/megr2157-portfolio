# A6 – [Bracket Drawing]

## Objective
The objective of this project is to create a parametric SolidWorks based on the pervious strength and stiffness analyses. The bracket is designed to support a strap force of 600 lbf per leg, with a safety factor of 4 and a maximum allowable deflection of 0.005 in for each feature. The project also included a fully dimensions Multiview CAD drawing in third angle projection, with tolerances for the three sliding fits over the rigid T-Beam. The portfolio will document the model parameters, design decisions, drawings, and lessons learned. 


![Project Image](Screenshot%202026-10-01%20at%2012.25.38%20AM.png)

**3D Models**

1) Designate Materials

   ![Project Image](Screenshot%202026-10-01%20at%202.34.57%20PM.png)

   I selected ASTM A36 steel for the bracket because it provides a practical balance of strength, stiffness, and ease of fabrication. For the design calculations, I used a yield strength of 36,000 psi and a modulus of elasticity of 29,000,000 psi. With the required safety factor of 4, the allowable normal stress is 9,000 psi. Steel’s stiffness helps limit deflection under the strap load. Although it is heavier than aluminum or titanium, low weight was not a primary requirement for this project, making ASTM A36 steel a suitable choice.

I started off by putting the initial known values into the global variable chart of Solid Works. 

![Project Image](Screenshot%202026-10-01%20at%202.39.35%20PM.png)

![Project Image](Screenshot%202026-10-01%20at%202.40.43%20PM.png)


Feature A is the solid cylindrical bar that supports the polyester strap. I modeled it as a cantilever beam attached to Feature B. Each strap leg carries 600 lbf, producing a combined load of 1,200 lbf. The bar is 2.00 inches long, with the load centered 1.50 inches from the modeled fixed connection. Using ASTM A36 steel and a safety factor of 4, the bending analysis gave a minimum diameter of 1.268 inches. I selected a diameter of 1.30 inches, which gives a calculated bending stress of approximately 8,345 psi and a maximum deflection of 0.000498 inches. These values are below the allowable stress of 9,000 psi and the deflection limit of 0.005 inches under the stated beam assumptions.

![Project Image](Screenshot%202026-10-01%20at%202.43.42%20PM.png)

![Project Image](Screenshot%202026-10-01%20at%202.45.31%20PM.png)

Feature B is the rectangular support that connects the cylindrical strap bar, Feature A, to the lower bracket section, Feature C. In the SolidWorks model, it has a width of 0.85 inches, a depth of 1.30 inches, and a clear height of 1.25 inches above the cylinder. I linked its depth to Feature A’s diameter so the dimensions remain consistent when the model changes. Feature B is made from ASTM A36 steel and transfers the strap load from Feature A into the upper bracket. 

![Project Image](Screenshot%202026-10-01%20at%202.47.45%20PM.png)

Feature C is the lower horizontal section of the bracket that connects Feature B to the two side walls, Feature D. In the SolidWorks model, it is 3.00 inches wide, 1.50 inches deep, and 0.90 inches thick. I created it using a rectangular sketch and a merged extrusion so it forms part of the same solid bracket. Feature C is made from ASTM A36 steel and transfers the load from Feature B toward the side walls. 
