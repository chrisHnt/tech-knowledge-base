# 📝 Fiche #002 — AFFiNE (toeverything)

**Source :** https://github.com/toeverything/AFFiNE  
**Catégorie :** Productivité / Knowledge Base / Workspace  
**Langage :** TypeScript 90% + Rust · Licence : MIT · ⭐ 65.4k · Forks : 4.6k  
**Auteur :** Toeverything  
**Date d'ajout :** 2026-05-25

---

## 🧠 Ce que c'est

Workspace tout-en-un qui fusionne trois outils en un seul : **éditeur de docs** (comme Notion), **tableau blanc infini** (comme Miro), et **base de données structurée** (comme Airtable). Local-first, offline-first, open source.

La particularité : docs et canvas sont vraiment intégrés — tu peux mettre n'importe quel bloc (texte riche, base de données, page liée, formes, slides, pages web embarquées) directement sur le canvas. Ce n'est pas deux modes séparés.

**Prononciation :** ə'fain ("a-fine")

---

## ⚙️ Fonctionnalités principales

- **Éditeur de docs** : blocs riches, markdown, collaboration temps réel
- **Canvas edgeless** : sticky notes, formes, slides, objets imbriqués
- **Database views** : tableaux, kanban, grilles, filtres
- **Local-first** : toutes les données sur ta machine, sync cloud optionnel
- **Collaboration** : sync temps réel via CRDT (Yjs + y-octo en Rust)
- **AI intégré** : AFFiNE AI (génération de texte, slides, mind maps, code)
- **Templates** : bibliothèque de templates préconstruits
- **Apps natives** : Electron (desktop), iOS/Android (mobile)
- **Self-host** : déploiement Docker complet

---

## 🏗️ Architecture technique

```
AFFiNE
├── BlockSuite       — éditeur collaboratif open source (sous-projet)
├── y-octo (Rust)   — implémentation CRDT YJS native, haute perf
├── OctoBase        — base de données locale, local-first
└── Electron        — app desktop cross-platform
```

**CRDT** (Conflict-free Replicated Data Type) : technologie qui permet la collaboration temps réel ET le fonctionnement offline sans conflit de données — même principe qu'Obsidian Sync ou Notion, mais open source et local.

---

## 🚀 Usage

**Cloud hébergé (le plus simple) :**
```
https://app.affine.pro  — version en ligne gratuite
```

**Self-host Docker :**
```bash
docker run -d \
  --name affine \
  -p 3010:3010 \
  -v ~/.affine:/root/.affine \
  ghcr.io/toeverything/affine-graphql:stable
```
Documentation complète : https://docs.affine.pro/self-host-affine

**Desktop app :** téléchargeable depuis https://affine.pro/download

---

## 📋 Éditions

| Édition | Statut | Licence | Fonctionnalités |
|---|---|---|---|
| Community (CE) | Disponible | MIT | Tout sauf EE |
| Enterprise (EE) | À venir | Commercial | SSO, rebranding, audit avancé |

---

## ⚠️ Limites à connaître

- **App desktop recommandée** pour l'usage local-first (la version web nécessite un serveur)
- **Moins mature que Notion** sur certaines fonctionnalités avancées de base de données
- **Écosystème de plugins** en cours de construction (pas encore aussi riche que Notion)
- **iOS/Android** : apps disponibles mais moins polies que le desktop

---

## 📌 Pertinence pour ce projet

**Alternative directe à Notion** si tu veux posséder tes données et ne plus payer d'abonnement mensuel. L'avantage unique est la fusion docs + canvas dans le même espace — idéal pour du knowledge management visuel.

Comparaison vs Notion :
| Fonctionnalité | Notion Free | Notion Pro ($10/mois) | AFFiNE CE |
|---|---|---|---|
| Blocs illimités | ❌ (limité) | ✅ | ✅ |
| Canvas/whiteboard | ❌ | ❌ | ✅ intégré |
| Offline | ❌ | ❌ | ✅ natif |
| Données sur ta machine | ❌ | ❌ | ✅ |
| Coût | $0 (limité) | $10/mois | $0 |

**Tags :** `notion-alternative` · `miro-alternative` · `knowledge-base` · `local-first` · `self-hosted` · `crdt` · `productivité`
