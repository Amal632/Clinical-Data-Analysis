# Analyse des données cliniques pour la prédiction de la maladie cardiaque

## 🎯 Objectif du projet
L'objectif de ce projet est de prédire la présence de maladie cardiaque chez des patients à partir de données cliniques et biologiques.  
L'idée est de comprendre quels facteurs (âge, sexe, cholestérol, type de douleur, etc.) influencent le plus le risque, et de construire un modèle prédictif simple et interprétable.

---

## 📂 Dataset utilisé
- Dataset : **Heart Disease UCI** (Kaggle)  
- Source : [https://www.kaggle.com/datasets/amalaitmoulay/heart-disease-uci/data](https://www.kaggle.com/datasets/amalaitmoulay/heart-disease-uci/data)  
- Contient des informations cliniques de patients (âge, sexe, tension artérielle, cholestérol, fréquence cardiaque maximale, type de douleur, etc.)  
- Variable cible : `num` (0 = pas de maladie, >0 = maladie)

---

## 🛠 Méthodes
### 1. Exploration des données (EDA)
- Vérification des types de données et valeurs manquantes
- Statistiques descriptives pour chaque variable
- Visualisation de la répartition des patients selon la maladie, l’âge, le sexe et d’autres facteurs

### 2. Préprocessing
- Transformation de la variable cible en binaire (`disease`) : 0 = pas de maladie, 1 = maladie  
- Imputation des valeurs manquantes (moyenne pour les numériques)  
- Encodage des variables catégorielles avec `get_dummies` pour les transformer en variables numériques

### 3. Modélisation
- Séparation du dataset en train (80%) et test (20%)  
- Modèle utilisé : **Régression logistique**  
- Évaluation du modèle : accuracy, precision, recall, F1-score  
- Analyse de l’importance des variables pour interprétation clinique

---

## 📊 Résultats et interprétation clinique
- Accuracy du modèle : ~XX% (remplacer par le résultat réel)  
- Les facteurs les plus influents sur le risque de maladie cardiaque :  
  - Âge : les patients plus âgés ont un risque plus élevé  
  - Cholestérol : niveaux élevés associés à un risque plus important  
  - Type de douleur (cp) : certaines douleurs sont plus fortement corrélées à la maladie  
  - Sexe : les hommes semblent plus touchés que les femmes dans ce dataset

> Cette analyse permet de comprendre, de manière simple et interprétable, quels facteurs cliniques influencent le risque de maladie cardiaque, tout en proposant un modèle prédictif utilisable pour de futures analyses.


