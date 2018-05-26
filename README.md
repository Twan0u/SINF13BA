# SINF13BA

## Utilisation de ce répertoire 
Les notes se situent dans le dossier note chaque dossier de cours.   
Elles sont disponiles au format **Markdown** classées par chapitre de cours **chapitre*.md**

## Compiler les notes en PDF
### Prerequis : installation

```
sudo apt-get update && sudo apt-get upgrade
sudo apt-get install pandoc
sudo apt-get install texlive
```

### Tout compiler 

```
    make all
``` 

### Compiler cours par cours
Il faut remplacer COURS par l'intitulé du cours 

```
    make COURS
```

## Upgrades possibles
* compilation chapitre par chapitre
* mettre tous les pdf dans un fichier séparré 
