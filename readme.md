# Projet 4 : Optimisation des Données Clients pour la Modélisation Prédictive

## Description  
Ce projet a pour objectif de préparer un ensemble de données clients pour une modélisation prédictive. Vous avez été engagé par Training Data Ltd., un fournisseur de formation en science des données en ligne, pour nettoyer et optimiser le jeu de données `customer_train.csv`. Ce jeu de données sera utilisé pour prédire si les étudiants recherchent un nouvel emploi, une information qui sera utilisée pour les diriger vers des recruteurs potentiels.

## Contexte  
Un problème courant lors de la création de modèles pour générer de la valeur commerciale à partir de données est que les ensembles de données peuvent être si volumineux qu'il peut falloir des jours pour générer des prédictions. Assurer que votre ensemble de données est stocké de manière optimale est crucial pour permettre aux modèles de fonctionner dans des délais raisonnables.

## Données  
Le fichier suivant est utilisé dans ce projet :
- `customer_train.csv` : Contient des informations anonymisées sur les étudiants et leur statut de recherche d'emploi.

## Méthodologie  
Voici les étapes suivies pour réaliser cette analyse :

1. **Chargement et Visualisation des Données**  
   Chargement du jeu de données et affichage des premières lignes pour avoir un aperçu.

2. **Analyse des Colonnes Catégorielles Binaires**  
   Identification et conversion des colonnes catégorielles à deux facteurs en booléens.

3. **Conversion des Types de Données**  
   - Conversion des colonnes `int64` en `int32`.
   - Conversion des colonnes `float64` en `float16`.
   - Conversion des colonnes nominales en catégories.
   - Conversion des colonnes ordinales avec un ordre naturel défini.

4. **Filtrage et Vérification des Données Transformées**  
   Vérification des types de données et de l'intégrité des transformations effectuées.

## Résultats  
Le DataFrame final, `ds_jobs_transformed`, contient des données prêtes pour la modélisation avec une utilisation efficace de la mémoire. Les conversions effectuées permettent de réduire l'empreinte mémoire tout en maintenant la qualité des données.