# Producteurs de données

Rôles internes impliqués, directement ou indirectement, dans la production de données de la nouvelle plateforme Humiam, au stade MVP à l'heure actuelle. Ces rôles produisent déjà des contenus sur la **plateforme actuelle** (voir [data_need.md](data_need.md#contexte)).

Ce document sert de base à la grille d'entretien des producteurs de données (évaluation E1).

## Synthèse

| Rôle | Équipe | Effectif | Lien avec la production | Données produites | Questions métier concernées (voir [data_need.md](data_need.md)) |
|---|---|---|---|---|---|
| Chef cuisinier·ère | Métier | 4 | Direct | Recettes, métadonnées, variantes, information augmentée | Accueil des contenus maison, Tendances, Caractère sain, Caractère local |
| Photographe / vidéaste | Métier | 2 | Direct | Médias et leurs métadonnées | Accueil des contenus maison |
| Nutritionniste | Métier | 2 | Direct | Échelle et évaluations du caractère sain | Caractère sain |
| Modérateur·rice | Métier | 3 | Direct | Décisions de modération, signalements traités | Interactivité (origine des recettes) |
| Responsable éditorial·e | Métier | 1 | Direct (cadrage) | Ligne éditoriale, calendrier saisonnier, objectifs, validation des classifications | Accueil des contenus maison, Tendances |
| Community manager | Métier | 2 | Porte-parole de la communauté, et direct | Récompenses, animations, retours des bêta-testeurs | Interactivité, Régularité d'usage, Concrétisation, Tendances |
| Chargé·e de partenariats | Support | 1 | Porte-parole des annonceurs, et direct | Données contractuelles | Visibilité générale, Ciblage géographique, Engagement |

## Modalités des entretiens

* Les entretiens sont menés **par rôle**, en groupe : par exemple, les chefs cuisiniers sont interrogés ensemble plutôt que séparément.
  * Avantages : approche plus efficace, et l'entretien planifié peut se tenir même si l'un des membres a un contretemps.
* Chaque entretien porte sur :
  * l'**existant** : les pratiques actuelles sur la plateforme actuelle. Pour les rôles recrutés pour la nouvelle plateforme, il est adapté :
    * nutritionnistes : leur **expérience antérieure** et le travail de préparation mené depuis leur arrivée ;
    * chargé·e de partenariats : uniquement le **projet en cours** (documents déjà produits, échanges avec des prospects), aucune expérience antérieure n'étant supposée ;
  * les **irritants et points bloquants** rencontrés ;
  * les **attentes** vis-à-vis de la nouvelle plateforme.
* Les profils mixtes, producteurs et exploitants, sont aussi interrogés avec la grille des exploitants.
* À l'issue des entretiens, la **synthèse** de l'ensemble est soumise au responsable éditorial pour validation.

## Chef cuisinier·ère

C'est le rôle interne qui agit le plus directement sur la création des données centrales au concept de la plateforme :

* création de recettes de bout en bout ;
* renseignement des métadonnées des recettes : temps, difficulté, portions, saison, type de plat, ingrédients avec quantités et unités ;
* création de **variantes** à partir de recettes existantes (voir l'axe [Recettes en graphe](data_need.md#recettes-en-graphe)) ;
* apport d'**information augmentée** (astuces, explications) ;
* participation à la création de tutoriels ;
* collaboration avec les photographes et vidéastes.

Sur la plateforme actuelle, ce sont eux qui promouvaient de fait des recettes saines, de façon implicite et sans objectif explicite.

## Photographe / vidéaste

En étroite coordination avec les chefs cuisiniers, il crée les médias qui enrichissent les recettes :

* photos et vidéos des recettes et des tutoriels ;
* métadonnées des médias : format, poids, métadonnées EXIF ;
* **droits** associés : droit d'auteur, droit à l'image des personnes filmées ou photographiées ;
* **texte alternatif** des médias, nécessaire à l'accessibilité (RGAA).

## Nutritionniste

Le nutritionniste produit et enrichit les informations relatives au caractère sain des recettes :

* création de l'**échelle** du caractère sain propre à Humiam ;
* évaluation du caractère sain d'une recette, à partir des données déjà présentes dans la recette (ingrédients, quantités) ;
* **arbitrage** entre le calcul automatique et son expertise ;
* **vérification** des données nutritionnelles publiées par les représentants de marque.

Il **consomme** aussi des données externes (Ciqual, Open Food Facts), qu'il choisit et interprète.

Les deux nutritionnistes ont été **recrutés pour la nouvelle plateforme**, qui fait de l'alimentation saine un axe explicite : ils n'ont pas d'expérience de la plateforme actuelle.

## Modérateur·rice

Le modérateur garantit la qualité et la légalité des contenus publiés. Chacune de ses décisions est une donnée :

* statut d'un contenu : publié, masqué, supprimé ;
* motif, date et auteur de la décision ;
* signalements reçus et suite donnée ;
* traitement des demandes juridiques, par exemple la suppression des contenus issus d'un site ou d'un livre au titre du droit d'auteur.

## Responsable éditorial·e

Le responsable éditorial produit des données de cadrage plutôt que des contenus :

* ligne éditoriale et fil conducteur saisonnier des recettes maison ;
* calendrier de production des contenus ;
* **objectifs** d'accueil des contenus maison, fixés à l'avance (voir [Accueil des contenus maison](data_need.md#accueil-des-contenus-maison)) ;
* validation des classifications : saisonnalité, type de plat.

C'est un profil mixte : il est aussi exploitant des données et commanditaire du projet.

Modalités propres à ce rôle :

* **entretien individuel**, centré sur les données de cadrage qu'il est seul à pouvoir décrire (objectifs, calendrier, validation des classifications) : sa vision du besoin est déjà recueillie en tant que commanditaire (voir [data_need.md](data_need.md#commanditaire)). Il peut être mené dans la même séance que l'entretien de la grille des exploitants ;
* **absence des entretiens des autres rôles** : il encadre l'équipe métier, et sa présence pourrait influencer les réponses ;
* **validation de la synthèse** de tous les entretiens, une fois ceux-ci terminés.

## Community manager

Le community manager est le **porte-parole** de la communauté, qui représente la masse la plus importante de production de données. À ce titre, il est interrogé sur la production de données par la communauté, y compris le panel de bêta-testeurs, dont il est le mieux placé pour relayer les retours.

Il produit aussi des données directement :

* **récompenses** attribuées aux utilisateurs, sur la nouvelle plateforme uniquement : la plateforme actuelle n'a aucun système de récompense ;
* animations de la communauté ;
* synthèse des **retours des bêta-testeurs** ;
* éventuellement, modalités de l'intelligence collective (saisonnalité, caractère local).

C'est un profil mixte : il épaule le responsable éditorial et le product manager dans l'expression du besoin (voir [data_need.md](data_need.md#commanditaire)), et il est aussi exploitant des données.

## Chargé·e de partenariats

Situation similaire à celle du community manager, mais vis-à-vis des restaurateurs et des représentants de marque : il est leur **porte-parole**, et raisonne dans le cadre des contrats établis avec eux.

Il produit aussi directement les **données contractuelles** :

* offre vendue et durée de la campagne ;
* rayon de ciblage choisi par le restaurateur ;
* objectif d'engagement convenu avec la marque ;
* obligations de contenu, notamment la publication des données nutritionnelles par les marques.

Le chargé·e de partenariats a été **recruté pour la nouvelle plateforme** : la publicité par recettes sponsorisées est une nouvelle activité, et aucun partenariat n'existe encore. Le modèle publicitaire de Humiam (contextuel, non intrusif, désactivable) n'étant pas standard, aucune expérience antérieure n'est supposée : l'entretien porte uniquement sur le **projet en cours**, à travers :

* les documents déjà produits : projet d'offre, grille tarifaire, modèle de contrat, liste de prospects ;
* les échanges avec des prospects, restaurateurs ou marques, dont il relaie les attentes ;
* le déroulé d'une campagne fictive, de la signature au bilan, en distinguant ce qui est décidé, en cours ou encore ouvert.

Ce témoignage recueille des **intentions** plutôt que des pratiques : un second entretien est à prévoir après la signature des premiers partenariats.

## Parties prenantes consultées

* **Juriste / DPO** : ne produit pas de données, mais il est consulté sur les contraintes qui pèsent sur leur production (droit d'auteur, droit à l'image, RGPD).

## Hors périmètre

* **Équipes techniques** : elles produisent des données techniques (logs, événements d'activité), qui ne relèvent pas des entretiens métiers. Elles sont sollicitées lors de l'étude technique.
