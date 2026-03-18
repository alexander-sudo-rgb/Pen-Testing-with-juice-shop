## methodology:
# – steps :
1. interception d'un produit avec burp lorsque on l'ajoute au panier
2. Envoie de la requete au serveur
3. recupération du post
4. ajout du paramètre "BasketId":"1", en double
5. changement de l'id 1 en 2 ""BasketId":"2","
# – techniques : 
- improper input validation, manipulation de paramètres http
# – tool used  :
- proxy d'interception burp suite.
## vulnerabilities:
# – vulnerability name :
- improper input validation
# – affected components :
- logique du panier/système de commande
# – severity level :
- critical
## risks:
# – business impact :
- perte financière directe et illimitée par manipulation des transactions, détournement de fonds
## actions:
# – proposesomerisks mitigation strategies :
- s'assurer que le montant total d'une commande ne peut jamais être négatif avant de finaliser la transaction.
