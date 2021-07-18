---
layout: page
title: ACP
subtitle: (1)
---


# Problème ? 

Lorsqu'on a des données de grande dimension (avec plus de 3 variables), il est plus difficile de les analyser et de les visualiser. 


# Notations 

Nous considérons des données avec I individus et K variables numériques. 

| |var 1|var 2|...|var k|...|var K|
|:----|:-----|:-----|:----|:----|:----|:----|
|ind 1|||||||
|ind 2|||||||
|...|||||||
|ind i||||$x_{ik}$|||
|...|||||||
|ind I|||||||

Pour chaque variable/colonne, on notera :
* la moyenne ${\bar x}_k$
* l'écart-type $s_k$.

<br/>

# Objectifs ?

## Etudier les individus

* On voudrait les étudier en considérant toutes les variables dans son ensemble, et non pas une par une. 
* Quelles sont les individus qui se ressemblent ? Quelles sont ceux qui diffèrent ? 
* Quelle est la tendance générale ? la structure générale ?  
* Y a-t-il des groupes homogènes d'individus ? 
* Quelle est la typologie des individus ?
* Quelles sont les principales dimensions de variabilité des individus ?

## Etudier les variables

* Quelles sont les variables corrélées positivement entre elles ? 
* Quelles sont les variables corrélées négativement entre elles ? 
* Existe-t-il des groupes de variables corrélées entre elles ?
* Quelle est la typologie des variables ?
* En ACP, on ne considère que les liaisons linéaires. 
* En grande dimension, avec beaucoup de variables, on voudrait en avoir moins : comment pourrait-on synthétiser ces variables ?  
  Ces variables synthétiques seront les fameuses composantes principales. <br/>
  
  
# Quelques points techniques

## Poids des données

Dans toute la suite, on attribuera :
* le même poids à chaque individu : $\frac{1}{I}
* le même poids à chaque variable : 1. <vr/>


## Préparation des données

{: .box-warning}
**Cadre** <br/>
Dans toute la suite, on considère les données **centrées-réduites**.

Cela signifie que pour chaque colonne :
* on soustrait la moyenne : $x_{ik} - {\bar x}_k$
* puis on divise par son écart-type : $\frac{x_{ik} - {\bar x}_k}{s_k}$. 
