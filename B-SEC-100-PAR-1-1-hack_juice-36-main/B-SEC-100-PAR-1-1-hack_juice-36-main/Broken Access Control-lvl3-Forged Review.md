Methodology :
Observation du fait que seuls les utilisateurs authentifiés peuvent laisser un avis sur un produit
Identification des paramètres
Altération du champ utilisateur
Test d’envoi afin de vérifier s’il est possible d’usurper l’identité d’un autre utilisateur

Vulnerabilities :
Broken Access Control
Manque de contrôle de l’intégrité des champs user
Composant impacté : - Système d’avis produits (severity level : High)
                    - API de soumission de reviews (severity level : High)

Risks : 
Faux avis pouvant manipuler la réputation d’un produit
Possibilité d’usurper n’importe quel compte
Impact sur la confiance des utilisateurs
Contenu malveillant injecté dans les avis

Actions:
Bloquer le champ d’identification de l’auteur dans le frontend
Implémentation stricte d’un contrôle d’accès basé sur les permissions
Audit régulier des API publiques