# Factors for different charges
The data from Kaggle cms-medicare database covers the US nationwide medicare bills from 3770 unique providers in the years of 2011-2015. 

## Providers and Services
Heatmaps display the charges per outpatient service by different providers (i.e., provider_id) and by type of service (i.e., Ambulatory Payment Classification, apc, n=42, labeled as "None-apc").      
![Figure1](OutPatientCharges.png)     
With all the charges normalized by the corresponding apc services, it is apparent that groups of providers tends to charge higher than others, irrespective of apc services.
![Figure2](OutPatientChargesNorm.png)

