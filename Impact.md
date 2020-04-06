## Simulation de l'impact des masques sur la propagation du Covid-19 en France

Cette simulation simple ne vise pas à se substituer à des études scientifiques détaillées, mais à donner un modèle simplifié et transparent qui illustre l'impact du port généralisé du masque sur le contrôle de l'épidémie.

En France, le taux de croissance des cas déclarés comme des décès liés au Covid-19 est de l'ordre de 30% avant confinement et environ moitié moindre après les mesures de confinement mises en oeuvre, ce qui correspond à un taux de reproduction de base (Ro) de l'ordre de 3,1 (sur la base de 10 jours de période de contagion) et un taux de reproduction (R) d'environ 1,4 après confinement.[1]  
  
<img src="https://github.com/fsteiner/K81/blob/master/Chart_Covid_France.png" width="600">  
  
Des estimations de l'efficacité des masques à l'inhalation (protection du porteur) et dans une moindre mesure à l'exhalation (protection d'autrui et non contamination de l'environnement) sont disponibles [2][3][4].  

Elles montrent des niveaux de protection à la réception d'environ d'environ 50% pour les masques artisanaux, 63-80% pour les masques chirurgicaux et de l'ordre de 95% pour les masques de protection type FFP2, pour des tailles de particules comparables (23 nm pour le test contre 60-100 nm pour le virus).
Les données disponibles de protection à l'émission sont moins directement exploitables - sur un échantillon limité, une efficacité quasi-totale a été mesurée pour les masques chirurgicaux dans le cas de coronavirus [4].  
Dans le présent document, nous avons pris l'hypothèse conservatrice d'aligner la performance à l'émission sur celle mesurée à la réception soit 50% pour les masques artisanaux et 63% pour les masques chirurgicaux.

Le risque de contracter la maladie étant proportionnel au degré d'exposition au virus, même une protection partielle réduit le risque. En particulier, les protections à l'émission et à la réception cumulant leurs effets positifs, l'efficacité du port généralisé du masque provient donc du double filtrage : réduction à l'émission, puis à la réception.  
Par exemple, le risque pour un porteur de masque artisanal d'être contaminé par un porteur de masque chirurgical seraient :
> (1-63%) *émission* x (1-50%) *réception* = 18,5%  

soit une efficacité de :
> 1 - 18,5% = 81,5%  

De la même manière, l'efficacité entre deux porteurs de masques artisanaux serait de 75%, et de 86% entre deux porteurs de masques chirurgicaux.

En faisant des hypothèses d'équipement de la population et en étendant ce calcul à tous les cas de figure on peut calculer une efficacité moyenne sur l'ensemble de la population.

Si on applique les taux de protection sélectionnés aux hypothèses suivantes (sans masques FFP2, supposés réservés au personnel médical) : 
- H1 (court terme) 20% de la population sans masque, 60% avec masque artisanal, 20% avec masque chirurgical
- H2 10% sans masque, 20% avec masque artisanal, 70% avec masque chirurgical

Les efficacités E1 et E2 résultantes seraient de respectivement 67% et 74%.
Pour calculer R, il suffit d'appliquer cette efficacité au coefficient Ro selon la formule suivante :
> R = (1-E) x Ro  

Les coefficients R en résultant seraient respectivement de 1,0 pour H1 et 0,8 pour H2.  
Si on retenait pour les masques chirurgicaux le haut de la fourchette d'efficacité (80% au lieu de 63%), E1 et E2 seraient respectivement de 71% et 82%, avec des coefficients R ramenés à 0,9 pour H1 et 0,6 pour H2.

Le tableau suivant montre une analyse de sensibilité pour R suivant diverses valeurs de Ro et d'efficacité E :  
| E \\ Ro | 2.5 | 3.0 | 3.5 |
| :----   | -:  | -:  | -:  | 
| **65%** | 0.9 | 1.1 | 1.2 |
| **70%** | 0.8 | 0.9 | 1.1 |
| **75%** | 0.6 | 0.8 | 0.9 |
| **80%** | 0.5 | 0.6 | 0.7 |

Ces calculs simples basés sur des hypothèses vérifiées ont pour seul objet de montrer l'effet du port généralisé de masques de protection sur le rythme de propagation de l'épidémie **en ordre de grandeur**.  
Ils permettent de conclure que le port généralisé du masque apporte une contribution du premier ordre à la lutte pour ramener le coefficient R au-dessous de 1 c'est-à-dire stopper la propagation de l'épidémie.

Ces résultats sont cohérents avec une étude scientifique détaillée [5] montrant qu'une épidémie de grippe peut être enrayée par le port de masques par 80% de la population.



#### Références
[1] On applique un modèle simpliste de propagation de l'épdémie suivant une courbe en S :  
> x = 1/(1 + e<sup>-kt</sup>)  

Où x est la proportion de la population contaminée, t le temps écoulé en jours et k un paramètre caractérisant la vitesse d'évolution.  
Dans la phase initiale de l'épidémie, la croissance est pratiquement exponentielle :
> x ~ e<sup>kt</sup> = (1 + r)<sup>t</sup>  

Où r est le taux de croissance journalier avec la relation :
> r =  e<sup>k</sup> - 1  

r correspond à l'accroissement journalier naturel du nombre de contaminations par personne infectée dans une population non immunisée, supposé constant dans ce modèle ultra-simplifié. Pour obtenir le Ro, toujours dans ce modèle basique il suffit de multiplier ce nombre par la durée de la période de contagion P exprimée en jours.
> Ro = r x P


[2]  Davies, Thompson, Giri, et al. Testing the Efficacy of Homemade Masks: Would They Protect in an Influenza Pandemic?  
Disaster medicine and public health preparedness 10.1017/dmp.2013.43  
https://www.cambridge.org/core/journals/disaster-medicine-and-public-health-preparedness/article/testing-the-efficacy-of-homemade-masks-would-they-protect-in-an-influenza-pandemic/0921A05A69A9419C862FA2F35F819D55

[3] Compilation de plusieurs études réalisées par l'entreprise sociale Smart Air  https://smartairfilters.com/en/blog/coronavirus-pollution-masks-n95-surgical-mask/

[4] Leung, N.H.L., Chu, D.K.W., Shiu, E.Y.C. et al. Respiratory virus shedding in exhaled breath and efficacy of face masks. Nat Med (2020).  doi.org/10.1038/s41591-020-0843-2

[5] Yan J, Guha S, Hariharan P, Myers M. Modeling the Effectiveness of Respiratory Protective Devices in Reducing Influenza Outbreak. Risk Anal. 2019;39(3):647–661. doi:10.1111/risa.13181
