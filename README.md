# prepareLaTable
Version 0.1 Beta
Description :

Prépare  la table, j'ai faim, j'arrive!. 
Ce script prépare l'environnement "Linux" après une nouvelle installation.

Crée les dossier suivants et leur attribue les droits nécessaires
  /scripts (775)
  /sources (644)
  /backups (644)
  /mnt/partage (777)

Il parametre les fichiers suviants:
- /etc/bash.bashrc
    PATH, ajout de 
      /sbin
      /scripts
    PS1 : 
      Formattage
      Coloration
    History
      Formattage
      Coloration
      Talle
      Options:
        Append
        Ignore doublons
        Suppr. doublons
        Ignore Spaces (pour cacher des commandes par exemple)
  
    Afficher les informations
      Configuration IP
      Table de routage
      Derniere connexions
