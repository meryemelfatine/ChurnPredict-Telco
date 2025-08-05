# 📊 ChurnPredict-Telco

Projet de classification visant à prédire le churn (désabonnement) des clients d'une entreprise de télécommunications en se basant sur des données clients.

---

## 📁 Description

L’objectif est de détecter à l'avance les clients susceptibles de se désabonner, à l’aide d’algorithmes de machine learning supervisé.  
Ce projet couvre les étapes complètes de data science : EDA, preprocessing, modélisation, évaluation et interprétation.

---

## 📚 Données

- **Source :** [Telco Customer Churn Dataset (Kaggle)](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Taille :** 7043 lignes – 21 colonnes
- **Colonnes cibles :** `Churn` (Yes/No)

---

## 🛠️ Technologies utilisées

- Python (v3)
- Pandas / NumPy
- Seaborn / Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## 📊 EDA (Analyse Exploratoire)

- Analyse de la répartition du churn (`Yes` vs `No`)
- Visualisation des corrélations et de l’impact des variables contractuelles, financières et démographiques
- Nettoyage et encodage des données

📌 Exemple :  
![Churn distribution](notebooks/figures/churn_distribution.png)

---

## 🤖 Modélisation

Le modèle utilisé est un **Random Forest Classifier**.

📌 **Métriques obtenues sur le test set :**

- **Accuracy :** 78.7%
- **Precision (classe 1 / churn) :** 63%
- **Recall (classe 1 / churn) :** 48%
- **F1-score (classe 1 / churn) :** 55%

📌 **Matrice de confusion :**  
![Confusion matrix](notebooks/figures/confusion_matrix.png)

---

## 📂 Arborescence du projet

ChurnPredict-Telco/
├── notebooks/
│ ├── 01_EDA.ipynb
│ └── 02_Modeling.ipynb
├── data/
│ └── WA_Fn-UseC_-Telco-Customer-Churn.csv
├── requirements.txt
├── .gitignore
└── README.md


---

## 🚀 Exécution rapide

```bash
git clone https://github.com/<meryemelfatine>/ChurnPredict-Telco.git
cd ChurnPredict-Telco
python -m venv venv
source venv/bin/activate  # ou .\venv\Scripts\activate sous Windows
pip install -r requirements.txt
jupyter notebook
👩‍💻 Auteure
Meryem El Fatine

Étudiante à l’INSEA — Projet personnel de classification supervisée
📬 Contact
Pour toute question ou suggestion : meryemelfatine37@gmail.com
