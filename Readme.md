📊 **Projet**

Fruits! est une jeune start-up appartenant au secteur de l'AgriTech qui souhaite proposer de nouvelles façons de récolter les fruits. Son ambition est de préserver la biodiversité fruitière en développant des robots cueilleurs intelligents, capables d’adapter leurs modes de traitement à chaque espèce, afin de garantir une récolte plus respectueuse et optimisée.
La start-up souhaite dans un premier temps accroître sa visibilité auprès du grand public en lançant une application mobile interactive. Cette application offrira aux utilisateurs la possibilité de photographier un fruit et de recevoir immédiatement des informations détaillées à son sujet, telles que son espèce, ses caractéristiques et son origine.

Le projet a donc consisté à configurer un environnement Big Data pour effectuer des traitements à grande échelle.

Pour cela, une première chaîne de traitement a été mise en place, comprenant le préprocessing, l’extraction de caractéristiques et la réduction de dimension. Cette chaîne a été développée en local sur un échantillon réduit d’images, ce qui a permis de valider sa faisabilité ainsi que la pertinence de la solution choisie pour gérer des volumes de données massifs. La chaine de traitement a ensuite été exécuté dans un environnement BigData au sein duqeul un EMR a été configuré.

🎓 **Compétences évaluées**
- Modéliser des données dans un environnement Big Data et en utilisant les outils du Cloud
- Réaliser des calculs distribués sur des données massives en utilisant les outils adaptés
- Sélectionner les outils du Cloud permettant de traiter et stocker des données Big Data


📂 **Architecture du repository**

*Note*: les données ne sont pas inclues et doivent être téléchargés via le lien ci-dessous

```
OC_P9_Realiser-un-environnement-BigData-sur-le-cloud/
│
├── Bootstrap/                    # script pour initialiser l'environnement BigData en installant les package nécessaire
├── Clé/                          # Clé de sécurité permettant de se connecter à l'EMR
├── Config/                       # Fichier de configuration permettant la persistance des notebook sur le S3       
├── Data/                         # Dossiers contenant les images traitées en locale et sur le cloud
├── Notebook/                     # Notebooks contenant les traitements a réaliser en local et sur le cloud                
├── Ouput/                                
│   ├── Test_Local/                   
│   │      ├── Features/          # Fichiers contenant les caractéristiques extraites des images en local
│   │      ├── PCA/               # Résultats de la réduction de dimension (PCA) sur l’échantillon local
│   │      ├── Projections/       # Données traitées en local projetées dans l’espace réduit          
│   ├── Cloud_sample/                 
│   │      ├── Features/          # Fichiers contenant les caractéristiques extraites des images sur le cloud (échantillon)  
│   │      ├── PCA/               # Résultats de la réduction de dimension (PCA) sur l’échantillon sur le cloud (échantillon)
│   │      ├── Projections/       # Données traitées sur le cloud (échantillon)  projetées dans l’espace réduit        
│   ├── Cloud_all/                   
│   │      ├── Features/          # Fichiers contenant les caractéristiques extraites des images sur le cloud
│   │      ├── PCA/               # Résultats de la réduction de dimension (PCA) sur l’échantillon sur le cloud
│   │      ├── Projections/       # Données traitées sur le cloud  projetées dans l’espace réduit   
├── Soutenance/                   # Présentation en pdf
├── README.md                     # Documentation générale du projet
├── Requirements                  # Liste des dépendances nécessaires

```

🗄️ **Données**

Les images de fruits utilisés dans le notebook d’analyse  peuvent être téléchargées sur [Kaggle](https://www.kaggle.com/datasets/moltean/fruits).


