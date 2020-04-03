## Simulation de l'impact des masques sur la propagation du Covid-19 en France

Cette simulation simple ne vise pas à se substituer à des études scientifiques détaillées, mais à donner un modèle simplifié et transparent qui illustre l'impact du port généralisé du masque sur le contrôle de l'épidémie.

En France, le taux de croissance des cas déclarés comme des décès liés au Covid-19 est de l'ordre de 27% avant confinement et 13% après les mesures de confinement mises en oeuvre, ce qui correspond à un taux de reproduction de base (Ro) de l'ordre de 4,4 (sur la base de 14 jours de période de contagion) et un taux de reproduction (R) d'environ 2,0 après confinement.  
  
<img src="https://github.com/fsteiner/K81/blob/master/Chart%20France.png" width="600">  
  
Des estimations de l'efficacité des masques à l'inhalation (protection du porteur) et dans une moindre mesure à l'exhalation (protection d'autrui et non contamination de l'environnement) sont disponibles [1][2].  

Elles montrent des niveaux de protection à la réception d'environ d'environ 50% pour les masques artisanaux, 63-80% pour les masques chirurgicaux et de l'ordre de 95% pour les masques de protection type FFP2, pour des tailles de particules comparables (23 nm pour le test contre 60-100 nm pour le virus).
Les données disponibles de protection à l'émission sont moins exploitables mais en considérant que la protection à l'émission est au moins aussi élevée qu'à la réception, nous avons pris l'hypothèse conservatrice de 50% pour les masques artisanaux et 63% pour les masques chirurgicaux à l'émission comme à la réception.

Le risque de contracter la maladie étant proportionnel au degré d'exposition au virus, même une protection partielle réduit le risque. En particulier, les protections à l'émission et à la réception cumulant leurs effets positifs, l'efficacité du port généralisé du masque provient donc du double filtrage : réduction à l'émission, puis à la réception.  
Par exemple, le risque pour un porteur de masque artisanal d'être contaminé par un porteur de masque chirurgical seraient :
> (1-63%) *émission* x (1-50%) *réception* = 18.5%

Si on applique les taux de protection sélectionnés à deux hypothèses d'équipement de la population (sans masques FFP2, supposés réservés au personnel médical) : 
- H1 (court terme) 20% de la population sans masque, 60% avec masque artisanal, 20% avec masque chirurgical
- H2 10% sans masque, 30% avec masque artisanal, 60% avec masque chirurgical

Les coefficients R en résultant sont respectivement de **1.3 pour H1 et 1.1 pour H2**

Ces calculs simples basés sur des hypotèses vérifiées montre l'effet significatif du port généralisé de masques de protection sur le rythme de propagation de l'épidémie.
Associé à d'autres mesures (tests, confinement sélectif) son application permettrait de ramener le coefficient R au-dessous de 1 et donc de stopper la propagation de l'épidémie.



#### Références
[1]  Testing the Efficacy of Homemade Masks: Would They Protect in an Influenza Pandemic?  
Davies, Thompson, Giri, et al. Disaster medicine and public health preparedness 10.1017/dmp.2013.43  
https://www.cambridge.org/core/journals/disaster-medicine-and-public-health-preparedness/article/testing-the-efficacy-of-homemade-masks-would-they-protect-in-an-influenza-pandemic/0921A05A69A9419C862FA2F35F819D55

[2] Compilation de plusieurs études réalisées par l'entreprise sociale Smart Air  https://smartairfilters.com/en/blog/coronavirus-pollution-masks-n95-surgical-mask/
