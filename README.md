# TVA-REFORME BP

Landing + simulateur (quiz) pour qualifier les entreprises françaises à la réforme de la facturation électronique (e-invoicing + e-reporting), et générer des leads :
•⁠  ⁠B2B : vente de leads qualifiés aux PDP (plateformes agréées / plateformes de dématérialisation partenaires)
•⁠  ⁠B2B2C : orientation des entreprises vers une PDP adaptée + mise en conformité (et/ou mise en relation partenaires)

## Contexte réglementaire (France)

Calendrier (généralisation) :
•⁠  ⁠1er septembre 2026 : toutes les entreprises doivent être en capacité de RECEVOIR des factures électroniques
•⁠  ⁠1er septembre 2026 : obligation d’ÉMETTRE au format électronique pour les grandes entreprises et les ETI
•⁠  ⁠1er septembre 2027 : obligation d’ÉMETTRE au format électronique pour les PME, TPE et micro-entreprises

Transmission : recours obligatoire à une plateforme agréée (PDP) pour transmettre/recevoir et pour le e-reporting.

Formats : UBL, CII, ou format mixte (Factur-X : PDF lisible + données structurées).

Sources officielles :
•⁠  ⁠https://www.economie.gouv.fr/tout-savoir-sur-la-facturation-electronique-pour-les-entreprises
•⁠  ⁠https://www.impots.gouv.fr/professionnel/je-decouvre-la-facturation-electronique
•⁠  ⁠https://www.impots.gouv.fr/je-consulte-la-liste-des-plateformes-agreees
•⁠  ⁠https://www.impots.gouv.fr/liste-des-plateformes-agreees-immatriculees

## Objectif business

1) Capturer une intention “mise en conformité 2026/2027” via SEO/SEA.
2) Qualifier rapidement (5 questions max) pour scorer le lead.
3) Router :
•⁠  ⁠soit vers une PDP partenaire (commission / lead vendu)
•⁠  ⁠soit vers un parcours “accompagnement conformité” (B2B2C)
4) Export/API vers CRM + traçabilité RGPD (consentement explicite, finalité, preuve).

## Modèle de monétisation (proposition)

Le pricing dépend du niveau de qualification + exclusivité.

Paliers (indicatifs) :
•⁠  ⁠Bronze : 25–40 € (email + type d’entreprise + secteur + urgence)
•⁠  ⁠Silver : 50–90 € (Bronze + téléphone + SIREN + volumétrie factures + logiciel actuel)
•⁠  ⁠Gold : 100–160 € (Silver + rendez-vous planifié ou besoin validé “chaud”)
•⁠  ⁠Exclusive : x1,5 à x2 (un lead = un seul partenaire)

Notes :
•⁠  ⁠Les CPL B2B observés sur SaaS/IT varient fortement selon canal/qualification ; l’objectif est d’ancrer tes prix sur la valeur “conformité obligatoire + urgence” plutôt que sur un simple formulaire.

## Quiz (MVP, 5 questions)

1.⁠ ⁠Taille : Micro / TPE / PME / ETI-GE
2.⁠ ⁠Secteur : BTP / Santé / Conseil / Commerce / Industrie / Autre
3.⁠ ⁠Volumétrie : 0–10 / 10–50 / 50–200 / 200+
4.⁠ ⁠Outil actuel : Excel / logiciel de facturation / expert-comptable / ERP
5.⁠ ⁠Échéance : urgent / < 3 mois / avant sept 2026 / je ne sais pas

Sortie :
•⁠  ⁠score (froid/tiède/chaud)
•⁠  ⁠recommandation : “type de PDP à privilégier” + CTA (mise en relation)

## Données à collecter (minimum utile)

•⁠  ⁠Nom / Prénom
•⁠  ⁠Email
•⁠  ⁠Téléphone
•⁠  ⁠Entreprise + SIREN
•⁠  ⁠Secteur
•⁠  ⁠Taille
•⁠  ⁠Volumétrie factures/mois
•⁠  ⁠Logiciel actuel
•⁠  ⁠Urgence / échéance

RGPD :
•⁠  ⁠consentement explicite
•⁠  ⁠mention claire : transmission possible à des partenaires PDP
•⁠  ⁠journalisation : date, IP (si pertinent), version de la politique de confidentialité

## Tech (cible)

Frontend :
•⁠  ⁠Next.js (React) + TypeScript
•⁠  ⁠SEO : pages “par secteur” + guides (blog)
•⁠  ⁠Tracking : GA4 + conversion API (si nécessaire)

Backend :
•⁠  ⁠API (Next route handlers ou service séparé)
•⁠  ⁠Stockage : Postgres (Supabase) ou Firestore
•⁠  ⁠Webhooks partenaires PDP (si contrat)

Déploiement :
•⁠  ⁠Recommandé SEO : Vercel
•⁠  ⁠Alternative : Google Cloud Run (container Next.js)
•⁠  ⁠Wix : uniquement si site statique/marketing et quiz embarqué via iframe ou redirection

## Roadmap

MVP (Semaine 1) :
•⁠  ⁠Landing + quiz 5 questions
•⁠  ⁠Formulaire lead + stockage + export CSV
•⁠  ⁠Page “liste PDP officielle” + CTA partenaires

V1 (Semaine 2–3) :
•⁠  ⁠Scoring + routage multi-partenaires
•⁠  ⁠Dashboard leads
•⁠  ⁠Pages SEO (10–30 mots-clés prioritaires)

V2 :
•⁠  ⁠Matching “PDP recommandée” + prise de RDV
•⁠  ⁠Packs leads (abonnements mensuels)
•⁠  ⁠Multi-tenant (plusieurs partenaires, règles par segment)

## Avertissement

Ce projet ne constitue pas un conseil juridique ou fiscal. Toujours vérifier les obligations applicables à l’activité et au statut de l’entreprise.
