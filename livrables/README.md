# Structure de l'évaluation pour la certification

## Documents de référence
* **Parcours formation:** https://drive.google.com/drive/folders/1wLOgogl8KnV31yrekCRxi955OqCFDLpx
* **Règlement spécifique certification:** https://drive.google.com/drive/folders/1wLOgogl8KnV31yrekCRxi955OqCFDLpx
* **Résumé certification:** https://drive.google.com/drive/folders/1wLOgogl8KnV31yrekCRxi955OqCFDLpx
* **Schéma certification & compétences:** https://drive.google.com/drive/folders/1wLOgogl8KnV31yrekCRxi955OqCFDLpx

## Résumé d'un projet data
voir [Schéma certification & compétences](https://drive.google.com/drive/folders/1wLOgogl8KnV31yrekCRxi955OqCFDLpx)

| Bloc 1                   | Bloc 2                  | Bloc 3           | Bloc 4              |
| ------------------------ | ----------------------- | ---------------- | ------------------- |
| Questionnement métiers   | Extraction des données  | Modélisation DWH | Architecture DLk    |
| Analyse du besoin data   | Aggrégation des données | Création DWH     | Intégration DLk     |
| Cartographie des données | Accès BDD               | ETL in/out DWH   | Catalogue données   |
| Cadre technique          | API REST                | Maintenance DWH  | Gouvernance données |
| Veille technique         |                         |
| Planification            |                         |
| Supervision              |                         |
| Lancement du projet      |                         |


## Liste des livrables

Chaque livrable est associé à une évaluation. Il y a au total 7 évaluations réparti en 4 blocs.

---

### Bloc 1: Piloter la conduite d’un projet data

Voir [document](BLOC1.md) dédié

---

### Bloc 2: Réaliser la collecte, le stockage et la mise à disposition des données d’un projet data

Voir [document](BLOC2.md) dédié

---

### Bloc 3: Élaborer et maintenir un entrepôt de données (data warehouse)

Voir [document](BLOC3.md) dédié

---

### Bloc 4: Encadrer la collecte massive et la mise à disposition des données issues de l’activité de l’organisation avec un data lake

Voir [document](BLOC4.md) dédié

---

## Fin d'examen

En fin d'examen, 10 minutes seront accordées pour un échange questions/réponses avec les membres du jury qui pourront portés sur l'ensemble des évaluations.

## Glossaire

- **RICE :** Acronyme qui désigne une méthode de priorisation des tâches en agilité. L’ordre de priorité est inversement proportionnel au score obtenu avec cette méthode (prio 1 correspond au score RICE le plus élevé). La calcul du score prend en compte les 4 éléments de priorisation qui sont : la portée (“Reach”), l’impact (“Impact”), la confiance (“Confident”) et l’effort (“Effort”).
  
- **SMART :** L’acronyme SMART peut correspondre à des termes différents selon les caractéristiques de l’objectif que l’on souhaite définir. Nous proposons ici : Spécifique, Mesurable, Acceptable (et Ambitieux), Réaliste, Temporellement défini

- **Feuille de route :** c’est une technique de planification stratégique qui place les objectifs d'un projet et les principaux livrables (tâches, jalons) sur une chronologie, tous regroupés dans une seule représentation visuelle ou graphique

- **Scrum burndown chart :** Un burndown chart ou BDC (en français, graphique d'avancement) est une représentation graphique de l'évolution de quantité de travail restante par rapport au temps sur une période de temps donnée

- **diagram de Gantt :** Le diagramme de Gantt est un outil utilisé en ordonnancement et en gestion de projet et permettant de visualiser dans le temps les diverses tâches composant un projet.
  
- **Versionner :** Garder la trace d’un ou plusieurs fichiers et de l’historique de leurs modifications grâce à un système de gestion de versions.
  
- **Dépôt Git :** Un dépôt Git est un entrepôt virtuel du projet. Il permet d'enregistrer les versions de code et d'y accéder au besoin.
  
- **SQL :** (sigle de “Structured Query Language”, en français : langage de requête structurée) Il s’agit d’un langage de programmation permettant d’écrire des instructions reconnues par la grande majorité des systèmes de gestion de bases de données relationnelles (abrégé SGBDR) du marché. Ces instructions couvrent 4 domaines :
    - Langage de définition de données,
    - Langage de manipulation de données,
    - Langage de contrôle de données,
    - Langage de contrôle des transactions.
  
- **Méthode MERISE :** Merise est une méthode d'analyse, de conception et de gestion de projet informatique.

- **endpoints :** Les endpoints sont les points de communication avec une API, ouvert publiquement ou nécessitant une authentification.
  
- **open API :** C’est une spécification pour une norme pour la définition d'interface programmable (ou API) lisible par machine pour décrire, produire, consommer et explorer des services Web RESTful (API REST).

- **Entrepôt de données :** base de données permettant l’analyse et la prise de décisions, alimentée à partir des données opérationnelles de l’organisation.

- **Encodage :** C’est l’action de transformation d’une donnée pour lui appliquer une nature ou une forme souhaitée.
  
- **Embedding :** Dans un contexte de base de données NoSQL, l’embedding consiste à stocker les données liée à une autre dans la même entité (document, collection...). Dans un contexte SQL, cela aurait donné lieu à une joint 1-n, par exemple.
  
- **Referencing :** De la même manière que l’embedding, le referencing est une technique pour lier des données entre elles en environnement NoSQL. Cette technique se rapproche de systèmes des jointures en SQL mais reste tout de même différente, notamment dans l’exploitation du lien réalisé entre les données.
  
- **Approche orientée requêtes :** C’est une méthode de modélisation des données, principalement utilisée dans un contexte NoSQL et / ou de Data Warehouse.
  
- **NoSQL :** “Famille” de base de données non structurées, notamment performantes dans la gestion de gros volumes de données non structurées.

- **MDM :** Master Data Management (en français : gestion des données de référence) : ensemble des méthodes, outils, concepts et processus permettant de s’assurer que les données de référence soient identifiées et exploitables.
  
- **RGPD :** Règlement Général sur la Protection des Données. Le RGPD encadre le traitement des données personnelles sur le territoire de l’Union européenne.

- **Fait :** élément issus de données opérationnelles stocké dans une table d’un entrepôt de données. On parle aussi de métrique, pour signifier l’élément de mesure de l’activité étudiée.

- **Dimension :** axe d’analyse stocké dans une table d’un entrepôt de données
  
- **datamart :** sous-ensemble d’un entrepôt de données destiné à répondre à un besoin spécifique

- **top-down :** approche de conception et modélisation de l’entrepôt de données dans laquelle chaque datamart doit respecter un modèle normalisé pour l’ensemble de l’entrepôt de données

- **bottom-up (approche de création et modélisation de l’entrepôt de données) :** approche de conception et modélisation de l’entrepôt de données dans laquelle chaque l’entrepôt n’est que la combinaison de datamarts indépendants.

- **ETL (Extract Transform Load) :** logiciel permettant de collecter des données en provenance de sources multiples et de les transformer afin de les intégrer à un système de stockage
  
- **procédure de backup :** sauvegarde des données, généralement sur un système externe, en cas de défaillance matérielle
  
- **SLA :** le “service-level agreement” (SLA) ou “accord de niveau de service“ est un document qui définit la qualité de service, prestation prescrite entre un fournisseur de service et un client.
  
- **les variations de dimension de type 1, 2 ou 3 de Ralph Kimball :** approches de gestion du changement des dimensions des données via l’écrasement des valeurs (type 1), l’ajout de lignes (type 2) ou l’ajout de colonnes (type 3).
  
- **data lake :** espace de stockage global des données relationnelles et non relationnelles d’une organisation permettant leur traitement en fonction de besoins non nécessairement
connus au moment de l’insertion

- **batch :** méthode de traitement reposant sur des la mise en lots. Cela permet principalement de réduire le nombre de traitements informatiques nécessaires à la réalisation d’une tâche de même nature. Il s’agira par exemple de regrouper plusieurs traitements d’import de données de petit volume en un seul traitement de volume supérieur.

- **catalogue (de données) :** inventaire organisé des données de l’organisation
  
- **VM (Machine Virtuelle) :** environnement qui reproduit un système informatique complet (processeur, mémoire, réseau, stockage) sur une machine qui l’héberge.
  
- **conteneur :** environnement qui isole les processus d’une application des autres processus d’un système d’exploitation.





