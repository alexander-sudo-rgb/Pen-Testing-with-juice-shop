Methodology :
Les utilisateurs peuvent soumettre une suggestion
Pas besoin d’être connecté
Modification du champ associé à l’utilisateur
Test d’envoi pour vérifier si le serveur contrôle réellement l’identité de l’auteur
La modification est acceptée

Vulnerabilities :
IDOR
Broken Access Control
Absence de validation serveur des champs d’identité
Composant impacté : - Système de feedback (severity level : High)
                    - API de création de feedback (severity level : High)

Risks :
Usurpation d’identité d’un utilisateur légitime
Contenu malveillant inséré
Manipulation de l’image des produits ou du service

Actions
Ignorer toute valeur d’identification envoyée par le client
Implémenter un contrôle d’accès robuste
Revue régulière des API exposées