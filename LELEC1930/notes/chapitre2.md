## Chapitre 2 : Lignes de transmission
### 2.1 Théorie des lignes
#### 2.1.1 Caractérisation des lignes
Quand on souhaite caractériser une ligne, il est interressant de connaître son atténuation ou sa dispersion le long de cette ligne. Ces caractéristiques dépendent de la géométrie des matériaux, des conditions (Impdance, mode, linéarité,...) et d'autres paramètres (paramètre S).

##### Types de lignes

![Types de lignes](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/201.png)

##### Matériaux utilisés
##### Modélisaion d'une ligne 

![Modèle d'une ligne](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/202.png)

##### Propagation sur une ligne avec pertes
Lorsque l'on utilise une ligne, on doit se confronter à une atténuation au cours du temps du signal 
![Atténuation signal](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/203.png)

##### Effet pelliculaire
Aussi appelé Skin effect, il s'agit d'un phénomène qui pousse les électrons à se déposer en couche ( à cause de l'attraction électromagnétique ). On peut compérer ça à du cholesterol.
![Effet Pelliculaire](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/204.png)

##### Calculs d'amplifications et d'atténuation
La force des signaux est calculée en dB (Décibels). On retrouve pour ces calculs, une puissance d'entrée (P1) et une puissance de sortie (P2). On calcule une **atténuation** avec la formule $10 log(P1/P2)$. Qui nous donne l'atténuation en dB. On peut par un calcul similaire calculer l'**amplificaion** d'un signal avec la formule $10 log(P2/P1)$ 

##### Dispersion 
La dispersion est causée par le *skin effect*. Elle à pour effet de lisser les pulsations électriques
![Dispersion](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/205.png)
![Dispersion](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/206.png)

##### Impédance
"L'**impédance** électrique mesure l'opposition d'un circuit électrique au passage d'un courant alternatif sinusoïdal" - *Wikipedia*. Z est la résistance pure et Z imaginaire pour pure induction/capacitée. Cette Impédance dépends généralement de la fréquence. L'**impédance caractéristique** d'une ligne peut être calculée si on imagine une ligne infinie, l'impédance caractéristique est notée Zc.

![impedance](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/207.png)

1. **Mauvais cas** : cas ou $wL << R$ 
Zc est un complexe et proportionnel à 1/racine(w)

2. **Bon cas** $wl>>R$ 
Zc est réel et indépendant de w

##### Pupinisation 
**Pupinisation** :Procédé qui consiste à introduire des bobines d'induction, à intervalles réguliers, dans les conducteurs d'une ligne de télécommunication afin de limiter la bande passante et d'accroître les distances de transmission. La pupinisation est donc une augmentation artificielle de L en insérant des inductances. mais L est localisé et on crée donc un filtre passe-bas.  
  
**Un filtre passe-bas** est un filtre qui laisse passer les basses fréquences et qui atténue les hautes fréquences, c'est-à-dire les fréquences supérieures à la fréquence de coupure.
 
### 2.2 Lignes Bifilaires
![bifilaire](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/208.png)
![quartes](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/209.png)

On peut ensuite regrouper es quartes en bottes de 50.

#### 2.2.1 Diaphonie
Le problème des lignes téléphoniques classiques est la diaphonie importante à laquelle elles sont confrontées. La **diaphonie** ou *crosstalk* est un problème lié avec le croisement périodique des fils qui crée des interférences entre ceux-ci.

#### 2.2.2 Avantages

* Faible coût
* Connexions aisées
* pré-installation dans les bâtiments
* faible atténuation aux basses fréquences

#### 2.2.3 Inconvénients

* Atténuation importante aux hautes fréquences
* Rayonnement important 
    * sensibilité aux interférences
    * Problèmes de confidentialité

### 2.3 Lignes Coaxiales
![coax](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/210.png)

Les cables coax peuvent êtres regroupées ou renforcées pour leur permettre de parcourir de plus grandes distances ou être sous-marins

#### 2.3.1 Avantages

* Large bande passante (500MHz)
* Protection contre les interférences
* Technique éprouvée et répendue
* Facilité de réparation et de connexion

#### 2.3.2 Inconvénients 

* Fréquence limitée +- 500MHz
* Blindage jamais parfait 

### 2.4 Communication optiques
![optique](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/211.png)

#### 2.4.1 Réflexion totale
Il existe un indice au dela duquel le rayon ne se réfracte plus mais il se reflette. C'est ce procédé qui est utilisé dans les fibres optiques
![reflection refraction](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/212.png)

#### 2.4.2 Types de fibres optiques
##### Fibre multimode à saut d'indice
![saut d'indice](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/213.png)

##### Fibre multimode à gradient d'indice
![gradiant](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/214.png)

##### Fibre monomode
![monomode](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/215.png)

#### 2.4.3 Cône d'acceptance 
Le **cône d'acceptance** est dle degré de latitude que possède la lumière pour être reflétée à l'interrieure de la fibre optique
![cone d'acceptance](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/216.png)

#### 2.4.4 La dispersion modale 
La **dispersion modale** est un des effets des rayons qui se reflettent plus que le rayon central et provoquent donc des erreurs de "retard" dans le signal
![Dispersion modale](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/217.png)

#### 2.4.5 Avantages

* Bande passante énorme
* Très faible atténuation
* Immuité à l'égard des rayonnements
* isolation électrique
* Encombrement, poids et coût faibles

#### 2.4.6 Désavantages
* Connexions difficiles
* Réparations difficiles
* Disponibilité de transducteurs
* Disponibilité de l'infrastructure














