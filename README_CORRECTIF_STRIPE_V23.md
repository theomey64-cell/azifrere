# Sonoria V23 — correctif paiement Stripe

Le checkout utilise maintenant les **tarifs Stripe existants** au lieu de créer des produits temporaires sans code fiscal. Le reste du site est conservé.

## Déploiement
1. Remplace les fichiers du dépôt GitHub par ceux de ce ZIP (conserve la branche utilisée par Render).
2. Render > SONORIA-NEW > Environment : conserve toutes tes variables actuelles.
3. Facultatif mais recommandé : ajoute `STRIPE_PRICE_FOOTBALL` et `STRIPE_PRICE_YOUTUBE` avec les identifiants **price_...** correspondant aux tarifs ponctuels à 1,99 € de tes deux produits Stripe. Ne mets pas les liens buy.stripe.com ou les identifiants prod_... ici.
4. Si ces deux variables sont absentes, Sonoria recherche automatiquement un produit actif au nom exact « Pack Footballeurs » ou « Pack YouTubeurs FR », avec un seul tarif actif ponctuel de 1,99 € en EUR et un code fiscal. En cas de doublon, renseigne les variables price_... pour éviter toute ambiguïté.
5. Relance le déploiement sur Render et essaie le checkout.
6. Le webhook Stripe existant reste `/api/stripe/webhook`. Vérifie qu'il écoute `checkout.session.completed` et `checkout.session.async_payment_succeeded`. Les droits sont enregistrés uniquement après confirmation du paiement.

## Attention
- `STRIPE_SECRET_KEY` doit correspondre au même compte Stripe et au même mode (test ou production) que les tarifs.
- Ne publie jamais les secrets Stripe ou Discord sur GitHub.
- Si le paiement échoue, consulte les logs Render : ils affichent désormais l'erreur détaillée du produit ou du tarif.
- Le déblocage automatique nécessite toujours `DATABASE_URL`, `STRIPE_WEBHOOK_SECRET` et un webhook fonctionnel.
