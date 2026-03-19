---
name: hormur-seo
description: >
  Expert en SEO, GEO (Generative Engine Optimization) et référencement pour Hormur.
  Utiliser cette skill pour TOUTE question liée au SEO de Hormur : création ou amélioration
  de pages de référencement, analyse de mots-clés, optimisation pour les moteurs de recherche
  et les IA génératives, stratégie de contenu, pages par ville/occasion/genre, maillage interne,
  schema markup, et toute optimisation de visibilité en ligne. Activer aussi quand l'utilisateur
  mentionne : SEO, GEO, référencement, mots-clés, Google, pages de redirection, landing pages,
  sitemap, backlinks, ou positionnement web pour Hormur.
---

# Hormur SEO & GEO - Guide Expert

## Architecture du site SEO Hormur

### Structure des pages (explore.hormur.com)
Le site SEO de Hormur est hébergé sur Netlify et déployé depuis le repo GitHub `MartinJeudy/hormur-seo-pages`.

**Hiérarchie des pages :**
- **Pages piliers** (priorité maximale) : spectacle-a-domicile, concert-prive-a-domicile, sortir-a-paris
- **Pages villes** : sortir-a-[ville] pour Paris, Lyon, Bordeaux, Nantes, Marseille, Toulouse, Lille
- **Pages occasions** : reserver-artiste-anniversaire, artiste-pour-mariage, animation-soiree-entreprise, offrir-concert-prive, spectacle-enfant-a-domicile, spectacle-a-domicile-anniversaire
- **Pages genres/artistes** : concert-jazz-prive, dj-soiree-privee, pianiste-pour-soiree, magicien-a-domicile
- **Pages informationnelles** : combien-coute-concert-prive
- **Pages hôtes** : organiser-concert-chez-soi, accueillir-artiste-chez-soi, devenir-hote-concert-prive
- **Pages artistes** : artiste-cherche-lieu-pour-jouer, trouver-artiste-evenement
- **Blog** : articles informationnels longs

### Stack technique
- HTML statique + CSS partagé (shared-styles.css)
- Charte graphique : corail #EE6553, navy #323242, Noto Sans (body), EB Garamond (headings)
- Schema.org : WebPage, FAQPage, BreadcrumbList, Service, Article
- Netlify hosting avec _redirects et netlify.toml
- Sitemap XML + robots.txt + llms.txt (pour GEO)

## Stratégie SEO

### Mots-clés prioritaires (208 identifiés)
- **Priorité 5 (critique)** : "concert privé à domicile", "spectacle à domicile", "sortir à paris", "concert intime paris", "spectacle chez l'habitant", etc.
- **Priorité 4 (haute)** : "spectacle à domicile clown", "artiste pour mariage", "lieu atypique événement paris", etc.
- **Priorité 3 (moyenne)** : pages villes secondaires, genres musicaux, types d'artistes
- **Priorité 2-1** : longue traîne, combinaisons ville × genre

### Audiences cibles
1. **Spectateurs** (160 mots-clés) : personnes cherchant des spectacles, concerts, sorties
2. **Hôtes** (25 mots-clés) : personnes voulant accueillir des artistes chez eux
3. **Artistes** (23 mots-clés) : artistes cherchant des lieux et des dates

### Concurrents SEO principaux
- **Linkaband** : 46.9K mots-clés, 122K trafic. Pages par ville + genre. Blog SEO fort. 30K artistes.
- **LiveTonight** : Pages locales automatisées, contenu par genre + ville
- **Eventbrite** : URLs paramétriques catégorie × ville × période
- **Fever** : Contenu éditorial fort, SEO par expérience

### Différenciation Hormur
Aucun concurrent ne se positionne directement sur "concerts chez l'habitant" / "art hors les murs". C'est le positionnement unique de Hormur. Les pages doivent capitaliser sur cette singularité.

## Template de page SEO

### Structure obligatoire
1. `<head>` : meta title (< 60 car), meta description (< 160 car, avec data point), canonical, OG, Twitter, schemas (WebPage + FAQPage + BreadcrumbList + Service si pertinent)
2. Header avec navigation Hormur
3. Breadcrumbs
4. Hero : H1 avec mot-clé principal + paragraphe d'introduction + barre de recherche
5. Trust badges (artistes vérifiés, événements organisés, satisfaction, réservation)
6. Cards grid : 6 cartes avec liens vers la plateforme
7. **Guide section** (NOUVEAU - essentiel) : 400-500 mots de contenu éditorial riche avec h2/h3, tableau comparatif, info-box, témoignage
8. Comment ça marche (3 étapes)
9. FAQ (5-7 questions, réponses de 3-4 phrases, schéma FAQPage)
10. Recherches associées (tags maillage interne)
11. CTA banner
12. Newsletter
13. Footer complet

### Règles de rédaction
- Écrire naturellement, comme un journaliste culture, PAS comme une IA
- Phrases variées (courtes + longues), questions rhétoriques, détails spécifiques
- Données chiffrées et statistiques dans les 200 premiers mots
- Tableaux comparatifs avec la classe CSS "comparison-table"
- Info-boxes avec la classe CSS "info-box"
- Témoignages réalistes avec la classe CSS "testimonial"
- FAQ détaillées (3-4 phrases par réponse)

## Stratégie GEO (Generative Engine Optimization)

### Principes pour être cité par les IA
1. **Densité factuelle** : chiffres, statistiques, prix dans les 200 premiers mots
2. **Réponse directe** : la première phrase doit répondre à la query
3. **Structure parsable** : schema.org, tableaux, listes numérotées
4. **Freshness** : date de mise à jour visible, contenu actualisé régulièrement
5. **Autorité** : citations, témoignages, données exclusives Hormur
6. **llms.txt** : fichier à la racine du site pour guider les crawlers IA

### Fichier llms.txt
Maintenu à la racine du site, résume l'offre Hormur, les services, les prix, la couverture géographique et la liste des pages. Doit être mis à jour à chaque ajout de page.

### Robots.txt
Autoriser explicitement GPTBot, ClaudeBot, PerplexityBot, Google-Extended.

## Métriques actuelles (mars 2026)

### Google Search Console (90 jours)
- 5 750 clics | 126 000 impressions | CTR 4.6% | Position moyenne 8.2
- Trafic SEO = 23% du trafic total (objectif : 40%)

### Matomo (février 2026)
- Entrées directes : 585 (46%)
- Moteurs de recherche : 292 (23%)
- Email : 199 (16%)
- Référents : 144 (11%)
- Réseaux sociaux : 42 (3%)

### Objectifs
| Métrique | Actuel | 3 mois | 6 mois |
|---|---|---|---|
| Visites SEO/mois | ~900 | 2 000 | 5 000 |
| Impressions/mois | ~42 000 | 80 000 | 150 000 |
| CTR moyen | 4.6% | 6% | 8% |
| Position moyenne | 8.2 | 6 | 4 |
| Pages indexées | ~50 | 80 | 150 |

## Prochaines actions recommandées

### Court terme
- Créer des pages pour les villes secondaires (Strasbourg, Montpellier, Nice, Rennes)
- Ajouter des pages spectacle-a-domicile-[ville] (Lyon, Bordeaux, Nantes, Marseille)
- Créer des pages concert-intime-[ville] pour chaque grande ville
- Enrichir les articles de blog existants avec du contenu GEO-optimisé

### Moyen terme
- Créer une matrice ville × genre (concert-jazz-lyon, pianiste-soiree-paris, etc.)
- Ajouter des pages saisonnières (spectacle-noel-a-domicile, concert-saint-valentin)
- Développer les pages B2B (team-building-musical, spectacle-comite-entreprise)
- Obtenir des backlinks de blogs culturels et presse locale

### Long terme
- Automatiser la création de pages par ville × genre × occasion
- SEA complémentaire sur les top 10 mots-clés transactionnels
- Monitoring GEO multi-plateforme (ChatGPT, Perplexity, Google AI Overviews)
