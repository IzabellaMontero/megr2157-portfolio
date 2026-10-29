# A8 – Gears

## Objective


## Shaft Design 

**Input Shaft - Power Transmission**

The objective of this section was to determine whether the specified 0.125-inch input shaft diameter was sufficient to transmit power through the gearbox. The analysis involved calculating the input torque, rotational speed, transmitted horsepower, minimum required shaft diameter, and maximum torsional shear stress. The results were compared with the allowable torsional shear stress from Machinery's Handbook, 31st Edition.

<img src="Screenshot 2026-10-27 at 7.29.07 PM.png" width="500">

<img src="Screenshot 2026-10-27 at 7.29.34 PM.png" width="500">

The gearbox was assumed to operate as an ideal gear train without mechanical power losses. The input shaft was modeled as a solid circular shaft subjected primarily to torsional loading, with bending moments neglected for this simplified analysis. An allowable torsional shear stress of 4000 psi was selected using the handbook's main power-transmitting shaft category.


The input shaft was determined to be sufficient under the simplified torsional loading conditions. The calculated maximum shear stress of 1222.31 psi was below the selected allowable shear stress of 4000 psi. Additionally, the minimum required shaft diameter of approximately 0.0842 inches was smaller than the specified 0.125-inch diameter.

Therefore, no increase in shaft diameter was necessary for the assumed loading conditions. The shaft was retained at its original diameter of 0.125 inches for the gearbox design.

**Output Shaft - Short Shaft** 

The objective of this analysis was to determine whether the specified 0.250-inch output shaft diameter was sufficient to transmit the required torque of 1.25 in·lbf at a rotational speed of 1100 rpm. The analysis included calculating the transmitted horsepower, minimum required shaft diameter, maximum torsional shear stress, and allowable horsepower capacity using the equations provided in Machinery's Handbook, 31st Edition.

<img src="Screenshot 2026-10-27 at 7.46.39 PM.png" width="500">

<img src="Screenshot 2026-10-27 at 7.47.03 PM.png" width="500">

The output shaft was determined to be sufficient under the simplified torsional loading conditions. The calculated maximum shear stress of 407.44 psi was significantly below the selected allowable torsional shear stress of 8500 psi. Additionally, the calculated minimum required shaft diameter of approximately 0.0909 inches was smaller than the provided diameter of 0.250 inches.

Therefore, the original output shaft diameter was retained without modification. The analysis confirms that the shaft satisfies the specified torsional strength criterion, subject to the assumptions made regarding loading and allowable stress.

**Journal Bearing Design**

Two journal bearings were selected for each shaft, with one bearing positioned on either side of the corresponding gear. This arrangement was chosen to provide support on both sides of the gear, improve shaft alignment, and distribute the gear-generated radial loads between the supports.

For the preliminary analysis, each gear was assumed to be centered between its two bearings, resulting in equal reaction forces. Additional radial loads, such as external shaft loads and component weights, were neglected.

<img src="Screenshot 2026-10-28 at 11.18.19 PM.png" width="500">

<img src="Screenshot 2026-10-28 at 11.18.41 PM.png" width="500">

<img src="Screenshot 2026-10-28 at 11.19.54 PM.png" width="500">

The preliminary analysis determined that each journal bearing supports approximately 1.330 lbf of radial gear loading under the assumed symmetrical arrangement.

The input bearings experience greater projected pressure and surface velocity because of their smaller dimensions and higher rotational speed. Consequently, the input bearings have the greater calculated PV requirement.

These calculations establish the operating requirements for selecting appropriate commercial journal bearings.

**Journal Bearing Wall Thickness Design**

The objective of this section was to evaluate the wall thicknesses of the journal bearings supporting the input and output shafts. The analysis involved using the dimensions of preliminary commercial sleeve-bearing candidates to determine their nominal wall thicknesses and establish the basis for evaluating their structural performance.

<img src="Screenshot 2026-10-28 at 11.39.47 PM.png" width="500">

<img src="Screenshot 2026-10-29 at 10.42.45 AM.png" width="500"> 

The journal bearing dimensions were selected from the McMaster-Carr catalog rather than choosing arbitrary wall thicknesses. This approach ensured that the proposed bearings corresponded to commercially manufactured components that could be incorporated into the gearbox CAD model.

The input bearing was selected with a nominal inside diameter of 0.125 inches and an outside diameter of 0.1875 inches. The output bearing was selected with a nominal inside diameter of 0.250 inches and an outside diameter of 0.375 inches

These dimensions were chosen to match the specified shaft sizes and provide suitable preliminary bearing geometry within the gearbox housing.

Two bearings were selected for each shaft, with one bearing positioned on each side of the gear. For the preliminary calculations, each gear was assumed to be centered between the supports, resulting in equal bearing reactions.

SAE 841 oil-embedded bronze was selected as the proposed journal bearing material due to its self-lubricating properties, widespread use in sleeve bearings, and availability in standard commercial dimensions.

The preliminary wall thicknesses of 0.03125 inches for the input journal bearings and
0.06250 inches for the output journal bearings were retained for the initial gearbox CAD design.

**Component Selection** 

Four SAE 841 oil-embedded bronze sleeve bearings were selected for the preliminary gearbox design, consisting of two bearings for the input shaft and two for the output shaft.

Input Shaft Bearings

- Manufacturer/Supplier: McMaster-Carr
- Component: Oil-Embedded Sleeve Bearing
- Part Number: 6391K611
- Quantity: 2
- Material: SAE 841 Bearing Bronze
- Nominal Shaft Diameter: 0.125 in
- Housing Bore Diameter: 0.1875 in
- Bearing Length: 0.125 in
- Nominal Wall Thickness: 0.03125 in

Output Shaft Bearings

- Manufacturer/Supplier: McMaster-Carr
- Component: Oil-Embedded Flanged Sleeve Bearing
- Part Number: 6338K411
- Quantity: 2
- Material: SAE 841 Bearing Bronze
- Nominal Shaft Diameter: 0.250 in
- Housing Bore Diameter: 0.375 in
- Bearing Length: 0.250 in
- Nominal Wall Thickness: 0.06250 in
- Flange Diameter: 0.500 in
- Flange Thickness: 0.0625 in

These bearing candidates were selected because their nominal shaft diameters match the gearbox specifications and their lengths match the preliminary length-to-diameter design ratio of 1.0.

SAE 841 oil-embedded bronze was selected due to its self-lubricating characteristics and suitability for rotating-shaft applications

**Gearbox Housing - Design**

A rounded two-piece gearbox housing was selected as the preliminary design concept. The housing follows the general outline of the meshing spur gears, providing a compact arrangement while reducing unnecessary material compared with a larger rectangular enclosure.
