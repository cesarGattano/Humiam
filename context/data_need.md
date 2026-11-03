# Besoin data

## Organisation du projet

* Les axes décrits ci-dessous forment un **projet global**.
* Chaque axe peut être traité comme un **module séparé**, pour répondre aux différentes évaluations de la certification.

## Contexte

* La plateforme Humiam n'existe pas encore : il s'agit de commencer à la **créer** de façon modulaire.
* Lors du premier lancement, une **version MVP** est mise à disposition d'un **panel de bêta-testeurs**, qui alimente les premières données par une pratique régulière.
* Aucune donnée n'existe au départ : les données disponibles sont des **données libres** ou des **données extraites de sites web** (voir [external_actors.md](external_actors.md)).
* Dans le cadre de la certification, des **données artificielles** peuvent être générées pour alimenter les bases de données.
* Périmètre géographique : **France** au lancement, ouverture à l'**Europe** ensuite, puis à l'**international**.
* Objectifs principaux de la plateforme :
    1. faciliter le quotidien des personnes en cuisine en leur permettant de gérer des catalogues de recettes et de facilement retrouver une recette pour préparer un repas.
    2. commencer à constituer une communauté d'utilisateurs autour du besoin de préparer à manger tous les jours et leur permettre d'interagir via des partages de recettes et des smileys en réaction aux recettes.

## Besoin premier

Permettre aux utilisateurs de gérer leurs catalogues de recettes et de se faciliter le quotidien en cuisine.

Exemple d'usage :

* Centraliser toutes les recettes utilisées au quotidien, quelle que soit leur origine : site internet, livre de cuisine, création personnelle.
* Les retrouver facilement.
* Lancer un assistant sur son téléphone qui énonce les étapes l'une après l'autre, au rythme de leur réalisation.

### Espaces personnels

En plus de ses catalogues, chaque utilisateur dispose de deux espaces distincts :

* **Inspiration** : les recettes qui lui donnent envie, sans intention précise de les réaliser.
* **Cuisine** : les recettes qu'il a l'intention de réaliser. La plateforme lui demande ensuite s'il les a réalisées ; s'il répond oui, il peut qualifier le résultat avec un smiley (le même système de smileys que pour les réactions, classés par humeur), ajouter la recette à un catalogue, etc.

## Commanditaire

* **Sponsor** : la **direction** finance le projet et arbitre ses orientations.
* **Expression du besoin** : le **responsable éditorial·e** et le **product manager**, épaulés des **community managers**.
* La grande majorité des données sont publiées par les utilisateurs. Les premières données sont produites par le **panel de bêta-testeurs**.
* L'équipe métier fournit des recettes de haute qualité suivant un fil conducteur qui évoluera au fil des saisons. Elle promeut une alimentation saine et de saison, favorisant les produits locaux.
* La communauté n'est pas commanditaire : elle est **bénéficiaire** du projet. Le commanditaire porte sa voix au sein de l'organisation.

### Questions métier et mesures

#### Interactivité

* **Question** : quel est le taux d'interactivité de la communauté ? Les utilisateurs centralisent-ils leurs propres recettes ou vont-ils plutôt chercher celles des autres ?
* **Mesures envisagées** : les interactions sont hiérarchisées en niveaux d'engagement croissants.

| Niveau | Type d'engagement | Interactions |
|---|---|---|
| 1 | **Passif** (invisible) | Temps passé sur une page, parcours du catalogue d'un autre utilisateur |
| 2 | **Réactif** (visible, sans effort) | Smiley posé sur un contenu, abonnement à un autre utilisateur |
| 3 | **Appropriation et partage** | Ajout d'une recette à son espace « Inspiration », partage volontaire d'une recette à un autre utilisateur (notification privée par exemple) |
| 4 | **Intention, conservation et création** | Ajout d'une recette à son espace « Cuisine », ajout de la recette d'un autre utilisateur à l'un de ses catalogues, création d'une variante |
| 5 | **Réalisation** | Réalisation déclarée d'une recette |

* Pour savoir si les utilisateurs centralisent leurs propres recettes ou vont chercher celles des autres : part des recettes de l'utilisateur et part des recettes des autres dans ses catalogues.
* Pour ses propres recettes, distinction selon leur **origine** : création personnelle, import depuis un site, saisie depuis un livre.
* L'origine (site ou livre source) est conservée : elle permet de répondre à des demandes juridiques, par exemple supprimer tous les contenus issus d'un site ou d'un livre au titre du droit d'auteur.

#### Tendances

* **Question** : quelles recettes sont en vogue à un instant t ? Suivent-elles une saisonnalité (ingrédients de saison, street food…) ?
* **Mesures envisagées** :
  * popularité d'une recette : interactions reçues sur une fenêtre de temps, pondérées selon leur niveau d'engagement (voir [Interactivité](#interactivité)) ;
  * les poids des niveaux sont différents les uns des autres ; leurs valeurs et la fenêtre de temps restent à définir ;
  * saisonnalité et type de plat (street food, plat de fête…) des recettes, renseignés de deux façons :
    * **calcul automatique** autant que possible, par exemple à partir de la saison des ingrédients ;
    * **intelligence collective** : l'équipe métier dispose d'un outil décisionnel qui met la communauté à contribution ; chaque utilisateur peut estimer la saisonnalité d'un plat, et l'information n'est validée qu'à partir de plusieurs avis convergents ;
  * règles d'arbitrage entre calcul automatique et avis de la communauté : à définir.

#### Caractère sain

* **Question** : les plats tendance du moment sont-ils sains ? Comment évolue dans le temps le caractère sain des recettes qui suscitent de l'engagement ?
* **Principe** : le caractère sain de chaque recette est évalué par un **calcul automatique** et par l'**expertise des nutritionnistes** de l'équipe métier. Il est affiché à l'utilisateur à chaque consultation d'une recette.
* **Mesures envisagées** :
  * caractère sain des recettes tendance (voir [Tendances](#tendances)) ;
  * évolution dans le temps du caractère sain des recettes, pondérée par l'engagement qu'elles suscitent (voir [Interactivité](#interactivité)) ;
  * échelle d'évaluation : **échelle propre à Humiam**, à définir par les nutritionnistes de l'équipe métier.

#### Caractère local

* **Question** : les recettes engageantes privilégient-elles les produits locaux ?
* **Principe** : le caractère local d'une recette ne dépend pas de la recette seule, mais du lien entre ses ingrédients et le lieu de l'utilisateur. Il ne se définit pas par une distance, mais à l'échelle minimale d'une **région**, voire d'un **pays ou d'un État** pour les grands pays.
* **Mesures envisagées** :
  * croisement de la ville de l'utilisateur avec les productions de sa région, à partir d'un référentiel externe des productions par territoire ;
  * contribution possible de l'intelligence collective, selon des modalités à définir.

#### Accueil des contenus maison

* **Question** : les recettes de l'équipe métier sont-elles bien accueillies ?
* **Mesures envisagées** :
  * la création de contenu interne est une création **alternative** à la création naturelle de la communauté ; son existence se justifie par sa **reprise par la communauté** ;
  * l'accueil est évalué par rapport à un **objectif fixé à l'avance** par l'équipe métier ;
  * l'objectif porte sur l'engagement suscité par les recettes maison (voir [Interactivité](#interactivité)), au service de la promotion de recettes saines, de saison et à base de produits locaux.

#### Régularité d'usage

* **Question** : les utilisateurs utilisent-ils la plateforme régulièrement ou occasionnellement ? Un usage occasionnel traduit-il un besoin particulier (repas de fête…) ?
* **Mesures envisagées** :
  * unité de mesure : la **semaine**, car la planification des repas d'un foyer se fait généralement à cette échelle ;
  * une semaine est **validée** si l'utilisateur se connecte au moins une fois ;
  * la régularité s'apprécie au fil des semaines : le cas idéal est une validation chaque semaine sans interruption ;
  * la régularité est évaluée sur une **fenêtre glissante des 16 dernières semaines** : un compte est considéré comme **occasionnel** lorsque le nombre de semaines manquées y dépasse le nombre de semaines validées ;
  * les semaines antérieures à l'inscription ne comptent pas comme manquées ;
  * un **nouvel inscrit** est occasionnel par défaut ; il devient régulier après **4 semaines consécutives** d'utilisation. Cette règle ne s'applique qu'une fois : ensuite, seule la fenêtre glissante compte ;
  * durant cette période, un **parcours d'initiation progressif** à la plateforme peut inciter les nouveaux inscrits à devenir réguliers ;
  * pour relier un usage occasionnel à un besoin particulier, l'équipe métier croise :
    * la **temporalité** de l'usage avec un **calendrier des fêtes et événements** (source externe) ;
    * le **type de plats** recherchés (voir la classification prévue dans [Tendances](#tendances)).

#### Concrétisation

* **Question** : les recherches aboutissent-elles ? Les utilisateurs ajoutent-ils la recette à un catalogue, à leur espace « Inspiration » ou « Cuisine », la réalisent-ils ?
* **Mesures envisagées** :
  * aboutissement des recherches, défini à partir des niveaux d'engagement (voir [Interactivité](#interactivité)) :
    * une **visite** est une période d'utilisation continue de la plateforme (session) ;
    * **recherche aboutie** : suivie, dans la même visite, d'une action de niveau 3 ou plus sur l'une des recettes trouvées ;
    * **recherche sans suite** : des résultats sont consultés, mais aucune action n'est réalisée ;
    * **recherche sans résultat** : aucune recette ne correspond ; ce signal révèle à l'équipe éditoriale les manques du contenu disponible ;
  * ajout d'une recette à un catalogue, à l'espace « Inspiration » ou à l'espace « Cuisine » ;
  * réalisation déclarée depuis l'espace « Cuisine » : mesure déclarative, qui ne donne qu'une borne basse du nombre de recettes réellement réalisées ;
  * signal complémentaire possible : lancement de l'assistant pas à pas.

## Second commanditaire

* **Chargé·e de partenariats**, pour tout ce qui concerne la visibilité des contenus des restaurateurs et des représentants de marque.

### Questions métier du chargé·e de partenariats

#### Visibilité générale

* **Question** : une recette sponsorisée est-elle présente dans les recherches des utilisateurs qui n'ont pas désactivé la publicité ?
* **Principe** : une recette sponsorisée n'apparaît que si elle correspond à la recherche de l'utilisateur. La publicité doit répondre à ses attentes, jamais être intrusive. Elle est clairement identifiée comme sponsorisée.
* **Mesures envisagées** :
  * nombre d'affichages de la recette sponsorisée parmi les résultats de recherche pertinents ;
  * position de la recette dans ces résultats.

#### Ciblage géographique (restaurateurs)

* **Question** : les recettes sponsorisées sont-elles diffusées auprès d'utilisateurs géographiquement susceptibles de venir au restaurant ?
* **Principe** : le restaurateur définit lui-même le rayon autour de son restaurant qu'il souhaite cibler. Un utilisateur est dans la zone si sa ville s'y trouve.
* **Mesures envisagées** :
  * part des affichages de la recette sponsorisée auprès d'utilisateurs situés dans la zone ciblée ;
  * clics de redirection vers le site du restaurant ou son moyen de réservation ;
  * le calcul suppose un référentiel des communes avec leurs coordonnées géographiques (source externe).

#### Engagement (représentants de marque)

* **Question** : les recettes sponsorisées déclenchent-elles de l'engagement chez les utilisateurs ?
* **Mesures envisagées** :
  * engagement suscité par les recettes sponsorisées, selon les niveaux d'engagement (voir [Interactivité](#interactivité)) ;
  * clics de redirection vers le site de la marque ;
  * évalué par rapport à un **objectif convenu avec la marque** au moment de la vente de l'offre.

## Axes envisagés

### Recettes en graphe

* Une recette peut être transformée : ajout ou remplacement d'un ingrédient, changement du mode de cuisson, etc.
* Les recettes peuvent être vues comme un arbre généalogique.
* Chaque recette s'accompagne de ses métadonnées et de ses médias (photos, vidéos).

### Comptes utilisateurs

* Minimisation des données personnelles pour respecter le RGPD

Exemple de minimisation :

* pseudos plutôt que prénom, nom
* Localisation géographique limitée à la **ville** : bon compromis entre une donnée vague et son utilité pour le ciblage géographique des restaurateurs (voir [Ciblage géographique](#ciblage-géographique-restaurateurs)) et pour l'évaluation du caractère local (voir [Caractère local](#caractère-local))

### Activité et réactions

* Collecte, stockage et transformation des données d'activité du réseau social.
* Les utilisateurs ne communiquent pas par texte mais par smileys.
* Les smileys sont personnalisables à l'infini avec des éléments du monde de la cuisine (fraise, pomme de terre, assiette…), tout en restant classables par type d'humeur.

### Données nutritionnelles

* Elles servent à évaluer le caractère sain des recettes (voir [Caractère sain](#caractère-sain)).
* Elles proviennent de données ouvertes (Ciqual, Open Food Facts…) ; les nutritionnistes définissent l'échelle du caractère sain et apportent leur expertise.
* Les représentants de marque publient aussi les données nutritionnelles de leurs recettes, par transparence envers la communauté.
* Mode de gestion détaillé non défini : dépend des données disponibles en open data.

## Paramètres laissés ouverts

Paramètres volontairement non fixés à ce stade, qui pourront être précisés lors des entretiens :

* poids de chaque niveau d'engagement ;
* fenêtre de temps des tendances ;
* règles d'arbitrage entre calcul automatique et intelligence collective pour la saisonnalité ;
* échelle du caractère sain, à définir par les nutritionnistes ;
* articulation entre les données nutritionnelles publiées par les marques et l'évaluation de Humiam (calcul automatique et nutritionnistes) ;
* modalités de l'intelligence collective pour le caractère local.

## Hors périmètre

* Données de fonctionnement interne de l'entreprise (RH, temps de travail, management…).

## Points de vigilance

* Les données personnelles évoquées sont recensées dans [rgpd_watchlist.md](rgpd_watchlist.md).
