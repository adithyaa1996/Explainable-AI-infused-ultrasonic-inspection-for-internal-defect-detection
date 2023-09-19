# Explainable-AI-infused-ultrasonic-inspection-for-internal-defect-detection
This GitHub repository maintains data associated with our accepted paper in CIRP Annals titled "Explainable-AI infused ultrasonic inspection for internal defect detection". To briefly summarize,

**1. Polishing_stagewise_data.zip** - Contains height values measured at 32 different locations on the 3D printed sample using an optical profilometer prior to polishing (Stage 0) and post every stage of polishing (Stages 1 to 6). Please refer to the following paper for experimentation details and process parameters: "_Jin, S., A. Iquebal, S. Bukkapatnam, A. Gaynor, and Y. Ding (2019, 10). A gaussian process model-guided surface polishing process in additive manufacturing. Journal of Manufacturing Science and Engineering 142, 1–17._"

**2. Initial_surface_generation.m** - Script containing the Initial surface generation algorithm using the random circle packing algorithm. This file generates the surface asperity distribution and their graph connectivity of a 3D printed sample prior to polishing (Figure 4(b) in paper). One such realization is stored and compared with experimental data (Refer #3).

**3. Stage0_fitted_data.mat** - .mat file containing data pertaining to height measures of the 3D printed sample prior to polishing and generated initial surface (simulation) which is statistically similar to the actual data. 

**4. Parameter_fitting_Polishing.m** - Script containing the model capturing polishing dynamics with network formation, evaluated at each stage of polishing. This file generates the Bearing Area Curves of the initial surface simulated after each stage of polishing and compares with experimental data (Figures 3, 5, 6, 7 and 8 in paper). (The script makes use of other functions defined in #5).
