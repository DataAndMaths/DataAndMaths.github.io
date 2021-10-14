---
layout: post
title: Application sur les données Agribalyse-synthèse
subtitle: Impacts environnementaux des produits agricoles et alimentaires en France
thumbnail-img: /assets/img/appli_agribalyse_img.png
gh-repo: DataAndMaths/agribalyse_data
gh-badge: [star, fork, follow]
tags: [environnement, alimentation]

comments: true
---

----------------------

🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜🚜    

🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎🍎  

🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐🥐 

🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚🚚 

🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴🍴  

---------------
<br/><br/>



## Bienvenue !

Voici une réutilisation des [données](https://datascience.etalab.studio/dgml/c763b24a-a0fe-4e77-9586-3d5453c631cd) d'Agribalyse :

[Lien vers l'application](https://share.streamlit.io/dataandmaths/agribalyse_data/main/main.py) (en construction 🏗️)   
[Lien Github](https://github.com/DataAndMaths/agribalyse_data)

{: .box-note}
**NB:**  Il y a une mise à jour très récente de Streamlit, il est possible que ce soit lent ou que ça bug, ... 😕

{: .box-warning}
**Warning:** Lors des sélections multiples, il est conseillé de faire une seule sélection, de laisser tourner, puis d'enclencher la sélection suivante, sinon la page peut bugger et revenir à zéro. 


------------------------------------
<br/>

## Cadre

### Qu'est-ce qu'Agribalyse ? 

[AGRIBALYSE](https://doc.agribalyse.fr/documentation/) est une base de données de référence des indicateurs d’impacts environnementaux des produits agricoles produits en France et des produits alimentaires consommés en France. 

### Que trouve-t-on dans ces données ?

Elles recensent des caractéristiques de plusieurs aliments ainsi que les émissions de polluants qui leur sont associés.

### Que pouvez-vous faire avec cette petite application ? 
Dans la version actuelle, elle vous permet :
* d'explorer les données à l'aide essentiellement de Plotly 🙂 (graphiques interactifs)
* de construire un tout premier modèle pour prédire le DQR en fonction de différents indicateurs.

### Qu'est-ce que le DQR

Une note de qualité - le **Data Quality Ratio (DQR)** - de 1, très bon, à 5, très mauvais - est associée à chaque produit agricole et alimentaire pour 
lequel Agribalyse fournit des inventaires de cycle de vie et des indicateurs d’impacts. La Commission Européenne recommande de la prudence dans l’utilisation des données avec des DQR supérieurs à 3. 
Dans la base de données AGRIBALYSE, 67 % des données ont un DQR jugé bon ou très bon (1 à 3).
              
   
 --------------------------  



