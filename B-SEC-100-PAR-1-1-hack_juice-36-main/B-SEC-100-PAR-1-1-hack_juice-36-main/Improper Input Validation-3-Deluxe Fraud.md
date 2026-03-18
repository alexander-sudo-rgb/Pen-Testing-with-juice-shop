## methodology:
# – steps :
1. direction la page pour achetez le pak deluxe
2. clicker sur payer et intercepter avec burp la requet
3. envoie de la requete dans le repeater
4. changement de la méthode de payment de 'Wallet' à '' (rien) 
5. envoie de la requete
6. profiter du pack deluxe
# – techniques : 
- manipulation de paramètres http
# – tool used  :
- burp suite
## vulnerabilities:
# – vulnerability name :
- transaction non validée
# – affected components :
- système de gestion des transactions
# – severity level :
- critical
## risks:
# – business impact :
- perte de revenus
## actions:
# – propose some risks mitigation strategies :
- 
