[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10912850.svg)](https://doi.org/10.5281/zenodo.10912850)
# PhD Project Data Repository
## "Axisymmetric Saturated Granular Column Collapses at Elevated Gravitational Accelerations" by William Webb

### Overview
Welcome to the online repository for William Webb's PhD project. This repository contains all the video data generated and used throughout the duration of the project. Below is an outline of the data included and how it's organized.

### Testcode Description
The test-specific files within this repository follow a standard naming convention. An example of how these files are titled is `20210914_08g_010w_050_050_005_1.extension`.
This naming convention can be decoded as Date_Grainprop_Fluidprop_Grainheight_Fluidheight_N_Cam where each term separated by an underscore is defined below:

- **Date**: The date on which the test was undertaken (YYYYMMDD format).
- **Grainprop**: Diameter (mm) and material of the inertial granular phase (e.g., glass (g) beads).
- **Fluidprop**: The viscosity of the fluid with respect to water (i.e. 010 refers to water while 050 refers to a solution 5 times more viscous than water) followed by the type of fluid. w stands for water, g refers to a glycerol-water mixture, and k refers to the tests conducted with a kaolin suspension. For the case of the kaolin suspension tests where the fluid's behavior is non-Newtonian, the number prior to the 'k' refers to the concentration of kaolin fines by mass relative to water (i.e. 020 refers to a kaolin mass concentration of 20%).
- **Grainheight**: Height of the granular phase (mm).
- **Fluidheight**: Height of the fluid phase (mm).
- **N**: Gravitational scale factor.
- **Cam**: Camera position (1 for upstream flow side, 2 for downstream flow side).

### Data Description
1. **Raw Video Files (`{Testcode}.MP4`):**
   - **Description:** Raw video files of the column collapse tests taken from two different positions using GoPro cameras at a frame rate of 240 fps. Filenames follow the naming convention outlined above.

2. **Runout Output Files (`{Testcode}.txt`):**
   - **Description:** Output files containing fluid and particle phase runout and velocity data extracted from image analysis of the raw videos. Data is presented with the following column headings:
     - Frame: Frame number after column release. Multiplying this value by the frame timestep (i.e. 1/frame rate) will provide the time after collapse initiation for each row of data.
     - r_f (m) (Cam 1): Average instantaneous runout distance of fluid phase front (Cam 1).
     - v_f (m/s) (Cam 1): Average instantaneous velocity of fluid phase front (Cam 1).
     - r_p (m) (Cam 1): Average instantaneous runout distance of particle phase front (Cam 1).
     - v_p (m/s) (Cam 1): Average instantaneous velocity of particle phase front (Cam 1).
     - r_f (m) (Cam 2): Average instantaneous runout distance of fluid phase front (Cam 2).
     - v_f (m/s) (Cam 2): Average instantaneous velocity of fluid phase front (Cam 2).
     - r_p (m) (Cam 2): Average instantaneous runout distance of particle phase front (Cam 2).
     - v_p (m/s) (Cam 2): Average instantaneous velocity of particle phase front (Cam 2).

3. **Pre-collapse Experimental Parameters (`Experimental_Conditions.txt`):**
   - **Description:** File containing pre-collapse experimental parameters for the tests in this repository. Each test includes the following parameters:
     - TestCode
     - N: Gravitational scale factor
     - rpm: Revolutions per minute of the geotechnical centrifuge
     - G: Imposed gravitational acceleration (m/s^2)
     - r_0: Initial column radius (m)
     - H_p0: Initial height of the particle phase (m)
     - H_f0: Initial height of the fluid phase (m)
     - d_p: Inertial particle diameter (m)
     - rho_p: Inertial particle density (kg/m^3)
     - phi_p: Average column solid volume fraction prior to collapse
     - IF: Interstitial test fluid: w for water, g for glycerol-water mixture, k for kaolin suspension
     - C_m: Mass concentration of the additive to the fluid phase (i.e. glycerol or kaolin) relative to water.
     - C_v: Volume concentration of the additive to the fluid phase (i.e. glycerol or kaolin) relative to water.
     - rho_f: Fluid phase density (kg/m^3).
     - mu_f: Fluid mixture viscosity (kg/m/s). For the non-Newtonian tests (i.e. IF=k), this is a representative viscosity value based on the characteristic shear rate of the collapse (see Thesis Appendix A.3.2).
     - sigma_f: Fluid surface tension (N/m)

### Data Citation
If you use any data from this repository in your research or publications, please cite the corresponding sources appropriately.

### Contact
For any inquiries or assistance regarding the data, please contact William Webb at williamoscarwebb@gmail.com.
