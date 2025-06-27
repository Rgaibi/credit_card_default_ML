# 💳 Credit Card Default - Machine Learning Project

Ce projet utilise des techniques de machine learning pour prédire si un client est susceptible de faire défaut sur ses paiements de carte de crédit, à partir d’un dataset bancaire disponible publiquement.

## 📁 Structure du projet

credit_card_default_ML/

│

├── .gitignore

├── LICENSE

├── README.md

├── credit_card_default_analysis.ipynb

├── data/
│   └── credit_card_data.csv


## 🎯 Objectif

Prédire la variable cible `default_payment_next_month`, qui indique si un client a fait défaut de paiement le mois suivant, à partir de ses données financières et démographiques.


## 🔍 Étapes du projet

1. **Chargement et exploration des données**
   - Analyse de la distribution des variables.
   - Visualisations selon la variable cible.
   - Tests statistiques (t-test, chi2) pour détecter les variables significatives.

2. **Prétraitement**
   - Encodage des variables catégorielles (`LabelEncoder`)
   - Séparation en ensembles d'entraînement/test
   - Feature selection avec `SelectKBest`

3. **Modélisation**
   - Trois modèles comparés :
     - `XGBoost`
     - `Random Forest`
     - `Régression logistique`
   - Évaluation avec `classification_report`, `confusion_matrix`, `learning_curve`.

4. **Optimisation de XGBoost**
   - Recherche des hyperparamètres via `RandomizedSearchCV`
   - Utilisation du `scale_pos_weight` pour gérer les classes déséquilibrées
   - Seuil personnalisé de prédiction pour maximiser le recall

5. **Évaluation finale**
   - Rapport de précision, rappel, F1-score
   - Analyse de la courbe précision/rappel
   - Meilleur compromis trouvé à `threshold = 0.4`


## ✅ Résultats

- **XGBoost** optimisé avec seuil personnalisé :
  - Accuracy : **68%**
  - Recall : **75%** (classe positive)
  - F1-Score : **50%**
  - Precision : **37%**

👉 Le modèle permet de détecter une majorité des défauts (rappel élevé), ce qui est crucial dans un contexte de crédit.


## 🛠️ Librairies utilisées

- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `scikit-learn`
- `xgboost`
- `scipy`


## 👤 Auteur

Karim Rgaibi  
GitHub : [github.com/Rgaibi](https://github.com/Rgaibi)



