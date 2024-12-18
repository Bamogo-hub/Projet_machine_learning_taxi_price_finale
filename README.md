"# Projet-machine-learning-Taxi-price" 
# Prédiction des Tarifs de Taxis à New York  

Ce projet vise à prédire les tarifs des trajets en taxi dans la ville de New York à partir de données réelles issué de kaggle , en utilisant diverses techniques d'analyse de données et de modélisation.  

## Structure du Projet  

### 1. Analyse Exploratoire  
Le premier notebook est consacré à l’analyse exploratoire des données.  
- **Objectifs :**  
  - Comprendre la structure des données.  
  - Nettoyer les données pour éliminer les anomalies (valeurs manquantes, aberrantes, etc.).  
  - Identifier les relations entre les variables (par exemple, la distance et le tarif).  
- **Résultats :**  
  Une visualisation approfondie des tendances principales, telles que les variations des tarifs en fonction de la distance, des horaires, ou de la proximité avec des aéroports.  

### 2. Modélisation des Tarifs  
Le deuxième notebook contient les implémentations des modèles de prédiction.  
- **Modèles testés :**  
  - Régression linéaire  
  - Ridge  
  - Lasso  
  - K-Nearest Neighbors (KNN)  
  - XGBoost  
- **Résultats :**  
  Après une comparaison des performances des modèles, **KNN** s'est révélé être le plus performant selon les métriques d'évaluation (MAE, MSE,RMSE) et selon le R^2.  

### 3. Dashboard Interactif  
Nous avons développé un **dashboard interactif** avec Streamlit pour rendre le projet accessible et pratique à utiliser :  
- **Page de visualisation :** Exploration des statistiques et des relations dans les données.  
- **Page de prédiction :** Estimation d’un tarif en fonction des informations fournies par l’utilisateur (lieux de départ et d'arrivée, nombre de passagers, date, heure).  
- **Page de soumission :** Prédictions en masse via un fichier CSV contenant les trajets à estimer.  

## Usage  
1. Clonez ce dépôt :  
   ```bash
   git clone <URL_du_dépôt>

2. Installez les dépendances requises :
    ```bash
    pip install -r requirements.txt

3. Lancer le dashboard : 
    ```bash
    streamlit run app.py

## Quelques captures du dashboard

### Page d'accueil 
![Page dd'accueil](IMAGES_DASH/accueil.png)
### Page de visualisation 
Informations générales

![Page de visualisation1](IMAGES_DASH/visual1.png)

Distributions univariées et bivariées avec un échantillon de 500000 lignes
![Page de visualisation2](IMAGES_DASH/visual2.png)

Boxplots suivi d'une visualisation avec le package pygwalker

![Page de visualisation](IMAGES_DASH/visual3.png)

### Page de prédiction 

![Page de prédiction](IMAGES_DASH/Prediction.png)

### page de soumission 

![Page de soumission](IMAGES_DASH/soumission.png)


