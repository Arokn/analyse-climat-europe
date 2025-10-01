# analyse-climat-europe
Analyse des profils climatiques en Europe à partir de données météorologiques via un **Jupyter Notebook**.

## Analyse des Climats Européens par Composantes Principales (ACP)
Ce projet analyse les profils climatiques des capitales européennes à partir de leurs températures mensuelles, en utilisant une approche statistique basée sur l'Analyse en Composantes Principales (ACP).

## Objectifs

Ce projet vise à analyser les profils climatiques des capitales européennes à partir de leurs températures mensuelles.  
Plus précisément, il s'agit de :  

- Identifier les principaux facteurs qui expliquent la variabilité climatique entre les capitales.  
- Construire une typologie des villes en fonction de leurs profils de température.  
- Visualiser les similarités et différences entre les climats européens.  
- Explorer les relations entre les températures des différents mois de l'année.

## Approche Mathématique

L'analyse repose sur l'**Analyse en Composantes Principales (ACP)**, une méthode statistique qui permet de réduire la dimensionnalité des données tout en conservant l'information la plus importante.  

Dans ce projet, l'ACP est utilisée pour :  
- Réduire les 12 variables mensuelles de température à 2 composantes principales, afin de visualiser facilement les similarités et différences entre les capitales.  
- Identifier les variables les plus influentes dans la variabilité climatique observée.  
- Explorer la structure globale des données et mettre en évidence des tendances ou regroupements de villes.  

**Particularité technique :**  
- L'ACP est implémentée **manuellement**, sans utiliser de bibliothèque prête à l'emploi comme `scikit-learn`.  
- Les étapes principales incluent :  
  - Centrage et réduction des données pour une analyse robuste.  
  - Calcul de la **matrice de corrélation**.  
  - Calcul des **valeurs propres et vecteurs propres** via `numpy.linalg.eig`.

## Données Utilisées

Le projet utilise un jeu de données regroupant les températures mensuelles des capitales européennes, ainsi que des informations complémentaires sur chaque ville.  

Les données incluent :  
- Températures de janvier à décembre  
- Température moyenne annuelle, latitude, longitude  

Ces données permettent d'étudier la variabilité climatique entre les villes, de construire des typologies et de visualiser les similarités et différences entre les profils climatiques européens.

## Technologies Utilisées

Ce projet a été réalisé en **Python**, en utilisant les bibliothèques suivantes :  

- **NumPy** : pour les calculs matriciels et l’algèbre linéaire (valeurs propres, vecteurs propres).  
- **Pandas** : pour la manipulation et le prétraitement des données.  
- **Matplotlib** : pour la visualisation des résultats   


## Conclusion

Cette analyse ACP a permis de révéler la structure des climats européens, mettant en évidence deux dimensions principales expliquant la majorité de la variation globale des températures.  
L'approche manuelle de l'ACP a renforcé la compréhension des mécanismes mathématiques de cette méthode multidimensionnelle et offre une bonne base pour explorer la diversité climatique en Europe.
