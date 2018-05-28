## Chapitre 5 :Applications
Ce chapitre couvre les applications des principes à la transmission radio et télévision.

### 5.1 Réception superhétérodyme
En électronique, un récepteur hétérodyne est un récepteurconçu sur le *principe du mélange de fréquences*, ou **hétéronynage**, pour convertir le signal reçu en une fréquence intermétiaire plus bas qu'il est plus facile d'utiliser que la fréquence reçue en direct. Il faut se ramener à une fréquence plus faible pour pouvoir amplifier et démoduler plus facilement le signal reçu. On obtient 2 fréquences symétriques autour de flocal et on récupère la fréquence la plus basse via un filtre passe bas.
![superhétérodyne](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/501.png)

### 5.2 Emetteur-récepteur radio
Dans l'émission de la fm on envoi dans dans l'intervalle 0-15kHz G+D. à la fréquence 19kHz on a un **signal pilote** qui nous indique que l'on utilise autour de la frequence 38kHz un signal stéréo. G-D est envoyé en LSB en modulation AM autour de la porteuse 38kHz.
![Radio stéréo](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/502.png)

### 5.3 Emetteur-Recepteur TV noir et blanc
cfr chapitre 1

### 5.4 TV couleur
Il existe différents formats pour la télévision analogique : 

* **NTSC** (USA, Japon, canada)
* **PAL** (UK, Allemagne)
* **SECAM** (France,URSS)

Pour conserver une compatibilité avec la télévision noir et blanc, on utilise le YUV (cfr chapitre 1).Il existe en fait 2 sortes de signaux : le YUV et YIQ. Y est identique mais IQ et UV diffèrent.

#### 5.4.1 NTSC (YIQ)
En NTSC, on envoi le son en FM, la chrominance Y en QAM et la luminance en VSB (bande latérale résiduelle). 

#### 5.4.2 PAL (YUV)
Le système pal possède les caractéristiques suivantes : 

* U et V possèdent la même largeur de bande
* la porteuse son est plus éloigné de la porteuse de l'imag et le spectre est plus compliqué

Y est envoyé sous la forme : v(T)= Usin(WcT)+-Vcos(WcT). 

#### 5.4.3 SECAM (Séquentiel à mémoire)
Chaque chrominance est envoyée une ligne sur deux et on complète avec la ligne précédente. La résolution en chrominance est donc la moitié de la resolution en luminance. mais cela ne pose pas de problèmes. On évite aussi les modulations FM

### 5.5 Télévision numérique 
En télévision numérique, les couleurs sont envoyées sur 8 bits.
![télévision numérique](https://raw.githubusercontent.com/Twan0u/SINF13BA/master/LELEC1930/img/503.png)
Y est échantillonné à 13.5MHz et les chrominances à 6.75MHz. Sans compression, on obtiens donc 216Mbit/s

#### Avantages

* **Compression**
* **Codes correcteurs d'erreur**
* **Enregistrement et stockage**

#### Désavantages

* **Délais de Zapping**
* **Dégradation rapide si le signal est mauvais**












