# Prédicteur de Charges d'Assurance Maladie

Petit projet d'exploration et de modélisation (régression) des charges d'assurance santé à partir du jeu de données `ensurance.csv`.

## Contenu du dépôt
- Dataset: [ensurance.csv](ensurance.csv)  
- Notebooks:
  - EDA & preprocessing: [main.ipynb](main.ipynb)  
  - Pipeline + saving/loading models: [pipline.ipynb](pipline.ipynb)  
  - Baseline & tuning comparisons: [performance.ipynb](performance.ipynb)  
  - Training scripts / simple examples: [trainmodel.ipynb](trainmodel.ipynb)  
  - SVR experiments: [SVR.ipynb](SVR.ipynb)  
- Script: [main.py](main.py)

## Objectifs
- Nettoyage et analyse exploratoire des données (voir [main.ipynb](main.ipynb)).
- Prétraitement reproductible via pipeline (voir [pipline.ipynb](pipline.ipynb)).
- Comparaison de modèles (LinearRegression, RandomForest, XGBoost, SVR) et tuning (voir [performance.ipynb](performance.ipynb) et [trainmodel.ipynb](trainmodel.ipynb)).
- Expérimentations SVR (log-target, scaling) dans [SVR.ipynb](SVR.ipynb).

## Installation (rapide)
1. Créez un environnement Python 3.8+.
2. Installez dépendances usuelles :
```sh
pip install pandas numpy scikit-learn matplotlib seaborn jupyterlab
# Optional: xgboost, joblib
pip install xgboost joblib
```

## Exécution
- Ouvrir les notebooks dans Jupyter / JupyterLab : par ex. `jupyter lab` puis charger [main.ipynb](main.ipynb).
- Pour exécuter le script d'exemple :
```sh
python main.py
```

## Notes
- Les notebooks s'attendent à trouver `ensurance.csv` dans le même répertoire.  
- Les notebooks contiennent cellules pour prétraitement, entraînement et évaluation ; si vous souhaitez réentraîner et sauvegarder des modèles vérifiez les chemins dans [pipline.ipynb](pipline.ipynb).

