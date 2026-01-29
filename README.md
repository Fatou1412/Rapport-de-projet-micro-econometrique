# Capital Humain, Croissance et Emploi en France (2013-2020)

Ce projet propose une analyse économétrique de l'impact du capital humain (niveau de diplôme) et de la croissance économique (PIB par habitant) sur le taux de chômage des régions françaises. L'étude repose sur des **données de panel** couvrant la période 2013-2020.

## 📊 Présentation du Projet

L'objectif est de déterminer si l'augmentation du stock de diplômés du supérieur dans une région réduit significativement son taux de chômage, tout en contrôlant par le dynamisme économique local (PIB). 

Le projet compare trois approches méthodologiques :
1. **MCO (Pooled OLS)** : Modèle de référence.
2. **Modèle à Effets Aléatoires (Random Effects)**.
3. **Modèle à Effets Fixes (Within)** : Pour capturer les spécificités structurelles de chaque territoire.

## 🛠️ Méthodologie & Outils

* **Langage** : R
* **Packages clés** : 
    * `plm` : Pour les régressions sur données de panel.
    * `stargazer` & `xtable` : Pour la génération de tableaux de résultats académiques.
    * `ggplot2` : Pour la visualisation de données.
* **Statistique clé** : Réalisation du **Test de Hausman** pour valider le choix du modèle final.

## 📈 Résultats Principaux

* **Validation du modèle** : Le test de Hausman ($p < 0.05$) a conduit à la validation du **Modèle à Effets Fixes**.
* **Impact du PIB** : La richesse produite par habitant est le déterminant le plus robuste de la baisse du chômage.
* **Nuance sur l'éducation** : Si le capital humain est corrélé à l'emploi, son effet marginal est souvent capté par les caractéristiques structurelles propres aux régions dynamiques.



## 📁 Structure du Dépôt

* `Rapport.Rmd` : Script principal contenant l'importation, le nettoyage, les tests et les modèles.
* `Rapport.pdf` : Le rendu final du projet exporté .


1. Clonez ce dépôt :
   ```bash
   git clone [https://github.com/votre-nom-utilisateur/projet-econometrie.git](https://github.com/votre-nom-utilisateur/projet-econometrie.git)
