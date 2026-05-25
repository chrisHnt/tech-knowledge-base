# 📄 Fiche #004 — Paperless-ngx

**Source :** https://github.com/paperless-ngx/paperless-ngx  
**Catégorie :** Productivité / Gestion documentaire  
**Langage :** Python + TypeScript · Licence : GPL-3.0 · ⭐ 40.7k  
**Date d'ajout :** 2026-05-25

---

## 🧠 Ce que c'est

Système de gestion documentaire qui numérise, indexe et archive tous tes documents physiques. Scanne une facture, un contrat, un relevé fiscal — Paperless-ngx applique l'OCR, extrait le texte, auto-tag via machine learning, et rend tout ça searchable depuis une interface web. Successeur officiel des projets Paperless et Paperless-ng.

---

## ⚙️ Fonctionnalités principales

- **OCR automatique** sur PDF, images scannées, photos
- **Auto-classification ML** : tags, correspondants, types de documents assignés automatiquement
- **Recherche full-text** dans le contenu de tous les documents
- **Workflows** : règles automatiques basées sur le contenu (ex: tout ce qui contient "EDF" → tag Énergie)
- **Consommateurs multiples** : dossier surveillé, email, API REST, scanner physique
- **Multi-utilisateurs** : permissions par document
- **i18n** : interface traduite en français

---

## 🚀 Installation

```bash
# Script one-liner
bash -c "$(curl -L https://raw.githubusercontent.com/paperless-ngx/paperless-ngx/main/install-paperless-ngx.sh)"
# Dashboard : http://localhost:8000
```

**Demo live :** https://demo.paperless-ngx.com (login: `demo` / `demo`)

**⚠️ Sécurité :** documents stockés en clair, à faire tourner uniquement en local/réseau domestique.

---

## 📌 Pertinence

Alternative à Adobe Scan + Evernote. Scanner toutes ses factures, contrats, documents fiscaux et les retrouver en 2 secondes via recherche full-text.

| | Adobe Scan + Evernote | Paperless-ngx |
|---|---|---|
| OCR + Recherche full-text | ✅ | ✅ |
| Auto-tags ML | Basique | ✅ |
| Coût | ~$15/mois | $0 + hébergement |
| Données | Cloud tiers | Chez toi |

**Tags :** `document-management` · `ocr` · `self-hosted` · `scanner` · `productivité`
