# classification_credit_bancaire
### Projet Data Science : Développement d'un modèle de machine learning pour un problème de classification de crédit bancaire.

### Ce Projet Python accomplit plusieurs tâches pour le traitement des données, l'exploration des données (EDA), la modélisation et l'évaluation d'un modèle de machine learning pour un problème de classification de crédit bancaire. Voici une explication détaillée de ce que fait chaque partie du code :

#### 1- Importation des bibliothèques : Les bibliothèques nécessaires telles que NumPy, Pandas, Matplotlib, Seaborn, scikit-learn, etc., sont importées pour effectuer diverses opérations.

#### 2- Chargement des données : Les données sont chargées à partir d'un fichier CSV appelé 'train_data.csv' dans un DataFrame Pandas.

#### 3- Traitement des données : Les données sont prétraitées pour remplacer les valeurs manquantes dans les variables catégoriques par les valeurs les plus fréquentes et les valeurs manquantes dans les variables numériques par les valeurs précédentes de la même colonne. Les variables catégoriques sont également encodées en utilisant LabelEncoder. Ensuite, les colonnes inutiles telles que 'Loan_ID' sont supprimées.

#### 4- Exploration des données (EDA) : Quelques visualisations graphiques sont effectuées pour comprendre la distribution des données. Cela inclut des graphiques de comptage pour la variable cible ('Loan_Status') et des graphiques de dispersion pour certaines variables numériques par rapport à la variable cible.

#### 5- Modélisation : Les données sont divisées en ensembles d'entraînement et de test à l'aide de StratifiedShuffleSplit. Trois algorithmes de classification (Régression logistique, KNN, et Arbre de décision) sont utilisés pour entraîner des modèles sur les données d'entraînement.

#### 6- Évaluation des modèles : Les modèles sont évalués en utilisant la précision (accuracy score) sur les données de test. Les résultats sont affichés pour chaque modèle.

#### 7- Réduction des variables : Une sélection de variables est effectuée, en gardant seulement certaines caractéristiques pour créer un nouveau jeu de données (X2).

#### 8- Nouvelle modélisation : La régression logistique est réappliquée sur le nouveau jeu de données (X2) et est évaluée de la même manière.

#### 9- Enregistrement du modèle : Le modèle de régression logistique final est entraîné sur l'ensemble de données complet (X2, y) et est enregistré dans un fichier 'model.pkl' à l'aide de la bibliothèque pickle.
