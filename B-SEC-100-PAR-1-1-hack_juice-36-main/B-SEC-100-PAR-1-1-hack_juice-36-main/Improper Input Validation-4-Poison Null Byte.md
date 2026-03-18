# methodology:
# – steps :
1. découverte du répertoire /ftp/ permettant l'accès aux fichiers du serveur. 
2. identification d'un filtre de sécurité basé sur l'extension des fichiers (dans ce cas là , seuls les fichiers .md sont autorisés)
3. construction d'une url d'exploitation en ajoutant le caractère NUL avant l'extension autorisée (.md). 
4. exécution de la requête, ce qui a permis au système de fichiers de tronquer l'extension au niveau du caractère NULL et de télécharger des fichiers
# – techniques : 
- injection de Caractère Null
# – tool used  :
navigateur web
# vulnerabilities:
# – vulnerability name :
- accès non autorisé aux fichiers
# – affected components :
- système des fichiers
# – severity level :
- high
# risks:
# – business impact :
- fuite de données
# actions:
# – propose some risks mitigation strategies :
- renforcer l'acces à ces fichiers