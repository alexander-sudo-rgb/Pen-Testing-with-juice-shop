## methodology:
# – steps :
1. direction page d'aceuille du site et interception d'un requête quand on recherce un objet dans la bar de recherche
2. envoie du http history vers le repeater. Envoie de la requete et j'ai pu apercevoir tout les produit sous format sql
3. ayant search?q= j'ai tapé banane pour un succes.
4. j'ai ajouter des guillemet pour avoir un erreur et donc savoir si y'a une faille. résultat oui il y en a eu une
5. j'ai mis : banane'))UNION%20SELECT%20sql,2,3,4,5,6,7,8,9%20FROM%20sqlite_master-- afin d'avoir toute la base
# – techniques : 
- SQL injection
# – tool used  :
- burp suit
## vulnerabilities:
# – vulnerability name :
- SQL injection
# – affected components :
- Data base
# – severity level :
- high
## risks:
# – business impact :
- fuite de base de donées
## actions:
# – propose some risks mitigation strategies :
- utiliser des instructions préparées pour que les entrées utilisateur ne soient jamais interprétées comme du code sql