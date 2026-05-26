# 022 — Uptime Kuma

- **Source** : [https://github.com/louislam/uptime-kuma](https://github.com/louislam/uptime-kuma)
- **Catégorie** : [Réseau]
- **Langage** : [JavaScript (Node.js)]
- **Licence** : [MIT]
- **Date** : 2026-05-26

## Ce que c'est
Uptime Kuma est un moniteur de disponibilité open-source et auto-hébergé, conçu pour surveiller la santé des services web (sites, API, bases de données, etc.). Il offre une interface intuitive et des alertes en temps réel.

## Fonctionnement
- **Surveillance active** : Ping HTTP(S), TCP, DNS, et vérifications de mots-clés dans les réponses.
- **Alertes flexibles** : Notifications via Discord, Telegram, Slack, Email, etc.
- **Tableau de bord personnalisable** : Vue globale des statuts avec historique et statistiques.
- **Authentification sécurisée** : Support OAuth2, authentification basique et LDAP.
- **Export/Import** : Sauvegarde et restauration des configurations.

## Cas d'usage typique
- Surveiller la disponibilité de services internes ou externes.
- Recevoir des alertes immédiates en cas de panne (ex : API critique).
- Centraliser la supervision de multiples endpoints depuis une seule interface.

## Installation rapide
```bash
docker run -d --name uptime-kuma -p 3001:3001 -v uptime-kuma:/app/data louislam/uptime-kuma:latest
```
Accéder à l'interface via `http://localhost:3001`.

## Pourquoi le retenir
Uptime Kuma combine simplicité, légèreté et puissance pour une surveillance autonome, sans dépendre de solutions SaaS coûteuses. Idéal pour les infrastructures auto-hébergées.