# 🛡️ Fiche #008 — AdGuard Home

**Source :** https://github.com/AdguardTeam/AdGuardHome  
**Catégorie :** Réseau / Sécurité / DNS  
**Langage :** Go + TypeScript · Licence : GPL-3.0 · ⭐ 28k  
**Date d'ajout :** 2026-05-25

---

## 🧠 Ce que c'est

Serveur DNS filtrant qui bloque pubs, trackers et domaines malveillants sur tout le réseau domestique — téléphones, tablettes, TV, ordinateurs — sans installer d'extension sur chaque appareil. Pi-hole amélioré avec une interface plus moderne et DNS chiffré (DoH/DoT) natif.

---

## ⚙️ Fonctionnalités principales

- **Blocage DNS réseau-wide** : toutes les pubs bloquées sur tous les appareils
- **DNS-over-HTTPS (DoH) et DNS-over-TLS (DoT)** : requêtes DNS chiffrées
- **Safe Browsing** : blocage phishing et malwares
- **Contrôle parental** : blocage par catégorie
- **Règles par appareil** : paramètres différents selon la machine
- **Stats détaillées** : quels domaines bloqués, par qui, quand
- **~50 Mo RAM** : tourne sur Raspberry Pi

---

## 🚀 Installation

```bash
curl -s -S -L https://raw.githubusercontent.com/AdguardTeam/AdGuardHome/master/scripts/install.sh | sh -s -- -v
# Dashboard : http://localhost:3000
# Puis pointer le DNS de ta box vers l'IP de cette machine
```

---

## 📌 Pertinence

Alternative à NextDNS Premium — même fonctionnalité, 100% local, zéro données qui quittent ton réseau. Efficacité typique : 20-40% des requêtes DNS bloquées sur un réseau domestique.

| | NextDNS Premium | AdGuard Home |
|---|---|---|
| Blocage réseau-wide + DoH/DoT | ✅ | ✅ |
| Coût | $20/mois | $0 |
| Données DNS | Serveurs NextDNS | Local |

**Tags :** `dns` · `ad-blocker` · `réseau` · `sécurité` · `self-hosted` · `raspberry-pi`
