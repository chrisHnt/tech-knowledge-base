# 🔐 Fiche #006 — Vaultwarden

**Source :** https://github.com/dani-garcia/vaultwarden  
**Catégorie :** Sécurité / Gestionnaire de mots de passe  
**Langage :** Rust · Licence : AGPL-3.0 · ⭐ 43k  
**Date d'ajout :** 2026-05-25

---

## 🧠 Ce que c'est

Implémentation alternative ultra-légère du serveur Bitwarden, écrite en Rust. Compatible 100% avec tous les clients officiels Bitwarden (iOS, Android, navigateurs, desktop). Tu héberges le serveur, tu utilises les apps Bitwarden gratuites. ~10 Mo RAM au repos — tourne sur un Raspberry Pi.

---

## ⚙️ Fonctionnalités

- Coffre-fort chiffré AES-256 : mots de passe, notes, cartes, identités
- 2FA : TOTP, YubiKey, FIDO2/WebAuthn
- Organisations et collections partagées
- **Bitwarden Send** : partage de fichiers chiffrés temporaires (expiration, mot de passe, limite de vues)
- Import depuis 1Password, LastPass, KeePass, Dashlane...
- Apps officielles Bitwarden : iOS, Android, Chrome, Firefox, Safari...

---

## 🚀 Installation

```bash
# Docker — une seule commande
docker run -d \
  --name vaultwarden \
  -v /vw-data/:/data/ \
  -p 80:80 \
  vaultwarden/server:latest

# HTTPS obligatoire pour les clients mobiles
# Utiliser Caddy (gère Let's Encrypt automatiquement)
```

**⚠️ Après création du compte :** mettre `SIGNUPS_ALLOWED=false`. Backups réguliers de `/data/db.sqlite3`.

---

## 📌 Pertinence

Alternative directe à 1Password Family / LastPass. Tes mots de passe ne quittent jamais ton infrastructure.

| | 1Password | Bitwarden Cloud | Vaultwarden |
|---|---|---|---|
| Chiffrement + 2FA avancé | ✅ | ✅ | ✅ |
| Partage famille | ✅ | Payant | ✅ |
| Bitwarden Send | ❌ | ✅ | ✅ |
| Coût | $5-10/mois | $3/mois | $0 + hébergement |
| Données | Cloud tiers | Cloud Bitwarden | Chez toi |

**Tags :** `password-manager` · `bitwarden` · `sécurité` · `self-hosted` · `rust` · `chiffrement`
