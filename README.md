This is for the project entitled [Score hospitals by the billing behavior](https://github.com/HannahhoHe/Medicare---Insight-into-the-Bills/blob/master/README_Intro.md). In this asset, I use data are from Kaggle CMS Medicare database, which covers the US nationwide Medicare bills from 3770 unique providers during the years of 2011-2015.
[See the codings](https://github.com/HannahhoHe/Medicare---Insight-into-the-Bills/blob/master/CROLChallenges_Section1.ipynb).

# 1st asset - Do some providers bill higher than others? 

This heatmap displays the charges (in US dollars) per outpatient service, listed with different providers (i.e., provider_id), and with different type of services (i.e., Ambulatory Payment Classification, apc, n=42, labeled as "None-apc"). This plot shows that the amounts of charges primarily depend on the type of services.  
![Figure1](OutPatientCharges.png)     


To evaluate if every provider charges equally compared to their peers, all the charges were normalized by the corresponding apc bills. The resulting plot shows that certain groups of providers tend to charge higher than others, irrespective of the types of apc services (i.e., see the providers with a persistent horizontal light-blue pattern).   
![Figure2](OutPatientChargesNorm.png)

For providers who tend to charge higher, do they file more claims for some specific apcs? In other words, are they tied to certain specialists? To analyze this, I classified the providers into "RegularCharge" vs. "HiCharge" from the above blue heatmap, with the providers in the latter having a value larger or equal to 15. This led to a total of 650 providers (17%) in the HiCharge class. As shown below, the resulting distribution of total bills indicates that the HiCharge providers provide a comparable variety of services to the RegularCharge providers, revealing that the providers from both classes have a similar distribution of types of hospitals.      

![Figure3](Providersbyapc.png)


Can differing standards (i.e. laws, cost of living) among US states account for the differences seen in this analysis? In this plot, I analyzed where (which state) the providers are located. The top five US states that have the highest numbers of HiCharge providers are CA, NY, MA, CT, and NJ. However, excluding MA and CT, three of these states also have a fair amount of RegularCharge providers, demonstrating that the pricier charge behavior is not due to differences in state's standards and yet occurs perferrentially in some of them.               

![Figure4](ProvidersbyState.png)

In conclusion, it is true that some providers tend to bill higher than others irrespective of the type of services. 
