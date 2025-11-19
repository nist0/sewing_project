# 📁 adr_template.md

**Architecture Decision Record Template – APS OS 2025**
Version : 1.0 — Yann (Founder)

---

# 0. Identification

**ADR N° :**
**Titre :**
**Date :**
**Projet :** *(RoomShield, FMdrone, détecteur, API, VoxPopuli…)*
**Rédacteur :** *(APS / Architecte IA / CTO / Toi)*
**Personas impliqués :** APS, Ton Second, Architecte IA, CPO, CTO, PMO, Juriste, Sécurité

---

# 1. Contexte

Décris ici la situation, le problème ou la décision à prendre.

* Que se passe-t-il ?
* Pourquoi cette décision ?
* Quelles contraintes ?
* Quel historique ?
* Quel risque si pas de décision ?

---

# 2. Problème à résoudre

Formule le problème de manière simple, précise et opérationnelle.

> **Le problème :**
> Ce que nous devons décider, pour éviter X et permettre Y.

---

# 3. Forces en présence (analyse)

Liste les facteurs qui influencent la décision.

### 3.1 Contraintes techniques

* …

### 3.2 Contraintes business

* …

### 3.3 Contraintes légales / conformité

* …

### 3.4 Contraintes ressources / temps

* …

### 3.5 Opportunités

* …

---

# 4. Options envisagées

Décrire 2 à 4 options réalistes.

### Option A —

**Résumé** :
**Avantages :**
---------------

## **Inconvénients :**

## **Risques :**

---

### Option B —

**Résumé** :
**Avantages :**
---------------

## **Inconvénients :**

## **Risques :**

---

### Option C —

*(option ambitieuse ou moonshot)*
**Résumé :**
**Avantages :**
---------------

## **Inconvénients :**

## **Risques :**

---

# 5. Analyse comparative

| Critère           | Option A | Option B | Option C |
| ----------------- | -------- | -------- | -------- |
| Impact            |          |          |          |
| Effort            |          |          |          |
| Risque            |          |          |          |
| Coût              |          |          |          |
| Délais            |          |          |          |
| Scalabilité       |          |          |          |
| Alignement vision |          |          |          |

---

# 6. Recommandation

> **Option recommandée :** A / B / C
> **Justification claire et concise :**

* Pourquoi cette option ?
* Quels risques sont acceptables ?
* Qu’est-ce qui a été priorisé ? (impact ? simplicité ? rapidité ?)

---

# 7. Conséquences

Décrire ce que cette décision implique :

### 7.1 Conséquences positives

*

### 7.2 Conséquences négatives / risques

*

### 7.3 Dette technique / dette organisationnelle

*

---

# 8. Plan d’action (PMO)

Plan clair et opérationnel pour mettre en œuvre la décision :

* Étape 1
* Étape 2
* Étape 3
* Étape 4

Inclure :

* Contraintes
* Deadlines
* Personas responsables

---

# 9. Impact sur la documentation

Mettre à jour :

* `/docs/*`
* `/projects/<project>/blueprint.md`
* MVP
* Architecture technique
* Roadmap 90 jours
* Legal / RGPD (si applicable)
* README des modules impactés

---

# 10. Validation

### 10.1 Review personas

| Persona       | Review | Validation |
| ------------- | ------ | ---------- |
| APS           | ☐      | ☐          |
| Ton Second    | ☐      | ☐          |
| Architecte IA | ☐      | ☐          |
| CTO           | ☐      | ☐          |
| CPO           | ☐      | ☐          |
| PMO           | ☐      | ☐          |
| Sécurité      | ☐      | ☐          |
| Juriste       | ☐      | ☐          |
| Reviewer      | ☐      | ☐          |

---

# 11. Versioning et statut

**Statut :**

* 🟢 Accepté
* 🟡 Proposé
* 🔴 Rejeté
* 🔵 Supersédé par ADR-XXX

**Lien vers ADR suivant :**
**Lien vers ADR précédent :**

---

# 12. Résumé exécutif (APS)

> **En 6–10 lignes — synthèse de la décision, raison, impacts, prochaines étapes.**

---

# 13. Notes complémentaires

* Cet ADR doit être ajouté dans `/decisions/adr-XXX-title.md`.
* Un ADR = une seule décision structurante.
* Toute évolution majeure doit créer un **nouvel ADR**, jamais remplacer un ancien.
* APS et Ton Second sont responsables du maintien de cohérence.
