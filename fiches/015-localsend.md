# 015 — LocalSend

- **Source** : [GitHub - LocalSend](http://github.com/localsend/localsend)
- **Catégorie** : [Ressources]
- **Langage** : [Dart]
- **Licence** : [MIT]
- **Date** : 2026-05-25

## Ce que c'est
LocalSend est une alternative open-source à AirDrop qui permet de partager des fichiers entre différents appareils (Windows, Mac, Linux, Android, iOS) **sans compte ni cloud**. Idéal pour transférer rapidement des données en local.

## Fonctionnement
- **Multiplateforme** : Fonctionne sur tous les systèmes d'exploitation majeurs.
- **Sans compte** : Pas besoin de créer un compte ou de se connecter.
- **Chiffrement** : Les transferts sont sécurisés par chiffrement.
- **Interface simple** : Une application légère et intuitive.
- **Pas de cloud** : Les fichiers restent sur les appareils, sans stockage externe.

## Cas d'usage typique
- Transférer des photos ou vidéos entre un smartphone et un PC.
- Partager des documents rapidement en réunion sans dépendre d'un service en ligne.
- Envoyer des fichiers à des collègues dans un réseau local.

## Installation rapide
```bash
# Via Docker (recommandé)
docker run -d --name localsend -p 1234:1234 -p 53317:53317 ghcr.io/localsend/localsend:latest

# Ou via les packages officiels :
# - Windows : .exe depuis GitHub Releases
# - Android : APK ou F-Droid
# - iOS : App Store
# - Linux/macOS : AppImage ou .deb/.rpm
```

## Pourquoi le retenir
LocalSend est la solution **open-source, sécurisée et sans dépendance** pour remplacer AirDrop dans tous les environnements, même hors écosystème Apple.