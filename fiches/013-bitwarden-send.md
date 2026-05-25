# 📨 Fiche #013 — Bitwarden Send (via Vaultwarden)

**Source :** https://github.com/bitwarden/server  
**Catégorie :** Sécurité / Partage de fichiers chiffré  
**Langage :** C# (.NET) · Licence : AGPL-3.0 · ⭐ 16k  
**Date d'ajout :** 2026-05-25

---

## 🧠 Ce que c'est

**Bitwarden** est le gestionnaire de mots de passe open source (serveur officiel). **Bitwarden Send** est une fonctionnalité intégrée pour partager des textes ou fichiers via un lien chiffré temporaire avec expiration configurable.

**⚠️ Pour le self-hosting, préférer Vaultwarden (fiche #006)** qui inclut Send et est 10x plus léger (~10 Mo vs plusieurs Go RAM). Ce repo concerne le serveur officiel Bitwarden, adapté plutôt aux équipes/entreprises.

---

## ⚙️ Bitwarden Send — fonctionnement

- **Chiffrement E2E** : contenu chiffré côté client avant envoi
- **Lien temporaire** : expiration configurable (heures/jours)
- **Mot de passe optionnel** : double protection sur le lien
- **Limite de vues** : autodestruction après N consultations
- **Texte ou fichier** : jusqu'à 500 Mo par envoi
- **Pas de compte requis** pour le destinataire
- **Intégré** dans toutes les apps Bitwarden

---

## 📌 Pertinence

Si tu utilises déjà Vaultwarden (fiche #006), tu as Send gratuitement. Remplace WeTransfer Pro pour le partage de fichiers sensibles.

| Outil | Self-hosted | Chiffrement E2E | Expiration | Taille |
|---|---|---|---|---|
| Bitwarden Send (Vaultwarden) | ✅ | ✅ | ✅ | 500 Mo |
| PrivateBin | ✅ | ✅ | ✅ | Texte |
| WeTransfer Pro | ❌ | ❌ | 7 jours | 200 Go |

**Tags :** `bitwarden` · `chiffrement` · `partage-fichiers` · `sécurité` · `e2e` · `self-hosted`
