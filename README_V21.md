# SONORIA V21 — Refonte visuelle

Basée sur la V20 fournie. Tous les fichiers serveur, fonctionnalités Discord, Stripe, avatars et les deux modes ont été conservés.

## Changements
- Nouvelle direction artistique cohérente violet profond, or et lavande sur SONOR et REFR'AIN.
- Barre de navigation et logo plus lisibles, boutons avec relief et états de survol/focus.
- Grand bandeau d'accueil et vinyle mieux mis en valeur.
- Panneaux de profil, choix du mode, création et entrée en salon restructurés visuellement.
- Champs, cartes, modales, boutique d'avatars, salons et phases de jeu harmonisés.
- Mise en page mobile adaptée, préférences d'animation réduite respectées.
- REFR'AIN bénéficie aussi du logo et de la nouvelle direction graphique.

## Déploiement
Remplacer les fichiers du dépôt GitHub par ceux du ZIP et pousser sur la branche réellement utilisée par Render. Ne pas supprimer les variables d'environnement Render. Les clés et secrets restent sur Render, jamais dans GitHub.

Cette version est une refonte front-end : elle ne modifie pas les paramètres OAuth Discord ni la logique de paiement Stripe. Une erreur `redirect_uri OAuth2 non valide` se corrige dans Discord Developer Portal et Render.
