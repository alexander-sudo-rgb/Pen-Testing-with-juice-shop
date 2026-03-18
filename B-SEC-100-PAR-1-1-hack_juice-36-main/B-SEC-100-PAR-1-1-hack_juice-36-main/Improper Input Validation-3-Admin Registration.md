## methodology:
# – steps :
1. direction vers la page registration pour crée un compte
2. entré de toutes les donées cécessaires
3. activation de burp pour intercepter la requete
4. Envoie de la requete dans le repeater, puis send pour avoir la réponse
5. remarque d'un rôle "customer"
6. ajout d'un role 'admin' dans le request
# – techniques : 
- broken access control,  manipulation de session
# – tool used  :
- burp suite
## vulnerabilities:
# – vulnerability name :
- improper input validation
# – affected components :
- logique d'autorisation
# – severity level :
- high
## risks:
# – business impact :
- usurpation d'identité de l'administrateur
## actions:
# – propose some risks mitigation strategies :
- implémenter une liste blanche
