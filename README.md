# Analyse de Série Temporelle — Ventes de Véhicules (FRED)

## Objectif du projet

Ce projet a pour objectif d’analyser une série temporelle de ventes de véhicules légers afin de :

* Comprendre la gestion des dates et du temps avec Pandas
* Manipuler un index temporel (`DatetimeIndex`)
* Transformer les données (resampling, décalage, différenciation)
* Identifier des tendances et dynamiques temporelles
* Visualiser l’évolution des ventes dans le temps

---

## Dataset

* Source : FRED (Federal Reserve Economic Data)
* Format : `.csv`
* Description : série temporelle des ventes de véhicules légers aux États-Unis

---

## Technologies utilisées

* Python
* Pandas
* Matplotlib
* Jupyter Notebook

---

## Instructions pour exécuter le projet

### 1. Cloner le dépôt GitHub

```
git clone https://github.com/cdjarabe07/serie-temporelle-pandas
cd serie-temporelle-pandas
```

---

### 2. Installer les dépendances

```
pip install pandas matplotlib jupyter
```

---

### 3. Lancer Jupyter Notebook

```
jupyter notebook
```

---

### 4. Exécuter le notebook principal

1. `01_time_series_analysis.ipynb`

---

## Préparation des données

* Chargement du dataset CSV
* Conversion de la colonne de date en format datetime
* Définition de la date comme index (`DatetimeIndex`)
* Tri chronologique des données

---

## Analyses réalisées

### Manipulation temporelle

* Création de plages de dates avec `pd.date_range()`
* Compréhension des fréquences :

  * Journalière (D)
  * Hebdomadaire (W)
  * Mensuelle (M)

### Resampling

* Agrégation des données :

  * Mensuelle
  * Trimestrielle

### Transformations temporelles

* Décalage des données (`shift`)
* Calcul des variations (`diff`)
* Analyse des évolutions d’une période à l’autre

### Analyse de tendance

* Calcul de la moyenne mobile (`rolling`)
* Lissage de la série pour identifier la tendance

---

## Insights principaux

* Identification d’une tendance globale des ventes
* Présence de fluctuations dans le temps
* Mise en évidence des variations d’une période à l’autre
* Amélioration de la lisibilité grâce à la moyenne mobile

---

## Recommandations

* Utiliser la moyenne mobile pour analyser les tendances à long terme
* Surveiller les variations importantes entre périodes
* Adapter l’analyse selon la granularité (mensuelle ou trimestrielle)
* Préparer les données avant toute modélisation prédictive

---

## Structure du projet

```
serie-temporelle-pandas/
│
├── data/
│   └── vehicle_sales_fred.csv
│
├── notebooks/
│   └── 01_time_series_analysis.ipynb
│
├── src/
│   ├── data.py
│   ├── preprocessing.py
│   ├── analysis.py
│   └── visualization.py
│
├── outputs/
│   └── figures/
│
├── requirements.txt
└── README.md
```

---

## Lien du projet GitHub

`https://roadmap.sh/projects/pandas-time-series`
