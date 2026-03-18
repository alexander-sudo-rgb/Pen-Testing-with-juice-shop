Methodology:
J’ai commencé par observer le mécanisme de récupération de mot de passe et les questions de sécurité proposées.
J’ai créé un compte test afin de comprendre le workflow normal de l’application. J’ai ensuite intercepté les requêtes pour analyser les champs et validations côté client.
J’ai soumis la réponse correcte à la question de sécurité et j’ai pu réinitialiser le mot de passe du compte cible.

Vulnerabilities:
-Broken Authentication
-Insecure Security Questions
-Misconfiguratio
système d’authentification / récupération de mot de passe (Sévérité : High)
mécanisme de validation des questions secrètes.(Sévérité : High)
interface utilisateur exposant des questions trop simples.(Sévérité : Medium)

Risks:
Accès non autorisé aux données personnelles de l’utilisateur Björn.
Perte de confiance des utilisateurs envers l’application.
Compromission massive si plusieurs comptes reposent sur des questions similaires.

Actions:
Je recommande de supprimer les questions de sécurité comme mécanisme principal et de privilégier des liens de réinitialisation 
envoyés par email ou sms
Implémenter une authentification multi-facteurs et de forcer des réponses non triviales ou aléatoires si les questions sont 
conservées.






