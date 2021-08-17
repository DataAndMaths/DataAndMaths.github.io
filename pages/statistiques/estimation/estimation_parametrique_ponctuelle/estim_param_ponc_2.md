---
layout: page
title: Estimation Paramétrique Ponctuelle
subtitle: (2) Qualité d'un estimateur
---

# Qu'est-ce qu'un Estimateur ? 

Une estimateur $T_n$ d'un paramètre inconnu $\theta$ est une expression qui ne fait intervenir 
* que les données de l'échantillon $X_1, ..., X_n$
* la taille de l'échantillon n
* et éventuellement des constantes fixés.

$$T_n = h(X_1,...,X_n)$$ pour un certaine fonction h. 

# Qu'est'ce qu'un bon estimateur ? 

Nous considérons ici les deux critères suivants. 

{: .box-note} Définition 1 

Un estimateur $T_n$ est dit **sans biais** si $E(T_n) = \theta$; autrement dit, s'il ne sous-estime ni ne sur-estime le paramètre $\theta$ en moyenne. 


{: .box-note} Définition 2

Un estimateur $T_n$ est dit **convergent** si : $(T_n) converge (en un certain sens) vers $\theta$ lorsque la taille de l'échantillon n tend vers l'infini.  

