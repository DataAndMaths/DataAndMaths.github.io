---
layout: page
title: Modèle ARIMA
subtitle: 
---

---
<br/>

# Overview
|Modèle ARIMA||
|:-----------------|:------------------------------------------------------------------------------------------|
|Idée              |capturer l'autocorrélation dans une série temporelle                                        |
|Utilisation       |pour la prévision                                                                                  |
|Concepts-clés     |l'ordre et la différenciation                                                              |
|Etapes            |1) differencier <br/> 2) entraîner un modèle ARMA sur la séries différenciées              |
|Notation du modèle|ARIMA(p,d,q)                                                                               |
|Hypothèse         |stationnarité de la série                                                                   |

<br/><br/>

# <u>Précisions</u>

ARIMA = AutoRegressive Integrated Moving Average

## <u>Etape 1 : Différenciation</u>
* Permet d'éliminer au préalable la tendance et/ou la saisonnalité
* On utilise la différenciation d'ordre 1 : $y_t' = y_t - y_{t-1}$
* L'ordre d est le nombre de fois où l'on applique cette différenciation d'ordre 1
    * d=0 : aucune différenciation
    * d=1 : différencier une fois
    * d=2 : différencier deux fois
    * Un ordre 1 ou 2 est généralement suffisant pour obtenir la stationnarité.
* Cette étape donne le I dans ARIMA. 
<br/><br/>

## <u>Etape 2 : Modèle ARMA(p,q)</u>

* Equation du modèle ARMA(p,q) : 
$$Y_t = \beta_0 + \beta_1 Y_{t-1} + \dots + \beta_p Y_{t-p} + \epsilon_t + \theta_1 \epsilon_{t-1} + \dots + \theta_q \epsilon_{t-q}$$ 
    * partie AR(p) : $\beta_0 + \beta_1 Y_{t-1} + \dots + \beta_p Y_{t-p}$ 
    * partie MA(q) : $\theta_1 \epsilon_{t-1} + \dots + \theta_q \epsilon_{t-q}$ <br/><br/>
    
* Modèle qui capture différents types d'autocorrélations 
    * avec les p valeurs précédentes de la série $Y_{t-1}, \dots, Y_{t-p}$ 
    * avec les q erreurs de prédiction précédentes $\epsilon_{t-1}, \dots, \epsilon_{t-q}$. 

