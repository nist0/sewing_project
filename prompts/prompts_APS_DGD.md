# 📚 Bibliothèque de prompts – APS / DGD

Fichier à utiliser comme **base de prompts de travail** dans :

- ChatGPT
- Mammouth AI
- VS Code / GitHub (commentaires, notes, etc.)

Tu as déjà défini tes personas (APS, DGD, CPO, CTO, etc.) :  
ces prompts servent à **les appeler / les utiliser facilement**.

Les sections ci-dessous sont organisées par type d’usage :

- **Section 1 : Prompts génériques APS / DGD** (clarifier, planifier, prioriser…).
- **Section 2 : Organisation personnelle & revue**.
- **Section 3 : Stratégie & business**.
- **Section 4 : Produit & tech**.
- **Section 5 : Communication & écrits**.
- **Section 6 : Prompts pour GitHub Copilot / code**.

Pour une vue d’ensemble plus large, voir aussi :

- `APS_README.md` – Vue globale du système APS.
- `chatmodes/chatmodes_APS_DGD.md` – Chatmodes associés.

---

## 0. Comment utiliser cette bibliothèque

- Copier/coller le bloc de prompt dont tu as besoin.
- Remplacer les `{{...}}` par ton contexte.
- Tu peux aussi créer des *snippets* dans VS Code ou des favoris dans ChatGPT / Mammouth.

Notation :

- `[RÔLE]` : quel persona tu veux activer.
- `[TÂCHE]` : ce que tu lui demandes précisément.
- `[ENTRÉE]` : ce que tu lui fournis.
- `[SORTIE ATTENDUE]` : forme du résultat que tu veux.

---

## 1. Prompts génériques APS / DGD

## 1.1 Clarifier & structurer une demande (APS)

[RÔLE]  
Tu es mon APS (Assistant Personnel Stratégique).

[TÂCHE]  
Clarifier et structurer ma demande pour qu’elle soit exploitable par mes autres personas (DGD, CPO, CTO, etc.).

[ENTRÉE]  
« {{COLLER ICI MA DEMANDE BRUTE}} »

[SORTIE ATTENDUE]  

1) Résumé de ma demande en 3 phrases max.  
2) Objectifs explicites (liste).  
3) Ambiguïtés / points à clarifier.  
4) Personas / pôles à impliquer (ordre de priorité).  
5) Brief prêt-à-envoyer à mon DGD.

---

## 1.2 Transformer en plan d’action (DGD)

[RÔLE]  
Tu es mon DGD / Chief of Staff.

[TÂCHE]  
Transformer la demande suivante en plan d’action opérationnel.

[ENTRÉE]  
« {{DESCRIPTION DE CE QUE JE VEUX OBTENIR / DU PROBLÈME / DU PROJET}} »

[SORTIE ATTENDUE]  

1) Résumé de la situation.  
2) Objectif principal + 2–3 objectifs secondaires.  
3) Plan en étapes (3–7 actions) avec : Qui / Quoi / Quand (priorité).  
4) Risques / points de vigilance.  
5) Messages prêts-à-coller pour les personas concernés.

---

## 1.3 Prioriser une liste de tâches / projets (APS)

[RÔLE]  
Tu es mon APS.

[TÂCHE]  
Prioriser ma liste pour éviter la dispersion et maximiser l’impact.

[ENTRÉE]  
Liste brute :  

- {{tâche / projet 1}}  
- {{tâche / projet 2}}  
- {{tâche / projet 3}}  
- …

[SORTIE ATTENDUE]  

1) Regroupement par thème / projet.  
2) Classement en :  
   - Crucial (à faire maintenant),  
   - Important (à planifier),  
   - À déléguer / à abandonner.  
3) Propositions de délégation (personas / rôles).  
4) Plan simple pour les 3 prochains jours (3–5 actions max).

---

## 1.4 Choisir entre plusieurs options (APS + DGD)

[RÔLE]  
Tu es mon APS, et tu convoques DGD + personas utiles (Stratégie, Finance, Legal…).

[TÂCHE]  
M’aider à choisir entre plusieurs options.

[ENTRÉE]  
Contexte :  
« {{DESCRIPTION DE LA SITUATION}} »

Options :  

- Option A : {{décrire}}  
- Option B : {{décrire}}  
- Option C : {{décrire}} (facultatif)

[SORTIE ATTENDUE]  

1) Résumé neutre du problème.  
2) Avantages / inconvénients majeurs de chaque option.  
3) Principaux risques par option.  
4) Recommandation (option préférée) + justification long terme.  
5) 2–3 questions que je dois me poser avant de trancher.

---

## 1.5 Transformer du vrac en document exploitable (APS)

[RÔLE]  
Tu es mon APS.

[TÂCHE]  
Transformer des notes en vrac en document structuré exploitable.

[ENTRÉE]  
« {{COLLER ICI MES NOTES EN VRAC}} »

[SORTIE ATTENDUE]  

1) Résumé exécutif en 5–10 lignes.  
2) Plan du document (titres / sous-titres).  
3) Version structurée en sections (avec listes si utile).  
4) Liste de décisions à prendre / actions à lancer.  
5) Suggestions de compléments d’information manquants.

---

## 2. Organisation personnelle & revue

## 2.1 Revue hebdo express (APS)

[RÔLE]  
Tu es mon APS.

[TÂCHE]  
Faire une revue hebdomadaire pour :  

- voir les progrès,  
- identifier les blocages,  
- préparer la semaine suivante.

[ENTRÉE]  
Bilan brut de la semaine :  
« {{NOTES, ÉVÉNEMENTS, PROJETS, RESSENTIS}} »

[SORTIE ATTENDUE]  

1) Bilan synthétique (faits marquants).  
2) Réussites / progrès.  
3) Blocages / problèmes récurrents.  
4) Axes d’amélioration.  
5) 3–5 priorités claires pour la semaine prochaine.

---

## 2.2 Revue mensuelle / trimestrielle (APS + DGD)

[RÔLE]  
Tu es mon APS et tu convoques mon DGD.

[TÂCHE]  
Faire une revue {{mensuelle / trimestrielle}} centrée sur :  

- ce qui a avancé,  
- ce qui bloque,  
- où va mon temps / énergie,  
- les décisions structurantes à prendre.

[ENTRÉE]  
« {{NOTES, CALENDRIER, PROJETS, INTUITIONS, CHIFFRES SI TU EN AS}} »

[SORTIE ATTENDUE]  

1) Synthèse globale (vision “photo” de la période).  
2) Faits marquants positifs / négatifs.  
3) Décisions prises et impacts.  
4) Points de friction / désalignement potentiels.  
5) 3–5 décisions structurantes à prendre pour la prochaine période.  
6) Plan macro pour la prochaine période (3–7 axes).

---

## 2.3 Cadrer un nouveau projet (APS + DGD)

[RÔLE]  
Tu es mon APS et tu travailles avec mon DGD.

[TÂCHE]  
Cadrer un projet de façon actionnable.

[ENTRÉE]  
« {{DESCRIPTION RAPIDE DU PROJET / CONTEXTE / POURQUOI}} »

[SORTIE ATTENDUE]  

1) Reformulation du projet en termes simples.  
2) Objectifs (Business, Produit, Organisation).  
3) Scope : ce qui est inclus / exclu (version actuelle).  
4) Parties prenantes (personas + rôles).  
5) Plan en étapes (cadrage, design, exécution, mesure).  
6) Risques et hypothèses critiques à vérifier.

---

## 3. Stratégie & business

### 3.1 Analyse d’opportunité (APS + Stratégie)

[RÔLE]  
Tu es mon APS et tu convoques le persona Stratégie.

[TÂCHE]  
Analyser une opportunité (nouveau produit / marché / partenariat) de manière structurée.

[ENTRÉE]  
« {{DESCRIPTION DE L’IDÉE / OPPORTUNITÉ}} »

[SORTIE ATTENDUE]  

1) Reformulation de l’opportunité (quoi, pour qui, pourquoi maintenant).  
2) Bénéfices potentiels (court / moyen / long terme).  
3) Risques et contraintes majeurs.  
4) Hypothèses à tester.  
5) 2–3 scénarios (prudent, réaliste, ambitieux).  
6) Recommandation + premières actions si on décide de creuser.

---

## 3.2 Définir ou challenger un business model (APS + Finance)

[RÔLE]  
Tu es mon APS et tu convoques le persona Finance / Business.

[TÂCHE]  
M’aider à définir ou challenger un business model.

[ENTRÉE]  
« {{DESCRIPTION DU PRODUIT / SERVICE / CIBLE}} »

[SORTIE ATTENDUE]  

1) Proposition de valeur résumée.  
2) Segments de clients principaux.  
3) Sources de revenus possibles.  
4) Principaux postes de coûts.  
<!-- 5) Hypothèses de volumes / pricing (ordres de grandeur, pas besoin de précision extrême).   -->
<!-- 5) Hypothèses de volumes / pricing (ordres de grandeur, pas besoin de précision extrême).   -->
1) 3–5 KPI clés à suivre.

---

## 4. Produit & tech

## 4.1 Cadrer un MVP produit (APS + CPO + CTO)

[RÔLE]  
Tu es mon APS et tu convoques CPO + CTO + UX.

[TÂCHE]  
Cadrer un MVP à partir de mon idée.

[ENTRÉE]  
« {{DESCRIPTION DU PRODUIT / FEATURE / PUBLIC CIBLE / PROBLÈME}} »

[SORTIE ATTENDUE]  

1) Reformulation de l’idée (pour qui, quel problème, quelle valeur).  
2) Hypothèses principales à tester.  
3) Proposition de MVP (fonctionnalités minimum).  
4) 5–10 user stories (En tant que…, je veux…, afin de…).  
5) 3 prochaines actions concrètes.

---

## 4.2 Roadmap produit macro (CPO + DGD)

[RÔLE]  
Tu actives CPO et DGD.

[TÂCHE]  
Construire une roadmap macro.

[ENTRÉE]  
« {{LISTE DE FEATURES / PROJETS / CONTRAINTES / DÉLAIS}} »

[SORTIE ATTENDUE]  

1) Regroupement en thèmes / epics.  
2) Priorisation (Must / Should / Could / Won’t).  
3) Roadmap par quarter ou par mois (macro, réaliste).  
4) Hypothèses et dépendances critiques.  
5) Risques et plans de mitigation.

---

## 4.3 Risques tech & dettes (CTO)

[RÔLE]  
Tu es mon CTO.

[TÂCHE]  
Identifier les principaux risques techniques et dettes sur ce projet / cette stack.

[ENTRÉE]  
« {{DESCRIPTION DE L’ARCHI, TECHNOS, CONTEXTE}} »

[SORTIE ATTENDUE]  

1) principaux risques (fiabilité, sécurité, scalabilité, maintenance).  
2) dettes techniques actuelles ou à venir.  
3) quick wins pour réduire le risque sans bloquer le business.  
4) recommandations de priorisation.

---

## 5. Communication & écrits

## 5.1 Synthèse exécutive (APS)

[RÔLE]  
Tu es mon APS.

[TÂCHE]  
Transformer ce contenu en synthèse exécutive “pour dirigeant pressé”.

[ENTRÉE]  
« {{COLLER LE TEXTE / NOTES / DISCUSSION}} »

[SORTIE ATTENDUE]  

1) Résumé en 5–10 lignes.  
2) Points clés (3–7 bullets).  
3) Décisions à prendre.  
4) Actions recommandées (et qui doit agir).

---

## 5.2 E-mail / message de cadrage (DGD)

[RÔLE]  
Tu es mon DGD.

[TÂCHE]  
Préparer un message de cadrage clair pour {{destinataire / équipe}}.

[ENTRÉE]  
Contexte :  
« {{CONTEXTE ET DÉCISION}} »

Objectif du message :  
« {{INFORMER / DEMANDER / ALIGNER / LANCER UN PROJET}} »

[SORTIE ATTENDUE]  

1) Sujet / titre possible.  
2) Message prêt-à-envoyer (ton pro, direct, bienveillant).  
3) Si utile : version encore plus courte (mode “SMS / Slack”).

---

## 6. Prompts pour GitHub Copilot / code

Ces prompts sont pensés pour être utilisés en commentaires dans le code, ou en description d’issue.

---

## 6.1 Contexte produit / technique pour Copilot

CONTEXTE POUR COPILOT  
Produit / fonctionnalité :  

- {{description simple}}

Utilisateurs :  

- {{qui l’utilise, pour quoi}}

Comportement attendu :  

- {{décrire ce que doit faire la feature, pas comment coder}}

Contraintes importantes :  

- {{performance / sécurité / lisibilité / compatibilité}}

À partir de maintenant, propose du code cohérent avec ce contexte.

---

## 6.2 Demander une implémentation précise

TÂCHE POUR COPILOT :  
Implémente une fonction qui fait ceci :  

- Entrée : {{décrire}}.  
- Sortie : {{décrire}}.  

Contraintes :  

- Code lisible, commenté,  
- Respect des bonnes pratiques de {{langage / framework}},  
- Pas de dépendances inutiles.

---

## 6.3 Refactor / amélioration de code

TÂCHE POUR COPILOT :  
Refactorer le bloc de code ci-dessous pour :  

- le rendre plus lisible,  
- mieux gérer les erreurs,  
- extraire les parties répétitives dans des fonctions séparées,  
sans changer le comportement observé.

---

## 6.4 Générer des tests

TÂCHE POUR COPILOT :  
Génère des tests unitaires pour les fonctions de ce fichier,  
en utilisant {{framework de test}}.  

Couvre les cas suivants :  

- cas nominal,  
- cas d’erreur,  
- cas limites (edge cases).

---

## 6.5 Workflow APS / DGD + Copilot

1) Dans ChatGPT / Mammouth (avec APS + DGD) :  
   - cadrer la feature,  
   - définir les user stories, règles métier, cas limites.  

2) Dans ton IDE (avec Copilot) :  
   - coller un résumé en commentaire,  
   - utiliser les prompts ci-dessus pour générer / refactorer le code.
