# EarlyWarning

Projet de prédiction du risque de décrochage universitaire,
à partir de données démographiques, socio-économiques et académiques.

## Données

Le projet utilise le jeu de données public de l'UCI
"Predict Students' Dropout and Academic Success".

Le fichier `data/raw/data.csv` n'est pas versionné sur Git.
Il faut le télécharger manuellement et le placer dans `data/raw/`.

## Organisation

- `notebooks/` : les notebooks d'exploration, exportés en `.ipynb`
- `src/earlywarning/` : le code Python réutilisé par les notebooks
  - `data.py` : chargement, nettoyage, split
  - `features.py` : pipelines de prétraitement
  - `models.py` : définition des modèles
  - `evaluation.py` : métriques, CV, graphiques
- `data/raw/` : les données brutes
- `data/processed/` : les données nettoyées
- `data/reports/` : les résultats et graphiques

## Installation

```
uv sync
```

## Lancement des notebooks

```
uv run jupyter lab
```

