# Sonoria V26
- Nouveau rendu violet et or 3D, son de rotation du carrousel généré localement par Web Audio (sans fichier audio tiers).
- REF R’AIN : créateur lance la partie, maître du jeu désigné au hasard parmi les joueurs, maître fournit ensuite un lien YouTube instrumental, puis 120 secondes pour soumettre les voix. Le navigateur doit autoriser le micro.
- La vidéo YouTube est intégrée via le lecteur officiel. Le navigateur peut empêcher la lecture automatique, et les deux lectures ne sont pas garanties synchronisées à l’échantillon près.
- Stripe : version d’API explicite 2025-03-31.basil pour résoudre l’incompatibilité Managed Payments observée. Vérifier le résultat avec un paiement test avant mise en production.
- Conserver les variables Render (DISCORD_CLIENT_ID, DISCORD_CLIENT_SECRET, SESSION_SECRET, PUBLIC_URL, DATABASE_URL, STRIPE_SECRET_KEY, STRIPE_WEBHOOK_SECRET). Aucun secret dans GitHub.
