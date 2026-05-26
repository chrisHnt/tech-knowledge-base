```markdown
# 020 — Jellyfin

- **Source** : [https://github.com/jellyfin/jellyfin](https://github.com/jellyfin/jellyfin)
- **Catégorie** : Médias
- **Langage** : C# (Backend), JavaScript (Frontend)
- **Licence** : GPL-2.0-only
- **Date** : 2026-05-26

## Ce que c'est
Jellyfin est une plateforme open source de streaming multimédia auto-hébergée, souvent comparée à Netflix. Elle permet de diffuser vos films, séries, musique et autres contenus sur n'importe quel appareil sans abonnement ni frais cachés.

## Fonctionnement
- **Auto-hébergement** : Installez Jellyfin sur votre propre serveur ou NAS pour contrôler vos données.
- **Compatibilité multi-appareils** : Accédez à vos médias via des applications dédiées (smartphones, TV, navigateurs, etc.).
- **Transcodage** : Convertit automatiquement les fichiers pour une lecture optimale sur différents appareils.
- **Bibliothèques personnalisables** : Organisez vos médias par type (films, séries, musique) avec métadonnées enrichies.
- **Communauté active** : Développement continu avec des plugins et intégrations tierces.

## Cas d'usage typique
- Remplacer les services de streaming payants (Netflix, Disney+) en utilisant vos propres fichiers.
- Créer une médiathèque familiale accessible à tous les membres du foyer.
- Diffuser des contenus locaux (films, podcasts, musique) sur tous vos appareils sans dépendre du cloud.

## Installation rapide
```bash
docker run -d \
  --name=jellyfin \
  -e PUID=1000 \
  -e PGID=1000 \
  -e TZ=Europe/Paris \
  -p 8096:8096 \
  -v /chemin/vers/config:/config \
  -v /chemin/vers/médias:/media \
  --restart unless-stopped \
  lscr.io/linuxserver/jellyfin:latest
```
*Pour plus d'options (Synology, bare metal, etc.), voir [la documentation officielle](https://jellyfin.org/docs/general/administration/installing/).*

## Pourquoi le retenir
Alternative open source et gratuite aux géants du streaming, idéale pour reprendre le contrôle de vos médias tout en évitant les coûts récurrents.
```