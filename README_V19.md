SONORIA V19 — SONOR + REFR'AIN

Nouveau mode accessible depuis la page d'accueil ou /refrain.html.
Le chef crée un salon et importe un court extrait instrumental (audio jusqu'à ~2 Mo).
Les autres joueurs disposent de 120 secondes pour enregistrer leur voix avec leur micro (20 s maximum par prise). Quand tous valident, la phase d'écoute commence; les joueurs peuvent écouter le mix instrumental + voix et voter.

IMPORTANT : version prototype. Les enregistrements et l'instrumental sont conservés en mémoire du processus Render, et sont perdus au redémarrage. Le mix utilise deux pistes audio HTML lancées ensemble et n'assure pas une synchronisation audio de précision studio. Pour une production publique, ajouter stockage externe, limites et protections supplémentaires, traitement audio serveur pour synchroniser les pistes, ainsi qu'une gestion des droits musicaux. L'enregistrement du micro requiert HTTPS et autorisation du navigateur.

Installation : remplacer les fichiers du dépôt GitHub, conserver les variables Render déjà configurées et redéployer avec npm install / npm start.
