## Chapitre 4 : Modulations
Il existe une modulation analogique et une modulation numérique. La moduation va permettre de **greffer de l'information sur un signal**. La modulation permet de transposer le signal contenant de l'information (appelé signal **modulant**) autour d'une autre dréquence appelé la **porteuse**. Le signal **modulé** ressemble à une sinusoïde et la variation contient l'information du signal **modulant**. Ce signal est de la forme : 

![fct modulation](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/401.png) 

Il existe 3 types de modulation : 

* **Modulation d'amplitude** (on joue sur Ac)
* **Modulation de fréquence** (on joue sur w)
* **Modulation de phase** (on joue sur Qc)

### 4.1 Modulation en bande de base
La transmission est dite en bande de base si elle ne subit **aucune transposition de fréquence par modulation**. Les fréquences initiales du signal émis sont donc préservées.

### 4.2 Modulation d'amplitude (AM)
On crée le signal **modulé** sur base d'une **porteuse** et d'un signal **modulant**. L'amplitude est multiplié par (1+ms(t)). s(t) étant le signal modulant. 
![fct modulation](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/402.png)
 
Mais atention à ne pas fixer un m trop grand au risque de voir apparaitre une surmodulation.
![fct modulation](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/403.png)

#### 4.2.1 Démodulateurs d'amplitude
Il en existe deux types : 

* Le **détecteur d'enveloppe** est un circuit dont la tension descend lentement mais augmente rapidement. Ce démodulateur nécessite un choix approprié de  la constante de temps pour la "chute" de la tension.

* Le **détecteur cohérent** est plus complexe et nécessite l'envoi de la fréquence de la porteuse.

##### Détecteur cohérent
Si on part du principe qu'un signal est modulé autour de sa fréquence. On utilisera un démodulateur de fourier : 

![fct modulation](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/404.png)

La fréquence de l'oscillateur local du démodulateur doit être la même que celle du modulateur.
![Modulateur - demodulateur](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/405.png)

#### 4.2.2 Bandes Latérales
Il y a (cfr supra) des fréquences négatives qui sont des doublons. On peut donc uniquement envoyer une seule des deux bandes et reconstruire l'autre lors de la modulation. il existe donc deux bandes : 

* **USB** : Upper side Band
* **LSB** : Lower side band

#### 4.2.3 Bande latérale unique ( QAM )
On utilise l'envoi en double bande latérale dans les cas généraux mais il existe une autre technique, l'envoi en bande latéral unique par modulation en quadrature (QAM). Pour cette modulation en quadrature, il faut convertir le signal m(t) en deux signaux s1(t) et s2(t). Cette technique à l'avantage de diviser la bande passante nécéssaire par deux.

#### 4.2.4 Bande latérale résiduelle
Lorsque la bande de base s'étend jusqu'à la fréquence nulle, il n'est pas toujours possibe de faire une modulation à bande latérale unique, au sens strict du terme. On peut toutefois obtenir une réduction sensible de la largeur de la bande en éliminant partiellement une des deux bades latérales. c'est la modulation à bande latérale résiduelle. 






















   

