# Block 3: Élaborer et maintenir un entrepôt de données

*Blocs de compétences C13-17*

## Évaluation 5: Mise en place d'un DWH

*Compétences: C13, C14, C15*

*Mise en situation - réelle ou fictive*

### Contexte

Le projet a pour but de couvrir toutes les étapes de mise en place d’un entrepôt de données, de sa modélisation à son usage fonctionnel (réponse au besoin d’analyse).

### Tâches à réaliser

- produire une liste des données nécessaires aux analyses envisagées ;
- réaliser les modélisations logiques et physiques de l’entrepôt de données et des datamarts* ;
- configurer les outils pour la mise en place de l’entrepôt de données et du/des datamarts ;
- configurer les accès aux données pour les équipes d’analyse ;
- configurer les accès aux données opérationnelles sources ;
- organiser la phase de test ;
- rédiger la documentation technique ;
- formaliser un retour d’expérience des outils techniques utilisés : cohérence avec les paramètres
et contraintes du projet ; avantages ; difficultés... ;
- intégrer les sources de données identifiées aux programmes d’ETL ;
- configurer les zones de sorties des ETL ;
- programmer les traitements appliqués aux données, nécessaire au nettoyage des données et
formatage des données en respect des schémas physiques de données des zones de sortie.

### Évaluations

* **Livrables:** Rapport professionnel (5 à 10 pages)
* **Oral:** Présentation orale (10 minutes)

### Contraintes

* L’évaluation doit se faire dans un contexte de réalisation d’un projet fictif proposé par l’équipe
pédagogique ou d’un projet professionnel réalisé en poste.

* Le projet évalué s’appuie sur le cadre
technique de l’entreprise et sur le cadre d’exploitation des données.

#### Contraintes d'évaluation C13

- Les données nécessaires aux analyses sont listées.
- La liste des données nécessaires aux analyses est exhaustive.
- Les modélisations logiques et les modélisations physiques sont
explicités sans erreur d’interprétation.
- Les modélisations appliquent les pratiques de modélisation d’entrepôt
de données : en flocon, en étoile, en constellation.
- L’approche - top-down* ou bottom-up* de création et modélisation de
l’entrepôt de données est justifiée en fonction des caractéristiques du
projet, par exemple : volume de données, fréquences des mise à jour,
nature(s) des analyses...

#### Contraintes d'évaluation C14

- L’entrepôt de données remplit les fonctionnalités attendues.
- Les configurations principales appliquées sont explicitées.
- Les accès aux données opérationnelles sources sont correctement
configurés.
- Les accès à l’entrepôt de données et/ou datamarts pour les équipes
analytiques sont correctement configurés.
- La procédure de test est présentée.
- La procédure de test couvre l’ensemble du spectre technique et
fonctionnel de l’entrepôt de données.
- La documentation technique détaille l’architecture technique et couvre
la procédure d’installation et de configuration de l’entrepôt de
données.
- La documentation respecte une structure permettant d’y rechercher
rapidement une information spécifique.
- La documentation respecte les règles d’accessibilités.
- Un retour d’expérience est fait concernant la pile technique utilisée au
regard des besoins d’analyse et du volume de données géré.

#### Contraintes d'évaluation C15
- Les formats et le volume des données sont connus et expliqués.
- Les ETL sont alimentés avec les données identifiées.
- Les formats des zones de sortie sont connus et expliqués.
- Les données en sortie respectent le format attendu.
- Les ETL appliquent les traitements nécessaires pour la mise en
conformité avec les schémas physiques de données des zones de
sortie.
- Les ETL appliquent les traitements de nettoyage des données utiles et
nécessaires à la qualité des jeux de données en sortie : unicité des
formats et des unités, détection des doublons, etc...,
- Le fonctionnement général et les règles de traitement de chacun des
ETL sont clairement explicités, sans ambiguïté.

### Critères d'un bon sujet

### Comment choisir mon sujet

### Exemples de sujets

---







## Évaluation 6: Maintien en conditions opérationnelles d'un DWH

*Compétences: C16, C17*

*Étude de cas fictive*

### Contexte

Le projet évalué s’appuie sur le cadre technique de l’entreprise et sur le cadre d’exploitation des données. Lors de cette étude de cas, le candidat rend compte de sa capacité à maintenir un entrepôt de données en conditions opérationnelles, qu'il s'agisse aussi bien d'évolutions techniques que d’évolutions du besoin d’analyse.

### Tâches à réaliser

- présenter la méthodologie et l’outillage pour la répartition des tâches de maintenance, leur priorisation et le suivi des indicateurs (par exemple : centre de service au sens ITIL, outils de ticketing, etc.)
- configurer la journalisation des alertes et des erreurs survenant dans l’exploitation de l’entrepôt de données
- mettre en place la procédure de backup* complet et partiel de l’entrepôt de données
- intégrer de nouvelles sources de données à l’entrepôt de données
- ajouter de nouveaux accès à l’entrepôt de données
- documenter les procédures pour l’évolution et la scalabilité de l’entrepôt de données : création d’accès, ajout d’un datamart, augmentation de l’espace de stockage, etc.
- modéliser les variations de dimension (type 1, 2 ou 3 de Ralph Kimball* par exemple)
- intégrer les variations à l’entrepôt de données
- intégrer les variations aux ETL impliqués par celle-ci
- documenter les variations et mettre à jour les modèles logiques et physiques des données

### Évaluations

* **Livrables:** Rapport professionnel (5 à 10 pages)
* **Oral:** Échanges questions/réponses (5 à 10 minutes)

### Contraintes

* Repose sur un entrepôt de données en place
* Repose sur un besoin d'évolution de cet entrepôt de données (technique, évolution dans le schéma des données sources, etc.) en environnement de test.

#### Contraintes d'évaluation C16

- Une journalisation de l’activité de l’entrepôt de données est mise en
place.
- La journalisation catégorise à minima les alertes et les erreurs.
- Un système d’alerte (e-mail, sms, notification..) est mis en place et
activé en cas d’erreur notifiée dans les journaux.
- Les tâches de maintenance sont priorisées selon les objectifs et les
exigences de maintenance.
- Les tâches de maintenance sont assignées entre les membres de
l’équipe de maintenance.
- Les indicateurs de service se base sur les SLA.
- Le tableau de bord permet de rendre compte de l’ensemble des
indicateurs de service.
- Des tâches planifiées de backup partiel et de backup complet du
datawarehouse sont programmées et configurées.
- Les tâches planifiées produisent les résultats attendus.
- La documentation couvre les principaux cas d’usage de gestion de
l’entrepôt : l’intégration de nouvelles sources de données, la création
de nouveaux accès à l’entrepôt de données, espace de stockage,
datamarts, capacité de calcul...
- La documentation est structurée par cas d’usage et explicite la mise
en œuvre des procédures concernées.
- Les nouvelles sources de données sont correctement configurées et
ajoutées au processus d’alimentation de l’entrepôt de données.
- Les ETL sont mis correctement à jour en fonction.
- Les nouveaux accès à l’entrepôt de données sont configurés
conformément au besoin.
- Le registre des traitements de données personnelles intègre
l’ensemble des traitements de données personnelles impliqués dans le
projet d’entrepôt de données.
- Les procédures de tri des données personnelles pour la mise en
conformité de l’entrepôt de données avec le RGPD sont rédigées.
- Les procédures de tri détaillent les traitements de conformité
(automatisés ou non) à appliquer ainsi que leur fréquence d’exécution.

#### Contraintes d'évaluation C17

- La modélisation des variations intègre pleinement les changements
dans les données sources.
- La modélisation des variations permet d’historiser les changements
dans les données sources.
- Les variations sont intégrées à l’entrepôt de données.
- L’intégration des variations respecte la modélisation initiale.
- Les ETL sont mis à jour en fonction des besoins liés aux variations.
La documentation est à jour, avec les variations.


### Critères d'un bon sujet

### Comment choisir mon sujet

### Exemples de sujets

---