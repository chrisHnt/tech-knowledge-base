# 📅 Fiche #001 — Cal.diy (calcom)

**Source :** https://github.com/calcom/cal.diy  
**Catégorie :** Productivité / Prise de rendez-vous  
**Langage :** TypeScript (Next.js) · Licence : MIT · ⭐ 44.5k · Forks : 13.7k  
**Auteur :** Cal.com (fork communautaire 100% open source)  
**Date d'ajout :** 2026-05-25

---

## 🧠 Ce que c'est

Alternative open source à Calendly, entièrement auto-hébergée. Cal.diy est le fork communautaire de Cal.com — 100% MIT, sans aucune fonctionnalité enterprise cachée ni licence commerciale requise. Tu possèdes tes données et ton infrastructure.

**Différence Cal.com vs Cal.diy :**
- **Cal.com** = produit commercial avec plan gratuit limité + fonctionnalités payantes (Teams, SSO, Workflows, Analytics...)
- **Cal.diy** = fork communautaire MIT, tout est open source, self-host uniquement, pas de version hébergée officielle

---

## ⚙️ Fonctionnalités principales

- Types d'événements illimités (one-on-one, groupe, round-robin...)
- Connexion calendriers : Google Calendar, Outlook/Office 365
- Vidéo intégrée : Zoom, Daily.co, Google Meet, Teams
- Paiements : Stripe, PayPal
- CRM : HubSpot, Salesforce, Zoho
- Routage de réservations (formulaires, questionnaires)
- API REST v2 complète
- Notifications email et webhooks
- Import Calendly en un clic
- i18n (multilingue)

---

## 🚀 Installation

```bash
# Docker (recommandé)
git clone https://github.com/calcom/cal.diy.git
cd cal.diy
cp .env.example .env
# Générer les secrets obligatoires
openssl rand -base64 32  # → NEXTAUTH_SECRET
openssl rand -base64 24  # → CALENDSO_ENCRYPTION_KEY
docker compose up -d
# Dashboard : http://localhost:3000

# Développement local
yarn dx  # Lance Postgres + app avec comptes de test
```

**Deploy one-click :** Railway, Northflank, Render, Vercel Pro, Elestio.

---

## 📦 Stack technique

- **Framework :** Next.js + tRPC + React
- **BDD :** PostgreSQL (via Prisma)
- **Auth :** NextAuth
- **Styles :** Tailwind CSS
- **Vidéo :** Daily.co
- **Rate limiting :** Unkey (optionnel)

---

## ⚠️ Limites à connaître

- **Self-host uniquement** — pas de version hébergée par Cal.diy (utiliser Cal.com si tu veux du SaaS)
- **Pas de fonctionnalités Teams/Org** — supprimées du fork (utiliser Cal.com Enterprise pour ça)
- **Nécessite PostgreSQL** — pas de SQLite
- **Setup initial technique** — variables d'env, secrets, base de données
- **Vercel** : nécessite le plan Pro (trop de serverless functions pour le plan gratuit)

---

## 📌 Pertinence pour ce projet

**Alternative directe à Calendly** — si tu paies Calendly, Cal.diy permet de s'en affranchir avec les mêmes fonctionnalités de base. Nécessite un hébergement (VPS ~5$/mois ou Railway).

Comparaison vs Calendly :
| Fonctionnalité | Calendly Free | Calendly Teams ($16/seat) | Cal.diy |
|---|---|---|---|
| Types d'événements | 1 | Illimité | Illimité |
| Intégrations calendrier | 1 | Illimité | Illimité |
| Paiements | ❌ | ✅ | ✅ |
| Vidéo intégrée | ❌ | ✅ | ✅ |
| Coût | $0 | $16/seat/mois | $0 + hébergement |

**Tags :** `calendly-alternative` · `scheduling` · `self-hosted` · `nextjs` · `postgresql` · `productivité`
