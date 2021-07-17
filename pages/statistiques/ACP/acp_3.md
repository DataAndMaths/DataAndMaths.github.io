---
layout: page
title: ACP
subtitle: (3)
---


# Comment représenter le nuage des individus $N_I$ plus simplement ? 

## Objectif général ? 

On voudrait obtenir une représentation approchée du nuage $N_I$, de petite dimension.

## Contraintes ?

On voudrait conserver au mieux les distances entre les individus. 

##  Comment trouver cettre représentation approchée ? 

On va le faire axe par axe : on recherche un 1e axe qui va représenter au mieux le nuage de points, puis un 2e axe, puis un 3e, ...

### 1e axe

* <u>Notations</u>
  * $u_1$ : un vecteur unitaire, qui donne la direction de l'axe que l'on cherche
  * $M_i$ : un point du nuage
  * $H^1_i$ : projeté de $M_i$ sur l'axe (l'exposant 1 est là pour rappeler qu'on projette sur le 1e axe)

* <u>Objectif</u>
  * On cherche la direction $u_1$ telle que la variance du nuage des points projetés $H^1_i$ soit maximale.
  * variance : $$ \sum_i \frac{1}{I} (OH^1_i)^2$$    
