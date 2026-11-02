# Projet Humiam

## Auteur

César Gattano, en apprentissage data engineer

## Description

Humiam est un réseau social virtuel autour de la cuisine, c'est-à-dire une plateforme web permettant la création et le partage de recettes de cuisine au sein d'une communauté utilisatrice. Les utilisateurs peuvent entre autres:
* Créer des recettes de cuisine et les partager à leurs contacts ou publiquement
* Créer des catalogues de recettes de cuisine et les partager à leurs contacts ou publiquement
* Organiser à leur convenance les recettes et catalogues dans leur espace personnel
* Retrouver facilement et rapidement une recette en fonction d'un mot-clé, d'une liste d'ingrédients, du temps disponible, etc.

## Contexte

Ce projet s'inscrit dans le cadre de la certification RNCP37638 "Experts en infrastructure de données massives" (Simplon). Il a pour but de couvrir l'ensemble des évaluations attendues pour la certification. Les livrables attendus sont détaillés dans le dossier [deliverables](deliverables). Les évaluations couvrent 21 compétences (C1 à C21) qui s'enchaînent logiquement, réparties en 4 blocs et évaluées au travers de 7 évaluations.

**Échéance : tous les livrables doivent être prêts pour le 1er avril 2027** (examen prévu en avril 2027, date exacte inconnue).

### Périmètre couvert par Humiam

* **Couvertes par ce projet : E1, E2, E3, E4, E5 et E7.**
* **E6 est hors périmètre** : déjà traitée séparément (voir [Takeoff-DBT](https://github.com/cesarGattano/Takeoff-DBT)). Ne pas en tenir compte, et notamment ne pas fusionner E2 avec E6 : E2 porte sur la dimension pilotage.
* E5 et E7 demandent en principe un projet fictif proposé par l'équipe pédagogique ou un projet réalisé en poste. Le formateur accepte de tenter de les couvrir avec Humiam ; en cas de difficulté, il fournira des briefs fictifs dédiés. Signaler tôt tout point où Humiam peine à satisfaire les critères de E5 ou E7.

### Points clés du règlement

* **Format de l'oral (titre complet, 90 min)** : 60 min de présentation des blocs 1 à 3, possiblement sous la forme d'une mise en situation unique qui agrège les modalités (avec une démonstration et la simulation de réunion de lancement), puis 10 min d'échange sur E6, 10 min de présentation de E7 et 10 min de questions du jury.
* **Les livrables sont transmis au jury au plus tard 5 jours avant la session.**
* **Évaluation en acquis / non acquis par compétence** : il faut couvrir l'ensemble des critères d'une compétence pour la sécuriser.
* **Référence prioritaire** : la grille d'évaluation individuelle (annexe 3 de `DE_reglement_specifique_certification.pdf`), car c'est elle que remplit le jury. Les documents officiels se contredisent par endroits (ex. E7 évaluée sur C19-C21 ou C18-C21, durée de l'oral E5) : en cas de doute, s'aligner sur la grille et choisir l'interprétation la plus exigeante.
* **C8 exige au moins 5 types de sources** (API REST, fichier de données, scraping, base de données, système big data) : à intégrer dès la conception de Humiam, y compris la légalité du scraping.

## Rôle de Claude : mentor

* César construit lui-même le projet, pas à pas. Le jury évalue **son** travail : Claude l'accompagne, il ne produit pas les livrables à sa place.
* Claude aide à trouver ensemble les meilleures solutions, à toutes les échelles (architecture globale, modélisation, choix d'outils, structure d'un livrable) : poser des questions, proposer des options argumentées avec leurs compromis, challenger les choix, relire.
* À chaque relecture ou proposition, confronter le travail aux **contraintes d'évaluation** des compétences concernées (sections « Contraintes d'évaluation Cx » des fichiers `deliverables/blocN/BLOCN.md`) et signaler explicitement les critères non couverts.
* Garder en tête la vision d'ensemble : un choix fait pour un bloc doit rester cohérent avec les autres (ex. les données du bloc 2 alimentent le DWH du bloc 3 et le data lake du bloc 4).

## Rôle de ce dépôt

* C'est l'**espace central** du projet : documentation, livrables, diagrammes, brainstorming.
* **Aucun code ici**, uniquement des fichiers de documentation. Le code vit dans des dépôts dédiés à des parties spécifiques du projet ; c'est ici qu'on réfléchit à leur mise en place avant d'y mettre les mains.

### Arborescence

* [official/](official) : copies des documents officiels de la certification (PDF), source de référence en cas de doute
  * `DE_parcours_formation.pdf` : parcours de formation
  * `DE_reglement_specifique_certification.pdf` : règlement spécifique de la certification
  * `DE_resume_certification.pdf` : résumé de la certification
  * `DE_schema_certification_competences_epreuves.pdf` : schéma des compétences et des épreuves
* [deliverables/](deliverables) : référentiel de la certification et livrables
  * `README.md` : vue d'ensemble des blocs, liste des évaluations, glossaire
  * `blocN/BLOCN.md` : description des évaluations du bloc (tâches, livrables, contraintes d'évaluation)
  * `blocN/competences.md` : intitulé des compétences du bloc
  * `blocN/evaluationN/` : travail en cours sur le livrable de l'évaluation N
* [diagrams/](diagrams) : diagrammes draw.io (source `.drawio` et export `.svg`), décrits dans `diagrams/README.md`
* [logbook/](logbook) : journal de bord personnel de César

### Dépôts associés

* [Takeoff-DBT](https://github.com/cesarGattano/Takeoff-DBT) : travail réalisé pour l'évaluation 6 (non cloné ici)

## Règles

* **Ne jamais modifier le dossier [logbook/](logbook)** : il est réservé à César. Il peut être lu pour le contexte.
* **Langue** : livrables et contenu des documents Markdown en français ; noms de fichiers, code, messages de commit et commentaires dans le code en anglais.
* **Commits** : format gitmoji conventionnel, en anglais (ex. `docs: :memo: Add interview grid`).

## Exigences transverses du référentiel

À vérifier sur chaque livrable concerné :
* **RGPD** : registre des traitements, procédures de tri et suppression des données personnelles
* **Accessibilité** : supports et outils conformes (RGAA, recommandations Valentin Haüy / Atalan - AcceDe), adaptation des postes de travail
* **Éco-conception** : référentiel général d'éco-conception des services numériques (RGESN)
* **Méthodes attendues** : objectifs SMART, priorisation RICE, modélisation MERISE (bloc 2), modélisation en étoile/flocon/constellation et SCD de Kimball (bloc 3)
