# A9 – Pulleys

## Objective

The objective of this project is to design and analyze a belt-driven pulley system using mechanical engineering principles and SolidWorks. The system consists of two equally sized pulleys connected by a polyurethane rubber belt to transfer rotational motion and torque. The design process involves selecting a suitable belt, determining shaft dimensions, choosing journal bearings, and developing a supporting frame.

Engineering calculations will be performed to evaluate belt tension, normal stress, torsional stress, bearing pressure, and overall system safety. The design must satisfy a minimum factor of safety of 3 while meeting the specified operating requirements. Components will be selected using engineering calculations and manufacturer specifications, and the final assembly will be modeled in SolidWorks.

(Insert image from A9 instructions) 

## Belt Driven Pulley System Design 

The belt selection process begins by identifying the known and unknown parameters and developing free-body diagrams of the pulley system. The belt-friction equation is used to estimate the maximum tight-side and loose-side tensions before slipping. The normal stress equation and required safety factor are then used to calculate the minimum belt cross-sectional area and diameter.

A standard belt diameter will be selected based on the calculations, followed by a safety factor verification and a determination of the required belt circumference. The final selection will be compared with available polyurethane round belts from McMaster-Carr.

![Screenshot](Screenshot%202026-11-02%20at%205.28.11%20PM.png)

![Screenshot 1](Screenshot%202026-11-03%20at%201.12.20%20PM.png)

![Screenshot 2](Screenshot%202026-11-03%20at%201.12.49%20PM.png)

![Screenshot 3](Screenshot%202026-11-03%20at%201.13.22%20PM.png)

A polyurethane rubber round belt was identified from McMaster-Carr based on the calculated minimum belt diameter and geometric requirements. The minimum belt diameter was calculated to be 0.242 inches, so a standard 0.250-inch diameter belt was chosen for evaluation.

The selected candidate has an outer circumference of 20.25 inches, compared with the calculated ideal geometric circumference of approximately 20.21 inches. Under the simplified tensile-stress analysis, the belt achieves a calculated safety factor of 3.21, exceeding the required minimum of 3.

After selecting the original 20.25-inch polyurethane belt, I reviewed the design and identified a problem with my initial selection method. I had chosen the belt based on how closely its catalog circumference matched my calculated geometric circumference of 20.21 inches. However, this approach did not account for installation stretch, which is necessary to generate tension in an elastic belt.

This was an important consideration because my design specifies a stationary belt tension of 5 lbf. Without sufficient installation tension, the belt may not grip the pulleys properly and could slip during operation.

To address this issue, I evaluated a shorter 19-inch polyurethane belt from the same McMaster-Carr product family while maintaining the original 1/4-inch diameter. I assumed a 3-inch effective pulley pitch diameter and calculated the approximate installation strain.

After evaluating the belt length, I investigated the maximum torque that could be transmitted without slipping. Using the limiting tight-side and loose-side tensions of 7.20 lbf and 2.80 lbf and a pulley radius of 1.5 inches, I calculated a theoretical maximum transmitted torque of 6.60 lbf·in.

Rather than designing the system to operate directly at the slipping limit, I selected a preliminary operating torque of 5.28 lbf·in, representing an assumed 20% reduction from the theoretical maximum.

At this operating torque, the calculated tight-side tension was 6.76 lbf, while the loose-side tension was 3.24 lbf. The resulting tension ratio was approximately 2.086, which is below the assumed friction-limit ratio of 2.566.

I then recalculated the belt's tensile stress using the 1/4-inch diameter and operating tight-side tension. The resulting tensile stress was approximately 137.7 psi, producing a calculated factor of safety of 3.42.These results indicate that the proposed belt satisfies the simplified tensile-strength requirement and operates below the calculated slipping threshold under the selected assumptions.

The belt selected for further evaluation is a McMaster-Carr polyurethane rubber round belt from product family 3044K606, with a nominal diameter of 1/4 inch and a proposed unloaded outer circumference of 19 inches.

The design process demonstrated the importance of considering more than the minimum required belt diameter. My initial selection accounted for material strength and geometric circumference, but further analysis showed that installation stretch and stationary tension also influence belt performance. Although the preliminary stress and friction calculations satisfy the selected design criteria, the actual belt tension and no-slip performance remain dependent on the belt's material properties and contact conditions. These quantities would need to be verified through manufacturer data. 

![Screenshot 1](Screenshot%202026-11-03%20at%202.00.38%20PM.png)

![Screenshot 2](Screenshot%202026-11-03%20at%202.01.49%20PM.png)

![Screenshot](Screenshot%202026-11-03%20at%202.04.37%20PM.png)

## Shaft Design Results 

In this part of the project, I calculated the minimum shaft diameter required to safely transmit torque through the pulley system using 1060 hardened steel. I began by identifying the known and unknown values and creating a free-body diagram showing the belt forces, torque, and bearing reactions.

Using the tight-side and loose-side tensions from Part 1, I calculated a transmitted torque of 6.60 lbf·in. I then used the material's yield strength and the required safety factor of 3 to determine the allowable shear stress. After rearranging the torsional stress equation symbolically, I calculated a minimum shaft diameter of 0.1311 inches.

I selected a standard 1/4-inch shaft to provide additional strength. After checking the torsional stress, I calculated a safety factor of 20.80, exceeding the required minimum of 3. This confirmed that the selected shaft meets the preliminary torsional strength requirements, although bending stresses still need to be evaluated.

![Screenshot 1](Screenshot%202026-11-04%20at%2011.41.08%20PM.png)

![Screenshot 2](Screenshot%202026-11-04%20at%2011.41.30%20PM.png)

![Screenshot 3](Screenshot%202026-11-04%20at%2011.41.48%20PM.png)

## Journal Bearing Design 

In this section, I designed and evaluated journal bearings to support the rotating shafts of the pulley system. I began by identifying the known and unknown values and creating a free-body diagram to determine the forces acting on each bearing. Based on the pulley arrangement, I calculated a load of 5 lbf per bearing.

Next, I modeled the equations symbolically and calculated the bearing pressure, surface velocity, and PV rating. The results were 40 psi, 98.17 ft/min, and 3,927 psi·ft/min, respectively.

Using these results, I selected oil-impregnated sintered bronze as a preliminary bearing material because of its lubrication properties and published operating limits. The calculated values were below the referenced manufacturer limits, indicating that the material is suitable for further consideration.

Overall, this section demonstrated how bearing loads, shaft speed, and material properties influence bearing selection. The final bearing dimensions and compatibility with the required handbook specifications still need to be verified.

![Screenshot 1](Screenshot%202026-11-04%20at%2011.53.39%20PM.png)

![Screenshot 2](Screenshot%202026-11-04%20at%2011.53.55%20PM.png)

## Frame Design Analysis 

For this section, I developed a preliminary support frame using 6061-T6 aluminum with dimensions of 7 × 1.5 × 0.25 inches. The frame was designed to maintain the required 5-inch spacing between the pulley shafts while supporting the belt forces.

Using a simplified 10 lbf compressive load, I calculated an average stress of 26.67 psi and a direct-stress safety factor of approximately 1312. I also estimated the frame's elastic buckling load to investigate its resistance to instability.

The results indicate that the proposed frame has substantial strength under the simplified loading conditions.




