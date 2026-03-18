methodology:
Observation du mécanisme de soumission de feedbacks
Capture des requêtes à l’aide d’un proxy
Identification des paramètres utilisés pour le CAPTCHA
Réémission manuelle ou automatisée de la requête POST vers l’API de feedbacks
Envoi rapide de multiples requêtes d’insertion de feedback

vulnerabilities:
Broken Anti-Automation
CAPTCHA Bypass
Composant impacté : - Endpoint de Feedback (severity level : medium)
                    - Anti-bot (severity level : medium)

Risks:
Spam massif sur la plateforme
Introduction de contenu malveillant
Atteinte à l’image

Actions:
Vérifier serveur-side le CAPTCHA et l’unicité du token
Ajouter un CAPTCHA éprouvé
Sécurisation des endpoints ouverts au public