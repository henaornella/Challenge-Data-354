# Analyse LinkedIn pour le Cyber Africa Forum

## Description

La 4e édition du Cyber Africa forum aura lieu le 15 et 16 avril 2024 sous le 
thème "Risques cybernétiques et Intelligence Artificielle (IA) : quelles stratégies de défense face aux nouvelles menaces numériques ?". 
Ce projet vise à fournir un outil permettant d'identifier les tendances sur le sujet,à l'aide du scrapping des posts LinkedIn, du nettoyage et de l'analyse des données récuperé, puis en créant des visualisations dans Power BI. 

## Structure du Projet

- **linkedin_scraper.ipynb** : Script Jupyter Notebook pour le scraping des posts LinkedIn. Ce script se connecte à LinkedIn, extrait les données des posts basés sur les mots-clés définis, et les enregistre dans un fichier CSV.
- **linkedin_posts_cleaned.csv** : Fichier CSV contenant les données nettoyées des posts LinkedIn. Les colonnes incluent : Auteur, Nombre de Likes, Nombre de Commentaires, Nombre de Reposts, Contenu des Posts, Keyword.
- **linkedIn_Analysis_Dashboard.pbix** : Fichier Power BI (.pbix) contenant le tableau de bord interactif pour l'analyse des données extraites. Le tableau de bord inclut plusieurs visualisations pour analyser les tendances des mots-clés, les engagements et les détails des contenus.


## Étapes du Projet

1. **Recherche de Mots-Clés**
   - Les mots-clés utilisés pour la recherche LinkedIn sont définis dans `linkedin_scraper.ipynb`.

2. **Script de Web Scraping**
   - Le script pour extraire les posts LinkedIn se trouve dans `linkedin_scraper.ipynb`.

3. **Nettoyage et Stockage des Données**
   - Les données nettoyées sont stockées dans `linkedin_posts_cleaned.csv`.

4. **Tableau de Bord Power BI**
   - Les visualisations et tableaux de bord sont créés dans `linkedIn_Analysis_Dashbord.pbix`.



## Utilisation

1. **Exécuter le Script de Scraping** :
   - Ouvrez `linkedin_scraper.ipynb` dans Jupyter Notebook et exécutez les cellules pour extraire les données.

2. **Analyse des Données** :
   - Importez `linkedin_posts_cleaned.csv` dans Power BI pour créer ou mettre à jour les visualisations.

3. **Consulter le Tableau de Bord** :
   - Ouvrez `linkedIn_Analysis_Dashboard.pbix` dans Power BI pour explorer les visualisations.


# Captures d'Écran du Tableau de Bord Power BI

### Page 1 : Vue d'ensemble de l'analyse
![Vue d'ensemble de l'analyse](sC:\Users\HP\Desktop\Challenge Data354\Challenge-Data-354\Capture d'ecran Dashboard\page1.png)

### Page 2 : Analyse des Engagements
![Analyse des Engagements](C:\Users\HP\Desktop\Challenge Data354\Challenge-Data-354\Capture d'ecran Dashboard\page2.png)

### Page 3 : Détails du Contenu
![Détails du Contenu](C:\Users\HP\Desktop\Challenge Data354\Challenge-Data-354\Capture d'ecran Dashboard\page3.png)   


## Prérequis

- Python 3.x
- Jupyter Notebook
- Power BI Desktop




 
