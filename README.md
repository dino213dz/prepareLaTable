# Auter:
 - Titre : prepareLaTable
 - Version : 0.1 Beta
 - Auteur :      CHORFA Alla-eddine
 - Contact : h4ckr213dz@gmail.com
      
# Description : 
- Prépare  la table, j'ai faim, j'arrive!.
- Ce script prépare l'environnement bash "Linux" après une nouvelle installation.

# Fichiers nécessaires au script
+ prepareLaTable.sh   : Le script en lui même
+ prepareLaTable.datas  : Fichier zip contenant les sources

# Etapes de la préparation :

# 1. Crée les dossiers suivants et leur attribue les droits nécessaires
+ /scripts (775)
+ /sources (644)
+ /backups (644)
+ /mnt/partage (777)

# 2. Décompresse le dossier de donénes prepareLaTable.datas dans /tmp/prepareLaTable.data/
+ /etc/aliases
+ /etc/styles

# 3. Copie des librairies personnalisées
+ Aliases : /etc/aliases
+ Styles : /etc/styles


# 4. Il parametre les fichiers suviants:
+ /etc/bash.bashrc
    - PATH, ajout de :
      - /sbin
      - /scripts
      - /mnt/partage
    - PS1 : 
      - Formattage
      - Coloration
    - History
      - Formattage
      - Coloration
      - Taille
      - Options:
        - Append
        - Ignore doublons
        - Suppr. doublons
        - Ignore Spaces (pour cacher des commandes par exemple)
    -  Afficher les informations
      -  Configuration IP
      -  Table de routage
      -  Derniere connexions

# 5. Fichiers divers :
+ /etc/ssh/sshd_config
  - PermitRootLogin yes
