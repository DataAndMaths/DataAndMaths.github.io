---
layout: page
title: ACP
subtitle: (4) Comment représenter le nuage des variables $N_K$ plus simplement ? 
---

## Objectif général ? 

On voudrait obtenir une représentation approchée du nuage $N_K$, de petite dimension.

## Contraintes ?

On voudrait conserver au mieux les angles entre les vecteurs, autrement dit les corrélations entre les variables. 

##  Comment trouver cette représentation approchée ? 

On applique le même procédé que précédemment. 

* <u>Notations</u>
  * $v_s$ : un vecteur unitaire, qui donne la direction de l'axe de rang s
  * $M_k$ : un point du nuage
  * $H^s_i$ : projeté de $M_i$ sur l'axe de rang s (l'exposant s est là pour rappeler qu'on projette sur l'axe de rang s) <br/><br/>

* <u>Critères</u>
  * On cherche une suite de vecteurs $v_1, v_2, ...$ telle que 
    * chaque direction $v_s$ maximise la quantité $$\sum_k (OH^s_k)^2$$ 
    * chaque direction $v_s$ est orthogonale aux axes de rangs inférieurs.  
  * Remarque : on somme sur les variables k, on utilise donc les poids des variables qu'on a fixé à 1. <br/><br/> 
  
* <u>Interprétation</u>
  * Rappelons que l'origine O du repère n'est pas confondue avec le centre de gravité $G_I$ du nuage : la somme précédente ne représente plus une variance.  
  * $OH^s_k$ est égal au cosinus de l'angle entre le vecteur initial $\vec{OM_k}$ et $v_s$, c'est-à-dire le coefficient de corrélation entre la variable initiale et la nouvelle variable.   
  * La variable $v_s$ maximise la quantité $$\sum_k [corr(v_s,vark)]^2$$ : $v_s$ est la nouvelle variable qui est la plus corrélée à l'ensemble des K variables.  
    En ce sens, elle constitue une bonne variable synthétique.   
    
<br/> 

## Comment obtenir ces axes ? 

* On peut montrer que ces axes sont aussi les vecteurs propres d'une autre matrice. 
* Ces axes sont liés aux vecteurs propres $u_s$ de la matrice de corrélation (cf partie suivante). 
 
