# Forced Convection over a Heated Cylinder: Simulation in COMSOL

## Overview
This repository contains the COMSOL simulation file and related documentation to simulate and analyze the heat transfer and flow characteristics for a heated cylinder subjected to a uniform crossflow of colder air.

### Key Features of the Simulation:
- Reynolds number range: 0.1 to 100 (adjusted by varying inlet velocity).
- Three distinct Prandtl numbers are analyzed.
- Analysis includes hydrodynamic and thermal boundary layer development and a correlation for average Nusselt number based on Reynolds and Prandtl numbers.

---

## Problem Statement
The problem involves studying the forced convection of air over a heated cylinder placed in a uniform crossflow. The cylinder is subjected to a constant temperature, while the air enters the domain at a lower temperature. The primary objectives are:

1. To determine the velocity and temperature fields in the domain.
2. To evaluate the hydrodynamic and thermal boundary layer thicknesses.
3. To calculate the average Nusselt number for a range of Reynolds numbers and distinct Prandtl numbers.
4. To correlate the Nusselt number with Reynolds and Prandtl numbers empirically.

---

## File Structure
### **Simulation File**
- `FFD_V3.mph`: The COMSOL simulation file for the project.

---

## Simulation Details

### **COMSOL Physics Setup**
1. **Physics Interfaces**:
   - **Laminar Flow (spf):** Solves the Navier-Stokes equations to capture velocity and pressure fields.
   - **Heat Transfer in Fluids (ht):** Governs heat transfer by conduction and convection in the domain.

2. **Geometry**:
   - Cylinder placed in a 2D rectangular domain representing the flow region.

3. **Boundary Conditions**:
   - Inlet: Uniform velocity adjusted to vary Reynolds number.
   - Outlet: Pressure boundary condition (P = 0).
   - Cylinder: No-slip boundary condition for velocity and constant temperature for heat transfer.

4. **Parametric Sweeps**:
   - **Reynolds Number:** Adjusted by varying inlet velocity.
   - **Prandtl Numbers:** Three distinct values are chosen, influencing thermal conductivity.

### **Outputs**
1. Velocity and temperature fields for different Reynolds and Prandtl number combinations.
2. Hydrodynamic and thermal boundary layer thickness along the cylinder.
3. Average Nusselt number and its empirical correlation with Reynolds and Prandtl numbers.

---

## How to Use
1. Open the simulation file `FFD_V3.mph` in COMSOL Multiphysics.
2. Run the simulation using the preconfigured **Parametric Sweep** for Reynolds and Prandtl numbers.
3. Analyze the results:
   - Use **Surface Plots** for velocity and temperature fields.
   - Evaluate boundary layer thickness using **Line Graphs**.
   - Derive the Nusselt number using **Derived Values**.
4. Compare the results with the provided objectives and empirical correlations.

---

## Results Interpretation
- The velocity field provides insights into the hydrodynamic boundary layer development.
- The temperature field illustrates the thermal boundary layer behavior.
- The Nusselt number correlation validates heat transfer performance.

---

## License
This project is licensed under [MIT License](LICENSE) (if applicable). Feel free to use, modify, and distribute the contents of this repository with appropriate attribution.

---

## Contact
For questions or clarifications, please contact Abhiram Ramachandran at 24250006@iitgn.ac.in.

