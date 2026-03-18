# methodology:
# – steps :
1. découverte d'une chaîne de caractères encodée dans le fichier easter egg téléchargé pendant une exploitation précédente
2. décodage de la chaîne en base64 qui me montre un chemin illisible
3. identification du besoin d'un 2iem décodage 
4. déchiffrement de la sortie base64 en utilisant rot13
5. obtention d'un chemin bcp plus clair : /the/devs/are/so/funny/they/hid/an/easter/egg/within/the/easter/egg
6. navigation vers l'url du chemin découvert, révélant le nested easter egg et complétant le défi.
# – techniques :
- déchiffrement, reconnaissance
# – tool used :
- éditeur de texte (vscode), décodeur base64, décodeur rot13
# vulnerabilities:
# – vulnerability name :
- accès non autorisé aux fichiers
# – affected components :
- fichiers de données qui peuvent être sensible
# – severity level :
- low
# risks:
# – business impact :
- la vulnérabilité expose un secret qui est un easter egg, sans impact direct sur la sécurité
# actions:
# – propose somerisks mitigation strategies :
- 