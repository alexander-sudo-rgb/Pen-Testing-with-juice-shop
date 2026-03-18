## methodology:
# – steps :
1. direction la page login du juiceshop (ayant fait le challenge "Login Admin" j'ai pu récupérer l'email de Jim)
2. Mettre l'email de jim dans la bar email suivi d'un apostophe (') suivi de -- avec des espace avant et après. exemple :
Jim@juiceshop' --
3. mettre n'importe qu'elle MDP et ce connécté
# – techniques : 
- SQL injection
# – tool used  :
- navigateur web
## vulnerabilities:
# – vulnerability name :
- SQL injection
# – affected components :
- système d'authentification
# – severity level :
- critical 
## risks:
# – business impact :
- usurpation d'identité
## actions:
# – propose some risks mitigation strategies :
- surveiller les tentatives de connexion contenant des caractères spéciaux sql.
