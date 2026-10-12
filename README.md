# Advanced Vehicle HVAC Thermal Management Using Fuzzy Logic

## Project Overview

The **Advanced Vehicle HVAC Thermal Management System Using Fuzzy Logic** focuses on regulating vehicle cabin temperature to improve passenger comfort under changing environmental conditions.

The project uses a Mamdani-type Fuzzy Logic Controller (FLC) with a cabin thermal model to determine suitable HVAC control actions based on temperature-related inputs. MATLAB/Simulink is used for model development and simulation, allowing the system's temperature response to be analyzed without requiring physical vehicle hardware.

## Objectives

- Develop a fuzzy logic-based controller for vehicle HVAC systems.
- Maintain cabin temperature near the desired setpoint.
- Study cabin temperature behavior under varying ambient conditions.
- Apply Model-Based Design techniques to automotive thermal management.
- Analyze simulation outputs to evaluate temperature regulation.
- Explore opportunities for improving passenger comfort and HVAC energy efficiency.

## Features

- Fuzzy logic-based HVAC control.
- Cabin temperature regulation.
- Simulation under changing ambient temperature conditions.
- Feedback-based temperature control.
- Visualization of temperature response and simulation results.
- Model-based development using MATLAB/Simulink.

## Tools and Technologies

- MATLAB
- Simulink
- Fuzzy Logic Toolbox
- Mamdani Fuzzy Inference System
- Python and Plotly / Scilab for supplementary visualization, if applicable

## Simulation Parameters

| Parameter | Value |
|---|---:|
| Initial cabin temperature | 40°C |
| Desired cabin temperature | 24°C |
| Ambient temperature | 35°C |
| Maximum HVAC cooling capacity | 8000 W |
| Cabin thermal capacitance | 50,000 J/K |
| Number of passengers | 2 |
| Heat contribution per passenger | 100 W |
| Simulation duration | 600 seconds |
| Simulation time step | 1 second |

*These values correspond to the configured simulation model and may be adjusted for further experiments.*

## System Working

1. The system receives the actual cabin temperature and desired temperature.
2. The temperature error is evaluated.
3. The Fuzzy Logic Controller processes the inputs using membership functions and predefined fuzzy rules.
4. The controller generates HVAC control outputs.
5. The cabin thermal model calculates temperature changes based on the HVAC response and thermal conditions.
6. Feedback from the cabin model is provided to the controller.
7. Simulation outputs are recorded and analyzed to evaluate the system response.

## Fuzzy Logic Controller

The project uses a **Mamdani-type Fuzzy Inference System (FIS)** to determine HVAC control actions.

The controller uses membership functions and fuzzy rules to interpret temperature conditions and generate suitable control responses. For example, if the cabin temperature is significantly higher than the desired temperature, the controller can request stronger cooling.

The control performance depends on the implemented fuzzy rules, membership functions, output scaling, and thermal model.

## Repository Structure

```text
Advanced-Vehicle-HVAC-Thermal-Management/
│
├── README.md
│
├── model/
│   ├── HVAC_Model.slx
│   └── HVAC_Controller.fis
│
├── src/
│   └── controller_code.m
│
├── outputs/
│   ├── cabin_temperature_response.png
│   ├── ambient_temperature_variation.png
│   ├── hvac_control_output.png
│   └── HVAC_24hr_results.csv
│
├── images/
│   ├── system_architecture.png
│   ├── simulink_model.png
│   └── fuzzy_controller.png
│
├── docs/
│   └── project_report.pdf
│
└── LICENSE
```

*The filenames above are examples. Keep only files that you have created and intend to upload.*

## Simulation Outputs and Results

This section contains the output files generated during the simulation and analysis of the HVAC thermal management system.

### 1. Cabin Temperature Response

**File:** `outputs/cabin_temperature_response.png`

Add your cabin temperature versus time graph here to demonstrate how the controller regulates cabin temperature toward the desired setpoint.

<img width="572" height="451" alt="Screenshot 2026-09-25 110846" src="https://github.com/user-attachments/assets/a42a9c3c-977b-4c91-ab52-a5a6e301f396" />

### 2. Ambient Temperature Variation

**File:** `outputs/ambient_temperature_variation.png`

Add the graph showing ambient temperature variations used in the simulation.

<img width="548" height="445" alt="Screenshot 2026-09-25 110323" src="https://github.com/user-attachments/assets/0b472857-a147-4141-908a-d160574e25e1" /><img width="587" height="437" alt="Screenshot 2026-09-25 110617" src="https://github.com/user-attachments/assets/fe2df465-b378-48ea-9186-8fed6c59f761" />
<img width="547" height="446" alt="Screenshot 2026-09-25 110522" src="https://github.com/user-attachments/assets/a743b00a-c6b6-4dfd-a844-aa7ef4da7be7" />


### 3. HVAC Control Output

**File:** `outputs/hvac_control_output.png`

Add your controller output graph here to illustrate how the HVAC control action changes in response to temperature conditions.

<img width="571" height="446" alt="Screenshot 2026-09-25 110250" src="https://github.com/user-attachments/assets/db8b7502-47de-425f-96e2-2327704bdace" /><img width="1197" height="797" alt="Screenshot 2026-10-03 163717" src="https://github.com/user-attachments/assets/ba81f18c-9e2d-4f64-8887-9660ee836d2e" />

### 4. Simulation Data

**File:** `outputs/HVAC_24hr_results.csv`

Store exported simulation data in CSV format when available. This file can be used for further analysis and visualization using Python, MATLAB, or spreadsheet software.

**Suggested data columns:**

- Time
- Ambient temperature
- Cabin temperature
- Desired temperature
- HVAC control output


## Applications

- Electric vehicle cabin climate control.
- Automotive HVAC systems.
- Intelligent thermal management.
- Passenger comfort regulation.
- Automotive control-system simulation.
- Model-Based Design and controller evaluation.

## Future Scope

- Integrate battery thermal management with cabin HVAC control.
- Compare fuzzy logic control with PID control.
- Analyze HVAC energy consumption under different conditions.
- Simulate varying passenger loads and external temperatures.
- Explore real-time implementation using automotive controllers.

## Conclusion

This project demonstrates the use of fuzzy logic control for vehicle HVAC thermal management through simulation. The combination of a Fuzzy Inference System and a cabin thermal model provides a foundation for analyzing temperature regulation under different environmental conditions. The generated simulation files and plots can be used to evaluate the controller's behavior and support further development.

## Author

**Meghana Jadhav**  
Electronics and Telecommunication Engineering  
Pimpri Chinchwad College of Engineering (PCCOE), Pune

---
