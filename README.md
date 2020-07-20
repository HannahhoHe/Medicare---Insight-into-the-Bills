Data are from Kaggle CMS Medicare database, which covers the US nationwide Medicare bills from 3770 unique providers during the years of 2011-2015. 
# 1st asset - Factors for different charges
## By providers, and by types of services
This heatmap displays the charges (in US dollars) per outpatient service, listed with different providers (i.e., provider_id), and with different type of services (i.e., Ambulatory Payment Classification, apc, n=42, labeled as "None-apc"). This plot shows that the amounts of charges primarily depend on the type of services.  
![Figure1](OutPatientCharges.png)     


To evaluate if every provider charges equally compared to the peers, all the charges were normalized by the corresponding apc bills. The resulting plot shows that certain groups of providers tend to charge higher than others, irrespective types of apc services (i.e., see the providers with a persistent horizontal light-blue pattern).   
![Figure2](OutPatientChargesNorm.png)

For these providers who tend to charge higher, do they file the claims more on some specific apc? In other words, are they more specialists providers? To analyze this, I classified the providers into "RegularCharge" vs. "HiCharge" from the above blue heatmap, with the providers in the latter catogy having a value larger or equal to 15. This led to a total of 650 providers (17%) in the HiCharge class. 



In the following plot, the bar graph gives a visualization of distribution of bills across different apc services, colored by classes of providers.   



![Figure3](Providersbyapc.png)

