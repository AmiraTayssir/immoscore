# immoscore-mlops

Projet d'atelier MLOps : preuve de concept de prédiction des prix de maisons avec une régression linéaire.

## Préparer l'environnement

Depuis la racine du projet, créer et activer un environnement virtuel, puis installer les dépendances :

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

## Données

Télécharger `train.csv` depuis la compétition Kaggle [House Prices - Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques), puis le renommer `data.csv` et le placer à la racine du projet.

`data.csv` est ignoré par Git : chaque membre doit disposer de sa propre copie locale. Ne pas ajouter de données au dépôt.

## Exécuter le notebook

Ouvrir `notebooks/house_prices_poc.ipynb` dans VS Code ou Jupyter et exécuter les cellules. Le notebook n'utilise que `data.csv`, entraîne le modèle et affiche les métriques train/test. Le modèle généré est enregistré dans `models/model.pkl`.

Les dossiers `models/` et `reports/` contiendront des sorties générées et sont également ignorés par Git.
