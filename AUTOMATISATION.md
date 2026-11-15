# Le 8 — architecture d'automatisation

## Déjà opérationnel
- Site public GitHub Pages, FAQ et conseiller de réponses vérifiées.
- Qualification des demandes (nom, e-mail, entreprise, date, effectif, projet).
- Estimation indicative CODIR à 149 € par personne pour 10 participants minimum.
- Export local des demandes, sans transmission ni stockage serveur.

## Agents à connecter (non actifs)
1. **Accueil IA** : service backend avec modèle LLM, instructions de sécurité et base de connaissances vérifiée ; aucun secret dans GitHub Pages.
2. **Réservations** : calendrier partagé et validation humaine avant confirmation.
3. **Commercial** : réception sécurisée des formulaires, CRM, consentement RGPD, notification propriétaire et relances.
4. **Devis** : règles tarifaires et génération de propositions, approbation humaine avant envoi.
5. **Prospection** : sources vérifiées, dédoublonnage, brouillons de messages et respect des règles de prospection.
6. **Publications** : préparation des contenus et validation avant diffusion.
7. **Suivi qualité** : journalisation minimisée, alertes d'erreur, tests et supervision.

## Dépendances avant activation
- Choisir un hébergement backend et configurer des secrets serveur (clé API IA, accès e-mail/CRM).
- Définir une adresse de réception et la politique de conservation des données.
- Connecter le calendrier, puis tester une demande de bout en bout.
- Ne jamais promettre de disponibilité ou d'envoi tant que les intégrations ne sont pas vérifiées.
- Les mises à jour automatiques du site doivent passer par tests et revue avant déploiement.
