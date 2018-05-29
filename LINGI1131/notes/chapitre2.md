## 2. Declarative programming

La programmation déclarative est un type de programmation qui ne se programme pas en instructions mais en indiquant au programme à quel résultat celui-ci doit arriver. Ce qui revient à dire à un chauffeur de taxi où vous voulez aller et non lui indiquer rue par rue toutes les indications pour rentrer jusque chez vous. Le programme est ainsi plus simple. Cependant, dans certains cas, il arrive que le programme fasse des choix surprenants. Il est aussi important de noté que la programmation déclarative est une programmation composée (= elle se compose de différentes parties pour former des parties plus grandes)

### 2.1 Réccursion
Le language OZ est un language qui utilise la réccusrion comme fondement. (ex: listes, trees, ...).
Il est donc toujours important de penser en réccusrion

### 2.2 Pattern Matching
Quand on programme, il arrive que l'on ai besoin d'accéder à un élément d'une structure. Dans l'exemple suivant, il s'agit d'une liste.
```
case Xs
  of nil then <premier code>
  [] X|Xr then <second code>
end
```
On analyse la liste Xs, si elle est nulle, c'est le premier code qui sera lancé. dans le second cas, le premier élément de la liste pourra facilement être accédé via le X et le suivant Xr dans le second code. Ceci s'appelle le pattern Matching, il est très utile en programmation en OZ

### 2.3 Time and space efficiency
L'efficacité temporelle est spatiale peut être calculée sur base du kernel language, elle décrit l'évolution de la consomation de mémoire ou le temps d'exécution si le problème de taille n venait à changer. (ex:  O(1) temps constant, O(n^{2}) évolution quadratique)
Il existe plusieurs notations pour décrire l'efficience : theta(borne minimum), Grand O (temps moyen), Omega (temps maximal). qui représentent généralement respectivement les cas, optimal, moyen et le pire cas.

### 2.4 Higher-order Programming
La programmation de haut degré est une programmation qui accepte une fonction comme argument d'une autre fonction.   

### 2.5 Genericity
La généricité est une des conséquences du High-order programming, elle permet l'utilisation de différentes fonctions placés en argument comme input de celle-ci (Ex: La fonction map prends une fonction et une liste en argument. la fonction map applique la fonction en argument à chaque élément de la liste)

### 2.6 Embedding
Les procédures peuvent être mises dans une structure de données, ce qui leur donne plusieurs usages :

* Explicit lazy evaluation (=exécution différée) : construit une petite partie de la structure et le reste en fonction des besoins sur le translated

* Modules : un Record qui groupe ensemble un set d'opérations ensemble

* Software Components : Un ensemble de modules en input et output d'un nouveau modules. On importe ainsi seulement ce dont on a besoin de chaque module

### 2.7 Data techniques (pattern matching)
#### List
```
case L
  of nil then ...
  []X|Xr then ...
  else ...
end
```
#### Trees
```
case T
  of nil then ...
  [] ??????
end
```