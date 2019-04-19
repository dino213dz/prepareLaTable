# ###################################################################################################################
#   Titre : prepareLaTable                                                                                :          #
#   Version : 0.1 Beta                                                                                              #
#   Auteur :      CHORFA Alla-eddine                                                                                #
#                 dino213dz@gmail.com                                                                               #
#                                                                                                                   #
#   Description : Prépare  la table, j'ai faim, j'arrive!.                                                          #
#                 Ce script prépare l'environnement "Linux" après une nouvelle installation.                        #
#                                                                                                                   #
# ###################################################################################################################

# Fichiers nécessaires au script
+ prepareLaTable.sh   : Le script en lui même
+ prepareLaTable.datas  : Fichier zip contenant les sources

# Crée les dossiers suivants et leur attribue les droits nécessaires
+ /scripts (775)
+ /sources (644)
+ /backups (644)
+ /mnt/partage (777)

# Décompresse le dossier de donénes prepareLaTable.datas dans /tmp/prepareLaTable.data/
+ /etc/aliases
+ /etc/styles

# Copie des librairies personnalisées
+ Aliases : /etc/aliases
+ Styles : /etc/styles


# Il parametre les fichiers suviants:
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

# Fichiers divers :
+ /etc/ssh/sshd_config
  - PermitRootLogin yes
