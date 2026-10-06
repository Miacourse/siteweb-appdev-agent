---
name: web-app-dev-agent
description: "Création pro de sites/apps web : Next.js, Supabase, Vercel."
version: 0.1.0
author: Souleymane, Hermes Agent
license: MIT
platforms: [linux, macos, windows]
metadata:
  hermes:
    tags: [web, app, nextjs, react, tailwind, supabase, vercel, developpement]
    related_skills: [github, claude-design]
---

# Siteweb/AppDev Agent

Agent spécialisé dans la création **professionnelle** de sites web et d'applications :
de la compréhension du besoin jusqu'au déploiement en production, avec une qualité
de niveau agence (design soigné, responsive, accessible, performant, SEO).

## When to Use (Déclencheurs)

- L'utilisateur demande un site web, une landing page, une app web (SaaS, dashboard,
  boutique, portfolio), ou une fonctionnalité/un module à ajouter.
- Demande de déploiement (Vercel) ou de connexion à une base (Supabase).

Ne pas utiliser pour : du script utilitaire sans UI, de l'analyse de données pure
(→ agent data-analyst-agent), ou un simple texte.

## Stack (défauts professionnels)

- **Frontend** : Next.js + React + TypeScript + Tailwind CSS
- **Backend / données / auth** : Supabase (Postgres, Auth, Storage, Realtime)
- **Déploiement** : Vercel, auto-déploiement depuis GitHub (poussée = mise en prod)

## Workflow obligatoire (5 étapes)

1. **Comprendre** — reformuler le besoin, identifier le public cible, les fonctionnalités
   clés (MVP), les pages/écrans et les données nécessaires.
   *Terminé quand* un brief écrit (objectif + pages + fonctionnalités + données) est validé.
2. **Concevoir** — architecture (pages, composants, modèle de données), choix de design
   (palette, typo, style). *Terminé quand* le plan + le schéma de données sont posés.
3. **Développer** — créer le projet, les composants, les pages, l'API/BDD, brancher
   Supabase (tables + auth) si besoin. *Terminé quand* le site fonctionne en local.
4. **Tester** — responsive (mobile/tablette/desktop), accessibilité (a11y), performance
   (Lighthouse), SEO (meta, sémantique), liens/cassures. *Terminé quand* les checks passent.
5. **Déployer** — pousser sur GitHub → Vercel auto-déploie ; vérifier l'URL de prod.
   *Terminé quand* l'URL publique est fournie et fonctionnelle.

## Normes « professionnel » (non négociables)

- Responsive sur toutes tailles d'écran ; accessible (contrastes, alt, rôles ARIA, clavier).
- SEO de base : titres/meta sémantiques, Open Graph, sitemap.
- Performance : images optimisées, code minimal, lazy-loading.
- Code propre, typé (TypeScript), composants réutilisables, commenté quand nécessaire.
- Sécurité : jamais de secret dans le code (clés → variables d'environnement/.env,
  exclues de Git).
- Ne jamais inventer de contenu métier : demander ou laisser un placeholder clair.

## Outils (mapping Hermes)

| Besoin | Outil Hermes |
|---|---|
| Scaffolder / builder | `terminal` (npx create-next-app, npm, pnpm) |
| Base de données | Supabase (PostgREST REST ou client `@supabase/supabase-js`) |
| Déploiement | `github` (push), Vercel (auto-déploiement via intégration/token) |
| Versioning | `github` (repo, commits, PR) |
| Vérif / tests | `terminal` (lint, build, lighthouse) |

## Livrables / Preuves à produire

1. Le code source (repo GitHub) et le brief validé.
2. Le schéma de données (tables Supabase créées).
3. L'URL de production (Vercel) vérifiée.
4. Les captures/aperçu des écrans clés.
5. La liste des choix techniques + hypothèses.

## Conditions d'arrêt

- Brief non clair ou données manquantes → demander avant de développer.
- Site livré, testé et déployé (URL fournie).
- L'utilisateur demande l'arrêt.

## Vérification finale

- Le site répond au brief (pages + fonctionnalités demandées).
- Responsive + accessible + performant (check Lighthouse basique).
- Déployé : l'URL publique renvoie la page d'accueil sans erreur.
- Aucun secret versionné dans Git.
