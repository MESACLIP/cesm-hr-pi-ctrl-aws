# cesm-hr-pi-ctrl-aws
Documentation and usage examples of Community Earth System Model (CESM) high-resolution (HR) Pre-Industrial Control (PI-CTRL) climate simulation data on Amazon AWS S3.

# Summary
This dataset provides several global fields describing the state of atmosphere, ocean, land and ice from a high-resolution (~0.1o) for the ocean/ice models 0.25o for the land/atmosphere models) numerical earth system model, the Community Earth System Model (CESM, https://www.cesm.ucar.edu/). Texas A&M University (TAMU) and National Center for Atmospheric Research together with international partners collaboratively carried out a large set of high-resolution climate simulations, including a 500-year long preindustrial control simulation (PI-CTRL) described here. The CESM uses dynamic equations with a climatological (observations, long-term averaged) initial state of the earth system and the preindustrial greenhouse gas forcing (kept constant at the 1850 conditions) for making this PI-CTRL. Compared to standard low-resolution (~1o) CMIP-class simulations, this high-resolution simulation dataset enables researchers to explore the contribution from processes at a wide range of spatial scales, from mesoscales to global scales, in shaping various observed climate phenomena with better accuracy. 

# CESM-HR Climate Simulations
CESM-HR simulations are designed to address the pressing need for improved understanding and prediction of the impact of climate change on extreme events like tropical cyclones, heat waves, droughts, floods and coastal sea level rise. Since CESM-HR can permit synoptic and mesoscale phenomena like tropical cyclones and ocean mesoscale eddies and, in turn, their interactions with the large-scale circulation, it offers a more advanced framework to study and predict potential changes in the future extreme events (Chang et al., 2020) compared to the existing low-resolution CMIP-class climate simulations. A detailed description of CESM-HR configuration and simulations can be found in Chang et al. (2020) and a brief summary is provided here. Validation of CESM-HR simulations focusing on various climate and weather processes is available from other publications listed in the Reference and Online Resources Section.

CESM (https://www.cesm.ucar.edu/) version 1.3 developed at NCAR with the support from the broader climate modeling community is used to carry out the simulations The component models of CESM-HR are the Community Atmosphere Model version 5 (CAM5), the Parallel Ocean Program version 2 (POP2), the Community Ice Code version 4 (CICE4), and the Community Land Model version 4 (CLM4). The horizontal resolution of ocean and ice models is ~0.1o and 0.25o for the land/atmosphere models. There are 30 vertical levels in the CAM5 and 62 in the POP2. PI-CTRL is carried out following the Coupled Model Intercomparison Project phase 5 (CMIP5) protocol (Eyring et al., 2016). The PI-CTRL ocean component was initialized using the World Ocean Atlas (WOA, Locarnini et al., 2013) climatological potential temperature and salinity for January from a state of rest. Existing restart files from other simulations were used for initializing other component models. The PI-CTRL simulation was run for 500 years, with a constant climate forcing set to the value in 1850. 	 	 	 		

Ongoing projects supporting CESM-HR historical and future transient climate simulations (HF-TNST) and high-resolution decadal prediction simulations (HRDP) include: 1) Understanding the Role of MESoscale Atmosphere-Ocean Interactions in Seasonal-to-Decadal CLImate Prediction (MESACLIP, https://project.cgd.ucar.edu/projects/MESACLIP/index.html), a project supported by National Science Foundation (NSF) to study the climate variability and predictability in the seasonal-to-decadal time scale, and 2) Improving Prediction and Projection of Gulf of Mexico Sea-Level Changes Using Eddy-Resolving Earth System Models (iPOGS, https://project.cgd.ucar.edu/projects/iPOGS/), a project funded by National Academy of Science (NAS) to study the mechanisms behind dynamical sea level rise and to make projections of sea level rise into 2100 under various emission scenarios. CESM (https://www.cesm.ucar.edu/) is one of the most popular climate models and is routinely used for performing simulations supporting Coupled Model Intercomparison Project (CMIP), which in turn is used in the Intergovernmental Panel for Climate Change (IPCC) reports. 

The PI-CTRL and HF-TNST simulations are released to the public in May/2022 through the Texas A&M datahub portal (https://ihesp.github.io/archive/products/ihesp-products/data-release/DataRelease_Phase2.html)
As a part of the AWS Public Datasets Program, the PI-CTRL data for years 0021-0500 is provided here. Depending on the availability of resources, attempts will be made to share more simulations from the CESM-HR suite on the AWS platform in the future.

Table.1: CESM-HR PI-CTRL component models (atmosphere (atm), ice, land (lnd), ocean (ocn) and runoff (rof)), list of available variables and data size. 

| Sl. No. | Comp. Model or Group | No. of Vars. | List of Variables | Total  Size |
| :---:   | :------------: | :------: | :----------------- | :-----: |
| 1       | atm  | 139   | https://ihesp.github.io/archive/products/ihesp-products/data-release/PI_control/atm/index.html  | 16.2 TB |
| 2       | ice  | 117   | https://ihesp.github.io/archive/products/ihesp-products/data-release/PI_control/ice/index.html  |  4.6 TB |
| 3       | lnd  | 152   | https://ihesp.github.io/archive/products/ihesp-products/data-release/PI_control/lnd/index.html  |  1.0 TB |
| 4       | ocn  | 48    | https://ihesp.github.io/archive/products/ihesp-products/data-release/PI_control/ocn/index.html  |   64 TB |
| 5       | rof  |  6    | https://ihesp.github.io/archive/products/ihesp-products/data-release/PI_control/rof/index.html  |    5 GB |

# Data Access Via AWS S3

This part will be completed after gaining access to AWS and obtaining technical help from AWS. 

# Tutorials

This set of CESM simulations have similar data structure and output variables as that of another CESM data product in the AWS Open Data program from NCAR, Community Earth System Model v2 Large Ensemble (CESM2 LENS) (https://aws.amazon.com/marketplace/pp/prodview-xilranwbl2ep2#overview). The tools and usage examples for CESM2 LENS (https://aws.amazon.com/marketplace/pp/prodview-xilranwbl2ep2#usage) should be usable for the current CESM-HR PI-CTRL dataset too, with a few necessary changes.

Once the AWS account for CESM-HR dataset has been approved and datasets are successfully transferred to AWS, it is possible to test a few Matlab based scripts using CESM-HR PI-CTRL data on the AWS and update the Tutorial related to this data product.

# License

This dataset is created in collaboration with NCAR and the NCAR’s “Creative Commons Attribution 4.0 International license” used for their CESM2 LENS data product on AWS (https://www.ucar.edu/terms-of-use/data) will be applicable for the CESM-HR datasets here. 

# Suggested Attribution

Community Earth System Model High-Resolution Pre-Industrial Control (CESM-HR) was accessed on DATE from LINK TO Registry.Opendata.AWS_link_when_it_is_availabe.

# Update Frequency

Rare. The CESM-HR PI-CTRL experiment is complete. Updates are expected only if any issues with the copy of the data on the AWS is reported in the future. Other experiments will be shared in the future according to the availability of resources.

# Reference and Online Resources

Chang et al. (2020): An Unprecedented Set of High‐Resolution Earth System Simulations for Understanding Multiscale Interactions in Climate Variability and Change. https://doi.org/10.1029/2020MS002298 

Chang et al. (2023): Uncertain future of sustainable fisheries environment in eastern boundary upwelling zones under climate change. https://doi.org/10.1038/s43247-023-00681-0

Eyring et al. (206): Overview of the Coupled Model Intercomparison Project Phase 6 (CMIP6) experimental design and organization. https://doi.org/10.5194/gmd‐9‐1937‐2016 
				
Locarnini et al. (2013). World Ocean Atlas 2013. Volume 1, Temperature, NOAA Atlas NESDIS 73 (p. 40). http://doi.org/10.7289/V55X26VD

Xu et al. (2024). High-resolution modelling identifies the Bering Strait’s role in amplified Arctic warming. https://doi.org/10.1038/s41558-024-02008-z

CESM Model: https://www.cesm.ucar.edu/

Texas A&M Datahub Portal: https://ihesp.github.io/archive/products/ihesp-products/data-release/DataRelease_Phase2.html

NetCDF Data Format: https://www.unidata.ucar.edu/software/netcdf/
	
MESACLIP: 	https://project.cgd.ucar.edu/projects/MESACLIP/index.html

iPOGS: https://project.cgd.ucar.edu/projects/iPOGS/
