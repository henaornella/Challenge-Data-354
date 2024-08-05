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
   - Les mots-clés utilisés pour la recherche LinkedIn sont définis dans [`linkedin_scraper.ipynb](https://github.com/henaornella/Challenge-Data-354/blob/main/linkedin_scraper.ipynb).

2. **Script de Web Scraping**
   - Le script pour extraire les posts LinkedIn se trouve dans `linkedin_scraper.ipynb`.

3. **Nettoyage et Stockage des Données**
   - Les données nettoyées sont stockées dans [`linkedin_posts_cleaned.csv`](https://github.com/henaornella/Challenge-Data-354/blob/main/linkedin_posts_cleaned.csv).

4. **Tableau de Bord Power BI**
   - Les visualisations et tableaux de bord sont créés dans [`linkedIn_Analysis_Dashbord.pbix`](https://github.com/henaornella/Challenge-Data-354/blob/main/LinkedIn_Analysis_Dashbord.pbix).


## Utilisation

1. **Exécuter le Script de Scraping** :
   - Ouvrez `linkedin_scraper.ipynb` dans Jupyter Notebook et exécutez les cellules pour extraire les données.

2. **Analyse des Données** :
   - Importez `linkedin_posts_cleaned.csv` dans Power BI pour créer ou mettre à jour les visualisations.

3. **Consulter le Tableau de Bord** :
   - Ouvrez `linkedIn_Analysis_Dashboard.pbix` dans Power BI pour explorer les visualisations.


# Captures d'Écran du Tableau de Bord Power BI

### Page 1 : Vue d'ensemble de l'analyse

![Vue d'ensemble de l'analyse](https://github.com/henaornella/Challenge-Data-354/blob/main/Captures%20d'ecran/page1.png)

- Top Mots Clés :
    - Description :
    - But : Identifier les mots clés les plus utilisés dans les posts pour analyser les tendances principales et les sujets d'intérêt.
    - Visualisation : Graphique en Barres
    - Axes :
       - Axe X : Nombre de posts (quantité de posts contenant chaque mot clé).
       - Axe Y : Mots clés (les différents mots clés utilisés).
         
- Nombre d'Utilisations des Mots Clés par Mois
     - But : Visualiser la fréquence d'utilisation des mots clés au fil du temps pour identifier les tendances mensuelles.
     - Visualisation : Graphique en Colonnes Groupées
     - Axes :
        - Axe X : Date (mois).
        - Axe Y : Nombre de posts.
     - Explication : Ce graphique montre combien de fois les mots clés ont été utilisés chaque mois, ce qui aide à identifier les périodes de forte activité.

- Répartition du Nombre de Posts et de Mots Clés par Auteurs 
     - But : Analyser la contribution des auteurs en termes de nombre de posts et de diversité de mots clés utilisés.
     - Visualisation : Graphique en Colonnes Groupées
     - Axes :
         - Axe X : Auteurs.
         - Axe Y : Nombre de posts.
         - Légende : Mots clés.
     - Explication : Ce graphique permet de voir quels auteurs publient le plus et quels mots clés ils utilisent, offrant ainsi une vue d'ensemble sur la participation des auteurs et la diversité des sujets abordés.
       

- Auteurs Fréquents
     - But : Identifier les auteurs les plus actifs en termes de nombre de posts.
     - Visualisation : Graphique en Colonnes
     - Axes :
       
         - Axe X : Auteurs.
         - Axe Y : Nombre de posts.
     - Explication : Ce graphique met en évidence les auteurs qui publient le plus fréquemment, aidant à identifier les contributeurs clés et à comprendre leur influence sur les discussions autour des mots clés.
  
- Filtres
    - But : Affiner l'analyse des graphiques en permettant de filtrer les données selon différents critères.
   - Filtres :
       - Année : Permet de filtrer les données pour une année spécifique ou une plage d'années.
       - Mots Clés : Permet de sélectionner un ou plusieurs mots clés pour voir leur utilisation spécifique.
       - Auteurs : Permet de filtrer les données par auteur pour analyser la contribution d'un ou plusieurs auteurs spécifiques.
     - Explication : Ces filtres permettent de personnaliser les vues des graphiques en fonction des critères sélectionnés. Par exemple, vous pouver voir la répartition des mots clés pour une année spécifique, ou identifier les auteurs les plus actifs sur certains mots clés.
       


### Page 2 : Analyse des Engagements

![Analyse des Engagements](https://github.com/henaornella/Challenge-Data-354/blob/main/Captures%20d'ecran/page2.png)

- Total Réactions par Mot Clé
     - But : Visualiser le nombre total de likes reçus par chaque mot clé.
     - Axes :
          - Axe X : Nombre de likes.
          - Axe Y : Mots clés.
     - Explication : Ce graphique montre combien de likes chaque mot clé a reçu, permettant d'identifier les sujets les plus appréciés et engageants.
       
- Total Commentaires par Mot Clé
     - But : Analyser le nombre total de commentaires par auteur pour chaque mot clé.
     - Axes :
        - Axe X : Auteurs.
        - Axe Y : Nombre de commentaires.
     - Explication : Ce graphique met en lumière quels auteurs génèrent le plus de discussions autour des différents mots clés, offrant des insights sur les auteurs les plus engageants.

- Total Reposts par Mot Clé
     - But : Visualiser le nombre total de reposts par auteur pour chaque mot clé.
     - Axes :
         - Axe X : Auteurs.
         - Axe Y : Nombre de reposts.
     - Explication : Ce graphique montre quels auteurs sont les plus prolifiques en termes de reposts, aidant à identifier les auteurs qui amplifient le plus les discussions autour des mots clés.

- Nombre Total d'Auteurs par Mot Clé
     - But : Visualiser le nombre total d'auteurs associés à chaque mot clé.
     - Axes :
         - Axe X : Auteurs.
         - Axe Y : Mots clés.
     - Explication : Ce graphique permet de voir combien d'auteurs différents utilisent chaque mot clé, offrant des insights sur la diversité et l'ampleur de l'engagement autour de chaque sujet



### Page 3 : Détails des Contenus

![Détails des Contenus]([https://github.com/henaornella/Challenge-Data-354/blob/main/Captures%20d'ecran/papier.png](https://github.com/henaornella/Challenge-Data-354/blob/main/Captures%20d'ecran/papier3.png))

- Nuage de Mots (Mots les Plus Fréquemment Utilisés dans les Posts)
     - But : Visualiser les mots les plus fréquemment utilisés dans le contenu des posts pour identifier les termes récurrents et les sujets dominants.
     - Visualisation : Nuage de mots.
     - Explication : Ce nuage de mots montre la fréquence des mots apparaissant dans les posts. Les mots plus fréquents apparaissent en taille plus grande, ce qui permet d’identifier rapidement les thèmes et sujets les plus communs.
       
- Tableau du Contenu des Posts
     - But : Afficher le contenu détaillé des posts pour une analyse qualitative.
     - Visualisation : Tableau.
     - Champs : Contenu des Posts
     - Explication : Ce tableau fournit une vue détaillée de chaque post, permettant aux utilisateurs d'examiner le contenu.
     - 
- Engagement par Auteur
     - But : Visualiser le nombre total de reposts, likes, et commentaires par auteur.
     - Axes :
         - Axe X : Auteurs.
         - Axe Y : Engagement (Reposts, Likes, Commentaires).
         - Légende : Reposts, Likes, Commentaires.
     - Explication : Ce graphique montre les niveaux d'engagement (reposts, likes, commentaires) de chaque auteur. Cela aide à comprendre quels auteurs obtiennent le plus de réactions et interactions pour leurs posts.


## Prérequis

- Python 3.
- Jupyter Notebook
- Power BI Desktop




 
