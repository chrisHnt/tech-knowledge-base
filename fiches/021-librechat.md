# 021 — LibreChat

- **Source** : [GitHub - LibreChat](http://github.com/danny-avila/LibreChat)
- **Catégorie** : [Productivité]
- **Langage** : [JavaScript/TypeScript]
- **Licence** : [MIT]
- **Date** : 2026-05-26

## Ce que c'est
LibreChat est une interface unifiée pour interagir avec plusieurs modèles d'IA (ChatGPT, Claude, Gemini, DeepSeek, etc.) en self-hosted. Contrairement aux solutions SaaS, il permet de centraliser l'accès aux APIs d'IA tout en ne payant que pour l'usage réel, sans abonnement mensuel.

## Fonctionnement
- **Multi-modèles** : Intègre plusieurs fournisseurs d'IA dans une seule interface.
- **Self-hosted** : Déploiement local ou sur un serveur privé pour une confidentialité totale.
- **Paiement à l'usage** : Seules les requêtes API consommées sont facturées (pas d'abonnement fixe).
- **Personnalisation** : Configuration avancée des modèles, clés API et paramètres.
- **Extensible** : Plugins et intégrations pour étendre les fonctionnalités.

## Cas d'usage typique
- **Centralisation des APIs** : Éviter de multiplier les abonnements pour chaque modèle d'IA.
- **Confidentialité** : Traiter des données sensibles sans dépendre de services cloud externes.
- **Économie** : Réduire les coûts en ne payant que pour l'usage réel des APIs.

## Installation rapide
```bash
docker run -d \
  -p 3080:3080 \
  -e MONGO_URI="mongodb://mongo:27017/LibreChat" \
  -e JWT_SECRET="votre_secret" \
  --name librechat \
  ghcr.io/danny-avila/librechat:latest
```

## Pourquoi le retenir
LibreChat offre une alternative open-source et économique aux interfaces propriétaires d'IA, avec une flexibilité totale pour les utilisateurs avancés. Idéal pour les développeurs ou les entreprises souhaitant maîtriser leurs coûts et leur infrastructure.