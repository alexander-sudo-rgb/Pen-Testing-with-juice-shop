Methodology:
J’ai identifié la fonctionnalité vulnérable dans OWASP Juice Shop 
J'ai mis un <iframe src="javascript:alert('xss')"> dans un champ de saisie.
Le script s’est exécuté dans le navigateur

vulnerabilities:
Cross-Site Scripting
Composant affecté : -Validation côté client (severity level : high)
                    -DOM manipulation (severity level : high)

Risks:
Vol de cookies et tokens de session.
Détournement de comptes utilisateurs.
Injection de contenu malveillant
Impact réputationnel et légal

actions:
Surveiller les entrées suspectes.
Implémenter une validation côté serveur.
Ne jamais se fier uniquement aux protections côté client.