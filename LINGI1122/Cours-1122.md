# Notes 1122
## Méthodes de Conceptionde Programmes
###  Informations Pratiques
#### Objectifs du cours
1. Spécifier
2. Concevoir
3. Démontrer

#### Devoirs (1pt)
Un exercice après chauque TP, à rendre sur Moodle ( 1 pt )

#### Projet(4pts)
Spécifier, concevoir et prouver un programme
en 3 phases à partir de la S6
avec évaluations croisées en groupes de 3 ( libres )

#### Examen (15pts)
écrit et exercices
(en septembre = 100% de note finale)

### I. Introduction
#### Programmes et bugs
##### Comment éviter les bugs? Le débogage?
Si l'on cherche à écrire un  programme correct, le débogage n'est **pas** une solution **efficace**. En effet, il force le programmeur à fonctionner par **essais erreur**. On peut essayer d'écrire des tests mais l'absence d'échecs dans la résolution de ceux-ci ne démontres pas que le programme est correct. **les tests **ne sont **pas** non plus **efficaces** pour démontrer que le programme est faux. (Chaque test augmente la confiance mais ne garantie rien)

*"L'absence de preuves n'est pas une preuve de l'absence"*
*"Program testing can used to show the prescence of bugs, but never to show their abscence"-Dijkstra*

On Définira donc une **Science de la programmation** par l'usage de la méthode scientifique pour construire des programmes corrects. On débute ar **spécifier** *les spécifications des programmes*, on **vérifie** *ensuite les programmes par rapport à leurs spécifications* et on **construira** *enfin le programme sur la base de ces spécifications*

#### Problème, solution et preuve
##### Conception de programme
**Théorie du problème**: Quelles structures, opérations, attributs interviennent? Quelles sont les propriétés utiles?
**Solution**: *"Comment résoudre le problème?"*
**Preuve**: *"La solution est-elle correcte?"*
**Représentation**: *"Comment réaliser la solution sous forme de programme?"*

Le problème réside dans la définition de correct. Il existe plusieurs définition qui peuvent convenir au caractère correct d'un programme. On définira donc un **programme correct** comme suit : *Un programme correct par rapport aux spécifications du problème*  

##### Les contracts
Il existe 4 formes de contracts qui jugent la validité d'un programme. La version la plus simple est appellée **Correction**, il dit que *'SI pré ALORS post'*. Cette vision du contract est un peu trop simpliste pour traiter tous les cas et fait abstraction de l'arrêt du programme. On obtiens donc les deux nouveaux contracts **Terminaison** : *'SI pré ALORS fin'* et **Correction Partielle** : *'SI pré ET fin ALORS post'*. Pour prouver l'exactitude d'un programme, il suffit de démontrer que les deux contracts sont remplis.
On peut aussi utiliser le contract dit de **Correction Totale**(Correction Partielle et Terminaison) : *'SI pré ALORS fin ET post'*.

##### La preuve de l'invariant
Un **invariant** est *une formule mathématique qui reste valide durant toute l'itération*.  
Les 3 preuves pour obtenir un invariant de boucle correct:
 * Si les préconditions sont vraies initialement, alors l'invariant est vrai à l'entrée dans la boucle.
 * Si l'invariant est vrai avant une itération de la boucle, alors l'invariant est vrai après l'itération.
 * Si l'invariant est vrai à la sortie de boucle, alors les post-conditions sont vraies finalement.

##### Preuve et réccurence
La preuve sur l'itération est une récurrence : un **cas de base** (L'invariant est vrai après 0 itérations), un **cas inductif** (si l'invariant est vrai après N itérations, alors l'invariant est vrai après N+1 itérations), **Conclusion**(l'invariant est toujours vrai)

##### Un problème de précision
Les *spécifications*(Quoi?), le *programme*(Comment?) et la *preuve*(Pourquoi?) doivent être exprimés de manière **précise** et **non-ambigüe**

#### Spécification de programmes
