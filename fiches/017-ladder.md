# 017 — Ladder

- **Source** : [GitHub - everywall/ladder](http://github.com/everywall/ladder)
- **Catégorie** : [Productivité]
- **Langage** : [Go]
- **Licence** : [MIT]
- **Date** : 2026-05-25

## Ce que c'est
Ladder est un outil auto-hébergé qui remplace les services cloud comme Dropbox, iCloud ou OneDrive. Il synchronise directement les fichiers entre vos appareils avec un chiffrement de bout en bout. Il permet également de contourner les paywalls de nombreux sites d'actualités (NYT, WSJ, Bloomberg, Nature, etc.).

## Fonctionnement
- **Synchronisation directe** : Les fichiers sont échangés directement entre vos appareils sans passer par un serveur central.
- **Chiffrement de bout en bout** : Toutes les données sont chiffrées localement avant d'être synchronisées.
- **Contournement de paywalls** : Fonctionne comme un proxy inverse pour contourner les restrictions d'accès aux articles.
- **Auto-hébergement** : Peut être déployé sur votre propre serveur ou machine locale.
- **Interface web et CLI** : Offre une interface web pour gérer les fichiers et une ligne de commande pour les opérations avancées.

## Cas d'usage typique
- **Remplacer les services cloud** : Synchroniser des fichiers entre plusieurs appareils sans dépendre de Dropbox ou Google Drive.
- **Accéder à des articles payants** : Lire des articles du *New York Times* ou du *Wall Street Journal* sans abonnement.
- **Collaboration sécurisée** : Partager des fichiers de manière chiffrée avec des collaborateurs.

## Installation rapide
```bash
docker run -d \
  --name ladder \
  -p 8080:8080 \
  -v /path/to/data:/data \
  everywall/ladder
```
*Consultez le [README](http://github.com/everywall/ladder#readme) pour plus d'options de configuration.*

## Pourquoi le retenir
Ladder combine synchronisation de fichiers sécurisée et contournement de paywalls, le tout en auto-hébergement. Idéal pour ceux qui veulent éviter les services cloud centralisés tout en gardant un contrôle total sur leurs données.