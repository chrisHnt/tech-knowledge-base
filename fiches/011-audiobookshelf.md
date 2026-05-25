# 🎧 Fiche #011 — Audiobookshelf

**Source :** https://github.com/advplyr/audiobookshelf  
**Catégorie :** Médias / Audiobooks / Podcasts  
**Langage :** JavaScript (Node.js + Vue) · Licence : GPL-3.0 · ⭐ 9.4k  
**Date d'ajout :** 2026-05-25

---

## 🧠 Ce que c'est

Serveur self-hosted pour audiobooks et podcasts avec applications mobiles natives (iOS + Android) reconnues comme les meilleures apps d'écoute open source. Gère ta bibliothèque de fichiers audio personnels (MP3, M4B, FLAC...) et les podcasts, accessible depuis tous tes appareils.

---

## ⚙️ Fonctionnalités principales

- **Bibliothèque audiobooks** : MP3, M4B, FLAC, OGG...
- **Métadonnées auto** : depuis Audible, OpenLibrary, Google Books
- **Podcasts** : abonnement flux RSS, téléchargement automatique
- **Progression sync** : reprendre où tu t'es arrêté sur n'importe quel appareil
- **Vitesse de lecture** : 0.5x à 3x avec préservation du pitch
- **Multi-utilisateurs** : bibliothèques séparées
- **Streaming + offline** : via les apps mobiles

---

## 🚀 Installation

```bash
docker run -d \
  --name audiobookshelf \
  -p 13378:80 \
  -v /path/to/audiobooks:/audiobooks \
  -v /path/to/podcasts:/podcasts \
  -v /path/to/config:/config \
  ghcr.io/advplyr/audiobookshelf
# Dashboard : http://localhost:13378
```

---

## 📌 Pertinence

Alternative à Audible + apps podcast payantes si tu possèdes des fichiers audio (achats DRM-free sur Libro.fm, Downpour...) ou télécharges des podcasts. À combiner avec Syncthing (fiche #009) pour synchroniser la bibliothèque sur un NAS.

| | Audible | Audiobookshelf |
|---|---|---|
| Apps mobiles | ✅ | ✅ (excellentes) |
| Progression sync | ✅ | ✅ |
| Podcasts | ❌ | ✅ |
| Coût | $15/mois | $0 + hébergement |

**Tags :** `audiobooks` · `podcasts` · `médias` · `self-hosted` · `streaming` · `nas`
