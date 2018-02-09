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
Si l'on cherche à écrire un  programme correct, le débogage n'est **pas** une solution **efficace**. En effet, il force le programmeur à fonctionner par **essais erreur**. On peut essayer d'écrire des tests mais l'absence d'échecs dans la résolution de ceux-ci ne démontres pas que le programme est correct. **les tests **ne sont **pas** non plus **efficaces** pour démontrer que le programme est faux. 

*"L'absence de preuves n'est pas une preuve de l'absence"*

#### Théorie de base
La **Théorie** est le cas général toujours vrai, est complétée par les **cas particuliers**. Il faut ensuite prouver que le **programme se termine** ( cfr : *Théorie de la variance* ) 

#### Les 2 Contracts 
