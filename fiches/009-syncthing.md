# 🔄 Fiche #009 — Syncthing

**Source :** https://github.com/syncthing/syncthing  
**Catégorie :** Productivité / Sync de fichiers / P2P  
**Langage :** Go · Licence : MPL-2.0 · ⭐ 68k  
**Date d'ajout :** 2026-05-25

---

## 🧠 Ce que c'est

Sync de fichiers peer-to-peer, chiffré de bout en bout, sans serveur central. Les fichiers se synchronisent directement entre tes appareils — Mac, iPhone, NAS, serveur — sans jamais passer par un cloud tiers. Zéro abonnement, zéro limite de stockage (ton propre disque).

---

## ⚙️ Fonctionnalités principales

- **P2P natif** : sync directe entre appareils, pas de cloud
- **Chiffrement TLS** : toutes les transmissions chiffrées
- **Contrôle par dossier** : lecture seule, envoi seul, ou bidirectionnel
- **Versioning** : garder N versions précédentes des fichiers modifiés
- **Relay servers** : si NAT bloque la connexion directe (chiffré)
- **Apps** : macOS, Windows, Linux, Android. iOS via Möbius Sync (~4€)

---

## 🚀 Installation

```bash
# macOS
brew install syncthing && brew services start syncthing
# Dashboard : http://localhost:8384
```

**Cas d'usage typiques :** dossier Documents entre Mac + iPhone + NAS • backup photos iPhone • sync projets entre machines • remplacement iCloud Drive/Dropbox

---

## 📌 Pertinence

Alternative directe à Dropbox / iCloud Drive. Zéro coût au-delà du stockage déjà possédé.

| | Dropbox 2TB | iCloud+ 2TB | Syncthing |
|---|---|---|---|
| P2P (pas de cloud) | ❌ | ❌ | ✅ |
| Chiffrement E2E | ❌ | Partiel | ✅ |
| Stockage | 2TB | 2TB | Illimité (ton disque) |
| Coût | $15/mois | $3/mois | $0 |

**Tags :** `sync` · `p2p` · `dropbox-alternative` · `self-hosted` · `chiffrement` · `nas`
