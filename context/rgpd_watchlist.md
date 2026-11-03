# Points de vigilance RGPD

Ce document recense toutes les données évoquées pour Humiam qui relèvent du RGPD, même si elles ne sont pas exploitées dans le projet data : elles pourraient l'être un jour.

Chaque point est un avertissement à traiter lors de la conception (registre des traitements, base légale, durée de conservation, procédures de tri et de suppression).

## Gouvernance et conformité

> [!WARNING]
> **DPO** : sa désignation est obligatoire (article 37), car le suivi des utilisateurs (activité, recommandations) constitue un suivi régulier et systématique à grande échelle. S'il cumule cette fonction avec celle de juriste, son indépendance doit être préservée.

> [!WARNING]
> **Analyse d'impact (AIPD)** : probablement obligatoire, en raison du profilage à grande échelle et des données sensibles pouvant être déduites de l'activité.

> [!WARNING]
> **Bases légales et durées de conservation** : à définir pour chaque traitement, notamment le sort des comptes inactifs.

> [!WARNING]
> **Sous-traitants** : l'hébergeur cloud, le prestataire de paiement et tout autre prestataire traitant des données personnelles doivent être encadrés par un contrat (article 28).

## Hébergement et transferts

> [!WARNING]
> **Ouverture internationale** : lors de l'ouverture hors de l'Union européenne, tout transfert de données personnelles vers un pays tiers (hébergement, prestataires) doit être encadré (décision d'adéquation ou clauses contractuelles types).

## Comptes utilisateurs

> [!WARNING]
> **Mineurs** : en France, un mineur de moins de 15 ans ne peut consentir seul au traitement de ses données ; le consentement de ses parents est requis. L'âge minimal d'inscription et la vérification associée doivent être définis.

> [!WARNING]
> **Pseudo** : un pseudo reste une donnée personnelle dès qu'il permet d'identifier une personne, directement ou par recoupement.

> [!WARNING]
> **Mot de passe** : donnée de sécurité, à ne stocker que sous forme hachée. Ne doit jamais entrer dans les traitements analytiques.

> [!WARNING]
> **Localisation (ville)** : dans une petite commune, la ville associée à un pseudo et à une activité peut suffire à identifier une personne. La granularité doit être justifiée par une finalité (minimisation). Granularité retenue : la ville, justifiée par le ciblage géographique des restaurateurs et par l'évaluation du caractère local des recettes.

> [!WARNING]
> **Préférences alimentaires** : certaines constituent des données sensibles (article 9) :
> * données de santé : allergies, intolérances, maladie cœliaque, régime médical ;
> * convictions religieuses : régime halal, casher, etc.
>
> Leur traitement exige un consentement explicite. Séparer les préférences de goût des contraintes de santé ou religieuses est une mesure de minimisation complémentaire, pas une alternative au consentement.

## Dons et paiements

> [!WARNING]
> **Données de paiement** : traitées par le prestataire de paiement, Humiam ne stocke aucune donnée bancaire. Les références de transaction, montants et dates restent des données personnelles.

> [!WARNING]
> **Statut de donateur et privilège associé** : révèle la situation de contribution d'une personne. Sa visibilité par les autres utilisateurs doit être maîtrisée.

## Publicité

> [!WARNING]
> **Affichage contextuel et ciblage** : afficher une recette sponsorisée parce qu'elle correspond à la recherche en cours est une publicité contextuelle, qui ne repose pas sur un profil. La désactivation de la publicité par l'utilisateur est un choix à respecter dans tous les traitements, mais ce n'est pas en soi un consentement au sens du RGPD.

> [!WARNING]
> **Ciblage publicitaire géographique** : diffuser des recettes sponsorisées en fonction de la localisation de l'utilisateur est un profilage à des fins publicitaires, qui requiert un consentement. Le ciblage publicitaire fondé sur des données sensibles, ou visant des mineurs, est interdit par le règlement européen sur les services numériques (DSA).

> [!WARNING]
> **Clics de redirection** : suivre les clics d'un utilisateur vers le site d'un annonceur est un suivi individuel. Seules des statistiques agrégées doivent être restituées aux annonceurs, et aucun identifiant d'utilisateur ne doit leur être transmis (paramètres d'URL notamment).

> [!WARNING]
> **Contacts des annonceurs** : les coordonnées des restaurateurs et des représentants de marque sont des données personnelles, en particulier lorsqu'il s'agit d'entrepreneurs individuels.

## Contenus publiés

> [!WARNING]
> **Photos et vidéos** : elles peuvent contenir des métadonnées EXIF (géolocalisation, appareil) et montrer des visages ou des lieux privés. Le droit à l'image des personnes représentées, utilisateurs comme salariés, doit être respecté.

> [!WARNING]
> **Suppression d'un compte et généalogie des recettes** : lorsqu'un auteur supprime son compte, le sort de ses recettes et des variantes créées à partir d'elles par d'autres utilisateurs doit être défini (anonymisation de l'auteur, maintien ou suppression des variantes).

## Activité et réactions

> [!WARNING]
> **Données d'activité** : réactions, consultations, recherches et abonnements permettent de profiler un utilisateur, notamment pour le système de recommandation.

> [!WARNING]
> **Historique de recherche** : les termes recherchés peuvent révéler des données sensibles (« sans gluten », « halal », « diabétique »…). Leur conservation et leur rattachement à un compte doivent être limités.

> [!WARNING]
> **Graphe social** : abonnements et partages privés entre utilisateurs révèlent leurs relations. Le contenu et les destinataires d'un partage privé relèvent de la confidentialité des échanges.

> [!WARNING]
> **Engagement passif** : mesurer le temps passé sur une page ou le parcours du catalogue d'un autre utilisateur constitue un suivi comportemental fin. Il nécessite un consentement, sauf s'il se limite à une mesure d'audience anonymisée répondant aux conditions d'exemption de la CNIL. La visibilité de ces consultations pour le propriétaire du catalogue doit aussi être tranchée.

> [!WARNING]
> **Inférences sur les habitudes alimentaires** : analyser la régularité d'usage, les repas occasionnels (repas de fête) ou les recettes réalisées peut révéler indirectement des données sensibles, par exemple une pratique religieuse à travers les fêtes célébrées.

> [!WARNING]
> **Réactions par smileys classées par humeur** : elles révèlent l'état émotionnel exprimé par l'utilisateur.

> [!WARNING]
> **Visiteurs non inscrits** : le suivi de navigation (cookies, traceurs) nécessite un consentement préalable.

## Entrepôt de données

> [!WARNING]
> **Données pseudonymisées** : des identifiants pseudonymisés dans l'entrepôt de données restent des données personnelles, soumises au RGPD. Seules des données réellement anonymisées en sortent.

## Assistant de cuisine

> [!WARNING]
> **Commande vocale** : si l'assistant écoute l'utilisateur, les enregistrements de voix sont des données personnelles. Ils deviennent des données biométriques s'ils servent à identifier la personne.
