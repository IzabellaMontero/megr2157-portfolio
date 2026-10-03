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

![Project Image](Screenshot%202026-10-01%20at%202.50.59%20PM.png)

Feature D consists of the two vertical side walls that connect the lower section, Feature C, to the upper retaining lips, Feature E. Each wall is 0.25 inches thick, 1.50 inches deep, and 1.50 inches high in the SolidWorks model. I created the walls symmetrically and merged them with the existing bracket. Made from ASTM A36 steel, these walls form the sides of the opening that surrounds the T-beam flange. The vertical gap between C and E is specified as 1.5000 ±0.0005 inches to provide clearance around the flange while limiting vertical play.

![Project Image](Screenshot%202026-10-01%20at%202.52.58%20PM.png)

Feature E consists of the two upper retaining lips that extend inward from the side walls, Feature D, and capture the T-beam flange. Each lip is 1.25 inches wide, 1.50 inches deep, and 0.85 inches thick in the SolidWorks model. I created the lips symmetrically and merged them with the bracket. Their width is linked to the overall bracket width and the center slot width so the geometry updates consistently. The center slot is specified as 0.500 ±0.001 inches to provide sliding clearance around the T-beam stem. Like the other features, Feature E is made from ASTM A36 steel.

**Drawing**

This section presents the bracket’s SolidWorks engineering drawing, including front, top, and right-side views arranged in third-angle projection and an isometric view to show its overall shape. Dimensions describe the size and location of each feature, while specific tolerances define the three sliding fits around the rigid T-beam. A general tolerance block specifies the allowable variation for dimensions without individual tolerances. Together, these details communicate the intended geometry and fit requirements for manufacturing and inspection.

![Project Image](Screenshot%202026-10-01%20at%202.56.44%20PM.png)

I arranged the drawing in third-angle projection, placing the top view directly above the front view and the right-side view to its right. This arrangement shows the bracket’s width, height, and depth consistently across the views. I also included an isometric view to help the reader understand the overall shape and how Features A through E connect.

I selected specific tolerances for the three bracket openings using the given T-beam dimensional limits. The center slot is 0.500 ±0.001 inches, providing 0.001–0.004 inches of total clearance where precise location is less important. Each shoulder space is 1.0000 ±0.0002 inches, providing 0.0006–0.0015 inches of clearance for a closer sliding fit. The vertical opening is 1.5000 ±0.0005 inches, providing 0.0005–0.0025 inches of clearance to limit vertical play. These custom tolerances keep each minimum opening larger than its corresponding maximum T-beam dimension. The clearance calculations assume centered, symmetric geometry.

I included the general tolerance block required by the assignment: X.X ±0.02 inches, X.XX ±0.01 inches, and X.XXX ±0.005 inches. These values define the allowable variation for dimensions without an individually specified tolerance. The three T-beam fit dimensions have their own tighter tolerances, which take precedence over the general block because those openings require closer control for assembly and sliding clearance.

**Reflections**
I connected Feature A’s diameter to the bending-strength equation in SolidWorks: d_min = [32(SF)Pa/(πS_y)]^(1/3). Using a safety factor of 4, a combined strap load of 1,200 lbf, a moment arm of 1.50 in, and an ASTM A36 steel yield strength of 36,000 psi gave a minimum diameter of approximately 1.268 in. I added a 0.032 in sizing allowance, producing a modeled diameter of approximately 1.30 in. The A_Diameter variable controls the cylinder’s sketch diameter, allowing the geometry to update automatically when the inputs change. I verified this relationship by temporarily increasing the load to 1,400 lbf, which increased the diameter to approximately 1.37 in, then restoring the original load. Feature B’s depth also updates because it is linked to A_Diameter.

![Project Image](Screenshot%202026-10-02%20at%205.27.12%20PM.png)


I applied a tighter tolerance of 0.500 ± 0.001 in to the slot that receives the T-beam stem because it is a functional mating surface. The stem ranges from 0.497 to 0.498 in, while the slot ranges from 0.499 to 0.501 in, providing clearance for sliding assembly. In comparison, the bracket’s 3.00 in overall width uses the general two-decimal tolerance of ±0.01 in because this outside dimension does not directly control the sliding fit. This looser tolerance allows more manufacturing variation while the mating openings remain controlled by their specific tolerances. Applying unnecessarily tight tolerances to non-critical dimensions would increase machining and inspection effort without improving the fit.

**Bracket Parametric Design**

![Project Image](Screenshot%202026-10-02%20at%205.56.53%20PM.png)

![Project Image](Screenshot%202026-10-02%20at%209.14.53%20PM.png)

I modeled the link in SolidWorks as a separate ASTM A36 steel plate with rounded ends and two through-holes. The plate is 2.00 in wide and 0.25 in thick, with hole centers spaced 2.50 in apart, giving an overall length of 4.50 in. Global variables control the width, thickness, spacing, and end radius. The lower hole connects to Feature A, and its diameter is defined as A_Diameter + 0.005 in using shared bracket parameters. This relationship allows the hole size to update when Feature A’s diameter changes. The upper hole has a nominal diameter of 1.00 in for the second shaft. The required sliding-fit and light press-fit tolerances will be specified on the engineering drawing.

**Reflections**

This project taught me that matching nominal dimensions alone does not guarantee compatibility between parts. The link’s hole and Feature A must have coordinated tolerances so the smallest hole remains larger than the largest shaft for a sliding fit. In contrast, the connection to the 1-inch shaft requires controlled interference for a light press fit. Linking the lower hole’s diameter to Feature A helps maintain their dimensional relationship, but the tolerance limits must still be checked separately. Dimensions communicate the link’s size and hole locations, while tolerances communicate the allowable variation needed for assembly and function. Specific fit and geometric tolerances help the manufacturer and inspector understand which surfaces require closer control.

### CAD Files

[SolidWorks Part – A6(2175)](A6%282175%29.SLDPRT)

[SolidWorks Drawing – A6 Drawing](A6_Drawing.SLDDRW)

[SolidWorks Part – Strength & Stiffness Bracket](Strength_Stiffness_Bracket.SLDPRT)

[PDF Drawing – A6(2175)](A6%282175%29.pdf)
