# methodology:
# – steps :
1. reconnaissance du nom du challenge pour identifier ce que je peux pottentioellement faire
2. recherche sur la liste des langues supportées par owasp juice shop
3. énumération de langue sur juice shop et j'ai trouvé une langue "extra" klingon
4. Identification d'un sorte d'id pour chaque langue ex : Français = fr_fr et pour Klingon = tlh-AA
4. utilisation d'un proxy pour intercepter la requête http de chargement du fichier de langue : get /assets/i18n/fr_fr.json http/2 
5. modification manuelle de la requête en remplaçant l'identifiant de la langue existante (fr_fr) par l'identifiant découvert (tlh-aa puis tlh_aa car le premier fonctionné pas)
6. envoi de la requête modifiée
# – techniques :
- énumération de ressources
# – tool used :
- moteur de recherche, proxy d'interception burp suite
# vulnerabilities:
# – vulnerability name :
- broken access control 
# – affected components :
- 
# – severity level :
- Low
# risks:
# – business impact :
- l'existence d'un accès non autorisé peut indiquer d'autres failles de contrôle,
# actions:
# – propose some risks mitigation strategies :
- liste blanche stricte