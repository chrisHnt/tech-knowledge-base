# 🔖 Fiche #005 — Karakeep

**Source :** https://github.com/karakeep-app/karakeep  
**Catégorie :** Productivité / Favoris / Read-it-later  
**Langage :** TypeScript · Licence : AGPL-3.0 · ⭐ ~22k  
**Date d'ajout :** 2026-05-25

---

## 🧠 Ce que c'est

Gestionnaire de favoris intelligent self-hosted qui remplace Pocket, Raindrop.io, Instapaper. Sauvegarde liens, screenshots, articles et PDFs, les archive localement (plus de lien mort), et les auto-tage via IA. Anciennement appelé **Hoarder**. Devenu la référence read-it-later après la fermeture de Pocket par Mozilla en 2025.

---

## ⚙️ Fonctionnalités principales

- **Archivage local** : snapshot des pages, plus de lien mort
- **OCR** : extraction de texte sur images et PDFs sauvegardés
- **Auto-tags IA** : via OpenAI ou Ollama (local)
- **Recherche full-text** dans le contenu archivé
- **Extensions navigateur** : Chrome, Firefox
- **Apps mobiles** : iOS, Android
- **Import** : depuis Pocket, Raindrop, Instapaper
- **API REST** pour automatisations

---

## 🚀 Installation

```bash
wget https://raw.githubusercontent.com/karakeep-app/karakeep/main/docker/docker-compose.yml
# Configurer NEXTAUTH_SECRET dans .env
# OPENAI_API_KEY optionnel (ou Ollama pour local)
docker compose up -d
# Dashboard : http://localhost:3000
```

---

## 📌 Pertinence

Remplace Pocket + Raindrop Pro. L'intégration Ollama (fiche #007 ai-kb) permettra du tagging IA 100% local avec le nouveau Mac.

| | Pocket (fermé) | Raindrop Pro | Karakeep |
|---|---|---|---|
| Archivage offline | ✅ | ✅ | ✅ |
| Auto-tags IA | ❌ | ❌ | ✅ |
| OCR | ❌ | ❌ | ✅ |
| Coût | Fermé 2025 | $3/mois | $0 + hébergement |

**Tags :** `read-it-later` · `bookmarks` · `pocket-alternative` · `self-hosted` · `ocr`
