# 💳 Credit Card Default - Machine Learning Project

Ce projet utilise des techniques de machine learning pour prédire si un client est susceptible de faire défaut sur ses paiements de carte de crédit, à partir d’un dataset bancaire disponible publiquement.

## 📁 Structure du projet

credit_card_default_ML/
│

├── credit_card_data.csv # Données brutes

├── credit_card_default_analysis.ipynb # Notebook principal d'analyse et de modélisation

├── README.md # Description du projet

└── .gitignore # Fichiers à exclure du suivi Git


## 🎯 Objectif

Améliorer la détection des clients à risque de défaut de paiement pour une éventuelle utilisation dans un modèle de scoring bancaire.

## 📊 Données

Le dataset contient des informations sur plus de 30 000 clients, avec des variables comme :
- Âge, genre, statut marital, niveau d’éducation
- Historique de remboursement sur 6 mois
- Montants des paiements, crédits et limites
- Variable cible : `default.payment.next.month`

## 🛠️ Techniques utilisées

- Nettoyage et préparation des données (pandas)
- Visualisation (matplotlib, seaborn)
- Modélisation avec XGBoost
- Équilibrage de classes (scale_pos_weight)
- Évaluation : confusion matrix, F1-score, recall, precision

## 🔍 Résultats

- Modèle final : `XGBClassifier`
- Score F1, recall et précision optimisés à l’aide de GridSearchCV
- Sauvegarde du modèle avec `joblib` pour une future réutilisation

## 👤 Auteur

Karim Rgaibi  
GitHub : [github.com/Rgaibi](https://github.com/Rgaibi)



