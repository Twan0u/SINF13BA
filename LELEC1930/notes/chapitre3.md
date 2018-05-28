## Chapitre 3 : Propagation et Antennes
### 3.1 La Propagation
La propagation d'une onde dépend de :

* la fréquence
* la taille de l'objet
* la surface ( matéraux, ... )
* obstacles physiques ( bâtiments, murs, sol, ... )

#### 3.1.1 L'onde Directe 

* Onde en ligne droite
* Portée limitée à l'horizon
* interférence avec l'onde réfléchie
* au plus la fréquence de l'onde est élevée, au moins sa portée est importante

![onde directe](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/302.png)

#### 3.1.2 L'ionosphère
L'**ionosphère** est une couche d'air ionisé par les rayons UV du soleil. L'ionosphère fonctionne comme un réflecteur à ondes. MUF (Maximal Usable Frequency) est la fréquence maximale telle que l'on est sur à 50% qu'elle est réfléchie par l'ionosphère (elle peut changer en fonction de l'activité solaire)

![ionosphère](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/303.png)

##### Réfraction dans l'ionosphère

![ionosphère](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/304.png)
![ionosphère](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/305.png)

#### 3.1.3 Satellite
Un satélite géostationnaire est un satélite situé à 36'000 Km d'altitude qui retransmet le signal. 
![ionosphère](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/306.png)


### 3.2 Caractérisation d'un canal
Un canal peut être caractérisé par son aténuation ( coût d'une liaison ) ou par sa distortion ( Trajets multiples ou Doppler
![Possibilitées](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/301.png)
![Possibilitées](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/307.png)

#### 3.2.1 Trajets Multiples
Dès que l'on parle d'ondes dans l'air, on s'expose au problème de trajets multiples. Il s'agit globalement du dépacement d'une onde (principale) qui est parasitée par elle même ralentie car rebondie avant d'atteindre le récepteur. (analogie d'une conversation avec beaucoup d'echo). Voici quelques exemples

*  Onde directe et onde par l'ionosphère
* Onde directe et l'onde réfléchie par un objet ou un bâtiment
* ...

### 3.6 Antennes
L'interêt des antennes sont des dispositifs capables de **rayonner** ou de **capter** des ondes électromagnétiques.  

#### 3.6.1 Onde TEM
**Onde TEM** (*mode Transverse Electrique-magnétique*) : mode de propagation tel que les champs électriques et magnétiques sont tous deux orthogonaux à la direction de propagation.  

Animation de l'onde : *https://www.edumedia-sciences.com/fr/media/222-onde-transverse-electro-magnetique*

![Onde TEM](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/308.png)

#### 3.6.2 Antennes isotropes
**L'antenne isotrope** antenne dont le diagramme de rayonnement est un cercle. 
L'antenne envoie un rayonnement dans une certaine direction mais provoque aussi un rayonnement inverse non désiré.  
Le **gain** de l'antenne peut se calculer : puissance dans la direction de puissance max / Puissance dans cette direction si l'antenne était isotrope.  
L'**angle d'ouverture** d'une antenne est l'angle de direction pour laquel la puissance rayonnée est la moitié de la puissance rayonnée dans la direction la plus favorable.

![Angle d'une onde](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/309.png)

La **puissance isotrope rayonnée équivalente** est la puissance qu'il faudrait appliquer à une antenne isotrope pour obtenir le même champ dans la direction de puissance maximum d'une antenne d'emission.

#### 3.6.3 Dipole Lambda/2
Une dipole est composée de deux tiges dont la taille est de Lambda/4. Les tensions sont minimales au centre et maximales sur les extrémitées
![dipole](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/310.png)

#### 3.6.4 Dipole replié
L'antenne dipole replié utilise le principe du miroir. L'antenne est de taille égale à Lambda/2 et permet d'avoir une bande passante plus large
![dipole replié](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/311.png)

#### 3.6.5 Antenne "endfire"
L'antenne est composée de deux "dipole" de longeur Lambda/2 et séparée par Lambda/4. L'antenne de droite est alimentée avec une avance de phase de 90° (Lambda/4 par rapport à celle de droite). Cela entraine un renforcement vers la gauche. 
![endfire](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/312.png)

#### 3.6.6 Antenne yagi
Une antenne yagi est composée d'un réflecteur, d'un dipole et d'un directeur. La directivité d'une antenne yagi est très étroite (elle est précise). Cette précision diminue les parasites dans la réception. Pour augmenter la directivité d'une antenne, il faut augmenter le nombre de directeur mais celà va diminuer la bande passante.
![dipole](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/313.png)
![directivité des antennes](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/314.png)

#### 3.6.7 Antenne parabolique
![parabole](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/315.png)

#### 3.6.8 Réseaux d'antennes
Un réseau d'antennes est utilisé pour récupérer un signal faible (normalement aérospatial) en "agrégant" des signaux similaires. Les antennes doivent pour celà être séparées d'un multiple de la longuer d'onde .
![réseaux d'antennes](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/316.png)

#### 3.6.9 Autres antennes
![autres antennes](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/317.png)



