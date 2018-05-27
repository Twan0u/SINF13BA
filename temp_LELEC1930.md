## Chapitre 1 : Introduction

* 11 cours magistraux
* 3-5 Séances d'exercices
* Examen :
    - Ecrit
    - Questions pour vérifier la compréhension des concepts
    - Inutile de retenir des tables de chiffres par coeur
    - Eventuellement 1 exercice simple d'application

### 1.1 introduction 
**Télécommunications** : "Transmission d'information, sous la forme de signaux électriques, sur le canal de communication".
Il existe des : 

* **canaux filaires**(téléphone, coax, optique) 
* **canaux sans fils**(ondes électromagnétiques dans l'air) + *Antennes*

### 1.2 Canaux de Communication

* Atténuation
	* Augmente avec la distance
		* Lié à perte d'énergie / radiation dans toutes directions
* Bruits / Interférences
* Distorsion = modification de la forme (Effet Doppler)

## 1.3 Représentation de l'information
un **Signal analogique** transporte de l'information via la forme de son signal.  

* *Avantage* : Insensibles à atténuation/amplification  
* *Problème* : Sensible à la distorsion 

un **Signal numérique** transporte de l'information via des 1 et 0.  

On peut transformer un *Signal analogique* en *Signal numérique* via un processus de **Numérisation**

La **transformation de Fourier** est une opération qui transforme un signal (fonction intégrable sur R) en une autre fonction, décrivant le spectre fréquentiel de cette dernière.

### 1.4  Bande de Fréquences
Une bande de fréquence est une limitation d'un système à sa fréquence. C'est obligatoire pour : 

* la standardisation  et la coexistance des systèmes
* Limite physique des circuits électroniques 

**Modulation** : Transposition du signal autour de la fréquence souhaitée. 

Le **multilexage** est la capacitée de faire passer plusieurs signaux par le même support. Ceci est possible via le multiplexage

### 1.5 Son Stéréo 
Le son stéréo est composé de 2 signaux : 

* Le S1 (G+D) pour la compatibilité mono
* Le S2 (G-D)  signal stéréo avec effet de compression 
	En Stétéo : (G = S1+S2) (D=S1-S2) 
	
### 1.6 Image en tv analogique
Le design est lié avec les caractéristiques de la vision humaine:

* clignotement si inférieure à 50 im/sec
* si distance est suppérieure à 6x la auteur : inférieure à 500 lignes


![scan et flyback](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/101.png)
![signal tv](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/102.png)

Avec cette technique, on peut tomber sur des parasites dans l'image si la fréquence du réseau est équivalente à celle de l'image. Pour éviter ce problème, on utilise une technique appelée entrelacement, elle consiste en une division en 2 de l'image (une ligne sur deux), évitant ainsi les parasites. 
![](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/103.png)

#### 1.6.1 Télévision couleur
On applique le même principe que précédemment mais avec les 3 couleurs.
![télévision couleur](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/104.png)

Cependant, pour des raisons de rétrocompatibilité, les signaux sont encore adaptables sur les anciennes tv en noir et blanc. LE *RGB* devient donc **YUV** : 

* **Y** = 0,3 *R* + 0,59 *G* + 0,11 *B*
* **U** = 0,493 (*B*-**Y**)
* **V** = 0,877 (*R*-**Y**)

#### 1.6.2 Télévision Haute définition
On double la résolution horizontale et verticale en passant du format 4/3 au format 16/9. Cette amélioration apporte une meilleure qualité d'image et un son numérique

### 1.7 Les Signaux numériques 
Les signaux numériques sont représentées via des bits.

#### Avantages :

* Traitement informatiques et stockages
* Régénération possible
* Pas de déterrioration 
* Codes correcteurs et détecteurs d'erreurs

#### 1.7.1 Code correcteur d'erreur
Un des avantages de la forme binaire est la possibilité de corriger les erreurs. Le principe est d'ajouter de la redondance en rallongant la transmission. Il y a cependant un risque de non détection d'erreurs si elles sont trop nombreuses.

### 1.8 échantillonnage
![échantillonnage](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/105.png)
L'échantillonnage est utilisé pour représenter au mieux la donnée analogique en donnée numérique. Il y parviens généralement bien mais il arrive que cette méthode ait des ratées. On différencie un bon échantillonnage d'un mauvais par sa capacité ou non à retransmettre la donneé.

**L'aliasing** résulte d'un mauvais échantillonnage.  
![Aliasing](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/106.png)

#### 1.8.1 Théorème de Shannon
La fréquence d'échantillonnage doit être au moins 2 fois la fréquence maximum du signal

* exemples
    * son hifi : 40kHz ( > 2x15kHz)











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
Aussi appelé Skin effect, il s'agit d'un phénomène qui pousse les électrons à se déposer en couche ( à cause de l'attraction électromagnétique )
![Effet Pelliculaire](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/204.png)

##### Calculs d'amplifications et d'atténuation
La force des signaux est calculée en dB (Décibels). On retrouve pour ces calculs, une puissance d'entrée (P1) et une puissance de sortie (P2). On calcule une aténuation avec la formule $P1/P2$

### 2.2 Lignes Bifilaires
### 2.3 Lignes Coaxiales
### 2.4 Communication optiques