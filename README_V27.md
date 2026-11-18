# Sonoria V27 — accueil et salons unifiés

- Retour à l’accueil classique (sans pancartes ni carrousel).
- Mascotte PNG fournie en arrière-plan, avec relief violet et or.
- Rejoindre un salon depuis l’accueil : le code détecte automatiquement SONOR ou REFR’AIN.
- Le mode reste choisi uniquement par le créateur du salon.
- Les codes sont uniques entre les deux modes.
- Le salon REFR’AIN est ouvert automatiquement via `/refrain.html?join=CODE&name=PSEUDO`.

Déploiement : remplacez les fichiers du dépôt GitHub, puis redéployez sur Render. Les variables Render sont conservées. Les salons restent en mémoire du processus serveur : un redémarrage efface les salons.
