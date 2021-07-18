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
  Ces variables synthétiques seront les fameuses composantes principales. 
