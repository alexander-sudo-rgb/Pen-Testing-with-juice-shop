Methodology:
J'ai collecté des informations publiques sur la personne.
J'ai dentificatié des services accessibles, portails de connexion et endpoints d’API.
J’ai testé les paramètres vulnérables, effectué du fuzzing et analysé les réponses du serveur.
J’ai tenté de découvrir des mots de passe faibles et de détourner des sessions.

vulnerabilities:
Injection SQL
Cross-Site Scripting
Mauvaise configuration
composant affecté : -Base de données (sévérité : critique)
                    -Section commentaires de l’application web (sévérité : high)
                    -Interface d’administration (sévérité : medium)

Risks:
exposition de données sensibles
perte de confiance des utilisateurs, mauvaise presse, sanctions réglementaires.
indisponibilité de service, compromission de l’intégrité des systèmes, risque de rançongiciel.

Actions:
Restriction d’accès au panneau admin via VPN ou liste blanche IP.
Utilisation de requêtes SQL paramétrées.
Tests d’intrusion et revues de code régulières.