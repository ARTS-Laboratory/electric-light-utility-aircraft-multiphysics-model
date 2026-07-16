# v0.2.1
Cleaned and streamlined version of v0.2.0 prepared for publication, with unnecessary components removed and structure aligned with the 2026 journal paper: *“Battery Degradation and Replacement Cost Impacts on Profitability in Electric Light Utility Aircraft using a Multiphysics Modeling Approach.”*

## Running the Simscape Models

### Overview
This repository contains the Simscape-based electric light utility aircraft model and its supporting files.  
The model was created in MATLAB/Simulink 2025b and may not run correctly in earlier releases.

### Required Files
To run the model successfully, download the entire repository contents, including all folders and supporting files.  
Do not move or rename any files, since the model depends on the folder structure remaining intact.

The key files in this directory are:

- `model_parameters.m`
- `light_utility_aircraft_model.slx`
- Supporting model folders and libraries used by the Simscape implementation

### Setup Instructions
1. Open MATLAB R2025b.
2. Add the repository folder and all subfolders to the MATLAB path.
3. Make sure the current folder is set to the model directory.
4. Confirm that all required files and supporting folders are present before running the model.

### Running the Model
Follow the steps below in order:

1. Run `model_parameters.m` first.  
   This file initializes the model inputs, constants, and configuration values required by the Simscape model.

2. Open and run `light_utility_aircraft_model.slx`.  
   This is the main Simscape model used for simulation.

3. Allow the simulation to complete.  
   During execution, the model will generate outputs such as:
   - State of Charge (SOC)
   - State of Health (SOH)
   - Other model results and logged signals

### Output Files
When the simulation finishes, results are saved automatically to files in the model folder or the configured output directory.  
These files can be used for post-processing, plotting, or further analysis.

### Model Notes
Some blocks responsible for battery degradation, SOC, SOH, and related calculations are distributed throughout the Simscape model.  
These blocks are already configured in the model and can be enabled or adjusted when needed.

### Repeatability
For consistent results:

- Always run `model_parameters.m` before the Simscape model.
- Keep the repository structure unchanged.
- Use MATLAB/Simulink 2025b or a compatible version.
- Check that any required supporting folders are included when copying or downloading the model.
