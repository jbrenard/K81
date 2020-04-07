## Simulation of the impact of generalised use of masks in France

This simulation aims at providing a simplified and transparent model illustrating the impact of the generalised use of masks on epidemic control. It is not a substitute for detailed scientific studies such as the ones quoted in reference.

In France cumulated cases and Covid-19 related death grew at circa 30% per day before confinement, and at roughly half that pace after confinement was put in place, corresponding to a basic reproduction rate (Ro) circa 3.1 (assuming a 10-day contagious period) and a reproduction rate circa 1.4 after confinement [1].

  
<img src="https://github.com/fsteiner/K81/blob/master/Chart_Covid_France_en.png" width="600">  
  
Estimates of the efficiency of masks inwards (protecting the wearer) and to some extent outwards (protecting others and preventing surface contamination) are available [2][3][4], showing a level of protection circa 50% inwards for homemade masks, 63-80% for surgical masks and circa 95% for protective masks of type FFP2, for particles of relevant size (23 nm as tested compared to 60-10 nm for the virus).  
Data for outwards protection are more difficult to interpret - on a limited sample, practically full protection was observed for surgical masks in the case of conronavirus [4].  
In this document, we took the conservative hypothesis to align outwards protection to the lower value measured for inwards protection i.e. 50% for homemade masks and 63% for surgical masks.  

The risk of contracting the disease being proportional to exposure, even partial protection has a positive impact.  
Specifically, as inwards and outwards protection add up, the overall efficiency of the systematic use of masks stems from the double barrier: filtering inwards and outwards.  
For instance the risk for the wearer of a homemade mask to be contaminated by the wearer of a surgical mask would be:
> (1-63%) *outwards* x (1-50%) *inwards* = 18,5%  

hence an efficiency in this particular case :
> 1 - 18,5% = 81,5%  

Similarly, efficiency between homemade masks would be 75% and 86% between wearers of surgical masks.  

Assuming various level of equipment throughout the population and extending the above calculation to all possible combinations, we calculate an average efficiency over the whole population.

Applying protection rates above to the following hypotheses (without FFP2 masks, supposed to be allocated to medical staff only):  
- H1 (short term) 20% of population without a mask, 60% with a homemade mask, 20% with a surgical mask
- H2 10% without a mask, 20% with a homemade mask, 70% with a surgical mask

Resultant efficiencies E1 and E2 are respectively 67% and 74%.  
To calculate R, we apply the efficiency to  Ro:  
> R = (1-E) x Ro  

Resulting R are 1.0 for H1, 0.8 for H2.
If we had retained for surgical masks the top of the efficiency range (i.e. 80% instead of 63%), E1 and E2 would be respectively 71% and 82%, with R down to 0.9 for H1 and 0.6 for H2.  

The table below presents a sensitivy analysis of R according to various values of Ro and efficiency E.  
| E \\ Ro | 2.5 | 3.0 | 3.5 |
| :----   | -:  | -:  | -:  | 
| **65%** | 0.9 | 1.1 | 1.2 |
| **70%** | 0.8 | 0.9 | 1.1 |
| **75%** | 0.6 | 0.8 | 0.9 |
| **80%** | 0.5 | 0.6 | 0.7 |

The simplified calculation above, based on verified hypotheses aim at showing the **order of magnitude** of the impact of the generalised use of masks in slowing the spread of the disease.  
They show that systematic use of protective masks contributes to the first order to lowering the R factor below 1, that is stopping the epidemic.  

These results are consistent with a detailed paper [5] showing that a flu epidemic can be stopped if 80% of the population uses a protective mask.  

#### Références
[1] We used a simplistic model of epidemic propagation, the "S-curve":  
> x = 1/(1 + e<sup>-kt</sup>)  

Where x is the infected proportion of the population, t time in days and k a parameter m reprenting the pace of evolution. In the initial phase, growth is practically exponential:
> x ~ e<sup>kt</sup> = (1 + r)<sup>t</sup>  

With r the daily growth rate and the relationship between k and r: 
> r =  e<sup>k</sup> - 1  

r is the daily increase of infected individuals per existing contagious case, in a population without immunity, this rate being assumed constant in our simplified model. The rate of replication Ro in this basic model is simply the number r multiplied by the length of the infectious period P expressed in days:  
> Ro = r x P


[2]  Davies, Thompson, Giri, et al. Testing the Efficacy of Homemade Masks: Would They Protect in an Influenza Pandemic?  
Disaster medicine and public health preparedness 10.1017/dmp.2013.43  
https://www.cambridge.org/core/journals/disaster-medicine-and-public-health-preparedness/article/testing-the-efficacy-of-homemade-masks-would-they-protect-in-an-influenza-pandemic/0921A05A69A9419C862FA2F35F819D55

[3] Compilation of various studies either performed or collected by social enterprise Smart Air  https://smartairfilters.com/en/blog/coronavirus-pollution-masks-n95-surgical-mask/

[4] Leung, N.H.L., Chu, D.K.W., Shiu, E.Y.C. et al. Respiratory virus shedding in exhaled breath and efficacy of face masks. Nat Med (2020).  doi.org/10.1038/s41591-020-0843-2

[5] Yan J, Guha S, Hariharan P, Myers M. Modeling the Effectiveness of Respiratory Protective Devices in Reducing Influenza Outbreak. Risk Anal. 2019;39(3):647–661. doi:10.1111/risa.13181
