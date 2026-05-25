# 📨 Fiche #003 — Postiz (gitroomhq)

**Source :** https://github.com/gitroomhq/postiz-app  
**Catégorie :** Productivité / Social Media / Scheduling  
**Langage :** TypeScript (Next.js + Node) · Licence : AGPL-3.0 · ⭐ ~20k · ~3M téléchargements Docker  
**Auteur :** Nevo David (gitroomhq)  
**Date d'ajout :** 2026-05-25

---

## 🧠 Ce que c'est

Alternative open source à Buffer, Hypefury, Later et Twitter Hunter pour la planification de posts sur les réseaux sociaux. Self-hostable, sans cap sur le nombre de comptes ou de posts, avec des fonctionnalités IA intégrées pour la création de contenu.

**Note licence :** AGPL-3.0 (copyleft fort) — si tu modifies et distribues, tu dois publier les sources. Pour usage personnel self-hosted, aucun impact.

---

## ⚙️ Fonctionnalités principales

- **30+ plateformes** : X/Twitter, Instagram, LinkedIn, Facebook, Reddit, Threads, Mastodon, Bluesky, Discord, YouTube, TikTok, Pinterest...
- **Planification visuelle** : calendrier de publication drag-and-drop
- **IA intégrée** : génération de contenu, suggestions de posts
- **Analytics** : suivi des performances et de l'engagement
- **Collaboration d'équipe** : invitations, commentaires, workflows d'approbation
- **Marketplace de posts** : achat/vente de posts entre utilisateurs
- **API** : intégration avec N8N, Make.com, Zapier
- **Zéro différence** hosted vs self-hosted — toutes les fonctionnalités disponibles

---

## 🏗️ Architecture technique

```
Postiz
├── Next.js + Node.js  — app unifiée frontend + backend
├── PostgreSQL         — stockage persistant
├── Redis              — file de jobs + cache
└── Temporal           — orchestration de workflows (v2.12+)
```

**Note v2.12+ :** les versions récentes nécessitent Temporal (moteur de workflows). Pour un déploiement simple sans Temporal, utiliser la v2.11.3 (dernière version sans cette dépendance).

---

## 🚀 Installation

```bash
# Docker Compose (recommandé)
git clone https://github.com/gitroomhq/postiz-app.git
cd postiz-app
cp .env.example .env
# Configurer DATABASE_URL, JWT_SECRET, API_URL dans .env
docker compose up -d
# Dashboard : http://localhost:3000
```

**Deploy one-click :** Railway (template v2.11.3 disponible), Elestio.

**Après déploiement :**
1. Créer le premier compte (devient admin)
2. Mettre `DISABLE_REGISTRATION=true` pour bloquer les inscriptions
3. Settings → Providers → connecter les réseaux sociaux via OAuth

---

## 💰 Comparaison vs alternatives payantes

| Outil | Prix | Posts | Comptes | IA |
|---|---|---|---|---|
| Buffer | $15-120/mois | Limité | Limité | ❌ |
| Hypefury | $19-49/mois | Illimité | Limité | Basique |
| Twitter Hunter | $23-49/mois | Illimité | Limité | ✅ |
| **Postiz self-hosted** | **$0 + hébergement** | **Illimité** | **Illimité** | **✅** |

---

## ⚠️ Limites à connaître

- **OAuth requis** pour chaque réseau social (Instagram, LinkedIn... nécessitent une app développeur)
- **Temporal** requis pour les versions récentes — complexité opérationnelle supplémentaire
- **AGPL** : à vérifier si usage commercial ou redistribution
- **Instabilité API réseaux** : les changements d'API Twitter/Meta peuvent casser des intégrations temporairement

---

## 📌 Pertinence pour ce projet

**Alternative directe à Buffer/Hypefury** si tu gères des comptes sur plusieurs réseaux et veux éviter les abonnements mensuels multiples. Idéal si tu publies régulièrement sur plusieurs plateformes (LinkedIn, X, Instagram simultanément).

L'intégration API avec N8N/Make.com le rend intéressant pour des workflows d'automatisation de contenu.

**Tags :** `buffer-alternative` · `social-media` · `scheduling` · `self-hosted` · `n8n` · `productivité`
