# 📋 Fiche #012 — Stirling-PDF

**Source :** https://github.com/Stirling-Tools/Stirling-PDF  
**Catégorie :** Productivité / Traitement PDF  
**Langage :** Java (Spring Boot) + JavaScript · Licence : MIT · ⭐ 55k  
**Date d'ajout :** 2026-05-25

---

## 🧠 Ce que c'est

Suite complète de 50+ opérations PDF, self-hosted, accessible via interface web. Toutes les opérations s'effectuent localement — aucun fichier n'est envoyé à des services tiers comme Smallpdf ou ILovePDF. Remplace Adobe Acrobat Pro pour tous les usages courants.

---

## ⚙️ Opérations disponibles (50+)

- **Organisation :** fusion, division, extraction, réorganisation, rotation de pages
- **Conversion :** PDF ↔ Word, Excel, PowerPoint, image, HTML
- **Optimisation :** compression, réduction de taille, réparation de PDFs corrompus
- **Sécurité :** chiffrement, mots de passe, signature numérique, rédaction (caviardage)
- **OCR :** Tesseract, 100+ langues, extraction de texte
- **Formulaires :** remplissage, aplatissement, extraction de données

---

## 🚀 Installation

```bash
docker run -d \
  --name stirling-pdf \
  -p 8080:8080 \
  -e LANGS="fra+eng" \
  frooodle/s-pdf:latest
# Dashboard : http://localhost:8080
```

---

## 📌 Pertinence

Alternative à Adobe Acrobat Pro et aux services web Smallpdf/ILovePDF. Particulièrement utile pour les documents sensibles (contrats, fiscalité, RIB) sans les envoyer sur des serveurs tiers. À combiner avec Paperless-ngx (fiche #004) : préparer les PDFs avant ingéestion.

| | Adobe Acrobat | Smallpdf | Stirling-PDF |
|---|---|---|---|
| Toutes opérations PDF | ✅ | Partiel | ✅ (50+) |
| Documents locaux | ✅ | ❌ | ✅ |
| Coût | $20/mois | $9/mois | $0 |

**Tags :** `pdf` · `ocr` · `adobe-alternative` · `self-hosted` · `productivité` · `sécurité`
