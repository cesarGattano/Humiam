# Block 2: Réaliser la collecte, le stockage et la mise à disposition des données d’un projet data

*Blocs de compétences C8-12*

## Évaluation 4: Mise à disposition de flux de données

*Compétences: C8, C9, C10, C11, C12*

*Mise en situation - Réel ou fictive*

### Contexte

Le projet évalué a pour but d’optimiser, d’automatiser, de pérenniser et de mettre à disposition les flux de données et les données, utiles et nécessaires à la réalisation du service numérique, par les équipes techniques (par exemple en analyse statistique, en business intelligence, en machine learning ou encore en intelligence artificielle).

### Tâches à réaliser

- présenter le projet et son contexte ;
- exposer les spécifications techniques :
- pour la connexion aux sources de données, la collecte des données, et l'agrégation des données
- pour le stockage des données en base de données ;
- de l’API REST et les accès directs à la base de données.
- fournir l’accès aux dépôt git de l’ensemble des scripts du projet dans la mesure du respect de la
confidentialité des données du projet réel éventuel ;
- faire une démonstration de l'exécution des scripts du projet sous réserve du respect de la
confidentialité des données projet réel éventuel ;
- présenter le fonctionnement logique et technique de l’ensemble des scripts du projet ;
- présenter le fonctionnement logique des requêtes de type SQL pour la collecte des données ;
- présenter les modèles de données (modèle conceptuel, modèle logique et modèle physique) de
la base de données ;
- rédiger les documentations techniques ou procédure :
- des scripts de collecte des données ;
- du script d’import des données ;
- de l’installation du système de base de données ;
- du script d’import des données en base de données ;
- de l’API (REST) ainsi que celle d’accès à la base de données ;
- faire une démonstration des appels à l’API (REST) développée pour l’accès aux données, avec
un client http (Postman par exemple) et illustrant les différentes règles d’accès aux données ;
- réaliser une analyse des vigilances, difficultés et actions spécifiques éventuelles rencontrées au
cours du projet, notamment pour la conformité RGPD ;
- conclure sur les apprentissages réalisés, et les améliorations envisagées.

### Évaluations

* **Livrables:** Rapport professionnel (5-10 pages)
* **Oral:** Présentation orale indivudelle incluant une démonstration (15 minutes)

### Contraintes

L’évaluation doit se faire dans un contexte de réalisation d’un service numérique réel ou fictif basé sur l’usage de données, à partir du cadrage pour la réalisation d’un service numérique (spécifications fonctionnelles et techniques par exemple).

#### Contraintes d'évaluation C8

- La présentation du projet et de son contexte est complète : acteurs,
objectifs fonctionnels et techniques, environnements et contraintes
techniques, budget, organisation du travail et planification.

- Les spécifications techniques précisent : les technologies et outils, les
services externes, les exigences de programmation (langages),
l’accessibilité (disponibilité, accès).

- Le périmètre des spécifications techniques est complet : il couvre
l’ensemble des moyens techniques à mettre en œuvre pour l’extraction
et l'agrégation des données en un jeu de données brutes final.

- Le script d’extraction des données est fonctionnel : toutes les données
visées sont effectivement récupérées à l’issue de l’exécution du script.

- Le script comprend un point de lancement, l’initialisation des
dépendances et des connexions externes, les règles logiques de
traitement, la gestion des erreurs et des exceptions, la fin du
traitement et la sauvegarde des résultats.

- Le script d’extraction des données est versionné* et accessible depuis
un dépôt Git*.

- L’extraction des données est faite depuis un mix entre au moins les
sources suivantes : un service web (API REST), un fichier de données,
un scraping, une base de données et un système big data.

#### Contraintes d'évaluation C9

- Les requêtes de type SQL pour la collecte de données sont
fonctionnelles : les données visées sont effectivement extraites suites
à l'exécution des requêtes.

- La documentation des requêtes met en lumières choix de sélections,
filtrages, conditions, jointures, etc., en fonction des objectifs de
collecte.

- La documentation explicite les optimisations appliquées aux requêtes.


#### Contraintes d'évaluation C10

- Le script d’agrégation des données est fonctionnel : les données sont
effectivement agrégées, nettoyées et normalisées en un seul jeu de
données à l’issue de l’exécution du script.

- Le script d’agrégation des données est versionné et accessible depuis
un dépôt Git.

- La documentation du script d’agrégation est complète : dépendances,
commandes, les enchaînements logiques de l’algorithme, les choix de
nettoyage et d’homogénéisation des formats données.


#### Contraintes d'évaluation C11

- Les modélisations des données respectent la méthode et le
formalisme MERISE.

- Le modèle physique des données est fonctionnel : il est intégré avec succès lors de la création de la base de données, sans erreur.
- La base de données est choisie au regard de la modélisation des données et des contraintes du projet.
- La reproduction des procédures d’installation décrites (base de données et API) a pour résultat un système conforme aux objets techniques attendus.
- Le script d’import fourni est fonctionnel : il permet l’insertion des données dans le système mis en place.
- La documentation technique du script d’import est versionné à la racine du même dépôt Git que celui utilisé pour le script d’import.
- Les documentations techniques des script couvrent les parties suivantes :     
  - les dépendances nécessaires pour la réutilisation des scripts (langages, dépendances externes, etc) 
  - les commandes pour l’exécution des scripts.
- Le registre des traitements de données personnelles intègre l’ensemble des traitements de données personnelles impliqués dans la base de données. 
- Les procédures de tri des données personnelles pour la mise en conformité de la base de données avec le RGPD sont rédigées.
- Les procédures de tri détaillent les traitements de conformité (automatisés ou non) à appliquer ainsi que leur fréquence d’exécution.

#### Contraintres d'évaluation C12

- La documentation technique de l’API (REST) couvre tous les points de terminaisons (endpoints*)
- La documentation technique couvre les règles d’authentification et/ou d’autorisation de l’API.
- La documentation technique respecte les standards du modèle choisi
(par exemple Open API*)
- L’API REST est fonctionnelle pour l’accès aux données du projet : elle
restreint par une autorisation (ou authentification) l'accès aux
données,
- L’API REST est fonctionnelle pour la mise à disposition : elle permet la
récupération de l’ensemble des données nécessaires au projet.

### Critères d'un bon sujet

### Comment choisir mon sujet

### Exemples de sujets

---