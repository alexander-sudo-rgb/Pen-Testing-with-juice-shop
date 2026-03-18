## methodology:
# – steps :
1. interception d'un produit avec burp lorsque on l'ajoute au panier
2. Envoie de la requete au serveur
3. recupération du post
4. modification du paramètre de quantité par une valeur entière négative élevée (ex: -100000)
5. désactivation du proxy pour permettre à l'application de valider et d'afficher le panier
6. validation de la commande qui coutera de l'argent négatif
7. être riche
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
# – propose some risks mitigation strategies :
- s'assurer que le montant total d'une commande ne peut jamais être négatif avant de finaliser la transaction.
