---
name: rapport-stage
description: Rédaction et vérification de conformité du rapport de stage technicien 3A (ESIROI, filière Informatique) selon les directives officielles d'août 2026. À utiliser dès que l'utilisateur mentionne son rapport de stage, sa soutenance de stage, le template LaTeX de rapport, le résumé/abstract, le plan IMRaD, les annexes obligatoires, la V0 ou la V1 du rapport — que ce soit pour écrire une section, structurer le rapport, préparer les slides, ou relire/auditer un rapport existant et vérifier sa conformité aux exigences. À utiliser aussi pour toute question sur les livrables, le calendrier de rendu ou le format attendu du stage technicien.
---

# Rapport de stage technicien 3A — ESIROI Informatique

Ce skill couvre les directives officielles du rapport et de la soutenance du stage technicien (3A). Il sert à deux usages :

1. **Rédiger** : aider à écrire le rapport (ou une section) conformément aux exigences.
2. **Vérifier** : auditer un rapport déjà écrit et produire un diagnostic de conformité (voir la checklist en fin de skill).

Il complète le skill `redaction` (méthodologie générale de rédaction : test première/dernière phrase, précision, sourcing, méthodologie de relecture de Tahiry). Quand les deux s'appliquent, utiliser les deux : `redaction` pour la qualité rédactionnelle, `rapport-stage` pour la conformité aux directives du stage technicien.

## Esprit du rapport (à rappeler avant toute rédaction)

- Le rapport s'adresse à un **lecteur extérieur** qui ne connaît ni l'entreprise ni les missions : tout le contexte doit être exposé depuis l'origine.
- C'est un document qui **montre du recul** : contexte, problème traité, et surtout **pourquoi les choix ont été faits** (comparaison des technologies/protocoles/frameworks avec avantages et inconvénients).
- **Toute affirmation factuelle est justifiée et référencée** (bibliographie obligatoire, fichier `source.bib`).
- Le stage est individuel : le rapport est un **travail personnel**.
- Le template dédié (https://git.inge.re/projets/template-rapport) est la **source de référence** : sa structure et ses consignes `\todo` paragraphe par paragraphe doivent être suivies.

### Ne pas confondre avec d'autres types de documents

Un rapport de stage n'est **ni** :
- un **tutoriel** (mode d'emploi pour débutant : par où commencer, où cliquer) ;
- un **howto/FAQ** (recette reproductible d'une manipulation, sans expliquer les concepts) ;
- une **documentation technique** (description détaillée d'un framework/protocole).

Ces trois types de documents ont leur place **en annexe**, pas dans le corps. Signe distinctif : ils n'ont peu ou pas de bibliographie ; le rapport de stage, lui, en a obligatoirement une.

Lors d'une relecture, repérer les passages qui glissent vers le tutoriel ("cliquer sur…", "il faut d'abord installer…") ou la documentation technique pure (explication d'un protocole sans lien avec un choix du stage) : les signaler et proposer un déplacement en annexe.

## Périmètre attendu

Le rapport couvre l'ensemble du stage, avec l'accent sur les **missions techniques effectivement conduites** et la **contribution personnelle** apportée à l'entreprise. Exemples d'apports valorisables : conception/développement/intégration d'un composant, mise en place ou amélioration d'une chaîne d'outils ou infrastructure, automatisation ou fiabilisation d'un existant, production de documentation/tutoriels/tests pour l'équipe, participation à la gestion de projet (workflow Git, tickets, jalons).

## Plan attendu (structure obligatoire)

1. **Page de titre, remerciements, résumé (FR), abstract (EN), table des matières.**
   - Résumé et abstract **tous deux obligatoires**, chacun suivant la trame en **cinq phrases** : ① contexte général, ② contexte spécifique, ③ problème et son importance, ④ état des solutions existantes, ⑤ contribution apportée et son apport.
   - (Formulation équivalente en quatre questions : quel est le problème, en quoi est-ce un problème, quelle solution est proposée, en quoi est-elle pertinente.)
2. **Introduction**, dans cet ordre :
   - un encadré **grayBox** résumant en une phrase la contribution principale du stage ;
   - le contexte général (entreprise, domaine d'activité) ;
   - le contexte spécifique (problème précis adressé pendant le stage) ;
   - l'exposé du problème (figure si pertinent) ;
   - un panorama des solutions existantes et de leurs limites ;
   - la contribution apportée et ses résultats principaux ;
   - un dernier paragraphe annonçant le plan du rapport.
3. **Section principale (contribution)** — le cœur du rapport. Titre **adapté au sujet** (jamais un titre générique), organisée en sous-sections de type **IMRaD** :
   - *Problématique et bibliographie* : reprise détaillée du problème, état de l'art des solutions envisageables, conclu par la **justification des choix retenus** ;
   - *Matériels et méthodes* (ou *Développement*) : environnement, données/briques manipulées, mise en œuvre — c'est ici que se concentrent les contributions personnelles ; **ce qui préexiste ou vient d'autrui est explicitement crédité** ;
   - *Résultats et discussion* : résultats (figures avant/après si pertinent), portée, **limites et pistes d'amélioration**.
4. **Missions annexes** : travaux secondaires (intégration ponctuelle, veille, documentation, support). Chaque mission suit le format condensé : **contexte → problème → action menée → résultat**.
5. **Conclusion**, en quatre temps :
   - rappel synthétique du contexte et du problème ;
   - état avant le stage et contribution apportée ;
   - projection à court terme (ce qui aurait été fait **avec deux mois de plus**) ;
   - projection à long terme (**avec six mois de plus**) ;
   - puis un dernier paragraphe **en première personne** : bilan personnel (ce que le stage a apporté).
6. **Bibliographie** : indispensable, alimentée depuis `source.bib`. Toute affirmation factuelle ou choix technique structurant est cité.
7. **Annexes** : au minimum les **trois annexes types du template** (voir ci-dessous), plus les annexes propres au stage.

## Corps vs annexes

Le corps est destiné à une **lecture continue** : synthèses, résultats, choix retenus, schéma d'ensemble. Les détails bruts vont en annexe.

| Dans le corps | En annexe |
|---|---|
| Schéma global d'architecture (vue unique) | Schémas détaillés par composant |
| Synthèse du cahier des charges | Cahier des charges et spécifications complètes |
| Jalons et points clés du planning | Diagramme de Gantt complet |
| Choix techniques majeurs et justification | Tableaux comparatifs exhaustifs |
| Illustration représentative d'un livrable | Captures d'écran exhaustives, jeux de tests |
| Extraits de code illustratifs (≈ 10 lignes) | Listings étendus, howto, tutoriels |
| Résultat synthétique d'un calcul/mesure | Calculs détaillés, données brutes |

Ne pas forcer les éléments qui ne s'appliquent pas au stage ; appliquer le même principe corps/annexes aux livrables réels.

### Les trois annexes obligatoires du template

1. **Description du contexte (entreprise)** : structure d'accueil, domaine, environnement, organigramme ou interlocuteurs principaux, positionnement du stagiaire.
2. **Déroulement du stage et Gantt** : conditions de travail, Gantt prévisionnel **et** réel si possible, commentaire sur les écarts.
3. **Extrait de code** : un extrait représentatif, commenté (rôle et place dans le projet), avec renvoi au dépôt Git pour l'intégralité du code lorsque communicable.

Toutes les annexes doivent être **numérotées, titrées, légendées et référencées depuis le corps** (ex. : "cf. Annexe A"). Une annexe jamais référencée dans le corps est une non-conformité.

## Conventions rédactionnelles

- **Posture** : corps technique en formulation **impersonnelle**, centrée sur les choix et les résultats. Le « je » est admis **uniquement** dans : les remerciements, le paragraphe de bilan personnel en conclusion, et certaines annexes (déroulement, conditions de travail).
- **Cohérence des paragraphes** : première et dernière phrase de chaque paragraphe cohérentes entre elles ; la dernière phrase d'un paragraphe prépare la première du suivant. (C'est le test du skill `redaction` — l'appliquer systématiquement.)
- **Figures et tableaux** : toujours référencés dans le texte ; légendes **complètes et auto-suffisantes** (un lecteur qui ne lit que la figure et sa légende comprend l'élément sans chercher dans le corps).
- **Définitions en note de bas de page** : les termes techniques et acronymes, même supposés connus, sont définis en note de bas de page pour ne pas interrompre la lecture.
- **Citations bibliographiques** : toute affirmation factuelle, donnée chiffrée ou choix technique structurant est accompagné d'une référence.
- **Crédit des contributions** : dans la section de contribution, ce qui vient d'autrui (collègues, code préexistant, bibliothèques tierces) est explicitement crédité ; les contributions personnelles apparaissent clairement comme telles.
- **grayBox** : à utiliser pour annoncer le contenu d'une section ou résumer une contribution en une ou deux phrases.
- **Orthographe et grammaire** : même en V0, aucune erreur détectable par un correcteur automatique (LanguageTool recommandé).

## Format, longueur, livrables

- **Outil obligatoire** : LaTeX (ou Markdown et dérivés). Compilation sur `main_it.tex`. **Overleaf déconseillé** (limitations incompatibles avec le template) — préférer une installation locale.
- **Longueur (3A)** : **15 pages minimum, 30 pages maximum, hors annexes**. Annexes sans limite.
- **Livrables** : le PDF compilé depuis le template + le cas échéant un **lien visible vers le dépôt Git à jour** (en introduction ou en page de garde).
- **Confidentialité** : si le stage l'impose, restreindre le partage à pierre.tournoux@univ-reunion.fr, tahiry.razafindralambo@univ-reunion.fr et joel.grouffaud@univ-reunion.fr.

## Calendrier 2026

| Échéance | Livrable |
|---|---|
| lundi 17 août 2026 | V0 du rapport |
| mercredi 19 août 2026 | V0 du support de présentation |
| lundi 24 août 2026 | V1 (définitive) du rapport et du support |
| semaine du 24 août 2026 | Soutenances |

La V0 est un **premier jet complet** (plan détaillé + premier jet rédigé) permettant un retour de l'équipe pédagogique ; la V1 est la version définitive.

## Soutenance

- **15 minutes** de présentation + **10 minutes** de questions.
- Outil : LaTeX (Beamer) ou Markdown et dérivés.
- Bonnes pratiques : slides **numérotés** ; **un message par slide**, peu de texte, figures lisibles (réf. : *Creating effective slides*, CTL Stanford) ; maîtrise du débit de parole (réf. : *How to sound smart in your TEDx Talk*, Will Stephen) ; **répéter** pour tenir le temps.

## Mode rédaction : comment aider

1. Identifier où en est l'utilisateur (plan ? section ? V0 ? V1 ?) et la section concernée.
2. Rappeler la trame exacte de la section avant de rédiger (ex. : les 5 phrases du résumé, les 7 blocs de l'introduction, le format contexte/problème/action/résultat des missions annexes).
3. Rédiger en posture impersonnelle (sauf zones où le « je » est admis), avec placeholders explicites `[à compléter : …]` pour les faits que seul le stagiaire connaît — ne jamais inventer de données sur le stage.
4. Pour chaque affirmation factuelle, signaler qu'une référence est attendue et proposer une entrée `source.bib` type.
5. Vérifier le résultat avec la checklist ci-dessous et les tests du skill `redaction`.
6. Rappeler la langue de sortie : résumé en français **et** abstract en anglais, les deux avec la même trame.

## Mode vérification : audit de conformité

Quand l'utilisateur fournit un rapport (PDF, LaTeX ou texte) à vérifier, produire un diagnostic structuré. Parcourir systématiquement la checklist et classer chaque point : ✅ conforme / ⚠️ partiel / ❌ non conforme / N/A, avec pour chaque ⚠️ ou ❌ une citation ou localisation précise dans le rapport et une correction proposée.

### Checklist de conformité

**Structure**
- [ ] Page de titre, remerciements, résumé FR, abstract EN, table des matières présents
- [ ] Résumé : 5 phrases suivant la trame (contexte général / contexte spécifique / problème et importance / solutions existantes / contribution et apport)
- [ ] Abstract EN : même trame que le résumé
- [ ] Introduction : grayBox initial, puis les 6 blocs dans l'ordre, terminée par l'annonce du plan
- [ ] Section principale avec titre adapté au sujet (pas de titre générique type "Travail réalisé")
- [ ] Sous-sections IMRaD : problématique et bibliographie / matériels et méthodes / résultats et discussion
- [ ] Justification des choix retenus en conclusion de l'état de l'art (comparaison avantages/inconvénients)
- [ ] Section « Missions annexes » : chaque mission au format contexte/problème/action/résultat
- [ ] Conclusion en 4 temps + bilan personnel en première personne
- [ ] Projections à 2 mois et à 6 mois présentes dans la conclusion
- [ ] Bibliographie présente et non vide
- [ ] Les 3 annexes obligatoires présentes (contexte entreprise, déroulement + Gantt, extrait de code)

**Corps vs annexes**
- [ ] Le corps se lit en continu (pas de listings de code étendus, pas de captures exhaustives, pas de tableaux comparatifs exhaustifs dans le corps)
- [ ] Extraits de code dans le corps ≈ 10 lignes maximum
- [ ] Aucun passage type tutoriel/howto/documentation technique dans le corps (à déplacer en annexe)
- [ ] Annexes numérotées, titrées, légendées
- [ ] Chaque annexe référencée au moins une fois depuis le corps

**Conventions**
- [ ] Posture impersonnelle dans le corps ; « je » limité aux remerciements, bilan personnel, annexes de déroulement
- [ ] Cohérence première/dernière phrase de chaque paragraphe (échantillonner l'intro et la conclusion en priorité)
- [ ] Toutes les figures/tableaux référencés dans le texte
- [ ] Légendes auto-suffisantes
- [ ] Termes techniques et acronymes définis en note de bas de page
- [ ] Affirmations factuelles, chiffres et choix structurants tous sourcés
- [ ] Travail d'autrui et existant explicitement crédités ; contributions personnelles clairement identifiées
- [ ] Pas d'erreurs détectables par un correcteur automatique

**Format et livrables**
- [ ] Rédigé avec le template LaTeX (ou Markdown/dérivés)
- [ ] 15 à 30 pages hors annexes
- [ ] Lien vers le dépôt Git visible (intro ou page de garde), si applicable
- [ ] Gantt prévisionnel et réel avec commentaire des écarts (annexe déroulement)

### Restitution de l'audit

Restituer dans cet ordre :
1. **Verdict global** en une phrase (conforme / conforme avec réserves / non conforme) et les 3 à 5 points les plus critiques.
2. **Tableau ou liste par catégorie** (structure, corps/annexes, conventions, format) avec le statut de chaque point.
3. **Corrections priorisées** : d'abord ce qui bloque la conformité (structure manquante, annexes obligatoires absentes, bibliographie vide, hors limite de pages), puis les améliorations rédactionnelles.
4. Si pertinent, appliquer en complément la méthodologie de relecture de Tahiry (skill `redaction`) : résumé → première/dernière phrase des paragraphes d'intro et de conclusion → figures et légendes.

## Objectif pédagogique (à garder en tête)

Ce rapport prépare directement le rapport de fin d'études (5A) : même structure, mêmes exigences, même posture — présenter un travail à un lecteur extérieur et expliquer **pourquoi** les choix ont été faits. Toute aide apportée doit renforcer cette posture, pas s'y substituer.
