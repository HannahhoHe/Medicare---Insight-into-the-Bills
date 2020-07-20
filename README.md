Data are from Kaggle CMS Medicare database, which covers the US nationwide Medicare bills from 3770 unique providers during the years of 2011-2015. 
# 1st asset - Factors for different charges
## By providers, and by types of services
This heatmap displays the charges (in US dollars) per outpatient service, listed with different providers (i.e., provider_id), and with different type of services (i.e., Ambulatory Payment Classification, apc, n=42, labeled as "None-apc"). This plot shows that the amount of charges primarily depends on the type of services.  

![Figure1](OutPatientCharges.png)     
To evalute if every provider charges equally, all the charges were normalized by the corresponding apc bills. The resulting plot shows that certain groups of providers tend to charge higher than others, irrespective types of apc services (i.e., see the providers with persistent horizontal light blues).   
![Figure2](OutPatientChargesNorm.png)

