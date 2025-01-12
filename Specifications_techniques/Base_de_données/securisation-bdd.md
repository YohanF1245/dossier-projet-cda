# Stratégie de sécurisation de la base de données
## Introduction

### Politique de retention

Afin d'assurer la sécurité de nos données, nous avons mis en place une politique de sauvegarde robuste et automatisée. Chaque jour, trois copies de sauvegarde sont effectuées entre 4 et 5 heures du matin, selon la règle de sauvegarde 3-2-1. Concrètement, cela signifie :

- 3 copies de la sauvegarde quotidienne ;
- 2 supports de stockage différents pour garantir la résilience des données ;
- 1 copie externe transférée via un tunnel VPN sécurisé.
Chaque sauvegarde quotidienne est conservée pendant 15 jours, et les nouvelles écrasent automatiquement la sauvegarde la plus ancienne.<br>

Une compromission de la base de données peut être détéctée tardivement, en plus des sauvegardes journalières nous effectuerons des copies de sauvegarde de manière hebdomaires avec un roulement toutes les 5 semaines et mensuel avec un roulement annuel.<br>

Toutes les sauvegardes sont chiffrées selon l'algorithme SHA-256. La clé privée utilisée pour ce chiffrement est stockée de manière sécurisée sur un serveur HSM (Hardware Security Module), spécifiquement conçu pour la gestion de clés cryptographiques.
### Stratégie de Sauvegarde

Pour sécuriser notre base de données, nous mettons en place plusieurs mesures essentielles pour protéger les données sensibles contre diverses menaces, y compris les erreurs humaines, les attaques malveillantes et les défaillances techniques. Tout d'abord, nous appliquons des contrôles d'accès stricts en utilisant des mécanismes d'authentification et d'autorisation robustes. Cela inclut la mise en œuvre de rôles et de permissions pour limiter l'accès aux données sensibles uniquement aux utilisateurs autorisés, réduisant ainsi le risque d'erreurs de manipulation par les employés.<br>

Nous utilisons également des requêtes préparées et des ORM (Object-Relational Mapping) pour prévenir les injections SQL, qui représentent une menace courante. Le chiffrement des données au repos et en transit est mis en œuvre pour protéger les informations sensibles contre les interceptions et les accès non autorisés, y compris les attaques par ransomware. De plus, nous mettons en place des sauvegardes régulières et des plans de reprise après sinistre pour nous prémunir contre les pertes de données dues à des pannes de serveur ou à des catastrophes physiques.<br>

Nous assurons également la journalisation des accès et des modifications pour surveiller les activités suspectes et réagir rapidement en cas d'incident. Enfin, nous réalisons des audits de sécurité réguliers et maintenons notre système à jour avec les derniers correctifs de sécurité pour nous protéger contre les vulnérabilités connues. En combinant ces mesures, nous renforçons la sécurité de notre base de données et protégeons les données des utilisateurs contre une variété de menaces, qu'elles soient humaines ou techniques.
### Partage de notes
