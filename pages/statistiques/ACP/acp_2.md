---
layout: page
title: ACP
subtitle: (2)
---


# Aspect géométrique

Nous avons deux nuages de points. 

## Nuage des individus $N_I$

### L'espace ambiant
* Chaque individu est décrit par K variables : ce nuage se trouve donc dans l'espace $R^K$.
* NB : il y a I individus, ce qui explique l'indice I dans $N_I$. <br/>

### Point particulier : le centre de gravité $G_I$

* Les données étant centrées, le centre de gravité du nuage est confondu avec l'origine O des axes. 
* On peut voir $G_I$ comme étant l'individu moyen. <br/>

### Distance entre les points

* La ressemblance des individus va se traduire par des points proches en terme de distance.
* L'ensemble des distances entre les points constitue la 'forme du nuage'. 
* Etudier la forme du nuage revient à déceler :
  * une partition de ces points : des groupes homogènes ;  une typologie des individus   
  * des directions d'allongement remarquables : les dimensions principales de variabilité. <br/>

### Problème en grande dimension
Dès que le nombre de variable est > 3, il est impossible d'étudier directement ce nuage.   
Il est alors nécessaire d'avoir une représentation plane de ce nuage, une qui approche au mieux le nuage initial. <br/><br/>


## Nuage des variables $N_K$

### L'espace ambiant
* Chaque variable décrit I individus : ce nuage se trouve donc dans l'espace $R^I$.
* NB : il y a K variables, ce qui explique l'indice K dans $N_K$.
* Plutôt que de considérer des points $M_k$, on considère plutôt des vecteurs $\vec{OM_k}$. <br/>

### Centrage et centre de gravité : Attention à l'interprétation
Contrairement au cas précédent, le nuage $N_K$ n'est pas centrée en $G_I$. <br/>

### Propriétés du nuage $N_K$

{: .box-note} 
**Propriétés** <br/>
P1 : Le cosinus de l'angle entre deux variables $V_k$ et $V_l$ est égal au coefficient de corrélation de $V_k$ et $V_l$ :
$$cos(V_k,V_l) = corr(V_k,V_l)$$.  <br/>
P2 : Tous les vecteurs sont de longueur 1.  
Les extrêmités des vecteurs sont donc tous situés sur la sphère de rayon 1.
