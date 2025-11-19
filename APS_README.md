# APS – Système d’Assistant Personnel Stratégique

Ce dépôt définit un **système APS** (Assistant Personnel Stratégique) structuré autour de :

- **Chatmodes** : modes de fonctionnement et de conversation de l’APS.
- **Prompts** : bibliothèques de prompts réutilisables pour activer l’APS et les personas associés.
- **Teams** : organisation en "équipe" de personas (APS, DGD, CPO, CTO, etc.).

L’objectif est de rendre tes interactions avec l’IA **cohérentes**, **réutilisables** et **actionnables**, sans sur‑complexifier.

---

## 1. Vue d’ensemble

- Les **chatmodes** définissent *comment* l’APS travaille dans une session donnée (style, format, workflow).
- Les **prompts** sont des blocs prêts à copier/coller pour lancer une tâche précise (clarifier, décider, cadrer un projet, etc.).
- Les **teams** expliquent comment tous les personas s’organisent et collaborent.

Tu peux utiliser ces éléments séparément ou ensemble :

1. Choisir un **chatmode APS** adapté à ta demande.
2. Compléter avec un ou plusieurs **prompts** issus de la bibliothèque.
3. T’appuyer sur la **team** pour planter le décor global (personas, hiérarchie, logiques de décision).

---

## 2. Fichiers principaux

### 2.1 Chatmodes APS / DGD

- Fichier : `chatmodes/chatmodes_APS_DGD.md`
- Contenu : une série de **chatmodes** (APS_STANDARD, DGD_PLAN_ACTION, DÉCISION_STRATÉGIQUE, etc.).
- Usage typique :
  - tu choisis un mode en fonction du besoin (clarifier, décider, planifier, focus, etc.),
  - tu colles la section correspondante comme **prompt système** / "mode" dans ton outil préféré (ChatGPT, Mammouth AI, VS Code, etc.).

### 2.2 Bibliothèque de prompts APS / DGD

- Fichier : `prompts/prompts_APS_FPO.md`
- Contenu : des **prompts structurés** (RÔLE / TÂCHE / ENTRÉE / SORTIE ATTENDUE) alignés avec les chatmodes et les personas.
- Usage typique :
  - tu copies le bloc adapté,
  - tu remplaces les `{{...}}` par ton contexte,
  - tu peux en faire des *snippets* dans VS Code ou des favoris dans ChatGPT / Mammouth.

### 2.3 Système de personas & team

- Fichier : `teams/basic_team.md`
  - Contient la description détaillée de tous les **personas** (APS, DGD, CPO, CTO, etc.), leur mission, compétences, livrables.
- Fichier : `teams/APS_team.md`
  - Décrit une **équipe APS** simplifiée pour ton usage courant (Designer / Coder / Reviewer / Stratégie, etc.).
  - S’appuie sur les personas de `basic_team.md` mais en version plus opérationnelle.

---

## 3. Comment démarrer une session APS

### 3.1 Cas simple – une seule question

1. Ouvrir `chatmodes/chatmodes_APS_DGD.md`.
2. Choisir le chatmode le plus proche de ton besoin, par exemple :
   - **APS_STANDARD** : clarifier et structurer une demande floue.
   - **DGD_PLAN_ACTION** : transformer une envie / idée en plan d’action.
   - **DÉCISION_STRATÉGIQUE** : trancher entre plusieurs options.
3. Copier la section du chatmode et la coller comme **prompt système** dans ton outil.
4. Poser ta question en langage naturel.

### 3.2 Cas plus avancé – projet avec plusieurs étapes

1. Dans `teams/APS_team.md`, choisir la **configuration d’équipe** qui te correspond.
2. Lancer une première phase avec un mode "Designer" (clarifier / cadrer) :
   - chatmode type **APS_STANDARD** ou **ATELIER_PRODUIT_MVP**.
3. Utiliser les prompts de `prompts/prompts_APS_FPO.md` pour :
   - cadrer un projet,
   - construire un MVP,
   - préparer une revue hebdo / mensuelle,
   - analyser une opportunité business, etc.
4. Pour la phase exécution / code, garder les instructions en **anglais** pour le code et les commentaires, mais continuer à utiliser les chatmodes / prompts en **français** pour tout ce qui est interaction et doc.

---

## 4. Conventions d’écriture

- **Langue** :
  - Interactions, descriptions, docs, prompts : **français**.
  - Code, noms de fonctions, commentaires dans le code : **anglais**.
- **Structure des prompts** :
  - `[RÔLE]`, `[TÂCHE]`, `[ENTRÉE]`, `[SORTIE ATTENDUE]` quand pertinent.
  - Utiliser `{{ACCOLADES}}` pour les éléments à remplir.
- **Style** :
  - Ton pro, direct, bienveillant.
  - Pas de blabla inutile, mais suffisamment de contexte pour être actionnable.

---

## 5. Ajouter / modifier des éléments APS

### 5.1 Ajouter un nouveau chatmode

1. Aller dans `chatmodes/chatmodes_APS_DGD.md`.
2. Copier un bloc existant (CHATMODE X – NOM) comme modèle.
3. Lui donner :
   - un **nom clair** (ex : `FOCUS_SESSION`, `MODE_COMPLIANCE`, etc.),
   - un **objectif** net,
   - une **manière de travailler** en 4–6 étapes,
   - un **style** et un **format** de sortie explicites.

### 5.2 Ajouter un nouveau prompt

1. Aller dans `prompts/prompts_APS_FPO.md`.
2. Créer une nouvelle section dans la bonne catégorie (organisation, stratégie, produit, etc.).
3. Suivre le pattern `[RÔLE] / [TÂCHE] / [ENTRÉE] / [SORTIE ATTENDUE]`.

### 5.3 Étendre la team APS

1. Partir de `teams/basic_team.md` pour comprendre les personas existants.
2. Dans `teams/APS_team.md`, ajouter un rôle APS supplémentaire si besoin (par ex. **APS_Research**, **APS_Tester**).
3. Définir pour chaque rôle : mission, responsabilités, mode de collaboration.

---

## 6. Liens utiles

- `chatmodes/chatmodes_APS_DGD.md` – Catalogue de chatmodes APS / DGD.
- `prompts/prompts_APS_FPO.md` – Bibliothèque de prompts APS / DGD.
- `teams/basic_team.md` – Système complet de personas.
- `teams/APS_team.md` – Configuration d’équipe APS opérationnelle.
