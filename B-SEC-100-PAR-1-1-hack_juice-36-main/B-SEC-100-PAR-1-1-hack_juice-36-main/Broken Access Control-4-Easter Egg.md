# methodology:
# – steps :
1. découverte d'un répertoire d'accès public /ftp/ exposant des fichiers du serveur 
2. identification que l'accès au fichier easter egg est bloque par un certain filtre de sécurité basé sur l'extension
3. construction d'une url d'exploitation en ajoutant le caractère null encodé %2500.md


# – techniques :
- null byte injection, broken access control.
# – tool used :
- navigateur web
# vulnerabilities:
# – vulnerability name :
- accès non autorisé aux fichiers.
# – affected components :
- système de gestion des fichiers
# – severity level :
- high
# risks:
# – business impact :
- fuite de données
# actions:
# – propose some risks mitigation strategies :
-