# methodology:
# – steps :
1. identification du répertoire /ftp/ non protégé. 
2. tentative de télécharger tout les fichiers (ex: coupons_2013.md.bak) dont l'extension est bloquée par un filtre de sécurité. 
3. injection d'un caractère NULL "%2500" entre le nom du fichier et l'extension .md attendue par le filtre. 
4. le filtre de sécurité ne voit que la partie précédant le NULL, validant le téléchargement du fichier complet.
# – techniques :
- injection de Caractère Null (Null Byte Injection)
# – tool used :
- navigateur Web
# vulnerabilities:
# – vulnerability name :
- contournement de filtre par Caractère Null/ Vulnérabilité d'Accès Non Autorisé aux Fichiers
# – affected components :
- accès aux fichiers
# – severity level :
- high
# risks:
# – business impact :
- fuite de Données
# actions:
# – proposesomerisks mitigation strategies :
- mise en œuvre d'un Contrôle d'Accès Fort: exiger une authentification et une autorisation appropriées avant d'accéder au répertoire /ftp/
# – suggest remediation fixes :
- utiliser une liste blanche stricte des extensions autorisées