---
name: redaction
description: Aide à la rédaction de rapports d'ingénieur en suivant la méthodologie enseignée (structure résumé/intro/conclusion, exigences de précision et de sourcing, méthodologie de relecture de Tahiry). À utiliser quand l'utilisateur rédige un rapport, un résumé, une introduction, une conclusion, ou demande une relecture de rapport.
---

# Rédaction de rapport d'ingénieur

Ce skill applique la méthodologie de rédaction de rapport vue en cours. Il sert à la fois pour écrire un rapport et pour relire/critiquer un rapport existant.

## Structure attendue d'un rapport

Le rapport répond à 6 questions, dans cet ordre :

1. **Contexte**
2. **Quel est le problème** *(peut être fusionné avec le point 3)*
3. **Pourquoi c'est un problème** *(peut être fusionné avec le point 2)*
4. **Que font les autres ?** Qu'est-ce qui est fait en général pour résoudre ce problème
5. **Qu'est-ce que nous avons fait** pour résoudre ce problème
6. **Résultats**

Ces 6 questions structurent le résumé, l'introduction et la conclusion.

## Le résumé

- **Une phrase par point** (6 phrases au total).
- Rester cohérent dans le propos.
- **Test de cohérence** : on doit pouvoir lire la première et la dernière phrase à la suite et avoir assez d'information pour deviner ce qu'il y a entre les deux.

## L'introduction

- Mêmes questions que le résumé.
- Mais **un paragraphe par point** au lieu d'une phrase.
- Le test de cohérence s'applique aussi : la première et la dernière phrase de chaque paragraphe doivent se lire à la suite de manière cohérente.

## La conclusion

- On reprend la structure de l'introduction.
- Mais on répond avec **2 ou 3 phrases** par point au lieu de 5 ou 6.
- **Important** : discuter des choix faits et expliquer pourquoi c'est mieux **pour notre projet** (pas de réponse générale type "le digital est mieux que le facial parce que plus sécurisé").

## Titres de sections

- Les noms de sections doivent être **explicites**.
- **Ne jamais** mettre un titre PNJ générique style "Rapport de stage".
- Choisir une chose concrète qu'on a faite et la mettre dans le titre.

## Exigences de précision

- **Pas de formulations vagues**. "Depuis des années…" → combien d'années ? Donner une date précise.
- Pour chaque phrase, trois possibilités seulement :
  1. C'est **nous** qui le disons (ex : "nous avons une augmentation de 50%…") — il faut alors que ce soit vérifiable dans notre travail.
  2. C'est **quelqu'un d'autre** qui le dit — il faut la **source**.
  3. **Personne** ne le dit → **on ne le met pas**.

## Sources

Les sources doivent **faire autorité** :
- Datasheets
- Papiers scientifiques
- Documentations techniques (sources **primaires**)
- ACM, IEEE, LNCS pour la vérité scientifique (sources **secondaires**)
- Articles **étoilés** sur Wikipédia

À noter pour la veille technologique : la **vérité scientifique** se trouve dans les sources **secondaires**, pas dans les sources primaires.

## Figures et tableaux

- Les figures doivent être **lisibles**.
- Chaque figure a une **description complète dans le caption** (titre + description).
- Le caption doit suffire à comprendre la figure : **ne pas obliger le lecteur à fouiller dans le texte**.
- Un caption de 5-6 lignes, ce n'est pas grave.
- Une redondance entre caption et texte, ce n'est pas grave non plus.

## Annexes

Si une information **doit figurer** dans le rapport mais n'est **pas utile à la lecture**, elle va en **annexe**.

## Méthodologie de correction de Tahiry (à anticiper)

Le correcteur lit dans cet ordre :
1. Le résumé en entier
2. La page de titre en entier
3. La 1ère phrase + dernière phrase de chaque paragraphe de l'**introduction**
4. La 1ère phrase + dernière phrase de chaque paragraphe de la **conclusion**
5. À ce stade, il a déjà une idée de la note.
6. Il feuillette en s'arrêtant sur les **figures et tableaux** (d'où l'importance des captions auto-suffisants).
7. S'il décide de lire une section : 1ère + dernière phrase de chaque paragraphe doivent se lire de manière cohérente.

→ Conséquence : optimiser **résumé, intro, conclusion, captions** en priorité. La cohérence "première + dernière phrase de paragraphe" est un test à appliquer partout.

## Outils

Pour l'IEEE en Typst : https://typst.app/universe/package/charged-ieee

## Comment utiliser ce skill

Quand l'utilisateur demande de l'aide à la rédaction :

1. **S'il écrit un résumé/intro/conclusion** : vérifier que les 6 points sont présents (ou 5 si 2+3 fusionnés), dans le bon ordre, et appliquer le test "première + dernière phrase".
2. **S'il écrit le corps du rapport** : vérifier titres explicites, précision (chiffres, dates), sourcing de chaque affirmation, captions auto-suffisants.
3. **S'il relit** : appliquer la méthodologie de Tahiry — lire résumé, puis 1ère/dernière phrase des paragraphes d'intro et de conclusion, puis vérifier les figures.
4. **Repérer activement** : les formulations vagues ("depuis longtemps", "beaucoup", "souvent"), les affirmations sans source, les titres génériques, les justifications générales au lieu de justifications spécifiques au projet.
