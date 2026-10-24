# BOS — Business Operating System

**Transforme Claude en COO personnel.**

BOS est un système d'exploitation business propulsé par l'IA pour les entrepreneurs. Ouvre ce dossier dans Cursor (ou Claude Code), et obtiens un associé business qui connaît ton business, identifie tes blocages, et te guide vers ton prochain palier — chaque jour.

## Ce que BOS fait

- **Première fois** : BOS te pose des questions pour comprendre ton business, diagnostique ton problème principal, et t'aide immédiatement à passer à l'action.
- **À chaque retour** : reviens et parle. BOS relit sa mémoire (`Core/`), fait le point sur ce qui s'est passé, et propose la tâche au plus grand levier.

## 10 skills spécialisés

| Skill | Ce qu'il fait |
|---|---|
| **Onboard** | Premier setup : profil, diagnostic, premier quick win |
| **Find** | Choisir le bon business / valider / décider de pivoter |
| **Diagnosis** | Trouver LE bottleneck qui bloque tout le reste |
| **Organize** | Structurer le plan d'action (début de semaine, post-diagnostic, quand perdu) |
| **Traffic** | Choisir et mettre en place UN canal d'acquisition |
| **Offer** | Construire une offre irrésistible (Grand Slam Offer) |
| **Funnel** | Diagnostiquer et réparer la conversion |
| **Mindset** | Quand l'entrepreneur EST le blocage (peur, croyances, discipline) |
| **Chase** | Accélérer le revenue (leviers de croissance, pricing, partenariats) |
| **Digestion** | Réparer les opérations (recrutement, process, qualité, rétention) |

Tu n'as jamais besoin d'« activer » un skill. Parle — BOS détecte ce dont tu as besoin et applique le bon spécialiste.

## Installation

### Avec Cursor
1. Clone le repo, puis dans Cursor : **File → Open Folder → `BOS/`** (ouvre bien le dossier `BOS`, pas la racine du repo).
2. Ouvre le chat (Agent mode, modèle Claude recommandé).
3. Écris : **« Salut »**. BOS lance l'onboarding.

Cursor charge automatiquement `.cursor/rules/bos.mdc`, qui renvoie vers `CLAUDE.md`.

### Avec Claude Code
```bash
cd BOS
claude
```
Puis : « Salut ». Claude Code lit `CLAUDE.md` et détecte les skills de `.claude/skills/`.

## Structure

```
BOS/
├── CLAUDE.md              ← Le cerveau (principes, routing, frameworks)
├── AGENTS.md              ← Pointeur pour les autres agents IA
├── .cursor/rules/bos.mdc  ← Règle Cursor (charge CLAUDE.md)
├── Core/                  ← État vivant de TON business (la mémoire de BOS)
│   ├── Profile.md         ← Toi (background, compétences, temps, motivation)
│   ├── Business.md        ← Ton business (offre, clients, métriques, équipe)
│   ├── Goal.md            ← Où tu vas (objectif, timeline, pourquoi)
│   ├── Diagnosis.md       ← Tes problèmes principaux, classés par impact
│   ├── Actions.md         ← Ce qu'il faut faire, priorisé
│   └── Journal.md         ← Log quotidien des avancées
├── Knowledge/             ← Reconnaissance de patterns
│   ├── Common_Problems.md ← 30 problèmes entrepreneurs les plus fréquents
│   └── Business_Principles.md ← Principes business (source de vérité)
├── .claude/skills/        ← 10 skills spécialisés
│   ├── onboard/  find/  diagnosis/  organize/  traffic/
│   └── offer/  funnel/  mindset/  chase/  digestion/
└── Output/                ← Rapports et livrables générés
```

## Personnaliser

- **Ta philosophie business** : édite `Knowledge/Business_Principles.md`. C'est la source de vérité de BOS.
- **Ton style de coaching** : précise-le dans `Core/Profile.md` (« direct », « doux », « chiffres »…) ou modifie la section 7 de `CLAUDE.md`.
- **Nouveau skill** : crée `.claude/skills/<nom>/SKILL.md` (avec un frontmatter `name` / `description`) et ajoute une ligne dans la table de routing de `CLAUDE.md`.

## Confidentialité

Les fichiers `Core/` et `Output/` contiennent les infos de ton business. Si tu forkes ce repo en public, pense à le passer en privé ou à ajouter `Core/` et `Output/` dans un `.gitignore`.

## Pour qui

- Entrepreneurs qui veulent lancer mais ne savent pas par où commencer
- Petits business (0–10 k€/mois) qui veulent grandir
- Fondateurs solo qui ont besoin d'un associé de réflexion, pas d'une énième formation
