# 🚀 Phase 0 – Préparation (30/07/2025)
## Objectifs :

Poser les bases de ton projet SR13

Tirer profit de ton rendez-vous « identité visuelle » dimanche

## Actions :

Brief identité

Prépare un moodboard (couleurs, typographies, exemples de sites)

Note tes valeurs clés (fiabilité, simplicité, automatisation…)

## Vision & cibles

Définis les personas (micro-entrepreneurs, TPE de 1–10 pers…)

Liste leurs « pains » prioritaires : facturation, gestion docs, CRM minimal

Backlog initial

Crée un dépôt Git (sr13/roadmap.md) et commence à y rédiger ces éléments

Planning sportif & pro

Bloque 2×45 min de créa (soirée) + 3×30 min de sport cette semaine

# 📐 Phase 1 – Affinage fonctionnel & maquettage (7/07/2025)
## Objectifs :

Transformer ta vision en périmètre de MVP

Valider l’expérience utilisateur avant le code

## Actions :

Atelier de cadrage (2 h)

Revue backlog, priorisation MoSCoW (Must/Should/Could)

User flows

## Schématise le parcours :

Visiteur arrive sur / (portfolio) → découvre le service → /services

S’inscrire/Se connecter → /api/auth → tableau de bord

Wireframes basse fidélité

Outils : Figma ou Balsamiq

## Pages clés :

Vitrine SR13 (home, à propos, contact)

Dashboard automatisation (upload doc, config script, exécution)

Revues & itérations

Implique ton ami du RDV dimanche pour feedback

Ajuste ton backlog après chaque session

# 💻 Phase 2 – Mise en place technique & prototype (14/07/2025)
## Objectifs :

Structurer le monorepo et l’infra

Avoir un premier prototype « réel » en multi-conteneurs

## Actions :

Monorepo & Docker-Compose

Crée repos sr13/monorepo avec 3 dossiers : vitrine/, services-frontend/, services-backend/

Écris des Dockerfile simples et un docker-compose.yml

Reverse-proxy host + tunnel Cloudflare

Réutilise ta conf Nginx + Cloudflared, oriente / → vitrine, /services → frontend, /api → backend

CI/CD minimal

Ajoute un workflow GitHub Action pour builder & déployer sur ton VPS à chaque push sur main

Prototype fonctionnel

Déploie en staging : home + route /services qui affiche « Coming soon »

# 🛠 Phase 3 – MVP Automatisation & Auth (21/07/2025-21/08/2025)
Objectifs :

Lancer le service d’automatisation basique

Mettre en place l’authentification

## Actions :

Backend FastAPI

Implémente /auth (JWT), /automation (CRUD)

Connecte PostgreSQL (multi-tenant simple : schema par client)

Frontend React

Formulaire job d’automatisation (upload PDF/excel, choix du script)

Affichage liste des jobs + logs

Tests end-to-end

Écris quelques tests Cypress ou Playwright

Itération sur UX/UI

Propose un thème léger (ton identité visuelle appliquée)

Ajoute un système de quota / facturation basique

# 🚀 Phase 4 – Go-to-Market & croissance (Septembre 2025)
## Objectifs :

Attirer les premiers clients TPE/PME

Automatiser la facturation & la relance

## Actions :

Studio de contenu

Rédige 1 article tuto “Comment automatiser l’export de facture”

Partage sur LinkedIn XEFI & groupes pro

Intégration IA

Ajoute un assistant Slack/Teams pour déclencher vos scripts via message

Prototype avec LLM (OpenAI) pour extraction de données de docs

Automatisation facturation

Générez PDF+envois emails automatisés

Intégrez un module de paiement (Stripe, etc.)

Suivi KPI et itérations

Mettez en place des dashboards (GA4, Metabase)

Revoyez le backlog chaque sprint (2 semaines)

# 🌟 Conseils pour tenir la cadence
Sport : 3 séances courtes (20 min) par semaine, plutôt le matin.

## XEFI : bloque 1 h « Deep Work » pour SR13 le midi, 2×45 min le soir.

## Week-ends : 2 h de prototypage/fix bug, 1 h de lecture veille IA/RPA.

## Revue hebdo : chaque vendredi, 30 min de bilan + ajustement roadmap.
