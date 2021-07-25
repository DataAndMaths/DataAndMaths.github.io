---
layout: page
title: ACP
subtitle: (3)
---


# Comment représenter le nuage des individus $N_I$ plus simplement ? 

## Objectif général ? 

On voudrait obtenir une représentation approchée du nuage $N_I$, de petite dimension.

##  Comment trouver cette représentation approchée ? 

On va le faire axe par axe : on recherche un 1e axe qui va représenter au mieux le nuage de points, puis un 2e axe, puis un 3e, ...

### 1e axe

* <u>Notations</u>
  * $u_1$ : un vecteur unitaire, qui donne la direction de l'axe que l'on cherche (le 1 en indice rappelle qu'il s'agit du 1e axe)
  * $M_i$ : un point du nuage
  * $H^1_i$ : projeté de $M_i$ sur l'axe (l'exposant 1 est là pour rappeler qu'on projette sur le 1e axe) <br/><br/>

* <u>Critère</u>
  * On cherche la direction $u_1$ telle que la variance du nuage des points projetés $H^1_i$ soit maximale.
  * variance du nuage projeté : $$ \sum_i \frac{1}{I} (OH^1_i)^2$$    
  * Cette variance s'appelle aussi l'inertie du nuage projeté. <br/><br/>
  
* <u>Remarques</u>
  * Rappelons que les données sont centrées : l'origine O du repère est confondu avec le centre de gravité $G_I$ du nuage. 
  * On peut montrer que maximiser la variance revient à maximiser les distances entre les individus projetés : $$\sum_{i,j} d(H^1_i,H^1_j)^2$$. 

### 2e axe

* <u>Notations</u>
  * $u_2$ : un vecteur unitaire, qui donne la direction de l'axe que l'on cherche (le 2 en indice rappelle qu'il s'agit du 2e axe)
  * $M_i$ : un point du nuage
  * $H^2_i$ : projeté de $M_i$ sur l'axe (l'exposant 2 est là pour rappeler qu'on projette sur le 2e axe) <br/><br/>

* <u>Objectif</u>
  * On cherche la direction $u_2$ telle que :
    * la variance du nuage des points projetés $H^1_i$ soit maximale : $$ \sum_i \frac{1}{I} (OH^2_i)^2$$ maximale
    * $u_2$ soit orthogonale à $u_1$.

### 3e axe, ...

On procède de même pour les axes suivants.


## Comment obtenir ces axes ? 

On considère la matrice de corrélations C. 

{: .box-note} **Propriétés** <br/><br/>
P1 : $u_1$, $u_2$, ... sont les vecteurs propres de C associés aux valeurs propres $\lambda_1 \geq  \lambda_2 \geq$ ... (rangées dans l'ordre décroissant). <br/><br/>
P2 : La valeur propre $\lambda_i$ est égale à l'inertie projetée sur $u_i$.
