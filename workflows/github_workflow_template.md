# 📁 github_workflow_template.md

**Workflow GitHub avancé – APS OS 2025**
Version 1.0 – Yann (Founder)

---

# 0. Objectif du fichier

Ce fichier définit :

* La structure de travail GitHub
* Les branches officielles
* La politique de commit & PR
* Le workflow complet (idée → merge)
* Le rôle des personas (APS, PMO, etc.) dans la boucle Git
* Les labels, checklists, templates
* L’automatisation CI/CD optionnelle
* Les conventions d’organisation des fichiers

Compatible avec :

* GitHub (cloud ou self-hosted)
* GitLab CE
* Repos single-project ou multi-project
* Systèmes IA (APS OS)

---

# 1. Structure du dépôt

Ton repo doit suivre une structure simple, scalable, claire :

```
/
├── docs/
│   ├── team_aps_optimised.md
│   ├── chatmodes_entreprise_projets.md
│   ├── instructions_ia_engineering_advanced.md
│   └── entrepreneur_prompt_library.md
│
├── src/                → code source (microdrone, API, scripts…)
│
├── hardware/           → schémas, BOM, plans, DXF, composants
│
├── workflows/          → automatisations CI/CD (YAML)
│
├── projects/           → un dossier par projet high-tech
│   ├── roomshield/
│   ├── fmdrone/
│   ├── detecteur/
│   └── voxpopuli/
│
├── roadmap/            → feuilles de route 30/90 jours
│
├── decisions/          → décisions structurantes (ADR) (format Markdown)
│
└── README.md
```

---

# 2. Branches officielles

Utiliser un **GitFlow simplifié**, idéal pour projets personnels ou équipes réduites :

```
main      → stable, production-ready
develop   → intégration des features avant merge final
feature/* → développement d’une fonctionnalité ou d'un module
bugfix/*  → corrections
experiment/* → prototypes IA, tests
docs/*    → documentation
```

### Règles essentielles

* **main** : toujours stable
* **develop** : merge toutes les PR avant passage en main
* Jamais commit direct sur `main`
* Une feature = une branche

---

# 3. Conventions de commit

Format **Conventional Commits** :

```
feat: nouvelle fonctionnalité
fix: correction d’un bug
docs: documentation / fichiers APS
style: mise en forme, pas de logique
refactor: modification interne sans changement de comportement
perf: optimisation
test: ajout/modif de tests
chore: maintenance
ci: actions CI/CD
```

### Exemples

```
feat(drone-control): add PID stabilization module
docs(aps): update chatmodes for tech launch
fix(sensor): correct microcamera detection threshold
```

---

# 4. Pull Requests (PR)

## 4.1. Règles générales

* 1 PR = 1 objectif clair
* PR **courte**, **lisible**, **autonome**
* Titre clair
* Checklist obligatoire
* Un reviewer IA (APS → Reviewer Persona)
* Merge via squash recommandé

---

## 4.2. Template pour PR (à mettre dans `.github/pull_request_template.md`)

```
# 🎯 Objectif de la PR
(But clair et concis)

# 📄 Contexte
(Pourquoi c’est nécessaire)

# 🔧 Modifications
- …
- …
- …

# 🧪 Tests
- Testés localement ? Oui / Non
- CI valide ? Oui / Non

# 📊 Impact
- Produit :
- Tech :
- Business :
- Risques :

# 🤖 Interventions personas
- APS a clarifié ? Oui/Non
- Ton Second a validé ? Oui/Non
- Architecte IA a revu ? Oui/Non
- PMO a intégré dans roadmap ? Oui/Non

# ✔️ Checklist
- [ ] Code propre
- [ ] Pas de dette technique inutile
- [ ] Documentation mise à jour
- [ ] Tests inclus ou mis à jour
- [ ] Branch prête à merger
```

---

# 5. Workflow complet (vision APS OS)

Voici la **boucle Git** adaptée à tes personas :

```
1. IDÉE → APS (clarification)
2. Cadrage technique → Architecte IA + CTO
3. MVP & Product → CPO
4. Tâches → PMO (roadmap / backlog)
5. Dev → feature/*
6. PR → APS + Reviewer
7. Merge → develop
8. Release → main
9. Post-mortem / feedback → APS
```

### Résultat :

Un pipeline **fluide**, **clair**, **sans friction cognitive**.

---

# 6. Labels GitHub

Créer des labels pour piloter tes projets high-tech et ton OS APS :

### Statut

* `status: todo`
* `status: in-progress`
* `status: review`
* `status: blocked`
* `status: done`

### Type de travail

* `type: feature`
* `type: bugfix`
* `type: docs`
* `type: design`
* `type: hardware`
* `type: analysis`
* `type: tech-architecture`
* `type: product`

### Priorité

* `prio: high`
* `prio: medium`
* `prio: low`

### Personas

* `persona: aps`
* `persona: second`
* `persona: architect-ia`
* `persona: cpo`
* `persona: cto`
* `persona: pmo`
* `persona: reviewer`

---

# 7. Issues – Structure officielle

Mettre ce template dans `.github/ISSUE_TEMPLATE/feature_request.md` :

```
# 🎯 Objectif
Décris ce que tu veux faire.

# 🤖 Personas nécessaires
(APS, Architecte IA, CTO, PMO…)

# 📄 Contexte
Pourquoi est-ce important ?

# 🧩 Solution proposée
(Esquisse ou intention)

# 🔧 Étapes
- [ ] Étape 1
- [ ] Étape 2
- [ ] Étape 3

# ⚠️ Risques
- …

# 📅 Délais / Deadline
…
```

---

# 8. Sync avec APS OS (Très important)

Lorsqu’un projet est lancé, ajouter dans chaque issue :

```
APS: Clarification OK  
Ton Second: Arbitrage OK  
Architecte IA: Cohérence OK  
PMO: Plannification OK  
Reviewer: Validé
```

Ce système suit le pipeline IA.

---

# 9. Roadmap & Milestones

Dans GitHub → Projects
Créer une roadmap “90 jours” :

* S1–S2 : Cadrage
* S3–S4 : MVP
* S5–S8 : Dev / tests
* S9–S10 : Release
* S11–S12 : Iterations + OS update

PMO met à jour chaque vendredi.

---

# 10. CI/CD (optionnel)

Créer un fichier `.github/workflows/ci.yml` :

```
name: CI
on:
  push:
    branches: [develop, main]
  pull_request:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Setup .NET
        uses: actions/setup-dotnet@v4
      - run: dotnet build

  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Run tests
        run: dotnet test --no-build --verbosity normal
```

---

# 11. Revue post-merge (optional but recommended)

Chaque semaine :

* APS → synthèse
* Ton Second → arbitrages
* PMO → blocages / next steps
* CTO → dette technique
* CPO → feedback produit
* Architecte IA → cohérence multi-agents

---

# 12. Résumé exécutif

Ce template fournit :

* Structure Git complète
* Branches officielles
* PR template
* Issue templates
* Labels optimisés
* Pipeline APS → Git
* CI/CD minimaliste
* Roadmap intégrée

Il transforme GitHub en une **extension naturelle** de ton OS cognitif APS.
