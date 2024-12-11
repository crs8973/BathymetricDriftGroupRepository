# Low-Cost, Open-Source Bathymetric Mapping Using a Drift Sensor
## Authors: Autumn, Grant, Teryn, and Camille

This GitHub repository provides updated designs for a low-cost, open-source, bathymetric drift sensor. The initial design is hosted in this repository: https://github.com/SUPScientist/smart-coasts-bathy-mapping

We aim to further develop and validate a low-cost bathymetric drift sensor to collect reliable and reproducible depth data in shallow and difficult-to-reach waterways, along with reducing extraneous noise in the data. We attempt to address the need for more accessible bathymetric mapping tools, particularly for public and small-scale research initiatives while reducing costs associated with traditional methods. 

Read the following for a high-level overview of the project and the contents of this repository.

## Introduction to the Bathymetric Sensor
![image](https://github.com/user-attachments/assets/5ab6d655-c179-49a8-b615-65a67e73bd60)
![image](https://github.com/user-attachments/assets/49afb274-79f5-4955-b173-9ab1973f7ebe)
![image](https://github.com/user-attachments/assets/94a8cc9f-7e87-456d-9d26-0d1454200074)

While traditional seafloor mapping technology has many useful applications, this technology is traditionally limited to scientists who have enough time, resources, and money to carry out mapping expeditions, meaning it is difficult to encourage public involvement in this field (Wölfl et al., 2019). Another limitation is the need for a boat and qualified personnel to transport and run the mapping instruments (Dierssen & Theberge, 2014). In areas inaccessible by boat, it is difficult to collect reliable bathymetric data through this methodology (Dierssen & Theberge, 2014; Wölfl et al., 2019). 

A possible solution to these limitations is the use of bathymetric drift sensors (Cocker et al., 2022). Low-cost bathymetric drift sensors have several benefits, including accessibility for public research and increased public involvement, the ability to map in shallow water, lower cost and time investments, and environmental benefits such as minimizing disturbances to fragile ecosystems. 

## Sensor Components and Specifications
For the advancement of the bathymetric drifter, there were several tools utilized. This included hardware such as a Particle Boron, an Adafruit adalogger, a JSN-SR04T ultrasonic depth sensor, an Adafruit Featherwing GPS, and an Adafruit MCP9808 temperature sensor. This also includes software such as VS code, Particle Workbench, Jupyter Notebook, and Python. The drifter functioned by using the integrated hardware components to collect bathymetric data. It relied on the Particle Boron microcontroller to process firmware written in VS code and connect to the other devices, the featherwing GPS to provide geolocation via satellite, the ultrasonic depth sensor for bathymetric measurements, the temperature sensor to adjust the speed of sound through water, and the adalogger to record the measured data. The collected data was stored on an SD card in the form of a time labeled comma separated value file (.csv). Analysis using Python was needed to georeferenced the data, as well as remove excess noise and other erroneous points. 

The structure of the drifter is a balance between stability and functionality. It consists of a large, central PVC pipe which houses the electronics and power supply. The transducer/receiver of the JSN-SR04T ultrasonic depth sensor extends through the bottom of the central housing to collect data. Other electronic equipment is stored in the top of the pipe near the end cap. When deployed, the end cap is threaded with Teflon tape to ensure a watertight seal. The square frame surrounding the central housing consists of pool noodles and smaller PCV pipes. This keeps the drifter positively buoyant in the water column and provides a large surface area to maintain stability in oncoming wake. Four 3D printed wings are also mounted to the sides of the central PVC pipe. These help the drifter maintain rotation stability.  

## How Does the Sensor Work?
The JSN-SR04T bathymetric sensor is at the bottom of the central drifter PVC pipe. The sensor releases ultrasonic waves to measure the distance to objects below it (Figure below). When combined with a drifter, the sensor can measure bathymetry along a specific stretch of river/ocean as it travels with the currents. Ultrasonic waves emitted from the sensor move through the water column, bounce off the seafloor/river bottom, and then travel back up through the water column to the sensor. 


## Repository Contents
Three main folders contain the material for this project: Data Analysis, Firmware, and Wiring.

#### Data Analysis: Tools & scripts for processing bathymetric data. 

#### Firmware: For operating the sensor, ensuring efficient & reliable performance. 

#### Wiring: Schematics & digrams to guide the assembly of the hardware components. 

## Sources

Cocker, E., Bert, J. A., Torres, F., Shreve, M., Kalb, J., Lee, J., Poimboeuf, M., Fautley, P., Adams, S., Lee, J., Lu, J., Chua, C., Chang, N., Neltner, S., & Gray, M. (2022). Low-Cost, Intelligent Drifter Fleet for Large-Scale, Distributed Ocean Observation. OCEANS 2022, Hampton Roads, 1–8. https://doi.org/10.1109/OCEANS47191.2022.9977209

Dierssen, H. & Theberge, A. (2014). Bathymetry: History of Seafloor Mapping. DOI: 10.1081/E-ENRW-120047531.

Pickens, B.A . (2021). Assessment of Frying Pan Shoals as a potential sand source in the Cape Fear Region of North Carolina. Sterling (VA): US Department of the Interior, Bureau of Ocean Energy Management. OCS Study BOEM 2021-028. https://espis.boem.gov/final%20reports/BOEM_2021-028.pdf

Wölfl, A.-C., Snaith, H., Amirebrahimi, S., Devey, C. W., Dorschel, B., Ferrini, V., Huvenne, V. A. I., Jakobsson, M., Jencks, J., Johnston, G., Lamarche, G., Mayer, L., Millar, D., Pedersen, T. H., Picard, K., Reitz, A., Schmitt, T., Visbeck, M., Weatherall, P., & Wigley, R. (2019). Seafloor Mapping-The Challenge of a Truly Global Ocean Bathymetry. Frontiers in Marine Science, 6, 283. https://doi.org/10.3389/fmars.2019.00283


Include a well organized readme in the repo's highest level folder such that when someone navigates to the repo, they immediately see a nicely rendered readme file. 

The readme should describe what content the repo intends to provide, what problems it aims to solve, and what material can be found within (and where). 
