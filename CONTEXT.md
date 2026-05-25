# Contexte — Tech Knowledge Base

## Repo GitHub
- Owner : chrisHnt
- Repo : tech-knowledge-base
- URL : https://github.com/chrisHnt/tech-knowledge-base

## Repo sœur (IA)
- Repo : ai-knowledge-base
- URL : https://github.com/chrisHnt/ai-knowledge-base

## Workflow
Quand l'utilisateur partage un lien :
1. Fetcher le contenu de la page
2. Classifier : IA → ai-knowledge-base / Tech → tech-knowledge-base (voir règles ci-dessous)
3. Produire une fiche structurée (voir format ci-dessous)
4. Créer le fichier `fiches/00X-nom.md` dans le bon repo
5. Mettre à jour l'index dans `README.md` du bon repo

## Règles de dispatch automatique

### → ai-knowledge-base
Tout ce qui touche à : LLMs, agents IA, RAG, embeddings, fine-tuning, IA locale, protocoles MCP/A2A, orchestration IA, sécurité IA, frameworks d'agents.

### → tech-knowledge-base
Tout ce qui ne concerne pas l'IA : dev tools, CLI, infra, DevOps, monitoring, data, productivité, utilitaires, sécurité générale, design, scripting.

### Cas ambigus
Si un outil est à cheval (ex. monitoring utilisable aussi pour agents IA), signaler le doute à l'utilisateur et choisir le repo le plus pertinent par défaut.

## Format d'une fiche
- Numéro séquentiel (001, 002…)
- Titre, source, catégorie, langage, licence, date
- Ce que c'est (résumé)
- Fonctionnement
- Pourquoi c'est utile / cas d'usage
- Usage rapide (si applicable)
- Notes personnelles

## Catégories
- Dev Tools
- CLI
- Infra / DevOps
- Productivité
- Sécurité
- Data
- Design
- Utilitaires
