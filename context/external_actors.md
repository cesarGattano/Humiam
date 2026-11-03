# Acteurs externes

Acteurs extérieurs à l'entreprise qui interagissent avec le réseau social Humiam.

## Communauté utilisatrice

| Acteur               | Description                                                                                                                                   |
| -------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| Visiteur             | Consulte les recettes publiques sans compte                                                                                                   |
| Utilisateur standard | Crée, recherche et organise des recettes et des catalogues, réagit aux recettes, s'abonne à d'autres utilisateurs, reçoit des recommandations |
| Créateur de contenu  | Utilisateur très actif qui produit des recettes de qualité (photos, vidéos, tutoriels) et enrichit les recettes existantes                    |
| Bêta-testeur         | Utilisateur du panel qui accède au MVP dès son lancement ; premier producteur de données de la plateforme                                     |

Tout utilisateur peut devenir **donateur** en versant des micro-paiements mensuels, volontaires et révocables. C'est un statut du compte, pas un rôle distinct (voir [business_model.md](business_model.md)). Ce statut permet de débloquer des privilèges (à définir), comme la possibilité de proposer et voter sur les idées de fonctionnalités à développer.

## Annonceurs

| Acteur                 | Description                                                                       |
| ---------------------- | --------------------------------------------------------------------------------- |
| Restaurateur           | Met en avant son restaurant en publiant des recettes de sa carte, contre paiement ; fournit un lien vers son site web ou un moyen de contact pour réserver |
| Représentant de marque | Publie des recettes utilisant les produits de sa marque, contre paiement ; fournit un lien vers son site web ; publie les données nutritionnelles de ses recettes, par transparence envers la communauté |

Les annonceurs consultent des statistiques de performance de leurs recettes pour évaluer leur partenariat, y compris les **clics de redirection** vers leur site.

## Prestataires

| Acteur                  | Description                                                                              |
| ----------------------- | ---------------------------------------------------------------------------------------- |
| Prestataire de paiement | Traite les dons et les paiements publicitaires ; Humiam ne stocke aucune donnée bancaire |
| Hébergeur cloud         | Fournit l'infrastructure de la plateforme                                                |

## Fournisseurs de données

Sources externes qui enrichissent les données de Humiam : données libres ou extraites de sites web. La liste est indicative et sera précisée lors du bloc 2.

| Acteur                                     | Données fournies                                                                                           |
| ------------------------------------------ | ---------------------------------------------------------------------------------------------------------- |
| Open Food Facts                            | Informations sur les produits alimentaires (API)                                                           |
| ANSES (table Ciqual)                       | Composition nutritionnelle des aliments (fichier)                                                          |
| Référentiel des communes                   | Communes et coordonnées géographiques, pour le ciblage des restaurateurs                                   |
| Référentiel des productions par territoire | Productions agricoles et alimentaires par région, pour le caractère local                                  |
| Calendrier des fêtes et événements         | Dates des fêtes et événements, pour l'analyse de la régularité d'usage                                     |
| Sites web                                  | Données extraites par scraping, sous réserve de légalité (CGU, droit d'auteur, droit des bases de données) |

## Autorités

| Acteur | Description                                   |
| ------ | --------------------------------------------- |
| CNIL   | Autorité de contrôle de la conformité au RGPD |
